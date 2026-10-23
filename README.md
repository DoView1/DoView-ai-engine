# DoView AI Engine

Optional local AI engine files for [DoView](https://github.com/DoView1/DoView-release).
Use the viewer's **Settings → AI → Download and install** control in a version
whose download button is enabled. The viewer downloads and checks the compatible
package before activating it. You do not need a separate Python installation.

DoView 1.2.11 predates public engine download configuration and only imports a
prepared engine folder. Install the viewer update that advertises engine download
support; uploading files here does not activate the old application's button.

The engine installs once and is reused for local translation, OCR, summaries and
questions. Viewing images and documents does not require it. This repository is
for engine distribution documents and component/source assets, not the whole
viewer source repository.

- [Download/component terms](TERMS.md)
- [Corresponding source and modification](SOURCES.md)
- [Release assets](https://github.com/DoView1/DoView-ai-engine/releases)

The engine includes its component notices and immutable file hashes. NVIDIA
libraries, models, GEOS and fonts retain their own licenses. The OCR corresponding
source archive is available alongside the engine assets. No usage telemetry or
account registration is added by this engine distribution.
