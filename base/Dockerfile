FROM centos

RUN yum update -y
RUN yum install -y wget &&  wget --no-cookies \
	 --no-check-certificate \
	--header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" \
	 "http://download.oracle.com/otn-pub/java/jdk/8u161-b12/2f38c3b165be4555a1fa6e98c45e0808/jdk-8u161-linux-x64.rpm" \
	-O jdk8-linux-x64.rpm

RUN rpm -ivh jdk8-linux-x64.rpm && rm jdk8-linux-x64.rpm
