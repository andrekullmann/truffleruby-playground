# Playground for truffleruby


```
docker build -t mri-ruby -f Dockerfile.mri .
```

```
docker build -t truffle-ruby -f Dockerfile.truffle .
```

```
docker run -it --rm mri-ruby /bin/bash -lc 'time rails r "exit 0"

```

```
docker run -it --rm truffle-ruby /bin/bash -lc 'time rails r "exit 0"
```
