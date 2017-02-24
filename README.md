# Docker Tomcat with volumes exposed

## Usage

```
docker run -it --rm \
    -v "$PWD"/PATH/TO/WAR:/usr/local/tomcat/webapps \
    -v "$PWD"/PATH/TO/CONF:/usr/local/tomcat/conf/api/classes \
    -v "$PWD"/PATH/TO/CATALINA:/usr/local/tomcat/conf/Catalina/localhost \
    -p 8080:8080 \
    --name tomcat \
    42bv/tomcat-volumes-exposed:1.0.0
```