``` 
docker build -t helloworld .  
docker run -d --name hellworld -p 8080:8080 helloworld
```
```
使用原生jenkins进行CI编译，Dockerfile中调整了docker-demo.war路径，去掉了灵雀云早期中间环节使用的alaudaci.yml文件
ADD target/docker-demo.war /usr/local/apache-tomcat-6.0.45/webapps/
