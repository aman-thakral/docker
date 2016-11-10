# Building
```
cd /path/to/repo
docker build . -t <name>:<version>
```

# Running the Container
```
docker run -d -p 8080:8080 -p 50000:50000 -e JENKINS_OPTS="--prefix=/jenkins" -v /path/to/jenkins/data:/var/jenkins_home -v /path/to/repo/:/usr/share/elasticsearch/config <NAME>
```
* Note the -e option above is to support a reverse proxy
