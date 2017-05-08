# Two simple steps to build optimized OpenJDK for Power:
1) Install docker - i.e. sudo apt-get install docker.io
2) execute below command
```
sudo docker run --rm -v `pwd`:/ws bigtop/slaves:trunk-ubuntu-16.04-ppc64le bash -l -c "cd /ws; ./build_openjdk.sh https://github.com/mtbrandy/openjdk-jdk8u.git jdk8u152-b03-opt"
```
