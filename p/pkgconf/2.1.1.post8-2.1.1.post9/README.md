# Comparing `tmp/pkgconf-2.1.1.post8.tar.gz` & `tmp/pkgconf-2.1.1.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgconf-2.1.1.post8.tar", last modified: Thu May 30 23:06:30 2024, max compression
+gzip compressed data, was "pkgconf-2.1.1.post9.tar", last modified: Sun Jun  2 01:49:05 2024, max compression
```

## Comparing `pkgconf-2.1.1.post8.tar` & `pkgconf-2.1.1.post9.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     1966 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/.github/workflows/build.yml
--rw-r--r--   0        0        0      526 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/.github/workflows/test.yml
--rw-r--r--   0        0        0      108 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/.gitmodules
--rw-r--r--   0        0        0     1695 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      214 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/.readthedocs.yaml
--rw-r--r--   0        0        0     1083 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/LICENSE
--rw-r--r--   0        0        0     1507 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/README.md
--rw-r--r--   0        0        0      421 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/docs/conf.py
--rw-r--r--   0        0        0     1956 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/docs/index.rst
--rw-r--r--   0        0        0      308 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/environment.yml
--rw-r--r--   0        0        0       53 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/examples/header-only-library/example/include/example.h
--rw-r--r--   0        0        0      148 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/examples/header-only-library/example/pkgconf/example.pc
--rw-r--r--   0        0        0      240 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/examples/header-only-library/pyproject.toml
--rw-r--r--   0        0        0     1025 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/meson.build
--rw-r--r--   0        0        0     2551 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/pyproject.toml
--rw-r--r--   0        0        0     1802 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/src/buildhack.py
--rw-r--r--   0        0        0     2918 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/src/pkgconf/__init__.py
--rw-r--r--   0        0        0     2331 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/src/pkgconf/__main__.py
--rw-r--r--   0        0        0      646 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/src/pkgconf/diagnose.py
--rw-r--r--   0        0        0       39 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/.gitattributes
--rw-r--r--   0        0        0       51 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/.github/FUNDING.yml
--rw-r--r--   0        0        0     3324 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/.github/workflows/test.yml
--rw-r--r--   0        0        0      836 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/.gitignore
--rw-r--r--   0        0        0       69 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/.mailmap
--rw-r--r--   0        0        0     1633 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/.woodpecker.yml
--rw-r--r--   0        0        0     1498 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/AUTHORS
--rw-r--r--   0        0        0     1051 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      509 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/COPYING
--rw-r--r--   0        0        0       60 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/Kyuafile.in
--rw-r--r--   0        0        0     6005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/Makefile.am
--rw-r--r--   0        0        0     2442 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/Makefile.lite
--rw-r--r--   0        0        0    26691 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/NEWS
--rw-r--r--   0        0        0     6599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/README.md
--rwxr-xr-x   0        0        0     1543 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/autogen.sh
--rw-r--r--   0        0        0     9641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/cli/bomtool/main.c
--rw-r--r--   0        0        0    17983 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/cli/getopt_long.c
--rw-r--r--   0        0        0     2645 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/cli/getopt_long.h
--rw-r--r--   0        0        0    46893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/cli/main.c
--rw-r--r--   0        0        0     3354 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/cli/renderer-msvc.c
--rw-r--r--   0        0        0      687 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/cli/renderer-msvc.h
--rw-r--r--   0        0        0     2488 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/configure.ac
--rw-r--r--   0        0        0     9790 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/conf.py
--rw-r--r--   0        0        0     5641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/extract.py
--rw-r--r--   0        0        0      136 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/index.rst
--rw-r--r--   0        0        0      709 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst
--rw-r--r--   0        0        0     1453 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-audit.rst
--rw-r--r--   0        0        0     1796 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-cache.rst
--rw-r--r--   0        0        0     9972 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-client.rst
--rw-r--r--   0        0        0     4395 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-dependency.rst
--rw-r--r--   0        0        0     5951 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-fragment.rst
--rw-r--r--   0        0        0     2936 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-path.rst
--rw-r--r--   0        0        0      758 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-personality.rst
--rw-r--r--   0        0        0     8183 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-pkg.rst
--rw-r--r--   0        0        0     4361 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-queue.rst
--rw-r--r--   0        0        0     3890 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-tuple.rst
--rw-r--r--   0        0        0      375 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf.rst
--rw-r--r--   0        0        0     3070 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/argvsplit.c
--rw-r--r--   0        0        0     2893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/audit.c
--rw-r--r--   0        0        0     3959 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/bsdstubs.c
--rw-r--r--   0        0        0     1076 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/bsdstubs.h
--rw-r--r--   0        0        0     5693 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/cache.c
--rw-r--r--   0        0        0    20527 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/client.c
--rw-r--r--   0        0        0     1883 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/config.h.meson
--rw-r--r--   0        0        0    14306 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/dependency.c
--rw-r--r--   0        0        0     1953 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/fileio.c
--rw-r--r--   0        0        0    19221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/fragment.c
--rw-r--r--   0        0        0     2016 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/iter.h
--rw-r--r--   0        0        0      599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/libpkgconf-api.h
--rw-r--r--   0        0        0    18850 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/libpkgconf.h
--rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/meson.build
--rw-r--r--   0        0        0     2945 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/parser.c
--rw-r--r--   0        0        0     8949 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/path.c
--rw-r--r--   0        0        0     9610 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/personality.c
--rw-r--r--   0        0        0    53445 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/pkg.c
--rw-r--r--   0        0        0    12364 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/queue.c
--rw-r--r--   0        0        0     1612 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/stdinc.h
--rw-r--r--   0        0        0    12752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/tuple.c
--rw-r--r--   0        0        0    23014 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/win-dirent.h
--rw-r--r--   0        0        0      339 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf.pc.in
--rw-r--r--   0        0        0     2104 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/m4/ax_check_compile_flag.m4
--rw-r--r--   0        0        0     5980 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/man/pc.5
--rw-r--r--   0        0        0     4005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/man/pkg.m4.7
--rw-r--r--   0        0        0     3417 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/man/pkgconf-personality.5
--rw-r--r--   0        0        0     7702 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/man/pkgconf.1
--rw-r--r--   0        0        0     4495 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/meson.build
--rw-r--r--   0        0        0      412 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/meson_options.txt
--rw-r--r--   0        0        0    12735 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/pkg.m4
--rw-r--r--   0        0        0      334 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/Kyuafile.in
--rwxr-xr-x   0        0        0     6956 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/basic.sh
--rwxr-xr-x   0        0        0     1242 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/builtins.sh
--rwxr-xr-x   0        0        0      388 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/conflicts.sh
--rwxr-xr-x   0        0        0      477 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/framework.sh
--rw-r--r--   0        0        0      237 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib-relocatable/lib/pkgconfig/foo.pc
--rw-r--r--   0        0        0      209 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/argv-parse-2.pc
--rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/argv-parse-3.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/argv-parse.pc
--rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/bar.pc
--rw-r--r--   0        0        0      253 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/baz.pc
--rw-r--r--   0        0        0      566 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/billion-laughs.pc
--rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/case-sensitivity.pc
--rw-r--r--   0        0        0      196 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/cflags-internal.pc
--rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/cflags-libs-only.pc
--rw-r--r--   0        0        0      146 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/cflags-whitespace-trailing.pc
--rw-r--r--   0        0        0      142 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/cflags-whitespace.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/circular-1.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/circular-2.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/circular-3.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/comments-in-fields.pc
--rw-r--r--   0        0        0      122 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/comments.pc
--rw-r--r--   0        0        0      248 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/conflicts.pc
--rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/depgraph-break.pc
--rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/dos-lineendings.pc
--rw-r--r--   0        0        0       84 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/empty-tuple.pc
--rw-r--r--   0        0        0      107 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/escaped-backslash.pc
--rw-r--r--   0        0        0      163 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/explicit-sysroot.pc
--rw-r--r--   0        0        0      229 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/flag-order-1.pc
--rw-r--r--   0        0        0      244 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/flag-order-3.pc
--rw-r--r--   0        0        0      250 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/foo.pc
--rw-r--r--   0        0        0      262 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/foobar.pc
--rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-collision-1.pc
--rw-r--r--   0        0        0       98 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-collision-2.pc
--rw-r--r--   0        0        0      170 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-collision-intermediary.pc
--rw-r--r--   0        0        0      199 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-collision.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-comment.pc
--rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-escaping-1.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-escaping-2.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-escaping-3.pc
--rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-quoting-2.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-quoting-3.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-quoting-5.pc
--rw-r--r--   0        0        0      168 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-quoting-7.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/fragment-quoting.pc
--rw-r--r--   0        0        0      195 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/framework-1.pc
--rw-r--r--   0        0        0      217 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/framework-2.pc
--rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/idirafter-ordering.pc
--rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/idirafter.pc
--rw-r--r--   0        0        0      114 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/incomplete.pc
--rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/intermediary-1.pc
--rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/intermediary-2.pc
--rw-r--r--   0        0        0      235 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/isystem.pc
--rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/malformed-1.pc
--rw-r--r--   0        0        0       70 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/malformed-quoting.pc
--rw-r--r--   0        0        0       95 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/malformed-version.pc
--rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/metapackage-1.pc
--rw-r--r--   0        0        0      126 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/metapackage-2.pc
--rw-r--r--   0        0        0      101 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/metapackage-3.pc
--rw-r--r--   0        0        0      116 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/metapackage.pc
--rw-r--r--   0        0        0      246 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/missing-require.pc
--rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/multiline-bogus.pc
--rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/multiline.pc
--rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/no-trailing-newline.pc
--rw-r--r--   0        0        0      174 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/nocflag.pc
--rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/nolib.pc
--rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/omg-sysroot-uninstalled.pc
--rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/omg-uninstalled.pc
--rw-r--r--   0        0        0      187 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/orphaned-requires-private.pc
--rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/paren-quoting.pc
--rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/prefix-foo1.pc
--rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/prefix-foo2.pc
--rw-r--r--   0        0        0      117 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/private-libs-duplication.pc
--rw-r--r--   0        0        0      151 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/provides-request-simple.pc
--rw-r--r--   0        0        0      284 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/provides.pc
--rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/quotes.pc
--rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/requires-internal-2.pc
--rw-r--r--   0        0        0      239 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/requires-internal-collision.pc
--rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/requires-internal-missing.pc
--rw-r--r--   0        0        0      223 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/requires-internal.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/spaces-in-paths.pc
--rw-r--r--   0        0        0      225 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/static-archive-libs.pc
--rw-r--r--   0        0        0      254 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/static-libs.pc
--rw-r--r--   0        0        0      188 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/sysroot-dir-2.pc
--rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/sysroot-dir-3.pc
--rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/sysroot-dir-4.pc
--rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/sysroot-dir-5.pc
--rw-r--r--   0        0        0      157 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/sysroot-dir.pc
--rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/tilde-quoting.pc
--rw-r--r--   0        0        0      255 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/tilde.pc
--rw-r--r--   0        0        0      131 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/tuple-quoting.pc
--rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/typelibdir.pc
--rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/unavailable-provider.pc
--rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/utf8.pc
--rw-r--r--   0        0        0      245 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/variable-whitespace.pc
--rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib2/foo.pc
--rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib3/bar.pc
--rw-r--r--   0        0        0      428 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/meson.build
--rwxr-xr-x   0        0        0     6752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/parser.sh
--rwxr-xr-x   0        0        0     6416 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/provides.sh
--rwxr-xr-x   0        0        0     7643 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/regress.sh
--rwxr-xr-x   0        0        0     3083 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/requires.sh
--rwxr-xr-x   0        0        0     2341 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/sysroot.sh
--rw-r--r--   0        0        0     1197 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/test_env.sh.in
--rwxr-xr-x   0        0        0      600 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post8/subprojects/pkgconf/tests/version.sh
--rw-r--r--   0        0        0      822 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/conftest.py
--rw-r--r--   0        0        0       74 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/data/needs-example-lib.c
--rw-r--r--   0        0        0       20 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/namespace/example/example.pc
--rw-r--r--   0        0        0      232 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/namespace/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/register-pkg-config-path/example/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/register-pkg-config-path/example/pkgconf/__init__.py
--rw-r--r--   0        0        0       41 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/register-pkg-config-path/lib.c
--rw-r--r--   0        0        0       23 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/register-pkg-config-path/lib.h
--rw-r--r--   0        0        0      445 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/register-pkg-config-path/meson.build
--rw-r--r--   0        0        0      178 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/register-pkg-config-path/pyproject.toml
--rw-r--r--   0        0        0      244 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/packages/use-pybind11/meson.build
--rw-r--r--   0        0        0      727 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/test_distribution.py
--rw-r--r--   0        0        0     1074 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/test_entrypoints.py
--rw-r--r--   0        0        0      549 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/test_examples.py
--rw-r--r--   0        0        0     1369 2024-05-30 23:05:47.000000 pkgconf-2.1.1.post8/tests/test_python_module.py
--rw-r--r--   0        0        0     4274 2024-05-30 23:06:30.306291 pkgconf-2.1.1.post8/PKG-INFO
+-rw-r--r--   0        0        0     1966 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/.github/workflows/build.yml
+-rw-r--r--   0        0        0      762 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      108 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/.gitmodules
+-rw-r--r--   0        0        0     1817 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      214 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/.readthedocs.yaml
+-rw-r--r--   0        0        0     1083 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/LICENSE
+-rw-r--r--   0        0        0     1507 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/README.md
+-rw-r--r--   0        0        0      421 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/docs/conf.py
+-rw-r--r--   0        0        0     1956 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/docs/index.rst
+-rw-r--r--   0        0        0      308 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/environment.yml
+-rw-r--r--   0        0        0       53 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/examples/header-only-library/example/include/example.h
+-rw-r--r--   0        0        0      148 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/examples/header-only-library/example/pkgconf/example.pc
+-rw-r--r--   0        0        0      240 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/examples/header-only-library/pyproject.toml
+-rw-r--r--   0        0        0     1025 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/meson.build
+-rw-r--r--   0        0        0     2671 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/pyproject.toml
+-rw-r--r--   0        0        0     1823 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/src/buildhack.py
+-rw-r--r--   0        0        0     3167 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/src/pkgconf/__init__.py
+-rw-r--r--   0        0        0     2366 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/src/pkgconf/__main__.py
+-rw-r--r--   0        0        0      609 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/src/pkgconf/diagnose.py
+-rw-r--r--   0        0        0       39 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/.gitattributes
+-rw-r--r--   0        0        0       51 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/.github/FUNDING.yml
+-rw-r--r--   0        0        0     3324 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/.github/workflows/test.yml
+-rw-r--r--   0        0        0      836 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/.gitignore
+-rw-r--r--   0        0        0       69 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/.mailmap
+-rw-r--r--   0        0        0     1633 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/.woodpecker.yml
+-rw-r--r--   0        0        0     1498 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/AUTHORS
+-rw-r--r--   0        0        0     1051 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      509 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/COPYING
+-rw-r--r--   0        0        0       60 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/Kyuafile.in
+-rw-r--r--   0        0        0     6005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/Makefile.am
+-rw-r--r--   0        0        0     2442 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/Makefile.lite
+-rw-r--r--   0        0        0    26691 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/NEWS
+-rw-r--r--   0        0        0     6599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/README.md
+-rwxr-xr-x   0        0        0     1543 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/autogen.sh
+-rw-r--r--   0        0        0     9641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/cli/bomtool/main.c
+-rw-r--r--   0        0        0    17983 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/cli/getopt_long.c
+-rw-r--r--   0        0        0     2645 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/cli/getopt_long.h
+-rw-r--r--   0        0        0    46893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/cli/main.c
+-rw-r--r--   0        0        0     3354 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/cli/renderer-msvc.c
+-rw-r--r--   0        0        0      687 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/cli/renderer-msvc.h
+-rw-r--r--   0        0        0     2488 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/configure.ac
+-rw-r--r--   0        0        0     9790 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/conf.py
+-rw-r--r--   0        0        0     5641 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/extract.py
+-rw-r--r--   0        0        0      136 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/index.rst
+-rw-r--r--   0        0        0      709 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst
+-rw-r--r--   0        0        0     1453 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-audit.rst
+-rw-r--r--   0        0        0     1796 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-cache.rst
+-rw-r--r--   0        0        0     9972 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-client.rst
+-rw-r--r--   0        0        0     4395 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-dependency.rst
+-rw-r--r--   0        0        0     5951 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-fragment.rst
+-rw-r--r--   0        0        0     2936 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-path.rst
+-rw-r--r--   0        0        0      758 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-personality.rst
+-rw-r--r--   0        0        0     8183 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-pkg.rst
+-rw-r--r--   0        0        0     4361 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-queue.rst
+-rw-r--r--   0        0        0     3890 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-tuple.rst
+-rw-r--r--   0        0        0      375 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf.rst
+-rw-r--r--   0        0        0     3070 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/argvsplit.c
+-rw-r--r--   0        0        0     2893 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/audit.c
+-rw-r--r--   0        0        0     3959 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/bsdstubs.c
+-rw-r--r--   0        0        0     1076 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/bsdstubs.h
+-rw-r--r--   0        0        0     5693 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/cache.c
+-rw-r--r--   0        0        0    20527 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/client.c
+-rw-r--r--   0        0        0     1883 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/config.h.meson
+-rw-r--r--   0        0        0    14306 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/dependency.c
+-rw-r--r--   0        0        0     1953 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/fileio.c
+-rw-r--r--   0        0        0    19221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/fragment.c
+-rw-r--r--   0        0        0     2016 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/iter.h
+-rw-r--r--   0        0        0      599 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/libpkgconf-api.h
+-rw-r--r--   0        0        0    18850 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/libpkgconf.h
+-rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/meson.build
+-rw-r--r--   0        0        0     2945 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/parser.c
+-rw-r--r--   0        0        0     8949 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/path.c
+-rw-r--r--   0        0        0     9610 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/personality.c
+-rw-r--r--   0        0        0    53445 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/pkg.c
+-rw-r--r--   0        0        0    12364 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/queue.c
+-rw-r--r--   0        0        0     1612 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/stdinc.h
+-rw-r--r--   0        0        0    12752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/tuple.c
+-rw-r--r--   0        0        0    23014 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/win-dirent.h
+-rw-r--r--   0        0        0      339 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf.pc.in
+-rw-r--r--   0        0        0     2104 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/m4/ax_check_compile_flag.m4
+-rw-r--r--   0        0        0     5980 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/man/pc.5
+-rw-r--r--   0        0        0     4005 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/man/pkg.m4.7
+-rw-r--r--   0        0        0     3417 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/man/pkgconf-personality.5
+-rw-r--r--   0        0        0     7702 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/man/pkgconf.1
+-rw-r--r--   0        0        0     4495 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/meson.build
+-rw-r--r--   0        0        0      412 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/meson_options.txt
+-rw-r--r--   0        0        0    12735 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/pkg.m4
+-rw-r--r--   0        0        0      334 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/Kyuafile.in
+-rwxr-xr-x   0        0        0     6956 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/basic.sh
+-rwxr-xr-x   0        0        0     1242 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/builtins.sh
+-rwxr-xr-x   0        0        0      388 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/conflicts.sh
+-rwxr-xr-x   0        0        0      477 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/framework.sh
+-rw-r--r--   0        0        0      237 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib-relocatable/lib/pkgconfig/foo.pc
+-rw-r--r--   0        0        0      209 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/argv-parse-2.pc
+-rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/argv-parse-3.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/argv-parse.pc
+-rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/bar.pc
+-rw-r--r--   0        0        0      253 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/baz.pc
+-rw-r--r--   0        0        0      566 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/billion-laughs.pc
+-rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/case-sensitivity.pc
+-rw-r--r--   0        0        0      196 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/cflags-internal.pc
+-rw-r--r--   0        0        0      221 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/cflags-libs-only.pc
+-rw-r--r--   0        0        0      146 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/cflags-whitespace-trailing.pc
+-rw-r--r--   0        0        0      142 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/cflags-whitespace.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/circular-1.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/circular-2.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/circular-3.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/comments-in-fields.pc
+-rw-r--r--   0        0        0      122 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/comments.pc
+-rw-r--r--   0        0        0      248 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/conflicts.pc
+-rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/depgraph-break.pc
+-rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/dos-lineendings.pc
+-rw-r--r--   0        0        0       84 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/empty-tuple.pc
+-rw-r--r--   0        0        0      107 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/escaped-backslash.pc
+-rw-r--r--   0        0        0      163 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/explicit-sysroot.pc
+-rw-r--r--   0        0        0      229 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/flag-order-1.pc
+-rw-r--r--   0        0        0      244 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/flag-order-3.pc
+-rw-r--r--   0        0        0      250 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/foo.pc
+-rw-r--r--   0        0        0      262 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/foobar.pc
+-rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-collision-1.pc
+-rw-r--r--   0        0        0       98 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-collision-2.pc
+-rw-r--r--   0        0        0      170 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-collision-intermediary.pc
+-rw-r--r--   0        0        0      199 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-collision.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-comment.pc
+-rw-r--r--   0        0        0      115 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-escaping-1.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-escaping-2.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-escaping-3.pc
+-rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-quoting-2.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-quoting-3.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-quoting-5.pc
+-rw-r--r--   0        0        0      168 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-quoting-7.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/fragment-quoting.pc
+-rw-r--r--   0        0        0      195 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/framework-1.pc
+-rw-r--r--   0        0        0      217 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/framework-2.pc
+-rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/idirafter-ordering.pc
+-rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/idirafter.pc
+-rw-r--r--   0        0        0      114 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/incomplete.pc
+-rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/intermediary-1.pc
+-rw-r--r--   0        0        0      210 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/intermediary-2.pc
+-rw-r--r--   0        0        0      235 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/isystem.pc
+-rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/malformed-1.pc
+-rw-r--r--   0        0        0       70 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/malformed-quoting.pc
+-rw-r--r--   0        0        0       95 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/malformed-version.pc
+-rw-r--r--   0        0        0      158 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/metapackage-1.pc
+-rw-r--r--   0        0        0      126 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/metapackage-2.pc
+-rw-r--r--   0        0        0      101 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/metapackage-3.pc
+-rw-r--r--   0        0        0      116 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/metapackage.pc
+-rw-r--r--   0        0        0      246 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/missing-require.pc
+-rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/multiline-bogus.pc
+-rw-r--r--   0        0        0      169 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/multiline.pc
+-rw-r--r--   0        0        0      270 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/no-trailing-newline.pc
+-rw-r--r--   0        0        0      174 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/nocflag.pc
+-rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/nolib.pc
+-rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/omg-sysroot-uninstalled.pc
+-rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/omg-uninstalled.pc
+-rw-r--r--   0        0        0      187 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/orphaned-requires-private.pc
+-rw-r--r--   0        0        0      120 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/paren-quoting.pc
+-rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/prefix-foo1.pc
+-rw-r--r--   0        0        0      257 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/prefix-foo2.pc
+-rw-r--r--   0        0        0      117 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/private-libs-duplication.pc
+-rw-r--r--   0        0        0      151 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/provides-request-simple.pc
+-rw-r--r--   0        0        0      284 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/provides.pc
+-rw-r--r--   0        0        0      259 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/quotes.pc
+-rw-r--r--   0        0        0      205 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/requires-internal-2.pc
+-rw-r--r--   0        0        0      239 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/requires-internal-collision.pc
+-rw-r--r--   0        0        0      232 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/requires-internal-missing.pc
+-rw-r--r--   0        0        0      223 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/requires-internal.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/spaces-in-paths.pc
+-rw-r--r--   0        0        0      225 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/static-archive-libs.pc
+-rw-r--r--   0        0        0      254 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/static-libs.pc
+-rw-r--r--   0        0        0      188 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/sysroot-dir-2.pc
+-rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/sysroot-dir-3.pc
+-rw-r--r--   0        0        0      230 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/sysroot-dir-4.pc
+-rw-r--r--   0        0        0      222 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/sysroot-dir-5.pc
+-rw-r--r--   0        0        0      157 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/sysroot-dir.pc
+-rw-r--r--   0        0        0       92 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/tilde-quoting.pc
+-rw-r--r--   0        0        0      255 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/tilde.pc
+-rw-r--r--   0        0        0      131 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/tuple-quoting.pc
+-rw-r--r--   0        0        0      206 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/typelibdir.pc
+-rw-r--r--   0        0        0      241 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/unavailable-provider.pc
+-rw-r--r--   0        0        0      212 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/utf8.pc
+-rw-r--r--   0        0        0      245 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/variable-whitespace.pc
+-rw-r--r--   0        0        0      208 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib2/foo.pc
+-rw-r--r--   0        0        0      184 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib3/bar.pc
+-rw-r--r--   0        0        0      428 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/meson.build
+-rwxr-xr-x   0        0        0     6752 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/parser.sh
+-rwxr-xr-x   0        0        0     6416 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/provides.sh
+-rwxr-xr-x   0        0        0     7643 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/regress.sh
+-rwxr-xr-x   0        0        0     3083 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/requires.sh
+-rwxr-xr-x   0        0        0     2341 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/sysroot.sh
+-rw-r--r--   0        0        0     1197 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/test_env.sh.in
+-rwxr-xr-x   0        0        0      600 2024-02-04 11:26:15.000000 pkgconf-2.1.1.post9/subprojects/pkgconf/tests/version.sh
+-rw-r--r--   0        0        0      912 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/conftest.py
+-rw-r--r--   0        0        0       74 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/data/needs-example-lib.c
+-rw-r--r--   0        0        0       20 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/namespace/example/example.pc
+-rw-r--r--   0        0        0      232 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/namespace/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/register-pkg-config-path/example/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/register-pkg-config-path/example/pkgconf/__init__.py
+-rw-r--r--   0        0        0       41 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/register-pkg-config-path/lib.c
+-rw-r--r--   0        0        0       23 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/register-pkg-config-path/lib.h
+-rw-r--r--   0        0        0      445 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/register-pkg-config-path/meson.build
+-rw-r--r--   0        0        0      178 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/register-pkg-config-path/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/packages/use-pybind11/meson.build
+-rw-r--r--   0        0        0      727 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/test_distribution.py
+-rw-r--r--   0        0        0     1074 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/test_entrypoints.py
+-rw-r--r--   0        0        0      549 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/test_examples.py
+-rw-r--r--   0        0        0     1369 2024-06-02 01:46:47.000000 pkgconf-2.1.1.post9/tests/test_python_module.py
+-rw-r--r--   0        0        0     4391 2024-06-02 01:49:05.446272 pkgconf-2.1.1.post9/PKG-INFO
```

### Comparing `pkgconf-2.1.1.post8/.github/workflows/build.yml` & `pkgconf-2.1.1.post9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/.pre-commit-config.yaml` & `pkgconf-2.1.1.post9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -51,7 +51,12 @@
       - id: python-check-mock-methods
       - id: python-no-eval
       - id: python-no-log-warn
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
       - id: text-unicode-replacement-char
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.15.2
+    hooks:
+    - id: pyupgrade
+      args: [--py38-plus]
```

### Comparing `pkgconf-2.1.1.post8/LICENSE` & `pkgconf-2.1.1.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/README.md` & `pkgconf-2.1.1.post9/README.md`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/docs/index.rst` & `pkgconf-2.1.1.post9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/meson.build` & `pkgconf-2.1.1.post9/meson.build`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2024 The pypackaging-native developers
 #
 # SPDX-License-Identifier: MIT
 
 project('pkgconf-pypi',
-  version : '2.1.1-8',
+  version : '2.1.1-9',
   license : 'MIT AND ISC',
   license_files : ['LICENSE'],
   meson_version : '>=1.3.2',
 )
 
 py = import('python').find_installation(pure: false)
 python_bin_dir = py.get_install_dir() / 'pkgconf' / '.bin'
