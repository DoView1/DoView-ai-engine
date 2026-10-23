# DoView AI Engine — download and component terms

The AI engine is an optional local component for DoView. Download it only if you
want local translation, OCR, summaries, or questions. It is a large Windows x64
package; the application shows its download size and required free storage before
installation. Once installed, inference is local. Downloading the package and
checking viewer updates still use the network. No user-count telemetry is added.

By choosing **Download and install**, you acknowledge the component notices below
and agree to the applicable NVIDIA terms for the included NVIDIA libraries.
If you do not agree, cancel the installation; normal viewing remains available.
The component license texts control their respective components. This page does
not relicense third-party software and does not change the viewer's license.

## Included licenses

- **Gemma 4 E4B derivative / Q4_K_M quantization, OCR models:** Apache 2.0.
  See the bundled model cards, `licenses/Apache-2.0.txt`, and the
  [official Gemma 4 Apache 2.0 text](https://ai.google.dev/gemma/apache_2).
  The E4B weights were modified by the named upstream derivative author and
  quantized by mradermacher; DoView does not present them as an unmodified Google
  model. There is no separate Gemma account or legacy Gemma license acceptance
  step in this download flow.
- **llama.cpp and DoView-authored OCR source:** MIT, as stated in their bundled
  license files. Other OCR dependencies retain their licenses, listed in
  `ocr/_internal/licenses/distributions/index.json`.
- **GEOS 3.13.1:** LGPL 2.1; **Shapely 2.1.2:** BSD 3-Clause. The accompanying
  `DoView-OCR-Source-20261023.zip` supplies corresponding source and instructions
  to modify, rebuild, and run the independent OCR program with a modified GEOS.
  DoView permits private modification of that OCR work and debugging such
  modifications. Normal viewer package integrity verification remains enabled;
  the official viewer accepts its published trusted package, while the supplied
  source can be built and run independently. See [SOURCES.md](SOURCES.md).
- **Fonts:** SIL Open Font License 1.1. Copyright notices and font-specific
  licenses are included. The OFL does not apply to images/documents rendered
  using the fonts.

## NVIDIA libraries

The package contains NVIDIA CUDA 12.4 libraries for translation and CUDA 13 /
cuDNN 9 libraries for OCR. They are licensed by NVIDIA, not under DoView's MIT
license. They are included only as private dependencies of the DoView AI
application, not as a general-purpose SDK for other applications.

Read the [CUDA 12.4.1 EULA](https://docs.nvidia.com/cuda/archive/12.4.1/eula/index.html),
[CUDA 13.0.0 EULA](https://docs.nvidia.com/cuda/archive/13.0.0/eula/index.html), and
[cuDNN EULA](https://docs.nvidia.com/cudnn/latest/reference/eula/).
The exact supplied license/acknowledgement copies are retained in the engine's
`licenses/publication/` and `ocr/_internal/licenses/` directories. The latter
cuDNN page is an upstream current URL, not a claim of a version-pinned document;
the distributed text is captured and hashed with this package.

NVIDIA's terms include limitations on copying, redistribution, modification,
reverse engineering of NVIDIA components, and use outside the granted license,
as well as warranty disclaimers and applicable export restrictions. Read the
full texts for their scope. These restrictions do not replace the independent
rights granted for GEOS, Shapely, DoView OCR source, or other open-source parts.
No NVIDIA endorsement of DoView is claimed.

## Scope and results

The initial supported package is Windows x64. GPU execution depends on compatible
hardware/drivers and free resources; it does not certify every GPU or CPU-only
computer. Resource checks, cancellation, byte-count checks and SHA-256 verification
remain active. Translation and OCR can be wrong; review results before saving.
Speech-bubble dialogue is the primary image translation scope. No five-second
first-request guarantee is made.
