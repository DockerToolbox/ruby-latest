FROM wolfsoftwareltd/rbenv-centos:8

RUN \
	VERSION=$(rbenv install -l | sed -n '/^[[:space:]]*[0-9]\{1,\}\.[0-9]\{1,\}\.[0-9]\{1,\}[[:space:]]*$/ h;${g;p;}') && \
	rbenv install ${VERSION} && \
	rbenv global ${VERSION}

WORKDIR /root

ENTRYPOINT ["/bin/bash"]

