ACLOCAL_AMFLAGS = -I libltdl/m4

SUBDIRS = libltdl src bindings

INCLUDES = $(LTDLINCL)

EXTRA_DIST = version-gen.sh

#if BUILD_PLUGIN_PYTHON
python_PYTHON = contrib/cephtool.py
#endif

install-exec-hook:
	$(mkinstalldirs) $(DESTDIR)$(localstatedir)/run
	$(mkinstalldirs) $(DESTDIR)$(localstatedir)/lib/$(PACKAGE_NAME)
	$(mkinstalldirs) $(DESTDIR)$(localstatedir)/log
