# Adobe → Affinity v3 keyboard shortcut files — mapping notes

A best-effort mapping of Adobe Photoshop and Adobe Illustrator keyboard shortcuts for Affinity v3 Pixel and Vector workspaces, respectively.

**Windows** (`.afshort`):

| File | Target studio | Workspaces inside |
|---|---|---|
| `affinity_pixel_v3_shortcuts_based_on_photoshop_windows.afshort` | **Pixel Studio** | `PhotoWorkspace.xml` + `PixelWorkspace.xml` (identical, for v2/v3 naming compatibility) + `LiquifyWorkspace.xml` |
| `affinity_vector_v3_shortcuts_based_on_illustrator_windows.afshort` | **Vector Studio** | `VectorWorkspace.xml` |

**macOS** (`.affshortcuts`):

| File | Target studio |
|---|---|
| `affinity_pixel_v3_shortcuts_based_on_photoshop_mac.affshortcuts` | **Pixel Studio** + **Liquify** |
| `affinity_vector_v3_shortcuts_based_on_illustrator_mac.affshortcuts` | **Vector Studio** |

**How to load:** Affinity → `Edit` menu (Windows) / `Affinity` menu (Mac) → **Settings** →
**Keyboard Shortcuts** → **Load…** and pick the file for your platform. Loading **replaces** all
shortcut allocations in the included workspaces (other studios are untouched). Save your current
setup first if you care about it.

The Mac files were built by editing a **real Affinity v3 macOS shortcut export** (all 14 studios,
~11,200 assignable entries), so their schema is guaranteed correct: only the Pixel/Liquify studios
(Photoshop file) and Vector studio (Illustrator file) were modified; every other studio is
byte-identical to a factory v3 export. Adobe keys were translated to their Mac forms
(Ctrl→Cmd, Alt→Opt), using Adobe's actual macOS shortcuts where they differ from Windows.

The good news up front: Affinity v3's defaults already match Adobe in a lot of places —
`[ ]` brush size, `Shift+[ ]` hardness, number-key opacity, `Shift+`numbers for flow,
`Alt+Shift+letter` blend modes, `X`/`D` color swap/defaults, `Q` Quick Mask, `Ctrl+E` merge down,
`Ctrl+Alt+Shift+E` stamp/merge visible, `Ctrl+Shift+S` Save As, `Ctrl+Alt+Shift+W` Export,
`Ctrl+Alt+I` image size, `Ctrl+Alt+C` canvas size, `Shift+F5` Fill, `Shift+F6` Feather,
`Ctrl+Alt+R` Refine Edges (Select & Mask), layer stacking `Ctrl+] [` / `Ctrl+Shift+] [`,
group `Ctrl+G` / `Ctrl+Shift+G`, `Ctrl+]`/`[` / front/back, text size `Ctrl+Shift+.` / `,`
(Affinity spells these `Ctrl+>` / `Ctrl+<` — same physical keys), guides `Ctrl+;`, grid `Ctrl+'`,
rulers `Ctrl+R`, zoom `Ctrl+=` / `Ctrl+-` / `Ctrl+0` / `Ctrl+1`. All of those are preserved in the files.

---

## Photoshop file — notable mappings

