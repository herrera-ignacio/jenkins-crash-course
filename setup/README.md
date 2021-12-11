# Initial Setup

1. Install docker
2. Install docker-compose
3. `docker pull jenkins/jenkins`
4. Create `docker-compose.yml`
5. `mkdir jenkins_home`
6. Get uid and qid with `id`
6. `sudo chown <uid>:<qid> jenkins_home -R`
7. Make sure your user is the owner: `ll`
8. `docker-compose up -d`
9. `docker ps`
10. `docker logs -f jenkins`
11. Try to navigate to `localhost:8080`.
12. From external hosts. you can also ssh using your jenkins user `ssh <user>@jenkins-ip` or simply navigating to the url if http port is exposed
13. From your host, you can execute a bash in the jenkins container: `docker exec -ti jenkins bash`