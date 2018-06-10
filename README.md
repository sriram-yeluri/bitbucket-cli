# bitbucket-cli
CLI for managing Atlassian bitbucket 


### Atlassian Bitbucket docker image is used for testing this CLI. 
Pull image from official docker hub atlassian bitbucket repository [docker-hub-bitbucket](https://hub.docker.com/r/atlassian/bitbucket-server/)  
Spin a container and test the CLI

```
docker pull atlassian/bitbucket-server
docker volume create --name bitbucketVolume
docker run -v bitbucketVolume:/var/atlassian/application-data/bitbucket --name="bitbucket" -d -p 7990:7990 -p 7999:7999 atlassian/bitbucket-server

```

Check the status of container by monitoring the logs:
``` docker logs -f image_id ```

Bitbucket is accessible on local host on 7990 port for http and 7999 for ssl
http://localhost:7990

