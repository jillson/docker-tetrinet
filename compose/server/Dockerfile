FROM fedora:latest

RUN groupadd -r gtserver \
    && useradd -r -g gtserver gtserver

# add the rpmfusion free repo (but not the unfree one)
#RUN dnf -y install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm 

# install gtetrinet (and way too much else because they didn't split it into server and client pieces)
RUN dnf install -y tetrinetx

ENV HOSTNAME=localhost.localdomain

USER gtserver

WORKDIR /home/gtserver

EXPOSE 31457

CMD ["/bin/bash","-c","tetrinetx && while :; do sleep 2; done"]