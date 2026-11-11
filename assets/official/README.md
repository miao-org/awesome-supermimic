# Official SuperMimic media credits

The three previews come from the [SuperMimic project website](https://supermimic.github.io/), by Qiayuan Liao, Yiyang Shao, Junfeng Long, Kevin Zakka, Roberto Horowitz, Pieter Abbeel, and Koushil Sreenath (UC Berkeley). The conference talk is the authors' CoRL 2026 presentation, supplied for inclusion in this catalog.

They illustrate **SuperMimic: Scaling Humanoid Whole-Body Control with One Differentiable World Model**, CoRL 2026. These are the original authors' demonstrations and explanation, not experiments run by this collection.

| Preview | Source | Source duration | GIF resolution |
| --- | --- | --- | --- |
| [simulation-wide.gif](simulation-wide.gif) | [Original MP4](https://supermimic.github.io/media/hero/hero_montage_desktop.mp4) | 14.20 s | 480 × 211 |
| [world-model.gif](world-model.gif) | [Original MP4](https://supermimic.github.io/media/world-model/wm_on.mp4) | 12.92 s | 960 × 435 |
| [real-g1-wide.gif](real-g1-wide.gif) | [Original MP4](https://supermimic.github.io/media/real/real_bay-wide.mp4) | 6.77 s | 480 × 211 |

Retrieved on 2026-10-26. Each GIF preserves the full corresponding source clip, its frame order and playback speed. The world-model preview is 960 pixels wide; the supporting simulation and real-G1 previews use matching 480 × 211 canvases. The real-G1 clip retains its complete original framing with no added borders. The simulation preview removes 20 pixels of unused white space above and 39 below its 480 × 270 scaled frame; the robot motion remains in view. All previews are sampled at 12 fps and palette-quantized for GitHub playback. Original transitions remain intact. No generated imagery, motion interpolation, or speed changes were added. GIF frame timing is rounded to centiseconds, with total duration within 0.1 seconds of each source.

- **Simulation:** the official site's hero montage of G1 whole-body motion.
- **World model:** the official prediction overlay; the blue figures depict learned world-model predictions over simulator motion.
- **Real G1:** the official bay-side hardware demonstration.

## Official CoRL 2026 talk

| Asset | Source | Duration | Format |
| --- | --- | --- | --- |
| [supermimic-official-talk-2026.mp4](supermimic-official-talk-2026.mp4) | CoRL 2026 presentation by Qiayuan Liao and the SuperMimic authors | 8:35 | H.264 High / AAC, 1280 × 720, 30 fps, 33 MiB |
| [supermimic-official-talk-poster.jpg](supermimic-official-talk-poster.jpg) | Frame at 7:50 showing the final code-release slide | — | JPEG, 960 × 575 |

The supplied QuickTime recording was transcoded to MP4 with its original frame geometry, frame order, playback speed, and stereo audio preserved. Video uses H.264 CRF 24 and audio uses AAC at 96 kbps; the MP4 is fast-start enabled for immediate playback access.

## Rights and attribution

All rights in the source footage, conference talk, slides, and paper figure remain with the original rights holders. These third-party assets are **excluded from this repository's CC0 dedication**. The source website did not state a separate media license when checked; this collection does not grant reuse rights to the footage, talk, or figure. Follow the source website and paper for the authors' materials and terms.

## Original paper framework

[training-loop.png](training-loop.png) reproduces **Figure 2** from [SuperMimic, arXiv:2610.28480v1, page 4](https://arxiv.org/pdf/2610.28480v1#page=4), by the authors credited above. Retrieved on 2026-10-26. The figure shows the original training loop; the README separately summarizes its legend and links to [Algorithm A.1 on page 15](https://arxiv.org/pdf/2610.28480v1#page=15).

The diagram is rendered directly from the PDF at 288 dpi as a 1632 × 548 PNG. Only surrounding page content is excluded; all diagram panels, labels, arrows, colors and symbols are preserved. The crop in PDF points is `(x=102, y=69, width=408, height=137)`, measured from the page's top-left corner. The figure has not been redrawn or generated. The paper's arXiv record lists the [arXiv non-exclusive distribution license](https://arxiv.org/licenses/nonexclusive-distrib/1.0/); this is not a CC0 asset.

## Conversion

Each original MP4 is sampled at 12 fps. The geometry filter depends on its role:

| Preview | Geometry filter |
| --- | --- |
| Simulation | `scale=480:-1:flags=lanczos,crop=480:211:0:20` |
| World model | `scale=960:-1:flags=lanczos` |
| Real G1 | `scale=480:-1:flags=lanczos` |

After scaling and the simulation-only crop, frames use square pixels, a 128-color palette, Bayer dithering (`bayer_scale=4`), and an infinite GIF loop. Original playback speed is preserved for every clip. World-model and real-G1 previews retain their complete source framing.
