Changelog
#########

<!-- Release notes generated using configuration in .github/release.yaml at main -->

v0.2.0
******

What's Changed
==============

Breaking Changes 🛠
-------------------
* Rename `aux` to `auxiliary` by @tky823 in https://github.com/tky823/ssspy/pull/268
* Detailed build status by @tky823 in https://github.com/tky823/ssspy/pull/288

New Features 🎉
---------------
* Implementation of harmonic vector analysis by @tky823 in https://github.com/tky823/ssspy/pull/271
* Implementation of ADMM-HVA by @tky823 in https://github.com/tky823/ssspy/pull/281

Bug Fixes 🐛
------------
* Fix test coverage by @tky823 in https://github.com/tky823/ssspy/pull/269
* Fix timing of uploading package by @tky823 in https://github.com/tky823/ssspy/pull/273
* Remove status badge of lint by @tky823 in https://github.com/tky823/ssspy/pull/274

Other Changes
-------------
* Upload package to TestPyPI by @tky823 in https://github.com/tky823/ssspy/pull/267
* Remove duplicate uploads to TestPyPI by @tky823 in https://github.com/tky823/ssspy/pull/270
* Use flooring function to compute norm. by @tky823 in https://github.com/tky823/ssspy/pull/276
* Regression tests by @tky823 in https://github.com/tky823/ssspy/pull/238
* Add `needs` to upload_package job in GHA. by @tky823 in https://github.com/tky823/ssspy/pull/277
* Update actions/checkout in GitHub actions by @tky823 in https://github.com/tky823/ssspy/pull/279
* Hugging Face demo by @tky823 in https://github.com/tky823/ssspy/pull/282
* Set permissions in workflows by @tky823 in https://github.com/tky823/ssspy/pull/289
* Bump up version to 0.2.0 by @tky823 in https://github.com/tky823/ssspy/pull/290


**Full Changelog**: https://github.com/tky823/ssspy/compare/v0.1.7...v0.2.0

v0.1.7
******

Summary
=======
In this version, we improve the management of the package.
As a new BSS method, ADMM-BSS is newly added.

What's Changed
==============

Breaking Changes 🛠
-------------------
* Include ssspy only as package by @tky823 in https://github.com/tky823/ssspy/pull/253
* Add ``MANIFEST.in`` by @tky823 in https://github.com/tky823/ssspy/pull/257

New Features 🎉
---------------
* Implementation of ADMM-IVA by @tky823 in https://github.com/tky823/ssspy/pull/263
* Support ADMM-BSS_multi-penalty by @tky823 in https://github.com/tky823/ssspy/pull/265

Bug Fixes 🐛
------------
* Fix document deployment by @tky823 in https://github.com/tky823/ssspy/pull/255
* Update some variables depending on ``demix_filter`` instead of ``self.algorithm``. by @tky823 in https://github.com/tky823/ssspy/pull/260

Other Changes
-------------
* Release notes by @tky823 in https://github.com/tky823/ssspy/pull/246
* Add label for breaking changes by @tky823 in https://github.com/tky823/ssspy/pull/247
* Notebooks/getting started by @tky823 in https://github.com/tky823/ssspy/pull/248
* Update docs and notebooks to install ``ssspy`` from pypi by @tky823 in https://github.com/tky823/ssspy/pull/251
* Detect reformatting by @tky823 in https://github.com/tky823/ssspy/pull/258
* Make PDSBSSBase inherit IterativeMethodBase by @tky823 in https://github.com/tky823/ssspy/pull/262


**Full Changelog**: `v0.1.6...v0.1.7 <https://github.com/tky823/ssspy/compare/v0.1.6...v0.1.7>`_

v0.1.6
******

Summary
=======
In this version, the following BSS methods are newly added 🚀

- Fast MNMF
- IVA-IPA
- ILRMA-IPA

What's Changed
==============
* Bump up version to v0.1.5 by @tky823 in https://github.com/tky823/ssspy/pull/222
* Rename "XXXbase" to "XXXBase" by @tky823 in https://github.com/tky823/ssspy/pull/224
* Move default pair_selector by @tky823 in https://github.com/tky823/ssspy/pull/225
* Implement Fast MNMF by @tky823 in https://github.com/tky823/ssspy/pull/226
* Score-based permutation solver by @tky823 in https://github.com/tky823/ssspy/pull/221
* Specify flooring function in each method by @tky823 in https://github.com/tky823/ssspy/pull/228
* Solver for cubic equations. by @tky823 in https://github.com/tky823/ssspy/pull/230
* Consider corner case of cubic polynomial by @tky823 in https://github.com/tky823/ssspy/pull/233
* Use pytest-xdist by @tky823 in https://github.com/tky823/ssspy/pull/235
* Implement IVA-IPA by @tky823 in https://github.com/tky823/ssspy/pull/234
* Update links to reference by @tky823 in https://github.com/tky823/ssspy/pull/237
* Fix shape of varphi in tests of IVA by @tky823 in https://github.com/tky823/ssspy/pull/240
* End support of python=3.7 by @tky823 in https://github.com/tky823/ssspy/pull/243
* Stabilize IVA-IPA related algorithms by @tky823 in https://github.com/tky823/ssspy/pull/241
* Implementation of ILRMA-IPA by @tky823 in https://github.com/tky823/ssspy/pull/244


**Full Changelog**: `v0.1.5...v0.1.6 <https://github.com/tky823/ssspy/compare/v0.1.5...v0.1.6>`_
