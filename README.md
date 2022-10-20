# docker-push-filter

This sample repo showcases how we can push built images by:

1. set `LABEL=` in Dockefiles (specifically, we can set maintainer label ([example](Dockerfile.foo#L3)))
2. use `docker image list --filter label=maintainer=xxx` and push each image

## NOTE

We can see that the `docker image list` without filter shows many images, besides the built images.
https://app.circleci.com/pipelines/github/kelvintaywl-cci/docker-push-filter/5/workflows/bff6508f-b3e9-4b7c-81c9-2e66667d8529/jobs/5?invite=true#step-107-3

However, we can see that, by filtering, we push the specific images only.
