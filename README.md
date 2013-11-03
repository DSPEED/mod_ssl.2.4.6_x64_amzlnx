mod_ssl.2.4.6_x64_amzlnx
========================

mod_ssl.2.4.6 Ist das Fehlende mod_ssl.so file einfach in /etc/httpd/modules/ copieren 

============ WARUM FEHLER============
Weil es nur mod_ssl für Apache 2.2 in den Amazon Repositorys gibt.
Hier Könnt ihr ein mit dem Neusten Amazon Linux Compiliertes mod_ssl.so Modul runterladen das ermöglicht dann das laden im apache2.4.6xxxxx


============ FEHLER =================
yum install mod_ssl
Loaded plugins: priorities, security, update-motd, upgrade-helper
amzn-main                                                                                                                             | 2.1 kB     00:00     
amzn-updates                                                                                                                          | 2.3 kB     00:00     
Setting up Install Process
Resolving Dependencies
--> Running transaction check
---> Package mod_ssl.x86_64 1:2.2.25-1.0.amzn1 will be installed
--> Processing Dependency: httpd-mmn = 20051115 for package: 1:mod_ssl-2.2.25-1.0.amzn1.x86_64
--> Processing Dependency: httpd = 2.2.25-1.0.amzn1 for package: 1:mod_ssl-2.2.25-1.0.amzn1.x86_64
--> Running transaction check
---> Package httpd.x86_64 0:2.2.25-1.0.amzn1 will be installed
--> Processing Dependency: httpd-tools = 2.2.25-1.0.amzn1 for package: httpd-2.2.25-1.0.amzn1.x86_64
--> Processing Dependency: apr-util-ldap for package: httpd-2.2.25-1.0.amzn1.x86_64
--> Running transaction check
---> Package apr-util-ldap.x86_64 0:1.4.1-4.14.amzn1 will be installed
---> Package httpd-tools.x86_64 0:2.2.25-1.0.amzn1 will be installed
--> Processing Conflict: httpd24-2.4.6-2.48.amzn1.x86_64 conflicts httpd < 2.4.6
--> Processing Conflict: httpd24-tools-2.4.6-2.48.amzn1.x86_64 conflicts httpd-tools < 2.4.6
--> Finished Dependency Resolution
Error: httpd24-tools conflicts with httpd-tools-2.2.25-1.0.amzn1.x86_64
Error: httpd24 conflicts with httpd-2.2.25-1.0.amzn1.x86_64
 You could try using --skip-broken to work around the problem
 You could try running: rpm -Va --nofiles --nodigest

