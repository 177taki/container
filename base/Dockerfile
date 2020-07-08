FROM ubuntu:20.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update \
&&	apt-get upgrade -y \
&&	apt-get install -y \
			iputils-ping \
			wget \
			curl \
			openssh-client \
			openssh-server \
			git \
			software-properties-common \
&&	apt-add-repository ppa:fish-shell/release-3 \
&&	apt-get update \
&&	apt-get install -y fish	

WORKDIR /lagom

CMD ["/bin/bash"]
