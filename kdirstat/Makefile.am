
# Makefile.am for kdirstat/kdirstat
#
# Initially generated by KDevelop, cleaned up by <sh@suse.de>

SUBDIRS		= pics

bin_PROGRAMS 	= kdirstat
bin_SCRIPTS	= kdirstat-cache-writer


kdirstat_SOURCES =				\
	kdirstatmain.cpp			\
	kdirstatapp.cpp				\
	kdirstatfeedback.cpp			\
	kfeedback.cpp				\
	kdirtreeview.cpp			\
	kdirtreeiterators.cpp			\
	kdirtree.cpp				\
	kfileinfo.cpp				\
	kdirinfo.cpp				\
	kdirreadjob.cpp				\
	kdirtreecache.cpp			\
	kexcluderules.cpp			\
	ktreemapview.cpp			\
	ktreemaptile.cpp			\
	kcleanup.cpp				\
	kstdcleanup.cpp 			\
	kcleanupcollection.cpp			\
	kdirstatsettings.cpp			\
	kdirsaver.cpp				\
	kactivitytracker.cpp			\
	kpacman.cpp


noinst_HEADERS =				\
	kdirstatapp.h				\
	kfeedback.h				\
	kdirtreeview.h				\
	kdirtreeiterators.h			\
	kdirtree.h				\
	kfileinfo.h				\
	kdirinfo.h				\
	kdirreadjob.h				\
	kdirtreecache.h				\
	kexcluderules.h				\
	ktreemapview.h				\
	ktreemaptile.h				\
	kcleanup.h				\
	kstdcleanup.h				\
	kcleanupcollection.h			\
	kdirstatsettings.h			\
	kdirsaver.h				\
	kactivitytracker.h			\
	kpacman.h


EXTRA_DIST =					\
	kdirstatui.rc				\
	kdirstat.desktop			\
	lo32-app-kdirstat.png			\
	lo16-app-kdirstat.png			\
	hi32-app-kdirstat.png			\
	hi16-app-kdirstat.png


updatedir	= $(kde_datadir)/kconf_update
update_DATA	= kdirstat.upd
update_SCRIPTS	= fix_move_to_trash_bin.pl

kdirstat_LDADD	= $(LIB_KFILE) $(LIBZ)
kdirstat_CXXFLAGS = $(KDE_INCLUDES)

KDE_ICON = kdirstat

applnkdir = $(kde_appsdir)/Utilities
applnk_DATA = kdirstat.desktop


# set the include path for X, qt and KDE
INCLUDES= $(all_includes)

METASOURCES = AUTO

# the library search path.
kdirstat_LDFLAGS = $(all_libraries) $(KDE_RPATH)

rcdir = $(kde_datadir)/kdirstat
rc_DATA = kdirstatui.rc

messages: rc.cpp
	LIST=`find . -name \*.h -o -name \*.hh -o -name \*.H -o -name \*.hxx -o -name \*.hpp -o -name \*.cpp -o -name \*.cc -o -name \*.cxx -o -name \*.ecpp -o -name \*.C`; \
	if test -n "$$LIST"; then \
	 $(XGETTEXT) $$LIST -o $(podir)/kdirstat.pot; \
	fi

