# Playground for truffleruby

### Links

- [truffleruby](https://github.com/oracle/truffleruby) github project.

### Performance 

Compare with MRI <br/>
ruby on rails startup 


```
# build the mri test image
docker build -t mri-ruby -f Dockerfile.mri .
# build the truffleruby test image
docker build -t truffle-ruby -f Dockerfile.truffle .
```

How long the rails framework startup took.

```
docker run -it --rm mri-ruby /bin/bash -lc 'time rails r "exit 0"
```
For MRI it's round about 5 seconds.

```
docker run -it --rm truffle-ruby /bin/bash -lc 'time rails r "exit 0"
```

For truffleruby it's round about 20 seconds.


### At first glance, truffle ruby doesn't seem like a good choice. 
