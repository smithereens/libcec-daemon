AUTOMAKE_OPTIONS = subdir-objects
ACLOCAL_AMFLAGS = -I m4

bin_PROGRAMS = libcec-daemon
libcec_daemon_SOURCES = src/accumulator.hpp \
                        src/hdmi.cpp \
                        src/hdmi.h \
                        src/libcec.cpp \
                        src/libcec.h \
                        src/main.cpp \
                        src/main.h \
                        src/uinput.cpp \
                        src/uinput.h

dist_noinst_SCRIPTS = bootstrap

dist_bin_SCRIPTS = share/mythbuntu/bin/myth-control \
                   share/mythbuntu/bin/myth-status

udevdir= $(sysconfdir)/udev/rules.d
dist_udev_DATA = share/mythbuntu/udev/libcec-daemon.rules \
                 share/mythbuntu/udev/pulse-eight-hdmi-cec-usb.rules

upstartdir= $(sysconfdir)/init
dist_upstart_SCRIPTS = share/mythbuntu/upstart/hdmi-cec-activate.conf \
                       share/mythbuntu/upstart/hdmi-cec-deactivate.conf \
                       share/mythbuntu/upstart/hdmi-cec-standby.conf \
                       share/mythbuntu/upstart/libcec-daemon.conf

dist_doc_DATA = LICENCE README.md
