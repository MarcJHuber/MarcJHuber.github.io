NOW=$(shell date +"%Y-%m-%dT%H:%M:%S%:z")
TARBALL="https://api.github.com/repos/MarcJHuber/event-driven-servers/tarball/master"

all:
	@wget -q -O - $(TARBALL) | tar --strip-components=1 -xzp && make

