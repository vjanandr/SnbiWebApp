Steps to install tomcat on ubuntu:

1. The first thing you will want to do is update your apt-get package lists:

    $sudo apt-get update

2. Now you are ready to install Tomcat. Run the following command to start the installation:

    $sudo apt-get install tomcat7

To change port of tomcat server

1. Edit server.xml and change port="8080" to "8082"

    $sudo vi /var/lib/tomcat7/conf/server.xml

    <Connector connectionTimeout="20000" port="8080" protocol="HTTP/1.1" redirectPort="8443"/>
2.  Now restart Tomcat with this command:

    sudo service tomcat7 restart

To run the web-app

1. copy the form-1 folder to location /var/lib/tomcat7/webapps/ROOT/
2. use this url in browser
        http://<IP adress of tomcat server>:<port>/jsp/form-1/index_final.html
        eg: http://10.64.69.123:8082/jsp/form-1/index_final.html