```

### Comparing `pkgconf-2.1.1.post8/pyproject.toml` & `pkgconf-2.1.1.post9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # build-backend = 'mesonpy'
 # requires = ['meson-python']
 build-backend = 'buildhack'
 requires = ['meson-python', 'wheel']
 
 [project]
 name = 'pkgconf'
-version = '2.1.1-8'
+version = '2.1.1-9'
 description = '`pkgconf` is a program which helps with discovering library dependencies and configuring compiler and linker flags.'
 readme = 'README.md'
 license = {file = 'LICENSE'}
 authors = [
   {name = 'Ralf Gommers', email = 'ralf.gommers@gmail.com'},
   {name = 'Filipe Laíns', email = 'lains@riseup.net'}
 ]
@@ -27,23 +27,28 @@
   'Programming Language :: C',
   'Topic :: Software Development',
   'Operating System :: Microsoft :: Windows',
   'Operating System :: POSIX',
   'Operating System :: Unix',
   'Operating System :: MacOS'
 ]
+requires-python = '>= 3.8'
+dependencies = [
+  'colorama; os_name == "nt"',
+  'importlib_metadata; python_version < "3.10"',
+]
 
 [project.optional-dependencies]
 test = [
   'pytest',
   'pytest-mock >= 2',
   'pytest-order >= 1',
   'pytest-github-actions-annotate-failures',
   'meson-python',
-  'environment-helpers >= 0.1.1.post1',
+  'environment-helpers >= 0.1.3',
 ]
 docs = [
   'sphinx ~= 7.0',
   'furo',
   'sphinx-design'
 ]
