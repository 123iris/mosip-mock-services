# mosip-mock-services

## 1. Create mock-abis docker image

* To build docker image

```
	$ git clone https://github.com/mosip/mosip-mock-services.git
	$ cd mosip-mock-services/
	$ git branch
	$ sudo apt-get install maven -y
	$ mvn clean install -Dgpg.skip=true -Dmaven.tests.skip=true
	$ cd ../
	$ docker build mock-abis/
	$ docker images
	$ docker tag a20396e09620 syedsalman041997/mock-abis:master
	$ docker images
	$ docker login
	$ docker push syedsalman041997/mock-abis:master
```