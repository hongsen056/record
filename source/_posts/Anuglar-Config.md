title: Anuglar Config
author: Hongsen
tags:
  - Angular
categories: []
date: 2018-07-16 23:09:00
---
##### Apache .htaccess
 angularjs pushstate (history) support:
 See http://www.josscrowcroft.com/2012/code/htaccess-for-html5-history-pushstate-url-routing/
* \<\ifModule mod_rewrite.c>
*     RewriteEngine On
*     RewriteCond %{REQUEST_FILENAME} !-f
*     RewriteCond %{REQUEST_FILENAME} !-d
*     RewriteCond %{REQUEST_URI} !index
*     RewriteRule (.*) index.html [L]
* \<\/ifModule>




* RewriteRule ^(.*)\.htm $1.html
* ^开始
* ()取值
* .*匹配任意
* \.html转意
* $结束
* $1括号内的内容