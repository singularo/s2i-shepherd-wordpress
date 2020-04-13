
# This is an s2i builder image for wordpress, see below for starter details

Original instructions available here - https://github.com/openshift/source-to-image

Execute build
```bash
IMAGE_NAME=singularo/s2i-shepherd-wordpress
docker build -t ${IMAGE_NAME} .
```

The builder image can also be created by using the *make* command since a *Makefile* is included.

Now when you deploy from shepherd, it will use the updated singularo/s2i-shepherd-wordpress image with your changes.
