---
title: "多站点WPMU注意事项/屏蔽IP方法"
post_status: publish
post_date: 2022-05-20 22:05:20
taxonomy:
 category: 
  - 好书精读
 post_tag: 
  - "投资"
---

WordPress多站点是指安装一个程序，就可以用来建立管理多个站点，属于自带功能。

```
// 开启前 缓存插件 比如wp-rocket、redis对象存储等最好先停用
// 开启功能 配置文件wp-config.php里面加入一行代码
// /* That’s all, stop editing! Happy blogging. */上面
define('WP_ALLOW_MULTISITE', true);
```

进入后台 工具>>站点网络配置，按照页面提示进行下一步操作。

主题里面要装一个默认的主题比如twentytwentytwo，以免出错。

## 如何使用宝塔面板拒绝拦截IP地址

宝塔面板提供屏蔽IP工具允许您阻止单个IP地址以及IP地址范围，而无需编辑Web服务器配置文件。

> **重要：**屏蔽IP工具是一项强大的功能，如果使用不当，可能会阻止合法服务或个人。

要在宝塔面板中屏蔽拦截IP地址，请导航至**安全**，选择屏蔽IP，填入屏蔽IP或者IP段，点击屏蔽按钮即可添加指定IP/IP段至屏蔽列表。

在“将IP地址添加到屏蔽”模式中，您可以将IPV4地址、IPV6地址和CIDR（无类域间路由）IP地址范围添加到阻止列表。CIDR范围可用于屏蔽IP地址的连续范围（例如127.0.0.1到127.0.0.255）。要生成有效的CIDR范围，我们建议使用这样的[工具](https://www.ipaddressguide.com/cidr)。

以下是一些您可以屏蔽的IP地址示例：

- IPV4地址 – 103.5.140.141
- IPV6地址 – 2001:0db8:0a0b:12f0:0000:0000:0000:0001
- CIDR范围 – 128.0.0.1/32

## 如何在Cloudflare中拒绝拦截IP地址

如果您是Cloudflare用户，您可以使用Cloudflare仪表盘中的“IP Access Rules”工具来屏蔽IP地址和IP范围。

在Cloudflare仪表盘中，导航到**Firewall > Tools**。

要创建新的IP访问规则，请添加IP地址，选择“Block”操作，选择“This Website”（如果您希望规则适用于所有Cloudflare域，则选择“All Websites in Account”），然后单击“Add”。

添加访问规则后，它将出现在“IP Access Rules”列表中。在这里，您可以对访问规则进行更改，例如更改操作、添加注释和删除规则。

除了“Block”动作，Cloudflare还支持“Challenge”、“Allow”和“JavaScript Challenge”。根据您要实现的目标，您可能希望使用这些其他操作之一，而不是“Block”。

#### 在Cloudflare中拦截IP范围、国家和ASN

除了单个IP地址，Cloudflare的IP访问规则还支持IP范围、国家名称和ASN（自治系统编号）。

- 要屏蔽IP范围，请为IP访问规则值指定CIDR范围。
- 要屏蔽某个国家/地区，请指定其为[Alpha-2国家/地区代码](https://www.iban.com/country-codes)。
- 要屏蔽ASN（由单个网络运营商控制的IP列表），请指定以“AS”开头的有效ASN。

## 如何在Nginx中拒绝拦截IP地址

如果您的站点是使用Nginx Web服务器自托管的，您可以直接在Web服务器配置中屏蔽IP地址。

要在Nginx中屏蔽IP地址，请通过SSH连接到您的服务器并使用`nano`文本编辑器打开Nginx配置文件，如下所示：

```
nano /etc/nginx/nginx.conf
```

#### 如何使用Nginx屏蔽单个IP地址

要在 Nginx 中阻止单个 IP（IPV4 或 IPV6）地址，请使用如下`deny`指令：

```
deny 190.60.78.31;
deny 4b73:8cd3:6f7b:8ddc:d2f9:31ca:b6b1:834e;
```

#### 如何使用Nginx屏蔽CIDR IP范围

要在Nginx中阻止CIDR IP范围，请使用以下指令：

```
deny 192.168.0.0/24;
```

#### 高级Nginx IP拦截技术

如果要阻止对特定目录的访问（ed domain.com/secret-directory/），可以使用下面的Nginx指令：

```
location /secret-directory/ {
<strong>deny</strong> 192.168.0.0/24;</p>
}
```

`deny`指令接受`all`一个值。这对于您想要阻止所有 IP 地址访问您的站点的情况很有用。`deny all;`指令通常与`allow` – 一起使用- 这使您可以允许特定的 IP 地址同时阻止其他所有内容。

```
location /secret-directory/ {
allow 192.168.0.0/16;
deny all;
}
```

#### 保存Nginx配置并重新加载Nginx

使用nano完成配置编辑后，请务必按Ctrl+O保存更改。保存文件后，按Ctrl+X 退出nano。

要激活新的IP屏蔽规则，您还需要使用以下命令重新加载Nginx配置：

```
sudo systemctl reload nginx
```

## 如何在Apache中屏蔽IP地址

如果您的站点是使用Apache Web服务器自托管的，您可以直接在Web服务器配置中屏蔽IP地址。要在Apache中屏蔽IP地址，您需要使用.htaccess文件，它允许您将唯一规则应用于特定目录。要在整个站点上应用规则，应将.htaccess文件放在站点的根目录中。

首先，通过SSH连接到您的服务器，导航到您站点的根目录，然后使用以下命令创建.htaccess文件：

```
touch .htaccess
```

接下来，使用`nano`文本编辑器打开.htaccess文件，如下所示：

```
nano .htaccess
```

屏蔽IP的确切规则取决于您使用的是Apache 2.2还是2.4，因此我们将包含两个版本的规则。编辑.htaccess文件时，请使用Apache版本对应的规则。

### 如何使用Apache拦截单个IP地址

要在Apache中拦截单个IP（IPV4或IPV6）地址，请使用以下规则：

**\# Apache 2.2**

> order allow, deny
> 
> allow 192.168.0.0
> 
> deny from all

**#Apache 2.4**

> **Require** all granted
> 
> **Require** not ip 192.168.0.0

### 如何使用Apache屏蔽CIDR IP范围

要在Apache中拦截IP范围地址，请使用以下规则：

**\# Apache 2.2**

> order allow, deny
> 
> allow 192.168.0.0/16
> 
> deny from all

**#Apache 2.4**

> **Require** all granted
> 
> **Require** not ip 192.168.0.0/16
