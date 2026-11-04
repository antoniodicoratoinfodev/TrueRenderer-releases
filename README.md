# TrueRenderer

## Downloads

<!-- macos-download:start -->

| Platform | Download | Version |
|---|---|---|
| **macOS · Apple Silicon** | **[Download for Mac — ZIP · 58 MB](https://github.com/antoniodicoratoinfodev/TrueRenderer-releases/releases/download/v0.1.7-macos.20261104/TrueRenderer-0.1.7-macos.20261104-arm64.zip)** | 0.1.7 · Preview |
| **Windows · x64** | **[Download for Windows — Installer EXE](https://github.com/antoniodicoratoinfodev/TrueRenderer-releases/releases/download/v0.1.8-windows.20261104/TrueRenderer-0.1.8-Setup-x64.exe)** | 0.1.8 · Preview |

<!-- macos-download:end -->

[Installation instructions](INSTALLAZIONE.md) · [SHA-256 checksum](https://github.com/antoniodicoratoinfodev/TrueRenderer-releases/releases/download/v0.1.7-macos.20261104/SHA256SUMS.txt) · [All releases](https://github.com/antoniodicoratoinfodev/TrueRenderer-releases/releases)

**Mac:** extract the ZIP, keep the entire folder together and start **Avvia TrueRenderer.command**. This experimental preview is ad-hoc signed and is not notarized. Downloads are publicly available; no GitHub account is required.

**Windows:** download and run the installer for Windows 10/11 x64. This experimental preview is unsigned; SmartScreen or Smart App Control may block it. See [installation instructions](INSTALLAZIONE.md#windows-x64) and the [Windows SHA-256 checksum](https://github.com/antoniodicoratoinfodev/TrueRenderer-releases/releases/download/v0.1.8-windows.20261104/TrueRenderer-0.1.8-Setup-x64.exe.sha256).

[Release notes](CHANGELOG.md) · [Compatibility](COMPATIBILITA.md) · [Roadmap](ROADMAP.md) · [Support](SUPPORTO.md)

---

### Your photographs. Your colour. Your way.

RAW development, expressive colour tools and photographic layers in one desktop workspace. TrueRenderer takes you from choosing your best frames to shaping the final image, with your originals untouched and your work stored locally.

![Avalanche Lake in Develop, with Explorer open and white-balance and light controls](assets/develop.png)

Bring out the light you remember. Give a series its own colour palette. Refine one part of a photograph without changing the rest. Compare your decisions as you work, then export at the size and precision you need.

**No account, photo upload or cloud subscription is required.**

## Shape the light. Make the colour yours.

Start with the essentials: exposure, contrast, highlights, shadows and white balance. Go further with editable curves, sampled colour corrections and four-wheel grading for shadows, midtones, highlights and the whole image.

In Develop, use **Auto white balance** to sample an unclipped white or neutral grey region. RAW sampling offers **1×1, 3×3, 5×5 or 11×11** areas, with 5×5 as the default; RGB photographs use a 3×3 sample. The correction can be undone, and **Esc** cancels the eyedropper.

TrueRenderer works in **linear Rec.2020 floating point**, giving its photographic adjustments a wide numerical range. Histograms, tonal-level sampling and pixel inspection help you connect what you see with the image data.

![Four-wheel grading on a photographic layer, with Library open](assets/colour.png)

| Make the image your own | Tools to get there |
|---|---|
| Balance light | Exposure, brightness, contrast, highlights, shadows, whites, blacks and automatic exposure |
| Set the white balance | RAW Temperature and Tint, As shot, automatic balance and neutral-area sampling |
| Sculpt the tones | Point curves, individual RGB curves, luminance and parametric curves; tonal levels with histograms and black, grey and white samplers |
| Refine individual colours | Saturation, vibrance, eight-band HSL, sampled colour and uniformity controls; selective colour and channel mixing |
| Create a signature palette | Four-wheel grading, colorize, colour filters, gradient maps and black-and-white mixing |
| Bring out detail | Texture, clarity, dehaze, sharpening and luminance/chroma noise reduction |
| Refine the optics | Manual distortion, vignette, chromatic aberration and defringe controls |

The searchable **Tools** catalogue puts adjustments within reach. Each tool has its own photographic symbol and visual controls; hover over a name to see what it does, in English or Italian.

For a vintage texture, use **Creative grain** in **Presence and detail**. Enable **Add grain**, choose **Uniform** or **Gaussian**, then adjust **Grain amount**, **Grain size (px)** and **Grain opacity**. **Monochrome grain** adds neutral grain; turn it off for coloured speckles. **New pattern** changes the arrangement, which is saved with the edit. Disabling the effect keeps its settings. Judge fine grain at 100% with **Verify final rendering**; smaller exports naturally soften it.

![Shared photographic and raster Tools beside Grand Teton at sunrise, with Explorer open](assets/tools.png)

## Build the look, layer by layer

The larger dot in a Develop section or layer effect switches that tool off and on.
Disabled tools retain their values, including after saving and reopening the edit.
An illuminated dot identifies an enabled tool with adjustments.

Keep different creative decisions independently editable. Add an adjustment to a new photographic layer or to the selected layer, then control where it acts and how strongly it contributes.

Use **Develop**, **Layers**, **Tools** and **Export** on the original photograph.
**Layer 0 — Starting photo** stays at the bottom of the stack and has its own visibility control.
Adjustment layers, masks, Paint, Eraser, Clone, Heal, Quick heal and Move remain
reversible parts of the photo recipe stored in your local library.

**Tools** follows one design in photo and raster editing, with three groups:

- **Shared adjustments:** the searchable colour and tonal catalogue, with the choice of a new layer or the selected layer.
- **Retouch and selection:** navigation, transformations, brushes, cloning, healing and freehand, polygonal or rectangular selections.
- **Raster composition:** independent images, blank pixel layers, visible copies and selected pieces. On a photograph, a **Raster** badge identifies commands that require conversion.

### Continue into raster editing

A raster composition starts with a confirmation. Complete RAW development first
when possible, then create a separate `.truerenderer` project with the developed
photo at layer 0 and new content above it. **Editing raster** identifies the mode
at the top of the inspector. Develop, Layers, Tools and Export keep the same
workspace and shared controls. **Image layers** contains independent images;
**Layer adjustments**, under **Adjustments and masks**, edits the selected image.
Its eye button can hide or reveal the starting photo, including after conversion
from a photograph whose base was hidden.

Return to the original photograph with the return-to-photo command. Its confirmation
explains that unsaved raster changes will be discarded; saved projects remain
available. New converted projects retain the original reference when reopened.
Older projects or moved photographs can be linked to an original through the
inspector. Save the project to retain that reference.

Create a blank canvas from **Open**, choosing pixel dimensions, units, PPI and
background. Projects appear beside photographs in the grid and filmstrip. They
embed their images and keep editable layers, adjustments and masks. Save, Save as
and Export project copy distinguish the working project from the finished image;
previous saves are retained as uniquely named `*.previous-*.truerenderer` files.

Photo-based compositions retain the original pixel dimensions and declared X/Y
PPI. Export size and PPI overrides affect the exported copy. Documents admit up to
67,108,864 pixels per canvas/image and 2 GiB of raster assets and masks, subject to
available memory. The reader accepts project versions 1, 2 and 3; new projects
with an original reference or CMYK destination use version 3. Sensor development
is embedded as pixels inside the project, so return to the RAW to change its
sensor white balance or rendering engine.

Photo retouch uses CPU replay and can be slower on large images. Its bounded
recipe admits 128 strokes and 1024 total path/selection points within 48 KiB.
See [compatibility and limits](COMPATIBILITA.md).

- **Local adjustments:** combine brush, linear and radial gradients, luminance and hue masks; add, subtract, intersect, soften and invert their coverage.
- **Independent layer controls:** name, duplicate, reorder, hide or lock layers and adjust Opacity and Fill.
- **Reusable looks:** save selected layers, preview them on another photograph and choose their intensity, with optional masks.

![Photographic layers and editable local adjustments, with Library open](assets/layers.png)

**Experiment freely.** Undo, Redo, Reset all and Before/After keep decisions reversible. Double-click a photographic slider to restore its default. Copy selected light, curve and RGB colour adjustments between photographs to carry a treatment through a series.

Photographic sliders move continuously. Hold Shift while dragging for fine adjustments of 0.01 or less, or use the arrow keys; Shift + arrows makes the step ten times smaller. Numeric fields accept additional decimals, including layer opacity and tool settings. Parameters defined as integers retain their units.

Colour guides appear directly in the slider tracks. The path bar has matching icons to show or hide the left and right panels. The filmstrip toggle is at the right of the bottom status bar. Keyboard shortcuts remain **Cmd/Ctrl+B** for the left panel, **I** for Develop / Information and **T** for the viewer filmstrip.

Choose the RAW engine in **Settings → Previews and RAW**, then **Apply and save**. The top bar shows the applied default; **Photo:** identifies a different engine stored in the selected RAW photo’s recipe. Changing the default preserves existing edits and compatible previews, including decoded JPEGs in the current session.

On macOS, choose **Previews → Embedded** (**Integrata** in Italian) to browse the camera JPEG inside a RAW without developing the sensor. It can work even when the selected RAW engine does not support the camera. The view is capped at 2048 pixels and retains the camera’s rendering; FP32 display processing does not restore missing RAW detail or dynamic range. Saved RAW edits are preserved but suspended. Choose **Develop RAW · Full** to resume editing or export. Missing previews and unsupported containers are reported explicitly. First-load time depends on the file and storage; cached navigation can be much faster. See [compatibility and limits](COMPATIBILITA.md).

On Windows, **Embedded** also supports RGB edits, crop, soft proofing and raster export up to 2048 pixels. The edit recipe is shared with Standard/Full; sensor white balance is preserved but suspended on the camera JPEG. Changing to RAW development can change the rendering. Only visible images and nearby previews are prepared while browsing.

Exposure and tone-curve previews preserve the detail available in the viewer, including at 100%. Later clicks on the interface do not restart a reduced editing preview. Spatial filters and active layers still use provisional previews during adjustments.

While you pause on a photograph in Fit, TrueRenderer prepares its detail and applied adjustments in the background for the first zoom. Preview quality stays unchanged. Immediate zooming, recent edits or limited memory can still require refinement.

## Give every frame the right composition

Crop directly on the photograph with draggable edges, a rule-of-thirds grid and free, original, preset or custom aspect ratios. Lock the proportions, switch orientation, move the frame or move the photograph inside it. Keyboard controls help with fine adjustments.

Rotation, flips, straightening and perspective controls complete the composition tools. Masks follow the photograph through crop and rotation, and the original remains available for a different framing later.

![Interactive crop with aspect-ratio controls, a composition grid and Explorer open](assets/crop.png)

## See the differences that matter

Choose between two frames with **side-by-side comparison and synchronized navigation**. Assign photographs to A and B from the context menu, keep the pair across folders, and inspect detail at physical 1:1. Use Before/After to compare the initial rendering with your current adjustments.

![Photographic comparison with synchronized navigation and Library open](assets/compare.png)

Shutter speed, aperture, ISO, focal length and lens information sit alongside the image, helping you understand each frame as you select and develop it.

## Find your keepers. Keep them organized.

Browse folders in **Explorer**, review a thumbnail grid in **Library**, or stay with the photograph and its filmstrip. Favourites, navigation history, search and filters help you return to the images that matter.

Use **star ratings, colour labels, reject flags and keywords** to organize a shoot. Context menus bring ratings, comparison, adjustments, file navigation and export to the photograph you are working on.

![The photograph grid with Explorer open on the demonstration gallery](assets/library.png)

Your originals remain read-only. Editing recipes, annotations and saved looks live in the local library and its backups.

## Choose your RAW rendering engine

Choose a rendering engine in Settings to explore different interpretations of your RAW files:

- **TrueRenderer**: our flagship independent RAW engine, available on macOS as **trueRendererExperimental 32fp**. Its 32-bit floating-point pipeline preserves negative values and values above nominal white, offering greater numerical headroom than the app's 16-bit integer LibRaw paths. Independent decoding, directional reconstruction and sensor-aware highlight treatment give it a dedicated path from the sensor mosaic to the developed image.
- **Apple RAW**: native macOS RAW development through Apple's camera support and rendering pipeline. Camera compatibility follows the decoder installed with macOS.
- **LibRaw AHD**: LibRaw decoding with Adaptive Homogeneity-Directed demosaicing, providing an alternative rendering for comparison.
- **LibRaw bilinear**: LibRaw decoding with bilinear interpolation, a straightforward rendering option for comparison.

TrueRenderer includes Temperature and Tint controls, neutral-area white-balance sampling, an As shot reset and DNG export of the decoded sensor mosaic. Its fp32 headroom is a concrete advantage; the best-looking rendering still depends on the photograph and the adjustments you choose.

### Camera compatibility

The following camera models and recording modes are currently supported by **TrueRenderer's independent engine**:

| Camera | RAW format | Supported recording modes |
|---|---|---|
| **Nikon D750** | NEF · Bayer | Full-frame FX, 14-bit lossless compressed RAW |
| **Nikon D800** | NEF · Bayer | Full-frame FX, 12-bit or 14-bit lossless compressed RAW |
| **Fujifilm X-T5** | RAF · X-Trans | Full-resolution, 14-bit lossy compressed RAW |

Supported Bayer and X-Trans **DNG files** can also use the independent engine. Compatibility depends on the file's compression and calibration features. Apple RAW and LibRaw have their own camera coverage.

**Camera compatibility is expanding week by week.** I am continually adding support for new models and recording modes. If you need a particular camera implemented, contact me with the manufacturer, exact model, RAW format, bit depth and compression settings, plus an original RAW sample if available. Your requests help shape the next additions.

## Stay in the photographic flow

GPU acceleration for light and colour adjustments works alongside parallel CPU processing. On a verified Vulkan device, supported combinations of exposure, noise reduction, texture, geometry and layers can stay on the GPU through display. Supported layer stacks reuse the prepared image for sampled colour, light, tonal levels and opacity changes, both at native zoom and in Fit view. Editing keeps the detail of the loaded preview throughout slider, tool and layer gestures; the last complete image stays visible while an update is calculated. Folder loading prepares detail, saved adjustments, thumbnails and the active image's GPU resources, and reuses completed results from the disk cache. Choose foreground loading to finish preparation before browsing, or keep working while it runs in the background. Editing gestures take priority over background preparation. Cache and memory limits still apply; unsupported tool combinations and limited memory can require slower CPU updates. Direct3D 12 retains the separately verified point and layer paths while the complete graph's release compilation remains under investigation.

Choose **Standard or Full preview quality**, globally or for an individual photograph. Set CPU, GPU and memory preferences to suit your machine, switch between Fit and physical 1:1, and choose an English or Italian interface with 100%, 150% or 200% UI scaling.

## Finish with the output you need

Choose **sRGB**, **Adobe RGB (1998)**, **Display P3**, **linear Rec.2020** or
**CMYK with an output ICC** as the destination. **Profile and soft proof** in
Develop lets you preview the destination while working on a RAW/photo or raster
composition; the proof remains visible when switching to Layers, Tools or Export.
Crop keeps your proof setting. Photographic tonal-level input analysis temporarily
suspends the proof to measure the input pixels, then restores your setting when
you leave the analysis.
The working calculations stay in extended linear Rec.2020 at 32 bits.

Photo and raster exports share RGB destinations for **JPEG, PNG and TIFF16**.
CMYK uses **TIFF16** with four ink channels and the ICC embedded. On macOS, the
system's generic CMYK profile is available; select a printer-provided ICC for a
specific printing process. The generic profile does not describe a particular
printer, paper or ink. Float TIFF and DNG retain their explicit colour contracts.

Export at native resolution or choose a target long edge and output PPI. PNG and
TIFF offer 16-bit output; floating-point TIFF preserves extended values in the
photo workflow. Project saving remains separate from exporting the finished image.

For scientific imagery, TrueRenderer also opens **2D FITS images**, with linear or asinh display, a histogram and native-value inspection.

## Try it with the included photographs

Open an image or a folder, select a photograph and choose **Develop**. Use **Adjustments** for the essentials, **Tools** to find a creative control, and **Layers** to build a local treatment. The **Actions** menu gives you looks, crop, copy/paste and output verification.

Four public-domain landscapes are included in **Library**, under **Sample photos**, including in the macOS bundle for offline use. Start there to explore the workspace. Photograph credits are included in [NOTICE.md](NOTICE.md).


## Rights and credits

TrueRenderer is proprietary software. Access to this repository does not grant a general license to run or redistribute it; prior permission from the owner remains required under the unchanged [license](LICENSE). See [third-party notices and photograph credits](NOTICE.md).