```

### Comparing `pkgconf-2.1.1.post8/src/buildhack.py` & `pkgconf-2.1.1.post9/src/buildhack.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,18 +25,21 @@
     name_parts = wheel_path.stem.split('-')
     name_parts[2] = 'py3'
     name_parts[3] = 'none'
     new_name = '-'.join(name_parts) + '.whl'
     assert new_name != wheel_path.name
     new_wheel_path = workdir / new_name
 
-    with (
-        wheel.wheelfile.WheelFile(wheel_path, 'r') as original_wheel,
-        wheel.wheelfile.WheelFile(new_wheel_path, 'w') as new_wheel,
-    ):
+    with wheel.wheelfile.WheelFile(
+        wheel_path,
+        'r',
+    ) as original_wheel, wheel.wheelfile.WheelFile(
+        new_wheel_path,
+        'w',
+    ) as new_wheel:
         for item in original_wheel.infolist():
             if item.filename.endswith('.dist-info/WHEEL'):
                 new_wheel.writestr(
                     item,
                     textwrap.dedent("""
                     Wheel-Version: 1.0
                     Generator: meson
```

### Comparing `pkgconf-2.1.1.post8/src/pkgconf/__init__.py` & `pkgconf-2.1.1.post9/src/pkgconf/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import importlib
-import importlib.metadata
-import importlib.resources
 import itertools
 import logging
 import os
 import pathlib
 import shutil
 import subprocess
+import sys
 import sysconfig
 import warnings
 
-from collections.abc import Sequence
-from typing import Any
+from typing import Any, Optional
 
 
-__version__ = '2.1.1-8'
+if sys.version_info >= (3, 9):
+    from collections.abc import Sequence
+else:
+    from typing import Sequence
+
+
+if sys.version_info >= (3, 10):
+    import importlib.metadata as importlib_metadata
+else:
+    import importlib_metadata
+
+
+__version__ = '2.1.1-9'
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def _get_system_executable() -> pathlib.Path | None:
+def _get_system_executable() -> Optional[pathlib.Path]:
     scripts = sysconfig.get_path('scripts')
     path_list = os.environ.get('PATH', os.defpath).split(os.pathsep)
     if scripts in path_list:
         path_list.remove(scripts)
     path = os.pathsep.join(path_list)
 
     executable = shutil.which('pkgconf', path=path) or shutil.which('pkg-config', path=path)
@@ -38,45 +48,47 @@
     if os.name == 'posix':
         executable_name = 'pkgconf'
     elif os.name == 'nt':
         executable_name = 'pkgconf.EXE'
     else:
         raise NotImplementedError
 
-    executable = pathlib.Path(importlib.resources.files('pkgconf') / '.bin' / executable_name)
-    if executable.exists():
-        return executable
+    for path in __path__:
+        executable = pathlib.Path(path) / '.bin' / executable_name
+        if executable.exists():
+            return executable
 
     warnings.warn('Bundled pkgconf not found, using the system executable', stacklevel=2)
     executable = _get_system_executable()
     if executable:
         return executable
 
     msg = 'No pkgconf/pkg-config executable available'
     raise RuntimeError(msg)
 
 
-def _get_module_paths(name: str) -> list[str]:
+def _get_module_paths(name: str) -> Sequence[str]:
     module = importlib.import_module(name)
-    if 'NamespacePath' in module.__path__.__class__.__name__:
+    if isinstance(module.__path__, list) or 'NamespacePath' in module.__path__.__class__.__name__:
         return list(module.__path__)
-    return [os.fspath(importlib.resources.files(name))]
+    assert isinstance(module.__path__, str), module.__path__
+    return [module.__path__]
 
 
 def get_pkg_config_path() -> Sequence[str]:
     """Calculate PKG_CONFIG_PATH for Python packages in the current environment.
 
     Python packages may register a directory for their pkg-config files by
     specifying a "pkg-config" entrypoint.
 
     TODO: Document the entrypoint creation and point to that here.
     [project.entry-points.pkg-config]
     entrypoint-name = 'project.package'
     """
-    entrypoints = importlib.metadata.entry_points(group='pkg_config')
+    entrypoints = importlib_metadata.entry_points(group='pkg_config')
     return itertools.chain.from_iterable([_get_module_paths(entry.value) for entry in entrypoints])
 
 
 def run_pkgconf(*args: str, **subprocess_kwargs: Any) -> subprocess.Popen:
     """Run the pkgconf executable.
 
     :param args: Arguments to pass to the pkgconf call.
```

### Comparing `pkgconf-2.1.1.post8/src/pkgconf/__main__.py` & `pkgconf-2.1.1.post9/src/pkgconf/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import subprocess
 import sys
 import warnings
 
-from typing import TextIO
+from typing import Optional, TextIO, Type, Union
 
 import pkgconf
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -59,20 +59,20 @@
     logging.basicConfig(
         stream=sys.stderr,
         format=f'{dim}> %(message)s{reset}',
         level=logging.INFO,
     )
 
     def _showwarning(
-        message: Warning | str,
-        category: type[Warning],
+        message: Union[Warning, str],
+        category: Type[Warning],
         filename: str,
         lineno: int,
-        file: TextIO | None = None,
-        line: str | None = None,
+        file: Optional[TextIO] = None,
+        line: Optional[str] = None,
     ) -> None:  # pragma: no cover
         print(f'{yellow}WARNING{reset} {message}', file=sys.stderr)
 
     warnings.showwarning = _showwarning
 
 
 def _entrypoint():
```

### Comparing `pkgconf-2.1.1.post8/src/pkgconf/diagnose.py` & `pkgconf-2.1.1.post9/src/pkgconf/diagnose.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import importlib.metadata
-import importlib.resources
 import os
 
 import pkgconf
 
 
 def report() -> None:
     print(f'pkgconf executable: {pkgconf.get_executable()}')
 
     entrypoints = importlib.metadata.entry_points(group='pkg-config')
     print('entrypoints:')
     for entry in entrypoints:
         print(f'  {entry.name}:')
         print(f'    value: {entry.value}')
-        print(f'    path: {os.fspath(importlib.resources.files(entry.value))}')
+        print(f'    paths: {pkgconf._get_module_paths(entry.value)}')
 
     print(f'PKG_CONFIG_PATH: {os.pathsep.join(pkgconf.get_pkg_config_path())}')
 
 
 if __name__ == '__main__':
     try:
         report()
```

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/.github/workflows/test.yml` & `pkgconf-2.1.1.post9/subprojects/pkgconf/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/.gitignore` & `pkgconf-2.1.1.post9/subprojects/pkgconf/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/.woodpecker.yml` & `pkgconf-2.1.1.post9/subprojects/pkgconf/.woodpecker.yml`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/AUTHORS` & `pkgconf-2.1.1.post9/subprojects/pkgconf/AUTHORS`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/CODE_OF_CONDUCT.md` & `pkgconf-2.1.1.post9/subprojects/pkgconf/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/Makefile.am` & `pkgconf-2.1.1.post9/subprojects/pkgconf/Makefile.am`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/Makefile.lite` & `pkgconf-2.1.1.post9/subprojects/pkgconf/Makefile.lite`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/NEWS` & `pkgconf-2.1.1.post9/subprojects/pkgconf/NEWS`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/README.md` & `pkgconf-2.1.1.post9/subprojects/pkgconf/README.md`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/autogen.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/autogen.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/cli/bomtool/main.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/cli/bomtool/main.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/cli/getopt_long.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/cli/getopt_long.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/cli/getopt_long.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/cli/getopt_long.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/cli/main.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/cli/main.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/cli/renderer-msvc.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/cli/renderer-msvc.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/cli/renderer-msvc.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/cli/renderer-msvc.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/configure.ac` & `pkgconf-2.1.1.post9/subprojects/pkgconf/configure.ac`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/conf.py` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/extract.py` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/extract.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-audit.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-audit.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-cache.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-cache.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-client.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-client.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-dependency.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-dependency.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-fragment.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-fragment.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-path.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-path.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-personality.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-personality.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-pkg.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-pkg.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-queue.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-queue.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/doc/libpkgconf-tuple.rst` & `pkgconf-2.1.1.post9/subprojects/pkgconf/doc/libpkgconf-tuple.rst`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/argvsplit.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/argvsplit.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/audit.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/audit.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/bsdstubs.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/bsdstubs.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/bsdstubs.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/bsdstubs.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/cache.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/cache.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/client.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/client.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/config.h.meson` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/config.h.meson`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/dependency.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/dependency.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/fileio.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/fileio.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/fragment.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/fragment.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/iter.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/iter.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/libpkgconf-api.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/libpkgconf-api.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/libpkgconf.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/libpkgconf.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/parser.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/parser.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/path.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/path.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/personality.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/personality.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/pkg.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/pkg.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/queue.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/queue.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/stdinc.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/stdinc.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/tuple.c` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/tuple.c`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/libpkgconf/win-dirent.h` & `pkgconf-2.1.1.post9/subprojects/pkgconf/libpkgconf/win-dirent.h`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/m4/ax_check_compile_flag.m4` & `pkgconf-2.1.1.post9/subprojects/pkgconf/m4/ax_check_compile_flag.m4`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/man/pc.5` & `pkgconf-2.1.1.post9/subprojects/pkgconf/man/pc.5`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/man/pkg.m4.7` & `pkgconf-2.1.1.post9/subprojects/pkgconf/man/pkg.m4.7`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/man/pkgconf-personality.5` & `pkgconf-2.1.1.post9/subprojects/pkgconf/man/pkgconf-personality.5`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/man/pkgconf.1` & `pkgconf-2.1.1.post9/subprojects/pkgconf/man/pkgconf.1`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/meson.build` & `pkgconf-2.1.1.post9/subprojects/pkgconf/meson.build`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/pkg.m4` & `pkgconf-2.1.1.post9/subprojects/pkgconf/pkg.m4`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/basic.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/basic.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/builtins.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/builtins.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/lib1/billion-laughs.pc` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/lib1/billion-laughs.pc`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/parser.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/parser.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/provides.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/provides.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/regress.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/regress.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/requires.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/requires.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/sysroot.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/sysroot.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/test_env.sh.in` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/test_env.sh.in`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/subprojects/pkgconf/tests/version.sh` & `pkgconf-2.1.1.post9/subprojects/pkgconf/tests/version.sh`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/tests/test_distribution.py` & `pkgconf-2.1.1.post9/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/tests/test_entrypoints.py` & `pkgconf-2.1.1.post9/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/tests/test_examples.py` & `pkgconf-2.1.1.post9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/tests/test_python_module.py` & `pkgconf-2.1.1.post9/tests/test_python_module.py`

 * *Files identical despite different names*

### Comparing `pkgconf-2.1.1.post8/PKG-INFO` & `pkgconf-2.1.1.post9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgconf
-Version: 2.1.1.post8
+Version: 2.1.1.post9
 Summary: `pkgconf` is a program which helps with discovering library dependencies and configuring compiler and linker flags.
 Home-page: https://pkgconf-pypi.readthedocs.io/en/latest/
 Author-Email: Ralf Gommers <ralf.gommers@gmail.com>, =?utf-8?q?Filipe_La=C3=ADns?= <lains@riseup.net>
 License: Copyright (c) 2024 pypackaging-native contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
@@ -32,25 +32,28 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Project-URL: Homepage, https://pkgconf-pypi.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/pypackaging-native/pkgconf-pypi/issues
 Project-URL: Source, https://github.com/pypackaging-native/pkgconf-pypi
-Provides-Extra: test
-Provides-Extra: docs
+Requires-Python: >=3.8
+Requires-Dist: colorama; os_name == "nt"
+Requires-Dist: importlib_metadata; python_version < "3.10"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock>=2; extra == "test"
 Requires-Dist: pytest-order>=1; extra == "test"
 Requires-Dist: pytest-github-actions-annotate-failures; extra == "test"
 Requires-Dist: meson-python; extra == "test"
-Requires-Dist: environment-helpers>=0.1.1.post1; extra == "test"
+Requires-Dist: environment-helpers>=0.1.3; extra == "test"
 Requires-Dist: sphinx~=7.0; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
+Provides-Extra: test
+Provides-Extra: docs
 Description-Content-Type: text/markdown
 
 # pkgconf-pypi
 
 [![CI test](https://github.com/pypackaging-native/pkgconf-pypi/actions/workflows/test.yml/badge.svg)](https://github.com/pypackaging-native/pkgconf-pypi/actions/workflows/test.yml)
 [![CI build](https://github.com/pypackaging-native/pkgconf-pypi/actions/workflows/build.yml/badge.svg)](https://github.com/pypackaging-native/pkgconf-pypi/actions/workflows/build.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pypackaging-native/pkgconf-pypi/main.svg)](https://results.pre-commit.ci/latest/github/pypackaging-native/pkgconf-pypi/main)
```

