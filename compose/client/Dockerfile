FROM jumanjiman/xrdp:latest

# add the rpmfusion free repo (but not the unfree one)
RUN dnf -y install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm 

# install gtetrinet (and way too much else because reasons)
RUN dnf install -y gtetrinet

# TODO: drop gtetrinet icon on foo's desktop or start it?