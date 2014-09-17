# 개발환경과 Vagrant

- - -
## Dev-environment
+ 프로젝트당 필요한 Application 은 많다
+ Application 의 조합은 더 많다
+ 프로젝트는 더 많다
+ 결국 로컬 머신은 각종 프로젝트의 Application 홍수
+ 시간이 믾이 지난 프로젝트의 개발 환경은 어떻게 되돌려야 하는가?

_ _ _
## Common solution
+ Virtual Machine!
+ 프로젝트마다 하나씩 생성해서 사용할 수 있다.
	+ 가상머신을 생성하고
	+ 가상머신을 설정하고
	+ 가상머신에 OS를 설치하고
	+ 필요한 Application을 설치하고
	+ 개발한다
	+ 팀원 모두가!

- - -
## About Vagrant
+ 로컬의 VM을 편하게 관리할 수 있도록 도와준다.
+ CLI 기반이다.
+ Box 단위로 가상머신의 이미지를 사용할 수 있다.
+ 만들어진 개발환경을 다시 Box로 만들어 공유할 수 있다.
+ [Vagrant Cloud](https://vagrantcloud.com/) 에서 쉽게 Box 를 구할 수 있다.
_ _ _
## 지원되는 VM 환경
+ virtualbox
+ parallels
+ vmware
+ hyperv
+ digitalocean, aws, rackspace 등의 Cloud 환경도 지원

- - -
## Installation
+ VirtualBox 를 기준으로
	+ 최신 버전을 다운받아 설치
+ [vagrantup.com](http://www.vagrantup.com/downloads.html) 에서 최신버전을 받아서 설치
- - -
## Getting Started
_ _ _
## Old method
	+ [http://www.vagrantbox.es/](http://www.vagrantbox.es/)에서 검색한다
	+ vagrant box add {title} {box url}
	+ vagrant init {title}
	+ vagrant up
_ _ _
## New method
	+ [Vagrant Cloud](https://vagrantcloud.com/)에서 검색한다
	+ vagrant init userName/boxName
	+ vagrant up

- - - 
## Distribution
+ repackage 를 이용하는 방법
+ Vagrant Cloud 를 이용하는 방법
+ VagrantFile 을 이용하는 방법

- - - 
## After Distribute - Box update
## Provisioning
	+ Available Scripts
		+ Shell Script
		+ Chef
		+ Puppet
- - -
## DEMO