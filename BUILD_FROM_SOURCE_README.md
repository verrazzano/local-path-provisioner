# Build Instructions

The base tag this release is branched from is `v0.0.14`


Create Environment Variables

```
export DOCKER_REPO=<Docker Repository>
export DOCKER_NAMESPACE=<Docker Namespace>
export DOCKER_TAG=v0.0.14
```

Build and Push Image

```
git tag -d v0.0.14
git tag v0.0.14
make 

docker tag rancher/local-path-provisioner:v0.0.14 ${DOCKER_REPO}/${DOCKER_NAMESPACE}/local-path-provisioner:${DOCKER_TAG}
docker push ${DOCKER_REPO}/${DOCKER_NAMESPACE}/local-path-provisioner:${DOCKER_TAG}
```