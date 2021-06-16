# VARIABLES
SHELL = /bin/sh
NAME = dmscripts

PREFIX ?= /usr
SCRIPTS := $(wildcard ./scripts/*)


build: 
	@echo "Done"



install:
	echo $(DESTDIR)$(MANPREFIX)
	install -Dm 775 $(SCRIPTS) -t $(DESTDIR)$(PREFIX)/bin/
	install -Dm644 LICENSE "$(DESTDIR)$(PREFIX)/share/licenses/$(NAME)/LICENSE"
	install -Dm644 README.md "$(DESTDIR)$(PREFIX)/share/doc/$(NAME)/README.md"
	install -Dm644 config/config "$(DESTDIR)/etc/dmscripts/config"

clean:
	@echo "done"

.PHONY: clean build install


