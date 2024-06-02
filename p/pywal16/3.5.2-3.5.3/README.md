# Comparing `tmp/pywal16-3.5.2.tar.gz` & `tmp/pywal16-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywal16-3.5.2.tar", last modified: Mon May  6 22:17:07 2024, max compression
+gzip compressed data, was "pywal16-3.5.3.tar", last modified: Tue May  7 20:18:17 2024, max compression
```

## Comparing `pywal16-3.5.2.tar` & `pywal16-3.5.3.tar`

### file list

```diff
@@ -1,347 +1,347 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.848708 pywal16-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 22:17:03.000000 pywal16-3.5.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 22:17:03.000000 pywal16-3.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 22:17:03.000000 pywal16-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-06 22:17:07.848708 pywal16-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-06 22:17:03.000000 pywal16-3.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.796709 pywal16-3.5.2/pywal/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.800709 pywal16-3.5.2/pywal/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/colorthief.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/colorz.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/fast_colorthief.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/haishoku.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/schemer2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/backends/wal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.796709 pywal16-3.5.2/pywal/colorschemes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.832709 pywal16-3.5.2/pywal/colorschemes/dark/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/3024.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/ashes.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-3024.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-apathy.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-ashes.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-cave.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-dune.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-estuary.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-forest.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-heath.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-lakeside.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-plateau.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-savanna.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-seaside.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-atelier-sulphurpool.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-bespin.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-bathory.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-burzum.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-funeral.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-gorgoroth.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-immortal.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-khold.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-marduk.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-mayhem.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-nile.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal-venom.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-black-metal.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-brewer.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-bright.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-brushtrees.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-chalk.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-circus.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-classic.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-codeschool.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-default.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-dracula.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-eighties.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-embers.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-flat.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-google.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-grayscale.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-greenscreen.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-gruvbox-hard.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-gruvbox-medium.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-gruvbox-pale.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-gruvbox-soft.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-harmonic.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-hopscotch.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-icy.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-irblack.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-isotope.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-macintosh.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-marrakesh.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-materia.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-material-palenight.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-material.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-materialer.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-mellow-purple.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-mocha.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-monokai.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-nord.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-ocean.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-oceanicnext.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-onedark.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-outrun.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-paraiso.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-phd.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-pico.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-pop.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-porple.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-railscasts.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-rebecca.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-seti.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-snazzy.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-solarflare.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-solarized.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-spacemacs.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-summerfruit.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-tomorrow-night.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-tube.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-twilight.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-unikitty.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-woodland.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-xcode-dusk.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16-zenburn.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/base16tooth.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/darktooth.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-5725.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-amiox.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-bark.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-blend.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-blok.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-bluetype.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-blumune.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-book.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-branch.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-brownstone.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-bulb.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-chaires.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-coco.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-corduroy.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-depth.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-designr.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-diner.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-escen.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-fendr.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-flapr.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-forst.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-fury.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-harbing.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-kit.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-leaf.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-link.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-mattd.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-novmbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-owl.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-paints.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-parkd.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-pastely.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-petal.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-poly.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-prevail.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-provrb.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-raild.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-relax.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-scag.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-scape.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-shade.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-simplicity.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-skigh.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-slate.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-soundwave.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-spire.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-sprout.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-squares.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-stv.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-subtle.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-sundr.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-tealights.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-traffic.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-transposet.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-urban.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-vans.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-victory.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-view.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/dkeg-wintry.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/gruvbox.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/hybrid-material.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/monokai.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-astromouse.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-belge.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-bitmute.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-cloud.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-colorfulcolors.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-dawn.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-deafened.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-derp.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-digerati.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-doomicideocean.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-dotshare.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-dwmrob.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-eqie6.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-euphrasia.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-gjm.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-gnometerm.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-gotham.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-gslob-nature-suede.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-hund.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-insignificato.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-invisibone.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-jasonwryan.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-kasugano.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-material.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-mikado.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-mikazuki.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-monokai.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-muse.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-nancy.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-navy-and-ivory.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-neon.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-numixdarkest.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-orangish.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-parker_brothers.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-phrak1.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-pretty-and-pastel.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-rasi.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-rezza.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-rydgel.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-s3r0-modified.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-sexcolors.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-simple_rainbow.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-splurge.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-swayr.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-sweetlove.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-tango.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-tangoesque.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-tartan.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-theme2.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-thwump.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-tlh.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-trim-yer-beard.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-user-77-mashup-colors.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-vacuous2.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-visibone-alt-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-visibone.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-x-dotshare.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/sexy-zenburn.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/solarized.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_autumn.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_dusk.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_future.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_rift.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_spring.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_summer.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_warp.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/tempus_winter.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/vscode.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/dark/zenburn.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.840709 pywal16-3.5.2/pywal/colorschemes/light/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/3024.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/ashes.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-cave.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-dune.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-estuary.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-forest.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-heath.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-lakeside.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-plateau.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-savanna.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-seaside.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-atelier-sulphurpool.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-classic.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-cupcake.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-cupertino.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-default.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-github.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-google.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-grayscale.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-gruvbox-hard.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-gruvbox-medium.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-gruvbox-soft.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-harmonic.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-materialer.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-mexico.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-one.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-shapeshifter.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-solarized.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-summerfruit.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-tomorrow.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/base16-unikitty.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/github.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/sexy-mostly-bright.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/solarized.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/tempus_dawn.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/tempus_fugit.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/tempus_past.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/colorschemes/light/tempus_totus.json
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/reload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.840709 pywal16-3.5.2/pywal/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/scripts/gtk_reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.844709 pywal16-3.5.2/pywal/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/Colors.hs
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors--nodim-alacritty.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-alacritty.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-alacritty.yml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-kitty.conf
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-konsole.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-leftwm-theme.ron
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-nqq.css
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-oomox
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-putty.reg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-rgb
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-rofi-dark.rasi
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-rofi-light.rasi
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-speedcrunch.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-sway
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-themer.js
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-tilix.json
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-tty.sh
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-vscode.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-wal-dmenu.h
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-wal-dwm.h
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-wal-st.h
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-wal-tabbed.h
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-wal.vim
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors-waybar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.Xresources
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.css
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.hs
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.sh
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.styl
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/templates/colors.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-05-06 22:17:03.000000 pywal16-3.5.2/pywal/wallpaper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.848708 pywal16-3.5.2/pywal16.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-06 22:17:07.000000 pywal16-3.5.2/pywal16.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-06 22:17:07.000000 pywal16-3.5.2/pywal16.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:17:07.000000 pywal16-3.5.2/pywal16.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 22:17:07.000000 pywal16-3.5.2/pywal16.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:17:07.000000 pywal16-3.5.2/pywal16.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 22:17:07.000000 pywal16-3.5.2/pywal16.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 22:17:07.848708 pywal16-3.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 22:17:03.000000 pywal16-3.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.844709 pywal16-3.5.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_colors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1514 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:17:07.848708 pywal16-3.5.2/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test.png
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test_file
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test_file.json
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test_file2.json
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_files/test_file3.json
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1788 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_sequences.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3223 2024-05-06 22:17:03.000000 pywal16-3.5.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.954130 pywal16-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 20:18:10.000000 pywal16-3.5.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 20:18:10.000000 pywal16-3.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 20:18:10.000000 pywal16-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-07 20:18:17.954130 pywal16-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-07 20:18:10.000000 pywal16-3.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.890130 pywal16-3.5.3/pywal/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.894130 pywal16-3.5.3/pywal/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/colorthief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/colorz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/fast_colorthief.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/haishoku.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/schemer2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/backends/wal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.886130 pywal16-3.5.3/pywal/colorschemes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.934130 pywal16-3.5.3/pywal/colorschemes/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/3024.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/ashes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-3024.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-apathy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-ashes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-cave.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-dune.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-estuary.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-forest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-heath.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-lakeside.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-plateau.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-savanna.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-seaside.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-atelier-sulphurpool.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-bespin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-bathory.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-burzum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-funeral.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-gorgoroth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-immortal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-khold.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-marduk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-mayhem.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-nile.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal-venom.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-black-metal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-brewer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-bright.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-brushtrees.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-chalk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-circus.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-classic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-codeschool.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-dracula.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-eighties.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-embers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-flat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-google.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-grayscale.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-greenscreen.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-gruvbox-hard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-gruvbox-medium.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-gruvbox-pale.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-gruvbox-soft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-harmonic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-hopscotch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-icy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-irblack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-isotope.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-macintosh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-marrakesh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-materia.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-material-palenight.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-material.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-materialer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-mellow-purple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-mocha.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-monokai.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-nord.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-ocean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-oceanicnext.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-onedark.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-outrun.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-paraiso.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-phd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-pico.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-pop.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-porple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-railscasts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-rebecca.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-seti.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-snazzy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-solarflare.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-solarized.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-spacemacs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-summerfruit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-tomorrow-night.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-tube.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-twilight.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-unikitty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-woodland.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-xcode-dusk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16-zenburn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/base16tooth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/darktooth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-5725.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-amiox.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-bark.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-blend.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-blok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-bluetype.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-blumune.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-branch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-brownstone.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-chaires.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-coco.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-corduroy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-depth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-designr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-diner.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-escen.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-fendr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-flapr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-forst.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-fury.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-harbing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-kit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-leaf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-link.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-mattd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-novmbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-owl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-paints.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-parkd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-pastely.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-petal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-poly.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-prevail.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-provrb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-raild.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-relax.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-scag.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-scape.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-shade.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-simplicity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-skigh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-slate.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-soundwave.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-spire.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-sprout.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-squares.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-stv.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-subtle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-sundr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-tealights.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-traffic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-transposet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-urban.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-vans.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-victory.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-view.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/dkeg-wintry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/gruvbox.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/hybrid-material.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/monokai.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-astromouse.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-belge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-bitmute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-cloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-colorfulcolors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-dawn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-deafened.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-derp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-digerati.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-doomicideocean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-dotshare.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-dwmrob.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-eqie6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-euphrasia.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-gjm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-gnometerm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-gotham.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-gslob-nature-suede.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-hund.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-insignificato.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-invisibone.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-jasonwryan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-kasugano.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-material.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-mikado.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-mikazuki.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-monokai.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-muse.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-nancy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-navy-and-ivory.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-neon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-numixdarkest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-orangish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-parker_brothers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-phrak1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-pretty-and-pastel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-rasi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-rezza.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-rydgel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-s3r0-modified.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-sexcolors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-simple_rainbow.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-splurge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-swayr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-sweetlove.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-tango.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-tangoesque.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-tartan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-theme2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-thwump.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-tlh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-trim-yer-beard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-user-77-mashup-colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-vacuous2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-visibone-alt-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-visibone.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-x-dotshare.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/sexy-zenburn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/solarized.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_dusk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_future.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_rift.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_spring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_summer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_warp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/tempus_winter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/vscode.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/dark/zenburn.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.942130 pywal16-3.5.3/pywal/colorschemes/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/3024.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/ashes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-cave.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-dune.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-estuary.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-forest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-heath.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-lakeside.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-plateau.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-savanna.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-seaside.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-atelier-sulphurpool.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-classic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-cupcake.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-cupertino.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-github.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-google.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-grayscale.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-gruvbox-hard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-gruvbox-medium.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-gruvbox-soft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-harmonic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-materialer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-mexico.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-one.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-shapeshifter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-solarized.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-summerfruit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-tomorrow.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/base16-unikitty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/github.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/sexy-mostly-bright.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/solarized.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/tempus_dawn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/tempus_fugit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/tempus_past.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/colorschemes/light/tempus_totus.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/reload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.942130 pywal16-3.5.3/pywal/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/scripts/gtk_reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.946130 pywal16-3.5.3/pywal/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/Colors.hs
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors--nodim-alacritty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-alacritty.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-alacritty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-kitty.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-konsole.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-leftwm-theme.ron
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-nqq.css
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-oomox
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-putty.reg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-rgb
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-rofi-dark.rasi
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-rofi-light.rasi
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-speedcrunch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-sway
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-themer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-tilix.json
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-tty.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-vscode.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-wal-dmenu.h
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-wal-dwm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-wal-st.h
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-wal-tabbed.h
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-wal.vim
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors-waybar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.Xresources
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.hs
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.styl
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/templates/colors.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-05-07 20:18:10.000000 pywal16-3.5.3/pywal/wallpaper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.950130 pywal16-3.5.3/pywal16.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-07 20:18:17.000000 pywal16-3.5.3/pywal16.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-07 20:18:17.000000 pywal16-3.5.3/pywal16.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:18:17.000000 pywal16-3.5.3/pywal16.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 20:18:17.000000 pywal16-3.5.3/pywal16.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:18:17.000000 pywal16-3.5.3/pywal16.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 20:18:17.000000 pywal16-3.5.3/pywal16.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:18:17.954130 pywal16-3.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-07 20:18:10.000000 pywal16-3.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.950130 pywal16-3.5.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1514 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:17.950130 pywal16-3.5.3/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test_file
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test_file2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_files/test_file3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1788 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_sequences.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3223 2024-05-07 20:18:10.000000 pywal16-3.5.3/tests/test_util.py
```

### Comparing `pywal16-3.5.2/.pylintrc` & `pywal16-3.5.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/LICENSE.md` & `pywal16-3.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/PKG-INFO` & `pywal16-3.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywal16
-Version: 3.5.2
+Version: 3.5.3
 Summary: Generate and change color-schemes on the fly
 Home-page: https://github.com/eylles/pywal16