### Tools (all single-key, matching PS)
V Move · M Marquees (cycle) · L Lasso→Freehand Selection · W Quick Select/Magic Wand→Selection Brush/Flood Select ·
C Crop · I Eyedropper · J Healing tools (cycle) · B Brush · **S Clone Stamp** (Affinity default was K) ·
E Erasers (cycle) · G Gradient/Bucket→Fill tools (cycle) · O Dodge/Burn/Sponge (cycle) · P Pen ·
T Text (cycle) · A Path/Direct Selection→Node · U Shapes (cycle) · H Hand · Z Zoom · Q Quick Mask ·
D Default colors · X Swap colors · Y Pixel tool (PS's History Brush has no equivalent) ·
R Color Replacement Brush (PS's Rotate View tool has no equivalent)

### Adjustments & image
| Photoshop | Affinity Pixel Studio |
|---|---|
| Ctrl+L Levels / Ctrl+M Curves / Ctrl+U Hue-Sat | identical (Levels / Curves / HSL) |
| **Ctrl+B Color Balance** | → Color Balance adjustment (v3 default Ctrl+B = Brightness/Contrast was moved off; PS has no shortcut for it) |
| **Shift+Ctrl+U Desaturate** | → Black & White adjustment (closest equivalent; its own default Alt+Shift+Ctrl+B also kept) |
| **Shift+Ctrl+L Auto Tone** | → Auto Levels |
| **Alt+Shift+Ctrl+L Auto Contrast** | → Auto Contrast |
| **Shift+Ctrl+B Auto Color** | → Auto Colors |
| Ctrl+I Invert | → Invert Pixels (destructive, exactly like PS) |
| **Shift+Ctrl+X Liquify** | → Live Liquify filter |
| Alt+Shift+Ctrl+S Save for Web | → Export (dual with v3's Alt+Shift+Ctrl+W) |

### Layers & selections
| Photoshop | Affinity |
|---|---|
| Ctrl+J Layer via Copy | → Duplicate (already Affinity's default) |
| **Shift+Ctrl+E Merge Visible** | → Merge Visible (Affinity's own Ctrl+Alt+Shift+E = PS's Stamp Visible also kept; "Merge Selected" was unbound to free the combo) |
| **Alt+Ctrl+G Clipping Mask** | → Move Inside |
| **Shift+Ctrl+N** and **Alt+Shift+Ctrl+N** New Layer | → New Pixel Layer (both) |
| **Ctrl+/ Lock Layers** | → Lock |
| **Alt+. / Alt+, top/bottom layer** | → Select Top/Bottom Layer |
| Alt+] / Alt+[ next/prev layer | identical (Affinity default) |
| **Shift+Ctrl+D Reselect** | → Reselect |
| **Shift+F7 Inverse** (legacy) | → Invert Pixel Selection (dual with Ctrl+Shift+I) |
| Ctrl+A / Ctrl+D / Shift+Ctrl+I | identical |
| Alt+Ctrl+A Select All Layers | identical |

### Panels & app
**F5 Brushes · F6 Color · F7 Layers · F8 Info · Alt+F9 Macro panel** (PS Actions) ·
**Ctrl+K Settings** (PS Preferences; Affinity's own Ctrl+, also kept) · **Alt+Shift+Ctrl+K** also opens Settings
(closest to PS's Keyboard Shortcuts dialog) · **Shift+Tab** show/hide panels (dual with v3's Ctrl+Shift+H) ·
**Ctrl+H** show/hide pixel selection edges (PS Extras; best available equivalent) ·
**Alt+Ctrl+;** Lock Guides · F1 Help · Tab Toggle UI · Ctrl+Tab next document.

### Liquify studio (PS Liquify keys)
**W Forward Warp** (was P) · **R Reconstruct** ✓ · **E Twirl** (was T) · **S Pucker→Pinch** (was U) ·
**B Bloat→Punch** (was N) · **O Push Left** (was L) · **F Freeze** ✓ · **D Thaw** (was W) ·
C Mesh Clone ✓ (+ M ≈ PS Mirror) · H Hand ✓ · Z Zoom ✓ · Turbulence unbound (no PS equivalent).

---

## Illustrator file — notable mappings

### Tools
V Selection ✓ · A Direct Selection→Node ✓ · P Pen ✓ · T Type ✓ · N Pencil ✓ · B Paintbrush→Path Brush ✓ ·
G Gradient→Fill tool ✓ · I Eyedropper ✓ · W Blend ✓ (same in both!) · H Hand ✓ · Z Zoom ✓ ·
**M Rectangle** · **L Ellipse** (U also still cycles shapes) · **Shift+M Shape Builder** ·
**Shift+W Width tool** → Stroke Width · **E Free Transform** → Point Transform tool (closest; F also kept) ·
**Shift+O Artboard tool** · **\ Line Segment** → Line tool (see deviations) ·
S Shape Builder / O Contour / C Corner / K Knife / R Vector Flood Fill / Y Transparency (v3 defaults kept;
AI's Scale/Reflect/Scissors/Live Paint/Magic Wand tools have no Affinity equivalents — see below).

### Objects & paths
| Illustrator | Affinity Vector Studio |
|---|---|
| Ctrl+G / Shift+Ctrl+G Group/Ungroup | identical |
| Ctrl+] [ and Shift+Ctrl+] [ arrange | identical |
| **Ctrl+2 Lock · Alt+Ctrl+2 Unlock All** | → Lock / Unlock All (Affinity's own Ctrl+L lock also kept) |
| **Ctrl+3 Hide · Alt+Ctrl+3 Show All** | → Hide / Show All |
| **Ctrl+7 / Alt+Ctrl+7 Clipping Mask & release** | → Move Inside / Move Outside |
| **Ctrl+8 / Alt+Ctrl+8 Compound Path & release** | → Create/Release Compound *(experimental — see below)* |
| **Ctrl+J Join** | → Join Curves when the **Pen or Node tool is active** (Affinity scopes this to those tools; with other tools Ctrl+J remains Duplicate) |
| **Alt+Ctrl+J Average** | → Average *(experimental)* |
| **Ctrl+D Transform Again** | → Duplicate (Affinity's duplicate is a *power duplicate* that repeats your last transform — same idea) |
| **Shift+Ctrl+A Deselect** | → Deselect (Ctrl+D was reassigned as above) |
| **Ctrl+6 Reselect** | → Reselect *(experimental)* |
| **Shift+Ctrl+O Create Outlines** | → Convert to Curves (Ctrl+Enter also kept) |
| **Shift+Ctrl+E Apply Last Effect** | → Repeat Last Command (closest) |
| **Alt+Ctrl+; Lock Guides** | → Lock Guides |

### Type
**Ctrl+T Character panel ✓ (same key!)** · **Alt+Ctrl+T Paragraph** · **Shift+Ctrl+T Tabs** → Typography panel ·
**Alt+Shift+Ctrl+T OpenType** · align **Shift+Ctrl+L / C / R** · justify **Shift+Ctrl+J** ·
justify-all **Shift+Ctrl+F** (Affinity's own Ctrl+Alt+L/C/R bindings also kept) ·
font size **Shift+Ctrl+. / ,** = Affinity's `Ctrl+>` / `Ctrl+<` (same physical keys, already default) ·
Bold/Italic/Underline keep Affinity's Ctrl+B/I/U (AI has no defaults for these).

### View & panels
**Ctrl+Y Outline** ✓ *(experimental command name — v3 already defaults to Ctrl+Y)* ·
Ctrl+; guides ✓ · Ctrl+' grid ✓ · Ctrl+R rulers ✓ · **Ctrl+Alt+0 Fit All** → Zoom to Fit (dual with Ctrl+0) ·
**F5 Brushes · F6 Color · F7 Layers ✓ (same!) · F8 New Symbol · Ctrl+F8 Info · Ctrl+F10 Stroke ·
Shift+F5 Graphic Styles → Styles panel · Shift+F8 Transform · Shift+Ctrl+F11 Symbols** ·
F1 Help ✓.

---

## Deliberate deviations & things that could not be mapped 1:1

**Photoshop side**
- **Ctrl+T / Ctrl+Shift+T / Ctrl+Alt+Shift+T (Free Transform / Again)** — Affinity has no transform *command*;
  the Move tool always transforms. These keys were left **unassigned** (Affinity's defaults on them were removed
  so you don't get a surprise panel). No equivalent exists.
- **Shift+Ctrl+J Layer via Cut** — no equivalent (use Ctrl+X then Ctrl+V).
- **F cycle screen modes** — Affinity on Windows has no full-screen shortcut; F stays on Affinity's
  Frequency-Separation toggle.
- **Step Forward/Back history (Alt+Ctrl+Z)** — Affinity has plain Undo/Redo only; Alt+Ctrl+Z was mapped to Undo.
- **Ctrl+, hide layer** (PS web) — left as Affinity's Settings shortcut; conflicted with PS's own Ctrl+K mapping.
- **Copy Merged vs text alignment** — Affinity can't scope keys by text-editing context, so PS's
  Shift+Ctrl+L/C/R text alignment lost to Auto Tone/Copy Merged/Rename Layer. Justify (Shift+Ctrl+J) did map.

**Illustrator side**
- **No equivalent tools:** Magic Wand (Y), Lasso (Q), Rotate (R), Reflect (O), Scale (S), Scissors (C),
  Blob Brush (Shift+B), Eraser (Shift+E), Shaper (Shift+N), Mesh (U), Graphs (J), Symbol Sprayer (Shift+S),
  Perspective Grid/Selection (Shift+P/V), Slice (Shift+K — Affinity's Slice *studio* is separate), Width…
  wait, Width **did** map (Shift+W → Stroke Width). For wand-style selection use Affinity's
  *Select Same / Select Object* menu commands.
- **Ctrl+B/F/V paste in back/front/in place** — Affinity pastes to the same position by default but has no
  front/back variants; keys keep Affinity defaults (Bold/Find/Paste).
- **Ctrl+E GPU preview, Shift+Ctrl+D transparency grid, Shift+Ctrl+H show artboards, Ctrl+U smart guides,
  Ctrl+5 make guides, F12 Revert, F2/F3/F4 cut-copy-paste** — no Affinity equivalent (or, for F2–F4,
  deliberately left on v3's studio-switching keys so you don't trap yourself in a studio).
- **Ctrl+8 conflict** — AI's Make Compound took Ctrl+8; Affinity's "Zoom to actual size" was unbound
  (Ctrl+1/0 still cover zooming).
- **Ctrl+L** — kept as Affinity's Lock (Designer's default) rather than Levels; AI's Ctrl+2 Lock also added.

**Both files**
- **F5–F8 panel keys shadow v3's studio-switching keys** (F5 Slice, F6 Canva AI, F7 Retouching, F8 Color
  Grading) *inside* the mapped studio. F2/F3/F4/F9 studio switching is preserved. If you'd rather have the
  studio keys, delete the panel bindings in Settings → Keyboard Shortcuts.
- v3's **Ctrl+B Brightness/Contrast** default was sacrificed for PS's Ctrl+B Color Balance (Pixel file only).

## Experimental entries (synthesized command names)

These commands exist in Affinity v3 (verified in a real v3 shortcut inventory) but their exact internal
Windows command names had to be inferred; if one doesn't work, assign it once via the GUI and it'll stick
(the rest of the file is unaffected): `SwitchToWorkspace0/1/2/7Command` (F2/F3/F4/F9 studio keys),
`SwitchToDevelopWorkspaceCommand`, `PreviewModeCommand` (Ctrl+Shift+W), and in the Illustrator file
`CompoundCommand`, `ReleaseCompoundCommand`, `AverageCommand`, `ReselectCommand`, `OutlineViewModeCommand`,
`AddSymbolCommand`, `ToggleStrokePageVisibilityCommand`, `ToggleSymbolsPageVisibilityCommand`, plus tool
names `ShapeBuilder`, `Knife`, `StrokeWidth`, `Contour`, `Blend`, `VectorFloodFill`, `ShapeLine`/`Line`.

## Compatibility notes

- `.afshort` (Windows) is a ZIP of per-workspace XML using the v1/v2/v3-compatible schema with
  assembly-qualified command names (`Version=2.5.5.2636` — Affinity ignores the version when loading;
  v1.8 files load fine in v2, and v3 loads earlier files).
- `.affshortcuts` (Mac) is a binary-plist keyed archive; these were produced by surgically editing a
  genuine v3 export and re-serializing, so format validity is not inferred but inherited.
- The Windows Photoshop file contains both `PhotoWorkspace.xml` (v2 Photo / possible v3 naming) and
  `PixelWorkspace.xml` (v3 Pixel Studio naming) with identical content, so it lands whichever name v3 uses.
- Everything was validated as well-formed with no unintended duplicate key combos (the only shared
  combos left — e.g. Alt+Shift+V Paste FX vs Vivid Light — are conflicts Affinity ships in its own
  factory defaults).
- Source shortcut lists: Adobe's official Photoshop (web + desktop) and Illustrator default-shortcut
  documentation, cross-checked against Affinity v3's official shortcut documentation and real
  exported shortcut files for both platforms.

---

## Mac-specific notes (`.affshortcuts` files)

Same mapping decisions as Windows, with these platform realities:

- **Panel toggles don't exist on Mac.** Affinity v3 for macOS exposes no shortcut actions for the
  Brushes/Color/Layers/Info/Stroke/Styles/Transform/Symbols/Macro panels, so F5–F8, Alt+F9, Ctrl+F8/F10,
  Shift+F5/F8 and Shift+Ctrl+F11 mappings are **Windows-only**. (Mac users toggle panels via the
  Window menu.) The two panel actions Mac does have — Character `Cmd+T` and Typography `Shift+Cmd+T` —
  already match Illustrator and are kept.
- **Cmd+2 Lock is unmappable on Mac** (v3 macOS has no lock/unlock-object action), so Cmd+2 keeps its
  factory Zoom 200%. Unlock All *did* map: Opt+Cmd+2. Hide mapped to Cmd+3 (layer-visibility toggle),
  Show All to Opt+Cmd+3.
- **Cmd+H in the Pixel studio** is PS's Hide Extras (show/hide selection edges); the macOS
  Hide-Application binding was removed *in the Pixel studio only* — Cmd+H still hides the app from
  every other studio. Undo it in Settings if it bothers you.
- **Already-correct factory mappings kept as-is:** Cmd+Y Outline view (AI), Cmd+J Join Curves with
  Pen/Node active (AI), Cmd+T Character panel (AI), Shift+Cmd+X Liquify (PS), Shift+Cmd+F Fade (PS),
  Opt+Cmd+G Move Inside (PS clipping mask), Shift+Cmd+E Merge Selected was *moved* to Merge Visible
  (PS) in the Pixel file and to Repeat/last-effect (AI) in the Vector file.
- **Tools:** Liquify studio uses PS's W/E/S/B/O/D keys exactly like the Windows file. Vector studio
  adds M Rectangle, L Ellipse, Shift+M Shape Builder, Shift+W Width, E Point Transform, plus
  *experimental* entries for the Artboard (Shift+O), Blend (W) and Line (\) tools — those three tools
  don't appear in the v3.0.x export these files are based on, so their entries use inferred tool IDs
  and are inert if the guess is wrong (assign once in Settings to fix).
- **Deliberate sacrifices (Vector file):** Cmd+B/I/U follow the factory (Brightness-Contrast was
  moved off Cmd+B for Bold; Italic/Underline yield to factory Invert/HSL); Zoom-to-Width lost
  Opt+Cmd+0 to AI's Fit All; studio-switch key F8 is shadowed by New Symbol *inside the Vector
  studio*; Copy Merged lost Shift+Cmd+C to AI's align-center; the Rename Layer, Fade,
  pixel-selection-from-object, Zoom-400% and Develop-studio defaults were unbound where they
  collided with AI keys.
- **Deliberate sacrifices (Pixel file):** New-from-Clipboard lost Opt+Shift+Cmd+N to PS's New Layer;
  Find lost Cmd+F to Repeat/last-filter (PS); Brightness/Contrast lost Cmd+B to Color Balance (PS);
  Merge Selected unbound for PS's Shift+Cmd+E Merge Visible; Character/Typography panels unbound so
  Cmd+T / Shift+Cmd+T stay free like PS's (unmappable) Free Transform keys.
