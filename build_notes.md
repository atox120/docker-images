## Notes on docker buildx.

docker buildx build . --platform linux/arm64,linux/amd64 --output type=image --push=true --tag namespace/image:version --tag namespace/image:laetst
