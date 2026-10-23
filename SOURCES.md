# OCR corresponding source and independent modification

Download **DoView-OCR-Source-20261023.zip** from the same release as the engine:
https://github.com/DoView1/DoView-ai-engine/releases.
It includes the exact GEOS 3.13.1 source archive, Shapely 2.1.2 source (including
Windows build scripts), DoView OCR Python source, its native-build scripts and
hooks, dependency versions, and a README describing independent use/rebuilding.
SHA-256 values and source URLs are recorded in the archive and in the engine's
`licenses/publication/provenance.json`.

GEOS is licensed under LGPL 2.1. The complete LGPL text is supplied, as are
Shapely's BSD and DoView OCR's MIT texts. You may modify the OCR work for your
own use and debug such modifications. NVIDIA libraries remain under their own
terms; this permission does not relicense those libraries.

The viewer starts OCR as a separate executable and exchanges line-delimited JSON
through standard input/output. It does not link or load GEOS into the viewer.
The supplied source allows this independent OCR executable to be rebuilt and
run with a changed GEOS library. The shipped viewer's normal trusted-package
hash verification is not disabled, and modified packages are not represented
as official supported engine packages.

This source delivery follows the complete source / relinking approach described
in LGPL 2.1 section 6(a), rather than claiming that the stock viewer automatically
accepts arbitrary replacement DLLs. The boundary is the independently runnable
OCR program which uses the library. The documentation records this implementation
and delivery approach; it is not a legal certification of every possible use.

Official source references:

- GEOS: https://download.osgeo.org/geos/geos-3.13.1.tar.bz2
- Shapely: https://github.com/shapely/shapely/tree/2.1.2
- Shapely's pinned GEOS build:
  https://github.com/shapely/shapely/blob/2.1.2/.github/workflows/release.yml
- LGPL 2.1: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html
- Separate-process discussion:
  https://www.gnu.org/licenses/gpl-faq.html#MereAggregation
