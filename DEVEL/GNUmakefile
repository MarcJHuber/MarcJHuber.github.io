NOW=$(shell date +"%Y-%m-%dT%H:%M:%S%:z")
TARBALL="https://api.github.com/repos/MarcJHuber/event-driven-servers/tarball/master"

all:
	@wget -q -O - $(TARBALL) | tar --strip-components=1 -xzp \
	&& mkdir -p .git/refs/heads ; touch .git/index \
	&& echo "#define VERSION \"${NOW} (GIT archive)\"" > misc/version.h \
	&& make

