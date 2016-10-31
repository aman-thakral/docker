# Running the Container
```
docker run -d -p 8080:8080 -p 50000:50000 -v /path/to/jenkins/data:/var/jenkins_home -v /path/to/repo/:/usr/share/elasticsearch/config <NAME>
```
