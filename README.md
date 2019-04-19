# Minimalist Docker Images

The motivation to create these images is due to other slim versions aren't any slim at all, since they bring several unrequired packages and configurations which make the image bigger than it is really needed to work. My major goal is to make them as small as possible and still full functional.

Though the ideal abordation would be using distroless images, I am not satisfied with the ones provided currently, since they also bring unrequired packages as ca-certificates, tzdata and glibc, which make me say they are not so distroless as they should be. First I would replace glibc to musl instead, once it is much more lightweight, second I would compile all packages with libc statically linked, so not even the musl would be required. Until I be able to do that I will stick to alpine version.
