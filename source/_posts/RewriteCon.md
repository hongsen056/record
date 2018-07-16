title: RewriteCon
date: 2018-07-15 15:32:56
tags: [linux]
---
#### RewriteCon





* RewriteEngine on
* RewriteCond $1 !^(index\.php|public|\.txt)
* RewriteCond %{REQUEST_FILENAME} !-f
* RewriteCond %{REQUEST_FILENAME} !-d
* RewriteRule ^(.*)$ index.php?$1


---


###### 修改apache的配置文件httpd.conf
1. 把"#LoadModule rewrite_module modules/mod_rewrite.so" 修改为 "LoadModule rewrite_module modules/mod_rewrite.so"

2. 找到对应的<Directory>段，把"AllowOverride None" 修改为 "AllowOverride All"