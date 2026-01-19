# linux_base_image

This repo consists of all binaries/src files required to build images that are mentioned here - https://docs.akto.io/dast/akto-dast-on-premise#deployment-steps

To build any image, go to that directory and run the following - 

```
docker build -t IMAGE_NAME:IMAGE_TAG .
```



1. Please ensure you build on amd64 platform (arm64 not supported for now - mainly due to Chrome dependency)
2. For any issues, please reach out to the Akto team through customer/vendor channels or contact support@akto.io
