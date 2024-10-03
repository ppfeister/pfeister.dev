---
title: "Sherlock 0.15.0"
description: "Major changes coming to Sherlock, including official support for Fedora"
slug: "sherlock-0.15.0"
type:
- "posts"
- "post"
categories:
- "Open Source"
tags: 
- "Fedora"
- "Sherlock Project"
cover: "/images/sherlock-demo-cropped.png"
CoverCaption: "Upstream repository : https://github.com/sherlock-project/sherlock"
toc: false
date: "2024-06-26T02:45:00-04:00"
#lastmod: "2024-06-26T02:45:00-03:00"
author: "Paul Pfeister"
#draft: true
---



- 📦 Official package now available on [__PyPI__][ext-pypi] ([#2127]) [@ppfeister]
- 📦 Official package now available on [__DockerHub__][ext-dockerhub] ([#2216]) [@ppfeister]
- 📦 Official package now available on [__Fedora__][ext-fedora] [@ppfeister]
- 📦 Community package now available on [__Homebrew__][ext-homebrew] [@p-linnane]
- ✨ New Sherlock wiki at [__sherlockproject.xyz__][ext-wiki] [@sdushantha] 
- ✨ \-\-dump\-response flag added for easier debugging ([#2214]) [@ppfeister]
- 🪲 Fixed uncaught exception when tor browser not found ([#2033]) [@joaomfbh]
- 🪲 ‼️ Importable module renamed to sherlock_project [(Debian#1072733)][ext-deb1072733] [@ppfeister]
- 🛠️ Adopted Poetry and restructured as a true package [@mjsir911] [@ppfeister] [@matheusfelipeog] [@sdushantha]
- 🛠️ Unit testing rewritten to better support contributors and packagers [@ppfeister]
  - Switched from unittest to pytest and tox
  - Expanded regression testing to include builds on Windows and MacOS
  - Added offline-only test environments for packagers (see below)
- 🛠️ Manifest schema added for regression testing and better in-IDE UX ([#2212]) [@ppfeister]
- 🛠️ Added detection mechanism for users running via legacy/unsupported methods ([#2213]) [@ppfeister]
- 🛠️ ‼️ Dependency [__torrequest__][ext-torrequest] made optional ([#2215]) [@ppfeister] [@matheusfelipeog] 
  - \-\-tor and \-\-unique\-tor are now DEPRECATED (see detail below)
- 🛠️ ‼️ Deprecated support for Python 3.6 and 3.7 (now ^3.8)
- 🛠️ Several minor UX improvements over the course of development
- 🏷️ Adopted properly tagged releases help out our downstream packagers
- ✍️ General improvements to and simplification of in-repo documentation

[@ppfeister]: https://github.com/ppfeister
[@p-linnane]: https://github.com/p-linnane
[@sdushantha]: https://github.com/sdushantha
[@joaomfbh]: https://github.com/joaomfbh
[@matheusfelipeog]: https://github.com/matheusfelipeog
[@mjsir911]: https://github.com/mjsir911

[#2127]: https://github.com/sherlock-project/sherlock/issues/2127
[#2216]: https://github.com/sherlock-project/sherlock/issues/2216
[#2214]: https://github.com/sherlock-project/sherlock/issues/2214
[#2033]: https://github.com/sherlock-project/sherlock/issues/2033
[#2212]: https://github.com/sherlock-project/sherlock/issues/2212
[#2213]: https://github.com/sherlock-project/sherlock/issues/2213
[#2215]: https://github.com/sherlock-project/sherlock/issues/2215

[release-diff]: https://github.com/sherlock-project/sherlock/compare/v0.14.4...v0.15.0

[ext-pypi]: https://pypi.org/project/sherlock-project/
[ext-dockerhub]: https://hub.docker.com/r/sherlock/sherlock
[ext-fedora]: https://src.fedoraproject.org/rpms/sherlock-project/
[ext-homebrew]: https://formulae.brew.sh/formula/sherlock

[ext-wiki]: https://sherlockproject.xyz
[ext-wiki-install]: https://sherlockproject.xyz/installation

[ext-rpm-spec]: https://src.fedoraproject.org/rpms/sherlock-project/blob/rawhide/f/sherlock-project.spec

[ext-torrequest]: https://pypi.org/project/torrequest/

[ext-deb1072733]: https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1072733
