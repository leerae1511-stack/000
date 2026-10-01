# Tool Pocket Generator V104 FINAL

## Provenance
V104 was built directly from the immediately preceding V103 FINAL build. V103 was the actual starting/source build. V98 was used only as the exact source for the approved photograph tool-outline implementation; it was not used as the starting build.

## Exact changes
1. Restored the exact V98 `extractPhotoSilhouette()` implementation for Detect exact tool outline.
2. Restored the exact V98 `measuredToolFromPhoto()` implementation so the detected outline and its physical measurement use the same proven V98 path.
3. Retained the existing V103 physical-grid calibration and all other V103 functionality.
4. Retained the existing historical inward semicircular FR STL construction already present in V103 (the V93/V79-era verified FR geometry path requested for this build).

## Problem / fix
V103 continued to produce an undersized detected outline on the user's photograph. The approved correction is to return to the exact V98 outline-detection and measurement path that previously worked, rather than further modifying the detector.

## Process / order
Photograph -> physical grid confirmation -> V98 tool silhouette detection -> V98 physical measurement bridge -> editable outline -> existing V103 downstream workflow/export.

## What was not changed
No changes were intentionally made to Close Profile, workspace rectangle behaviour, point editing, curves, Save Tool, JSON import/export, Geometry Check, FR controls, STL hand-off, or other unrelated V103 functions.

## FR STL
The existing V103 FR STL implementation is retained: inward semicircular recess, width controlling XY span, depth controlling Z floor, main cutter with recesses removed, FR cap added back from its shallower floor to tray top, and ear-clipping triangulation for concave profiles.

## Verification
- JavaScript syntax check: PASS
- ZIP integrity check: PASS
- Exactly four build files: PASS
- Exactly one README: PASS
- V103 -> V104 source provenance: PASS
- Exact V98 `extractPhotoSilhouette()` restored: PASS
- Exact V98 `measuredToolFromPhoto()` restored: PASS
- Existing V103 FR STL implementation retained: PASS
