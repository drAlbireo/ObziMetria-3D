# ObziMetria 3D

**Plan your observatory around the telescope — not the other way around.**

ObziMetria 3D is an interactive 3D observatory-planning tool for amateur astronomers and astrophotographers. Explore building dimensions, pier heights and positions, roof clearance, telescope movement, local obstacles, and observing conditions *before* you build.

**Current version: ObziMetria 3D v3.0**  
**Alternative visual edition: Observatory Forge 2.0.0**

Both editions contain the **same planning features and calculations**. They differ in their visual presentation.

**[Get the latest release](../../releases/latest)** · **[What's new](CHANGELOG.md)** · **[Contact the developer](mailto:makszem.berci@gmail.com)**

## What can you plan?

| Area | Tools |
| --- | --- |
| Observatory layout | Building dimensions, walls, pier placement, raised platforms and parapets |
| Roof and dome | Roof-opening clearances, clamshell domes, rotating-dome slit checks and dome synchronization |
| Telescope equipment | Telescope, equatorial-mount, fork-mount and wedge configurations with 3D geometry |
| Safety and access | Telescope sweeps, parked positions, collision checks, furniture, doorways and walkways |
| Local observing sky | Site coordinates, imported or manually entered horizon obstacles and visible-sky checks |
| Night planning | Sky map, scheduled targets, Moon warnings, recommended targets and a year overview |
| Design workflow | 3D views, plans and sections, undo/redo, saved designs and side-by-side comparison |

## Highlights in v3.0

### Realistic telescope and mount configurations

- **21 named telescope models**, using manufacturer-based tube dimensions in the clearance calculations.
- **19 named equatorial mounts**, with moving RA/DEC assemblies and model-specific geometry.
- **13 fork and single-arm mounts**, including the Meade LX200-ACF, Meade LX600-ACF, Celestron CPC Deluxe HD, NexStar Evolution, Celestron Origin and Sky-Watcher AZ-GTi families.
- Built-in telescope configurations for supported fork mounts, plus configurable equipment for applicable single-arm mounts.
- A payload check when both a modeled telescope and a modeled mount are selected; camera and accessory weights are estimated.

### Equatorial wedges for fork mounts

Compatible forks can be used upright in **alt-azimuth** or placed on an **equatorial wedge**:

- **Meade X-Wedge:** latitude adjustment from 25° to 65°.
- **Celestron HD Pro Wedge:** latitude adjustment from 0° to 90°.
- The wedge latitude can follow the observing site's latitude, or be adjusted manually.
- Checks warn when the selected wedge angle misses the celestial pole or falls outside the supported range.
- A wedged fork is modeled as tracking equatorially, without a German-equatorial meridian flip.

### Build for your actual observing site

- Add obstacles such as trees or buildings by azimuth and altitude, or import horizon data in N.I.N.A. `.hrz`, Stellarium or azimuth/altitude-pair formats.
- Check the local horizon alongside observatory walls; export a combined `.hrz` horizon.
- Plan raised floors, rooftop platforms, parapets and roof-opening space.
- Choose concrete or steel piers and inspect the corresponding drawings and materials calculations.
- Add furniture and check a walkway from the entrance to the telescopes.

### Plan the observing night

- Explore a configurable sky map, with star limits, constellation overlays and Messier/Caldwell objects.
- Build a timed target list for each pier and follow the targets in the night simulation.
- See Moon-related warnings, local horizon obstructions, dome-slit issues and other observing constraints.
- Find **Best targets tonight** and review weekly observing opportunities in the **Year** view.

### Dome and roof planning

- Check the dome slit against the telescope's light path and model a dome that follows a chosen pier.
- Calculate dome settings intended for N.I.N.A./ASCOM setup, including center offsets and GEM axis length.
- Model a clamshell dome with east–west or north–south folding direction.
- Evaluate the effect of prevailing wind on the building's orientation and roof design.

### Explore and compare designs

- Inspect the observatory in 3D, on a floor plan, and in section views.
- Use **Undo/Redo** for recent design changes.
- Save a design snapshot and compare it with the current version side by side.
- Save and reload plans with the newer settings retained.

## Download and run

1. Open **[Releases](../../releases)** and choose the latest published version.
2. Under **Assets**, download the build provided for your intended platform. A Windows executable and/or a browser-based HTML build may be supplied with a release.
3. For a portable Windows `.exe`, run the downloaded application. For an HTML build, open the file in a compatible modern browser.
4. Set your site and observatory dimensions, add your piers and equipment, then review the checks and 3D views before building.

**Note:** The availability and precise startup steps depend on the files attached to each release. Download builds only from a source you trust. On Windows, an unsigned application may produce a security prompt; verify the source before deciding whether to run it.

## Suggested planning workflow

1. **Site:** Enter latitude/longitude, prevailing wind and any local horizon obstacles.
2. **Structure:** Set the building, floor or platform, walls, roof type and opening direction.
3. **Piers and equipment:** Choose pier types and positions, telescope and mount models, and any wedge settings.
4. **Clearances:** Review movement, parking, roof, furniture and walkway checks; adjust dimensions as required.
5. **Night sky:** Pick targets, run the night simulation and inspect the observing timeline.
6. **Compare and save:** Try alternative designs, compare them and save your preferred configuration.

## Important accuracy notes

ObziMetria 3D is a **planning and visualization aid**, not a substitute for on-site measurement, structural design or professional engineering review.

- **Mount, fork and wedge housings** are scaled from manufacturer photos where exact head dimensions are unavailable. Measure your actual setup when clearances are tight; use Custom settings where appropriate.
- **Dome-sync offsets** use typical mount dimensions. Measure the installed equipment before entering values in N.I.N.A. or an ASCOM dome driver.
- **Payload estimates** use typical accessory masses and are guidance, not a manufacturer certification.
- **Furniture, accessories and walking space** are approximated. The walkway analysis uses a floor grid, so narrow gaps can vary by a few centimeters.
- **Parapets/railings** are treated as solid horizon obstacles. Open railings may block less sky in practice.
- **Clamshell geometry** represents nested shells folding beside the ring; other DIY hinge designs may obstruct more of the low sky.
- **Best targets** and the **Year** view account for the selected pier's wall, roof and local horizon, but not neighboring telescope movement; the night simulation includes other telescopes. The year overview samples weekly.

Always verify critical clearances, roof travel, mechanical loads, weather protection, local regulations and building safety on site.

## Versions

| ObziMetria 3D | Observatory Forge | Main addition |
| --- | --- | --- |
| **v3.0** | **2.0.0** | Fork and single-arm mounts, equatorial wedges, more detailed imaging train |
| v2.9 | 1.9.0 | 19 equatorial mount models and payload checks |
| v2.8 | 1.8.0 | 21 telescope models |
| v2.7 | 1.7.0 | Steel piers and improved 3D materials/lighting |
| v2.6 | 1.6.0–1.6.1 | Furniture, walkways, imaging accessories and overall verdict |
| v2.5 | 1.5.0 | Target schedules, Moon checks, best targets and Year view |
| v2.4 | 1.4.0 | Raised platforms, clamshell dome, undo/redo and design comparison |
| v2.3 | 1.3.0 | Local horizon, dome sync and collapsible settings |

For the full details, see **[CHANGELOG.md](CHANGELOG.md)**.

## Contact and support

**Created by Mákszem Albert**  
Questions, suggestions or bug reports: **[makszem.berci@gmail.com](mailto:makszem.berci@gmail.com)**

If the program helps with your observatory project and you'd like to support continued development, you can leave an optional tip via **[Revolut](https://revolut.me/makszemalbert)**.

Community suggestions are welcome — including real-world equipment measurements and reports of any clearance discrepancies.
