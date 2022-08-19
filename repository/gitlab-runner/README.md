#### GitLab Runner

Documentation: [https://docs.gitlab.com/runner/register/](https://docs.gitlab.com/runner/register/)

One-line registration command:
```
docker-compose exec gitlab-runner \
    gitlab-runner register \
    --non-interactive \
    --url <GITLAB-URL> \
    --registration-token <GITLAB-REGISTRATION-TOKEN> \
    --executor docker \
    --description "<DESCRIPTION>" \
    --tag-list "<TAGS>" \
    --docker-image "alpine:latest" \
    --docker-volumes /var/run/docker.sock:/var/run/docker.sock
```