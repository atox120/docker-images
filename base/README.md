
# Base docker image


## Summary v0.0.2

1) Added multi-architecture support for (amd64, linux and arm64). 
2) Removed support for gcloud sdk, as there is currently no officially supported ubuntu-ARM64 version. For gcloud SDK, see image [base-gcloud](https://github.com/atox120/docker-images/tree/master/base-gcloud)

## Summary v0.0.1
Forked from midsw205/docker-images. Key changes:

1) Updated to ubuntu focal. 
2) Installed cassandra python driver. 
3) Upgraded to python 3.8

Image gets pushed to  <https://hub.docker.com/u/atox120/>.



# Misc Notes
https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu
