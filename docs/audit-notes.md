# Audit and selection notes

[Back to the case study](../README.md)

## Scope

The confirmed set contains House of Fireborn, Back to My Roots, and Organic Humanoid Head / MetalMask. Palm is excluded at the ownerâ€™s request. The two head pages describe overlapping material and are represented by one repository.

The audit recursively covered the supplied Fireborn process folder, chair screenshots, every folder in `playblast_files_folders_links.txt`, the project pages and their local asset folders. Review included movie metadata and sampled frames, numbered-sequence detection, sample comparisons with existing videos, and inspection of process screenshots.

## Evidence and exclusions

- The separate `REEL01_Knitting / SC030` branch contains cloth camera experiments, Vellum captures and six AVI files. It was audited, but no reliable attribution to these four projects was established; its footage is excluded from their narratives. This includes 425 MiB AVIs and numerous similar camera paths.
- Automata is outside the confirmed scope. Sparse numbered hero stills and separate clay viewpoints are not treated as animation.
- Repeated movie copies were identified by SHA-256. The Fireborn collection duplicates nine movies in the linked R&D directories; each selected movie is included once.
- The charcoal JPG batch matches its 93-frame AVI. The coating JPG batch matches its 136-frame movie. Existing movies were used, with delivery compression, rather than rebuilding these sequences.
- The incomplete `Viscosity_By_8.avi` cannot be decoded. Its numbered `.pic` batch was recoverable through Houdini `iconvert` and is included in the head repository.
- Movie frame rates are preserved. 24 fps is the documented review assumption for newly encoded image sequences, based on adjacent playblasts. No scene FPS was recovered directly.
- Masters, Houdini scenes and caches remain in their original locations. This repository is a process-media case study, not a reproducible simulation project.

## New sequence encodes

| Review | Original batch | Frames | FPS |
|---|---|---:|---:|
| [mushroom-cam21](../media/video/mushroom-cam21.mp4) | `D:\Apps\MaisonDatelier\assets\images\palm\original_palm\4k\FRez_cam21_begining_4k\HRez_cam21.{frame}.png + D:\Apps\MaisonDatelier\assets\images\palm\original_palm\4k\FRez_cam21_4k\HRez_cam21.{frame}.png` | 1â€“100 (100) | 24 |
| [closeup-cam7-continuation](../media/video/closeup-cam7-continuation.mp4) | `D:\Apps\MaisonDatelier\assets\images\palm\original_palm\FRez_cam7\FRez_cam7.Redshift_ROP33.{frame}.png` | 103â€“122 (20) | 24 |

## Delivery

H.264, yuv420p, fast-start MP4; source aspect ratio retained, up to 1920 Ã— 1080. Images are web delivery copies, resized only above 2800 pixels; larger PNGs in the head, chair and Palm archives use high-quality WebP compression. Most GIFs are 640 pixels wide; the noisy HQ transformation preview uses 480 pixels and 8 fps. Compression settings and file checksums are recorded in the manifest.

## Larger source files

| Source | Original | Delivery |
|---|---:|---:|
| `palm-video-portfolio.mp4` | 204.42 MiB | [6.62 MiB](../media/video/portfolio-film.mp4) |

## Palm sequence matching and re-audit

- `FRez_cam21_begining_4k` PNG frames 1–48 and `FRez_cam21_4k` PNG frames 49–100 were joined into `mushroom-cam21.mp4`. Parallel JPG exports were not encoded again.
- `FRez_cam7_beginning` frames 50–102 match the existing 53-frame close-up movie (first, middle and last samples checked). That movie was reused. Only `FRez_cam7` frames 103–122 were newly converted as a continuation.
- `FRez_cam8` frames 102–123 match the existing 22-frame Original Palm movie. The supplied 44-frame slow version covers that view and was selected for review.
- The 780-frame portfolio export contains the same finished compositions as the existing edited movie, in a different edit. The existing 511-frame portfolio film was selected rather than making a redundant portfolio delivery.
- The five numbered drawings are separate concept stages, not animation frames. Their review is labeled as a still comparison.
- `rec709_vimeo_satu-contrast_stronger_90000kbs_youtube00086863.png` was unreadable and excluded. The composition is represented by other intact media.
- The hand holding an electronic object and the `NATURAE` website/video captures are external reference imagery with no established production relationship; they were inspected and excluded. Near-duplicate capture exports were also omitted.
- The new Houdini image directly shows a Color SOP using Random from Attribute with the point attribute `variant`; the README limits the technical explanation to what is visible.
