# howto_compile_docker

easy!

## prerequisites
* a working docker environment
* GNU Make

## compilation
1. clone moby repo (branch 17.05.x)
```
git clone https://github.com/moby/moby.git -b 17.05.x
```
2. run make from the repo directory
```
cd moby
make
```
3. install: 
``make install``

## binaries generated
* bundles/17.05.0-ce/binary-client/docker-17.05.0-ce
* bundles/17.05.0-ce/binary-daemon/dockerd-17.05.0-ce
* bundles/17.05.0-ce/binary-daemon/docker-containerd
* bundles/17.05.0-ce/binary-daemon/docker-containerd-ctr
* bundles/17.05.0-ce/binary-daemon/docker-init
* bundles/17.05.0-ce/binary-daemon/docker-proxy
* bundles/17.05.0-ce/binary-daemon/docker-runc

also, there are some init files (systemd, sysvinit, upstrart, openrc ...) under contrib/init
