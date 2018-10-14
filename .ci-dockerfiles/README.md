# Build image

```bash
docker build -t ponylang/ponyc-ci:main.actor .
```

# Run image to test

Will get you a bash shell in the image to try cloning Pony into where you can test a build to make sure everything will work before pushing:

```bash
docker run --name ponyc-ci-main-actor --rm -i -t ponylang/ponyc-ci:main.actor bash
```

# Push to dockerhub

You'll need credentials for the ponylang dockerhub account. Talk to @jemc or @seantallen for access

```bash
docker push ponylang/ponyc-ci:main.actor
```
