AM_LIBADD = \
	$(PULSEAUDIO_LIBS) \
	$(HYBRIS_LIBS)
AM_CFLAGS = \
	$(DROID_DEVICE_CFLAGS) \
	$(PULSEAUDIO_CFLAGS) \
	$(DROIDHEADERS_CFLAGS) \
	$(HYBRIS_CFLAGS) \
	-DPULSEAUDIO_VERSION=@PA_MAJOR@ \
	-I$(top_srcdir)/src/common


modlibexec_LTLIBRARIES = libdroid-util.la

libdroid_util_la_SOURCES = droid-util.c droid-util.h
libdroid_util_la_LDFLAGS = -avoid-version -Wl,-no-undefined -Wl,-z,noexecstack -lhybris-common
libdroid_util_la_LIBADD = $(AM_LIBADD)
libdroid_util_la_CFLAGS = $(AM_CFLAGS)
