```
./configure --help
`configure' configures Bitcoin Core 0.19.0 to adapt to many kinds of systems.

Usage: ./configure [OPTION]... [VAR=VALUE]...

To assign environment variables (e.g., CC, CFLAGS...), specify them as
VAR=VALUE.  See below for descriptions of some of the useful variables.

Defaults for the options are specified in brackets.

Configuration:
  -h, --help              display this help and exit
      --help=short        display options specific to this package
      --help=recursive    display the short help of all the included packages
  -V, --version           display version information and exit
  -q, --quiet, --silent   do not print `checking ...' messages
      --cache-file=FILE   cache test results in FILE [disabled]
  -C, --config-cache      alias for `--cache-file=config.cache'
  -n, --no-create         do not create output files
      --srcdir=DIR        find the sources in DIR [configure dir or `..']

Installation directories:
  --prefix=PREFIX         install architecture-independent files in PREFIX
                          [/usr/local]
  --exec-prefix=EPREFIX   install architecture-dependent files in EPREFIX
                          [PREFIX]

By default, `make install' will install all the files in
`/usr/local/bin', `/usr/local/lib' etc.  You can specify
an installation prefix other than `/usr/local' using `--prefix',
for instance `--prefix=$HOME'.

For better control, use the options below.

Fine tuning of the installation directories:
  --bindir=DIR            user executables [EPREFIX/bin]
  --sbindir=DIR           system admin executables [EPREFIX/sbin]
  --libexecdir=DIR        program executables [EPREFIX/libexec]
  --sysconfdir=DIR        read-only single-machine data [PREFIX/etc]
  --sharedstatedir=DIR    modifiable architecture-independent data [PREFIX/com]
  --localstatedir=DIR     modifiable single-machine data [PREFIX/var]
  --runstatedir=DIR       modifiable per-process data [LOCALSTATEDIR/run]
  --libdir=DIR            object code libraries [EPREFIX/lib]
  --includedir=DIR        C header files [PREFIX/include]
  --oldincludedir=DIR     C header files for non-gcc [/usr/include]
  --datarootdir=DIR       read-only arch.-independent data root [PREFIX/share]
  --datadir=DIR           read-only architecture-independent data [DATAROOTDIR]
  --infodir=DIR           info documentation [DATAROOTDIR/info]
  --localedir=DIR         locale-dependent data [DATAROOTDIR/locale]
  --mandir=DIR            man documentation [DATAROOTDIR/man]
  --docdir=DIR            documentation root [DATAROOTDIR/doc/bitcoin]
  --htmldir=DIR           html documentation [DOCDIR]
  --dvidir=DIR            dvi documentation [DOCDIR]
  --pdfdir=DIR            pdf documentation [DOCDIR]
  --psdir=DIR             ps documentation [DOCDIR]

Program names:
  --program-prefix=PREFIX            prepend PREFIX to installed program names
  --program-suffix=SUFFIX            append SUFFIX to installed program names
  --program-transform-name=PROGRAM   run sed PROGRAM on installed program names

System types:
  --build=BUILD     configure for building on BUILD [guessed]
  --host=HOST       cross-compile to build programs to run on HOST [BUILD]

Optional Features:
  --disable-option-checking  ignore unrecognized --enable/--with options
  --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
  --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
  --enable-silent-rules   less verbose build output (undo: "make V=1")
  --disable-silent-rules  verbose build output (undo: "make V=0")
  --disable-maintainer-mode
                          disable make rules and dependencies not useful (and
                          sometimes confusing) to the casual installer
  --enable-dependency-tracking
                          do not reject slow dependency extractors
  --disable-dependency-tracking
                          speeds up one-time build
  --enable-shared[=PKGS]  build shared libraries [default=yes]
  --enable-static[=PKGS]  build static libraries [default=yes]
  --enable-fast-install[=PKGS]
                          optimize for fast installation [default=yes]
  --disable-libtool-lock  avoid locking (might break parallel builds)
  --disable-wallet        disable wallet (enabled by default)
  --enable-upnp-default   if UPNP is enabled, turn it on at startup (default
                          is no)
  --disable-tests         do not compile tests (default is to compile)
  --disable-gui-tests     do not compile GUI tests (default is to compile if
                          GUI and tests enabled)
  --disable-bench         do not compile benchmarks (default is to compile)
  --enable-extended-functional-tests
                          enable expensive functional tests when using lcov
                          (default no)
  --enable-fuzz           enable building of fuzz targets (default no).
                          enabling this will disable all other targets
  --disable-hardening     do not attempt to harden the resulting executables
                          (default is to harden when possible)
  --enable-reduce-exports attempt to reduce exported symbols in the resulting
                          executables (default is no)
  --disable-ccache        do not use ccache for building (default is to use if
                          found)
  --enable-lcov           enable lcov testing (default is no)
  --enable-lcov-branch-coverage
                          enable lcov testing branch coverage (default is no)
  --enable-glibc-back-compat
                          enable backwards compatibility with glibc
  --enable-threadlocal    enable features that depend on the c++ thread_local
                          keyword (currently just thread names in debug logs).
                          (default is to enabled if there is platform support
                          and glibc-back-compat is not enabled)
  --disable-asm           disable assembly routines (enabled by default)
  --disable-zmq           disable ZMQ notifications
  --enable-bip70          enable BIP70 (payment protocol) support in the GUI
                          (default is to disable)
  --disable-man           do not install man pages (default is to install)
  --enable-debug          use compiler flags and macros suited for debugging
                          (default is no)
  --enable-gprof          use gprof profiling compiler flags (default is no)
  --enable-werror         Treat certain compiler warnings as errors (default
                          is no)
  --enable-util-cli       build bitcoin-cli
  --enable-util-tx        build bitcoin-tx
  --enable-util-wallet    build bitcoin-wallet
  --disable-largefile     omit support for large files

Optional Packages:
  --with-PACKAGE[=ARG]    use PACKAGE [ARG=yes]
  --without-PACKAGE       do not use PACKAGE (same as --with-PACKAGE=no)
  --with-pic[=PKGS]       try to use only PIC/non-PIC objects [default=use
                          both]
  --with-aix-soname=aix|svr4|both
                          shared library versioning (aka "SONAME") variant to
                          provide on AIX, [default=aix].
  --with-gnu-ld           assume the C compiler uses GNU ld [default=no]
  --with-sysroot[=DIR]    Search for dependent libraries within DIR (or the
                          compiler's sysroot if not specified).
  --with-miniupnpc        enable UPNP (default is yes if libminiupnpc is
                          found)
  --with-rapidcheck       enable RapidCheck property-based tests (default is
                          yes if librapidcheck is found)
  --with-qrencode         enable QR code support (default is yes if qt is
                          enabled and libqrencode is found)
  --with-system-univalue  Build with system UniValue (default is no)
  --with-protoc-bindir=BIN_DIR
                          specify protoc bin path
  --with-sanitizers       comma separated list of extra sanitizers to build
                          with (default is none enabled)
  --with-utils            build bitcoin-cli bitcoin-tx bitcoin-wallet
                          (default=yes)
  --with-libs             build libraries (default=yes)
  --with-daemon           build bitcoind daemon (default=yes)
  --with-gui[=no|qt5|auto]
                          build bitcoin-qt GUI (default=auto)
  --with-qt-incdir=INC_DIR
                          specify qt include path (overridden by pkgconfig)
  --with-qt-libdir=LIB_DIR
                          specify qt lib path (overridden by pkgconfig)
  --with-qt-plugindir=PLUGIN_DIR
                          specify qt plugin path (overridden by pkgconfig)
  --with-qt-translationdir=PLUGIN_DIR
                          specify qt translation path (overridden by
                          pkgconfig)
  --with-qt-bindir=BIN_DIR
                          specify qt bin path
  --with-qtdbus           enable DBus support (default is yes if qt is enabled
                          and QtDBus is found)
  --with-incompatible-bdb allow using a bdb version other than 4.8
  --with-boost[=ARG]      use Boost library from a standard location
                          (ARG=yes), from the specified location (ARG=<path>),
                          or disable it (ARG=no) [ARG=yes]
  --with-boost-libdir=LIB_DIR
                          Force given directory for boost libraries. Note that
                          this will override library path detection, so use
                          this parameter only if default library detection
                          fails and you know exactly where your boost
                          libraries are located.
  --with-boost-system[=special-lib]
                          use the System library from boost - it is possible
                          to specify a certain library for the linker e.g.
                          --with-boost-system=boost_system-gcc-mt
  --with-boost-filesystem[=special-lib]
                          use the Filesystem library from boost - it is
                          possible to specify a certain library for the linker
                          e.g. --with-boost-filesystem=boost_filesystem-gcc-mt
  --with-boost-thread[=special-lib]
                          use the Thread library from boost - it is possible
                          to specify a certain library for the linker e.g.
                          --with-boost-thread=boost_thread-gcc-mt
  --with-boost-chrono[=special-lib]
                          use the Chrono library from boost - it is possible
                          to specify a certain library for the linker e.g.
                          --with-boost-chrono=boost_chrono-gcc-mt
  --with-boost-unit-test-framework[=special-lib]
                          use the Unit_Test_Framework library from boost - it
                          is possible to specify a certain library for the
                          linker e.g.
                          --with-boost-unit-test-framework=boost_unit_test_framework-gcc

Some influential environment variables:
  ARFLAGS     Flags for the archiver, defaults to <cr> if not set
  CXX         C++ compiler command
  CXXFLAGS    C++ compiler flags
  LDFLAGS     linker flags, e.g. -L<lib dir> if you have libraries in a
              nonstandard directory <lib dir>
  LIBS        libraries to pass to the linker, e.g. -l<library>
  CPPFLAGS    (Objective) C/C++ preprocessor flags, e.g. -I<include dir> if
              you have headers in a nonstandard directory <include dir>
  OBJCXX      Objective C++ compiler command
  OBJCXXFLAGS Objective C++ compiler flags
  CC          C compiler command
  CFLAGS      C compiler flags
  LT_SYS_LIBRARY_PATH
              User-defined run-time library search path.
  CPP         C preprocessor
  CXXCPP      C++ preprocessor
  PYTHONPATH  Augments the default search path for python module files
  PKG_CONFIG  path to pkg-config utility
  PKG_CONFIG_PATH
              directories to add to pkg-config's search path
  PKG_CONFIG_LIBDIR
              path overriding pkg-config's built-in search path
  QT5_CFLAGS  C compiler flags for QT5, overriding pkg-config
  QT5_LIBS    linker flags for QT5, overriding pkg-config
  QT_TEST_CFLAGS
              C compiler flags for QT_TEST, overriding pkg-config
  QT_TEST_LIBS
              linker flags for QT_TEST, overriding pkg-config
  QT_DBUS_CFLAGS
              C compiler flags for QT_DBUS, overriding pkg-config
  QT_DBUS_LIBS
              linker flags for QT_DBUS, overriding pkg-config
  QTPLATFORM_CFLAGS
              C compiler flags for QTPLATFORM, overriding pkg-config
  QTPLATFORM_LIBS
              linker flags for QTPLATFORM, overriding pkg-config
  QTFONTDATABASE_CFLAGS
              C compiler flags for QTFONTDATABASE, overriding pkg-config
  QTFONTDATABASE_LIBS
              linker flags for QTFONTDATABASE, overriding pkg-config
  QTEVENTDISPATCHER_CFLAGS
              C compiler flags for QTEVENTDISPATCHER, overriding pkg-config
  QTEVENTDISPATCHER_LIBS
              linker flags for QTEVENTDISPATCHER, overriding pkg-config
  QTTHEME_CFLAGS
              C compiler flags for QTTHEME, overriding pkg-config
  QTTHEME_LIBS
              linker flags for QTTHEME, overriding pkg-config
  QTDEVICEDISCOVERY_CFLAGS
              C compiler flags for QTDEVICEDISCOVERY, overriding pkg-config
  QTDEVICEDISCOVERY_LIBS
              linker flags for QTDEVICEDISCOVERY, overriding pkg-config
  QTACCESSIBILITY_CFLAGS
              C compiler flags for QTACCESSIBILITY, overriding pkg-config
  QTACCESSIBILITY_LIBS
              linker flags for QTACCESSIBILITY, overriding pkg-config
  QTFB_CFLAGS C compiler flags for QTFB, overriding pkg-config
  QTFB_LIBS   linker flags for QTFB, overriding pkg-config
  QTXCBQPA_CFLAGS
              C compiler flags for QTXCBQPA, overriding pkg-config
  QTXCBQPA_LIBS
              linker flags for QTXCBQPA, overriding pkg-config
  QTCLIPBOARD_CFLAGS
              C compiler flags for QTCLIPBOARD, overriding pkg-config
  QTCLIPBOARD_LIBS
              linker flags for QTCLIPBOARD, overriding pkg-config
  QTGRAPHICS_CFLAGS
              C compiler flags for QTGRAPHICS, overriding pkg-config
  QTGRAPHICS_LIBS
              linker flags for QTGRAPHICS, overriding pkg-config
  QTCGL_CFLAGS
              C compiler flags for QTCGL, overriding pkg-config
  QTCGL_LIBS  linker flags for QTCGL, overriding pkg-config
  BDB_CFLAGS  C compiler flags for BerkeleyDB, bypasses autodetection
  BDB_LIBS    Linker flags for BerkeleyDB, bypasses autodetection
  SSL_CFLAGS  C compiler flags for SSL, overriding pkg-config
  SSL_LIBS    linker flags for SSL, overriding pkg-config
  CRYPTO_CFLAGS
              C compiler flags for CRYPTO, overriding pkg-config
  CRYPTO_LIBS linker flags for CRYPTO, overriding pkg-config
  PROTOBUF_CFLAGS
              C compiler flags for PROTOBUF, overriding pkg-config
  PROTOBUF_LIBS
              linker flags for PROTOBUF, overriding pkg-config
  QR_CFLAGS   C compiler flags for QR, overriding pkg-config
  QR_LIBS     linker flags for QR, overriding pkg-config
  EVENT_CFLAGS
              C compiler flags for EVENT, overriding pkg-config
  EVENT_LIBS  linker flags for EVENT, overriding pkg-config
  EVENT_PTHREADS_CFLAGS
              C compiler flags for EVENT_PTHREADS, overriding pkg-config
  EVENT_PTHREADS_LIBS
              linker flags for EVENT_PTHREADS, overriding pkg-config
  ZMQ_CFLAGS  C compiler flags for ZMQ, overriding pkg-config
  ZMQ_LIBS    linker flags for ZMQ, overriding pkg-config
  UNIVALUE_CFLAGS
              C compiler flags for UNIVALUE, overriding pkg-config
  UNIVALUE_LIBS
              linker flags for UNIVALUE, overriding pkg-config

Use these variables to override the choices made by `configure' or to help
it to find libraries and programs with nonstandard names/locations.

Report bugs to <https://github.com/bitcoin/bitcoin/issues>.
Bitcoin Core home page: <https://bitcoincore.org/>.
```
