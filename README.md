# Three simple steps to build an optimized OpenJDK binary for Power:
1) Install docker - i.e. sudo apt-get install docker.io
2) Execute below command from the command line:
```
git clone https://github.com/OpenPOWER-BigData/build-opt-openjdk.git; cd build-opt-openjdk
```
3) Execute below command from the command line:
```
sudo docker run --rm -v `pwd`:/ws bigtop/slaves:trunk-ubuntu-16.04-ppc64le bash -l -c "cd /ws; ./build_openjdk.sh https://github.com/mtbrandy/openjdk-jdk8u.git jdk8u152-b03-opt"
```
