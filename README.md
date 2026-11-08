# microb-engine

An archive (a "fork" for safekeeping) of the source of **MicroB**, the Mozilla based browser engine of the Nokia N900 (Maemo 5, Fremantle):
Debian source package `microb-engine` **20100401-1.9.2-5.2+0m5** (Gecko 1.9.2, NSS 3.12.6.2, NSPR 4.8.3), the exact version installed on the phone.
The original server `repository.maemo.org` is gone; the sources were recovered from the Internet Archive and are kept here so that they do not have
to be hunted again.

Origin (snapshot 2020-09-28 of `http://repository.maemo.org/pool/maemo5.0/free/m/microb-engine/`):

| file | MD5 |
|---|---|
| `microb-engine_20100401-1.9.2.orig.tar.gz` (58423455 bytes) | `2ca3769f819f25b8e2afe5a9159c64a0` |
| `microb-engine_20100401-1.9.2-5.2+0m5.diff.gz` (1528164 bytes) | `3a34d1a2485d961f31daf21b138128b8` |

Contents of this repository: the unpacked upstream tree (`orig.tar.gz`) with the Debian diff applied, i.e. the `debian/` directory (control files, build
configuration `debian/configs`, preferences `debian/prefs`, 33 patches in `debian/patches` managed by quilt, **not applied** to the tree). The source package
builds libnspr4, libnss3, libnss3-certs, microb-xulrunner, microb-engine, microb-full and others. Maintainer of the package: Oleg Romashin (Nokia).

Licence: the Mozilla tri-license (MPL 1.1 / GPL 2 / LGPL 2.1), see `LICENSE`, `LEGAL` and the headers of the files.

Used by the N900 project (`DOC/microb.md`): the experiment of replacing NSS by a newer version so that MicroB speaks TLS 1.2. Nothing here is built by the
project yet.
