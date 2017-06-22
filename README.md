## SpringOAuth2RestDemo 2 ## 

The project uses the following technologies: 

- Web/REST : Spring 3.2.14.RELEASE / Spring Security 3.1.0.RELEASE
- database : Mysql 5.1.36 / Hibernate 5.3.4 RELEASE
- Security : Oauth2 1.0.5.RELEASE 
- REST API
- Tool : Eclipse NEON , Java 1.7

## Build and Run ##

1. Download  **SpringOAuth2RestDemo-master.zip**
2. Unzip SpringOAuth2RestDemo-master.zip
3. Start Eclipse 
4. import -> Existing Maven Projects -> select 3 project (AuthServer, RESTClient, RESTServer)
5. Edit `db.properties`

<pre><code>
db.driver=com.mysql.jdbc.Driver
db.jdbcurl=jdbc:mysql://localhost:3306/oauthdb
db.username=root
db.password=root
</code>
</pre>

6. insert database [DDL](https://github.com/yks8890/SpringOAuth2RestDemo/blob/master/AuthServer/src/main/resources/schema_MySql.sql)/[DML](https://github.com/yks8890/SpringOAuth2RestDemo/blob/master/AuthServer/src/main/resources/test-data.sql)
7. Run on Server : AuthServer(404Error) -> RESTServer(404Error) -> RESTClient(Success View page)   
*(Server : Tomcat 7 or Tomcat 8 .etc)*

**RESTClient server  Result View** 
<img style="max-width: 100%; height: auto;" src="https://github.com/yks8890/SpringOAuth2RestDemo/blob/master/capture.PNG">

