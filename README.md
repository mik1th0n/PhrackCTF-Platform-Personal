# PhrackCTF-Platform-Personal

This is the full version of phrackCTF-Platform including backend & frontend. This platform is for personal competition, user register as single person and take part in competition. Team version is here:[https://github.com/zjlywjh001/PhrackCTF-Platform-Team](https://github.com/zjlywjh001/PhrackCTF-Platform-Team)   
虽然我不能保证这是前端最炫的CTF平台，但我相信这会是后台功能最友好的CTF平台。

Based on Spring and SpringMVC framework.

### Demo
See demo photos here [http://photo.163.com/zjlywjh002/#m=1&aid=303094421&p=1](http://photo.163.com/zjlywjh002/#m=1&aid=303094421&p=1)

## Techniques

### Base Framework
spring & spring MVC
### Database Connect Pool:
Alibaba Druid
### SQL mapper framework
Mybatis
### Security framework
Apache Shrio

### Database
postgresql-9.5

### FrontEnd
Bootstrap & jQuery

## Notice
It's highly recommanded to use https when deploy this platform.  
Before using :  
1. Install umeditor maven dependencies commons-fileupload-1.2.2.jar and ueditor-mini.jar in src/main/webapp/umeditor/jsp to local Maven repository:   
**mvn install:install-file -Dfile=path_to_umeditor_mini_jar\ueditor-mini.jar -DgroupId=umeditor -DartifactId=ueditor-mini -Dversion=1.2.2 -Dpackaging=jar -DgeneratePom=true -DcreateChecksum=true**    
2. Set mail server info in resources/spring-mail.xml because this platform using mail system to activate user.   
3. Set database information in system.properties   
4. Mail template in mail.properties
5. Create a user and set column "role" to "admin" for setting a user as administrator.
6. ***Important Security Issue!!! Change Cookie Encryption key in spring-shiro.xml before deployment.***

## Docker
The docker image for this project is available now.   
See here: https://github.com/zjlywjh001/phrackCTF-Personal-Docker   

## License
Apache Public License v2.

