FROM centos:7.9.2009
RUN yum install sudo \ 
		vim \
 		iproute \
	 	net-tools \
		openssh-server \
		openssh-clients \
		git \
		mlocate \
		gcc \
         	make \
                epel-release \
		libmpc.x86_64 \
		java-11-openjdk.x86_64 -y
RUN yum install ninja-build -y
RUN useradd -ms /bin/bash oushu
RUN echo "oushu:909970" |chpasswd
RUN usermod -aG wheel oushu
USER oushu
WORKDIR /home/oushu
