# docker-push-filter

This sample repo showcases how we can push built images by:

1. set `LABEL=` in Dockefiles (specifically, we can set maintainer label ([example](Dockerfile.foo#L3)))
2. use `docker image list --filter label=maintainer=xxx` and push each image

