# sync-docker-image

1. Copy the github workflow file 
2. Configure your secrets:
    - Docker Authentication: DOCKER_REGISTRY (e.g. quay.io), DOCKER_USERNAME, DOCKER_PASSWORD
    - Docker image name: IMAGE_NAME (e.g. quay.io/sammyteillet/copy-of-dd:latest) 
3. Configure weather manual trigger `workflow_dispatch` (default) or cron (replace code with the following, every day at 8am):
```yaml
on:
  schedule:
    - cron: '0 8 * * *'
```



![Alt text](<CleanShot 2023-07-18 at 15.49.01@2x.png>)