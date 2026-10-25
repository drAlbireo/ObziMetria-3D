# Changelog — ObziMetria 3D / Observatory Forge

This changelog summarizes the changes **from ObziMetria 3D v2.2 to v3.0**, based on the development summary dated **24 October 2026**. Both ObziMetria 3D and Observatory Forge contain the same functionality; their visual styles differ.

## ObziMetria 3D v3.0 · Observatory Forge 2.0.0

**Fork mounts, wedges and imaging trains**

- Added **13 fork and single-arm mount configurations**:
  - **Meade:** LX200-ACF 8″, 10″, 12″; LX600-ACF 10″, 12″, 14″.
  - **Celestron:** CPC Deluxe 800, 925, 1100 HD; NexStar Evolution 8, 9.25; Origin.
  - **Sky-Watcher:** AZ-GTi.
- Added built-in optical tubes for supported forks and a configurable telescope for the AZ-GTi.
- Added compatible **equatorial wedges**: Meade X-Wedge (25°–65°) and Celestron HD Pro Wedge (0°–90°).
- Added wedge-latitude control, optional matching to site latitude, and misalignment/range warnings.
- Added alt-azimuth vs. equatorial-wedge fork configurations, including field-rotation advice for alt-az use and no-meridian-flip tracking for wedged forks.
- Fork arms, drive bases and tilted wedge plates are represented in 3D and clearance checks.
- Enhanced imaging train models: adapter/spacer/filter ring, cooled camera and fan, guide scope/guide camera, filter wheel, off-axis guider and focuser motor.

## ObziMetria 3D v2.9 · Observatory Forge 1.9.0

**Equatorial mount models and payload guidance**

- Added **19 named equatorial mounts**:
  - **Celestron:** AVX, CGEM II, CGX, CGX-L.
  - **Sky-Watcher:** Star Adventurer GTi, Star Adventurer 2i, HEQ5 Pro, EQ6-R Pro, EQ8-R Pro, Wave 100i, Wave 150i.
  - **ZWO:** AM3, AM5, AM7.
  - **iOptron:** CEM26, CEM40, CEM70.
  - **Losmandy:** G11.
  - **Rainbow Astro:** RST-135.
- Animated RA and DEC assemblies, saddle and counterweights in pointing, parking, meridian-flip and night-simulation views.
- Used model-specific dimensions for swing, roof and collision checks.
- Added payload comparison against rated capacity when modeled telescopes and mounts are selected, including a 75%-of-rating advisory and counterweight guidance for selected harmonic mounts.
- **Accuracy note:** where detailed manufacturer head dimensions were unavailable, geometry was estimated from product photographs.

## ObziMetria 3D v2.8 · Observatory Forge 1.8.0

**Telescope model library**

- Added **21 named telescope models**:
  - **Refractors:** William Optics SpaceCat 51, RedCat 51/61, ZenithStar 61 II, FLT 120; Sky-Watcher Evolux 62ED, Esprit 100/120; Askar FRA400; Takahashi FSQ-106.
  - **Schmidt–Cassegrain, Maksutov and RC:** Celestron C8, C9.25, C11, EdgeHD 8/11; 8-inch Ritchey–Chrétien; Sky-Watcher Skymax 127.
  - **Fast astrographs and Newtonians:** Celestron RASA 8/11; Sky-Watcher Explorer 150P-DS, Quattro 200P.
- Selecting a model fills in telescope type, aperture, focal length and physical dimensions.
- Editing model parameters converts the configuration to a Custom telescope; Undo can restore the preset.
- Added telescope-specific 3D details and physical geometry to clearance checks.
- Added appropriate front-camera placement for RASA models and side focuser/camera placement for Newtonians.

## ObziMetria 3D v2.7 · Observatory Forge 1.7.0

**Steel piers and improved 3D rendering**

- Added Concrete/Steel pier types per pier.
- Modeled steel pier tube, flanges, gussets, base plate, anchor bolts and cable access.
- Included pier details in drawings and materials calculations.
- Improved lighting, tone mapping, materials, reflections and soft shadows.
- Refined mount-adapter plates, rods and hardware details.

## ObziMetria 3D v2.6 · Observatory Forge 1.6.0–1.6.1

**Interior planning and overall checks**

- Added furniture placement and collision detection for telescope swing, park and night simulation.
- Added entrance-to-pier walkway-width analysis, reachable floor shading and access warnings.
- Added guide scopes, filter wheels, off-axis guiders and focuser motors to equipment and clearance calculations.
- Added a consolidated overall design verdict with actionable issue messages.
- Moved longitude to the Site section, with East/West entry.

## ObziMetria 3D v2.5 · Observatory Forge 1.5.0

**Night-planning features**

- Added sky-map zoom, pan, constellation and object-display controls.
- Added prevailing-wind input and roof/door wind-orientation advice.
- Added timed observing target lists per pier, including target switches in the simulation and night plan.
- Added Moon illumination, proximity and observation warnings.
- Added **Best targets tonight** ranking for Messier/Caldwell objects and planets.
- Added the **Year** view of weekly dark observing hours, Moon conditions and favorable periods.

## ObziMetria 3D v2.4 · Observatory Forge 1.4.0

**Platforms, roof options and design comparisons**

- Added raised observatory floors and platforms, configurable placement and parapets.
- Checked platform fit for the building and roof-opening envelope.
- Added a clamshell dome with folding direction and 3D opening animation.
- Added consistent per-pier colors in charts, floor plans and 3D views.
- Added 100-step Undo/Redo history and 3D-label spacing improvements.
- Added saved snapshots and side-by-side design comparison.

## ObziMetria 3D v2.3 · Observatory Forge 1.3.0

**Local horizons, dome synchronization and settings organization**

- Added manual local-horizon obstacles and import of `.hrz`, Stellarium and azimuth/altitude horizon data.
- Added local-horizon visibility in charts, sky maps and night simulation.
- Added optional wall-height recommendations that account for natural obstacles.
- Added combined building/local-horizon `.hrz` export.
- Added dome diameter, slit width, rotation speed and followed-pier settings.
- Added N.I.N.A./ASCOM dome-offset values with copy controls, dome slit/beam checks and animated dome positioning.
- Added collapsible settings groups with remembered state and Open all/Close all controls.

## Improvements and known modeling simplifications

**Improvements**

- Resolved an older pier-placement implementation overriding the newer placement logic.
- Improved collision and parking warnings to identify the wall or furniture involved.
- Improved phone-width behavior, scrollable tabs and sky-map readability.

**Modeling approximations**

- Open railings are conservatively treated as solid parapets.
- Clamshell geometry approximates a nested-shell design; other construction methods may obstruct more low sky.
- Dome-sync values use typical mount dimensions and should be verified on the actual installation.
- Best-target and Year calculations do not account for other telescope motion; the night simulation does. The Year view samples once a week.
- Walkway calculations use a 4–10 cm grid. Some furniture/equipment dimensions and payload masses are estimates.
- Mount heads, forks and wedges may be photo-scaled approximations; confirm tight clearances against actual equipment dimensions.
- Tube balance and pivot assumptions are simplified, especially for fork-mounted instruments.

**Reported validation in the 24 October 2026 change summary:** approximately 3,160 passing engine checks, plus light- and dark-mode view testing for both editions. This is a report of testing, not a guarantee of engineering accuracy.
