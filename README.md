# let us host together this
@ start here
- 1 https://infinityfree.net/

* then here
- https://www.freenom.com/



# .htaccess DOCUMENT
RewriteEngine On
RewriteCond %{HTTP:X-Forwarded-Proto} !https [OR]
RewriteCond %{HTTPS} off
RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]