-Download-URL: https://github.com/eylles/pywal16/archive/3.5.2.tar.gz
+Download-URL: https://github.com/eylles/pywal16/archive/3.5.3.tar.gz
 Author: Dylan Araps
 Author-email: dylan.araps@gmail.com
 License: MIT
 Keywords: wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pywal16 Version: 3.5.2 Summary: Generate and change
+Metadata-Version: 2.1 Name: pywal16 Version: 3.5.3 Summary: Generate and change
 color-schemes on the fly Home-page: https://github.com/eylles/pywal16 Download-
-URL: https://github.com/eylles/pywal16/archive/3.5.2.tar.gz Author: Dylan Araps
+URL: https://github.com/eylles/pywal16/archive/3.5.3.tar.gz Author: Dylan Araps
 Author-email: dylan.araps@gmail.com License: MIT Keywords: wal colorscheme
 terminal-emulators changing-colorschemes Classifier: Environment :: X11
 Applications Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3.5 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE.md ## This
 project is a 16 colors fork of [pywal](https://github.com/dylanaraps/pywal)
```

### Comparing `pywal16-3.5.2/README.md` & `pywal16-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/__init__.py` & `pywal16-3.5.3/pywal/__init__.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/__main__.py` & `pywal16-3.5.3/pywal/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     arg.add_argument("-a", metavar="\"alpha\"",
                      help="Set terminal background transparency. \
                            *Only works in URxvt*")
 
     arg.add_argument("-b", metavar="background",
                      help="Custom background color to use.")
 
+    arg.add_argument("--fg", metavar="foreground",
+                     help="Custom foreground color to use.")
+
     arg.add_argument("--backend", metavar="backend",
                      help="Which color backend to use. \
                            Use 'wal --backend' to list backends.",
                      const="list_backends", type=str, nargs="?")
 
     arg.add_argument("--theme", "-f", metavar="/path/to/file or theme_name",
                      help="Which colorscheme file to use. \
@@ -195,14 +198,19 @@
                                   sat=args.saturate)
 
     if args.b:
         args.b = "#%s" % (args.b.strip("#"))
         colors_plain["special"]["background"] = args.b
         colors_plain["colors"]["color0"] = args.b
 
+    if args.fg:
+        args.fg = "#%s" % (args.fg.strip("#"))
+        colors_plain["special"]["foreground"] = args.fg
+        colors_plain["colors"]["color15"] = args.fg
+
     if not args.n:
         wallpaper.change(colors_plain["wallpaper"])
 
     if args.p:
         theme.save(colors_plain, args.p, args.l)
 
     sequences.send(colors_plain, to_send=not args.s, vte_fix=args.vte)
```

### Comparing `pywal16-3.5.2/pywal/backends/colorthief.py` & `pywal16-3.5.3/pywal/backends/colorthief.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/backends/colorz.py` & `pywal16-3.5.3/pywal/backends/colorz.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/backends/fast_colorthief.py` & `pywal16-3.5.3/pywal/backends/fast_colorthief.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/backends/haishoku.py` & `pywal16-3.5.3/pywal/backends/haishoku.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/backends/schemer2.py` & `pywal16-3.5.3/pywal/backends/schemer2.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/backends/wal.py` & `pywal16-3.5.3/pywal/backends/wal.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,24 @@
 
 def imagemagick(color_count, img, magick_command):
     """Call Imagemagick to generate a scheme."""
     flags = ["-resize", "25%", "-colors", str(color_count),
              "-unique-colors", "txt:-"]
     img += "[0]"
 
-    return subprocess.check_output([*magick_command, img, *flags]).splitlines()
+    try:
+        output = subprocess.check_output([*magick_command, img, *flags],
+                                         stderr=subprocess.STDOUT).splitlines()
+    except subprocess.CalledProcessError as Err:
+        logging.error("Imagemagick error: %s", Err)
+        logging.error(
+          "IM 7 disables stdout by default, check the wiki for the fix."
+        )
+        sys.exit(1)
+    return output
 
 
 def has_im():
     """Check to see if the user has im installed."""
     if shutil.which("magick"):
         return ["magick", "convert"]
 
@@ -62,8 +71,12 @@
 
     return colors.generic_adjust(raw_colors, light, cols16)
 
 
 def get(img, light=False, cols16=False):
     """Get colorscheme."""
     colors = gen_colors(img)
+    # it is possible we could have picked garbage data
+    garbage = "# Image"
+    if garbage in colors:
+        colors.remove(garbage)
     return adjust(colors, light, cols16)
```

### Comparing `pywal16-3.5.2/pywal/colors.py` & `pywal16-3.5.3/pywal/colors.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/export.py` & `pywal16-3.5.3/pywal/export.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/image.py` & `pywal16-3.5.3/pywal/image.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/reload.py` & `pywal16-3.5.3/pywal/reload.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/scripts/gtk_reload.py` & `pywal16-3.5.3/pywal/scripts/gtk_reload.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/sequences.py` & `pywal16-3.5.3/pywal/sequences.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/settings.py` & `pywal16-3.5.3/pywal/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Created by Dylan Araps.
 """
 
 import os
 import platform
 
 
-__version__ = "3.5.2"
+__version__ = "3.5.3"
 __cache_version__ = "1.1.0"
 
 
 HOME = os.getenv("HOME", os.getenv("USERPROFILE"))
 XDG_CACHE_DIR = os.getenv("XDG_CACHE_HOME", os.path.join(HOME, ".cache"))
 XDG_CONF_DIR = os.getenv("XDG_CONFIG_HOME", os.path.join(HOME, ".config"))
```

### Comparing `pywal16-3.5.2/pywal/templates/Colors.hs` & `pywal16-3.5.3/pywal/templates/Colors.hs`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors--nodim-alacritty.yml` & `pywal16-3.5.3/pywal/templates/colors--nodim-alacritty.yml`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-alacritty.toml` & `pywal16-3.5.3/pywal/templates/colors-alacritty.toml`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-alacritty.yml` & `pywal16-3.5.3/pywal/templates/colors-alacritty.yml`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-kitty.conf` & `pywal16-3.5.3/pywal/templates/colors-kitty.conf`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-konsole.colorscheme` & `pywal16-3.5.3/pywal/templates/colors-konsole.colorscheme`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-nqq.css` & `pywal16-3.5.3/pywal/templates/colors-nqq.css`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-putty.reg` & `pywal16-3.5.3/pywal/templates/colors-putty.reg`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-rofi-dark.rasi` & `pywal16-3.5.3/pywal/templates/colors-rofi-dark.rasi`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-rofi-light.rasi` & `pywal16-3.5.3/pywal/templates/colors-rofi-light.rasi`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-tilix.json` & `pywal16-3.5.3/pywal/templates/colors-tilix.json`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-tty.sh` & `pywal16-3.5.3/pywal/templates/colors-tty.sh`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-wal-dwm.h` & `pywal16-3.5.3/pywal/templates/colors-wal-dwm.h`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-wal-st.h` & `pywal16-3.5.3/pywal/templates/colors-wal-st.h`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-wal.vim` & `pywal16-3.5.3/pywal/templates/colors-wal.vim`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors-waybar.css` & `pywal16-3.5.3/pywal/templates/colors-waybar.css`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors.Xresources` & `pywal16-3.5.3/pywal/templates/colors.Xresources`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors.css` & `pywal16-3.5.3/pywal/templates/colors.css`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors.hs` & `pywal16-3.5.3/pywal/templates/colors.hs`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors.json` & `pywal16-3.5.3/pywal/templates/colors.json`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/templates/colors.sh` & `pywal16-3.5.3/pywal/templates/colors.sh`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/theme.py` & `pywal16-3.5.3/pywal/theme.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal/util.py` & `pywal16-3.5.3/pywal/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Misc helper functions.
 """
 
 import colorsys
 import json
 import logging
 import os
+import fcntl
 import platform
 import re
 import shutil
 import subprocess
 import sys
 from hashlib import md5
 
@@ -172,17 +173,25 @@
 
 def save_file(data, export_file):
     """Write data to a file."""
     create_dir(os.path.dirname(export_file))
 
     try:
         with open(export_file, "w") as file:
+            # Get the current flags and add non-blocking mode
+            # to skip TTYs suspended by Flow Control
+            # https://www.gnu.org/software/libc/manual/html_node/Getting-File-Status-Flags.html
+            # https://www.gnu.org/software/libc/manual/html_node/Open_002dtime-Flags.html
+            flags = fcntl.fcntl(file, fcntl.F_GETFL)
+            fcntl.fcntl(file, fcntl.F_SETFL, flags | os.O_NONBLOCK)
             file.write(data)
     except PermissionError:
         logging.warning("Couldn't write to %s.", export_file)
+    except BlockingIOError:
+        logging.warning("Couldn't write to %s, not accepting data", export_file)
 
 
 def save_file_json(data, export_file):
     """Write data to a json file."""
     create_dir(os.path.dirname(export_file))
 
     with open(export_file, "w") as file:
```

### Comparing `pywal16-3.5.2/pywal/wallpaper.py` & `pywal16-3.5.3/pywal/wallpaper.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/pywal16.egg-info/PKG-INFO` & `pywal16-3.5.3/pywal16.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywal16
-Version: 3.5.2
+Version: 3.5.3
 Summary: Generate and change color-schemes on the fly
 Home-page: https://github.com/eylles/pywal16
-Download-URL: https://github.com/eylles/pywal16/archive/3.5.2.tar.gz
+Download-URL: https://github.com/eylles/pywal16/archive/3.5.3.tar.gz
 Author: Dylan Araps
 Author-email: dylan.araps@gmail.com
 License: MIT
 Keywords: wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pywal16 Version: 3.5.2 Summary: Generate and change
+Metadata-Version: 2.1 Name: pywal16 Version: 3.5.3 Summary: Generate and change
 color-schemes on the fly Home-page: https://github.com/eylles/pywal16 Download-
-URL: https://github.com/eylles/pywal16/archive/3.5.2.tar.gz Author: Dylan Araps
+URL: https://github.com/eylles/pywal16/archive/3.5.3.tar.gz Author: Dylan Araps
 Author-email: dylan.araps@gmail.com License: MIT Keywords: wal colorscheme
 terminal-emulators changing-colorschemes Classifier: Environment :: X11
 Applications Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3.5 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE.md ## This
 project is a 16 colors fork of [pywal](https://github.com/dylanaraps/pywal)
```

### Comparing `pywal16-3.5.2/pywal16.egg-info/SOURCES.txt` & `pywal16-3.5.3/pywal16.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/setup.py` & `pywal16-3.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_colors.py` & `pywal16-3.5.3/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_export.py` & `pywal16-3.5.3/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_files/test.jpg` & `pywal16-3.5.3/tests/test_files/test.jpg`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_files/test2.jpg` & `pywal16-3.5.3/tests/test_files/test2.jpg`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_files/test_file.json` & `pywal16-3.5.3/tests/test_files/test_file.json`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_files/test_file2.json` & `pywal16-3.5.3/tests/test_files/test_file2.json`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_files/test_file3.json` & `pywal16-3.5.3/tests/test_files/test_file3.json`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_image.py` & `pywal16-3.5.3/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_sequences.py` & `pywal16-3.5.3/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `pywal16-3.5.2/tests/test_util.py` & `pywal16-3.5.3/tests/test_util.py`

 * *Files identical despite different names*

