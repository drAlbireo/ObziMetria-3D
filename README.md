# ✦ ObziMetria 3D v2.2

### Interactive Observatory Designer & Night Sky Planning Tool

**Design your observatory. Test the clearances. Explore your night sky — before you build.**

ObziMetria 3D is an interactive observatory design and planning application for amateur astronomers, astrophotographers, and anyone preparing to build a personal observatory. It combines a real-time 3D model, technical drawings, telescope and roof clearance checks, and astronomical night simulation in one place.

A building can look perfectly adequate on paper and still leave too little room for counterweights, a camera, a moving roof, or a second telescope. ObziMetria 3D helps you investigate those problems while your design can still be changed.

![ObziMetria 3D: interactive observatory with an open roll-off roof and telescope](screenshots/01-3d-observatory.png)

> **Version 2.2** supports up to **six telescope piers**, both hemispheres, realistic mount geometry, multiple roof types, full-aperture horizon checks, and night-long target tracking. The bundled HTML application works **offline**.

## ✨ Highlights

- **Interactive 3D observatory:** rotate, zoom, inspect and adjust your design, with animated roof movement and see-through walls.
- **Up to six independent piers:** configure each telescope and mount, move piers on the floor plan, and inspect movement envelopes and possible collisions.
- **Full-aperture horizon and swing checks:** consider the optical tube, camera, counterweights, mount, walls, rails and opened roof—not merely a single sightline.
- **Roof clearance and design options:** explore roll-off gable, shed and flat roofs, hinged flaps, and domes.
- **Real night-sky planning:** search astronomical targets, follow telescope pointing from sunset to sunrise and see when observations are obstructed.
- **Both hemispheres:** set the site's latitude, longitude and building orientation; celestial-pole pointing adapts automatically.
- **Save and export:** reopen JSON plans, export SVG drawings, PNG images, N.I.N.A.-compatible `.hrz` horizons and text observation plans.

## 🏗️ Design an observatory in 3D

Start with the setup wizard or edit the building directly. Configure the floor dimensions, wall height and thickness, door location, roof style, pier geometry and telescope equipment. The model, plan views and checks update as you change values.

Use the **Overview**, **Equator side**, **Above**, **Mount close-up**, **See-through** and **Labels** controls to examine details from different perspectives. A red night-vision mode is also available.

### Multiple telescopes, one building

A single design can contain **one to six piers**, each with its own telescope and mount settings. Drag piers around the plan, enter precise positions, or ask the application to find additional room. Dashed movement envelopes help show where instruments could interfere with walls or with each other.

![Floor plan showing two telescope piers and their swing envelopes](screenshots/02-floor-plan.png)

### Real telescope and mount dimensions

Specify aperture, focal length, optical tube dimensions, focuser and camera extensions, dew shield, pier dimensions and adapters. The mount library includes representative **EQ5, HEQ5, EQ6-R, CEM26, CEM40, CEM70/EQ8, AM3/AM5**, and alt-azimuth classes. Custom German equatorial and alt-azimuth mounts allow you to enter your own measurements.

The **Sections** view displays the relationship between the building, the selected pier and its telescope, with tools for checking dimensions.

![Technical section view of the observatory and telescope](screenshots/03-sections.png)

## 📐 Know what can move—and what can see the sky

ObziMetria 3D checks more than whether the telescope fits in the room when parked.

- **Horizon visibility:** the full telescope aperture is checked against walls, rails and the open roof at multiple azimuths.
- **Telescope swing:** the instrument is evaluated through a range of pointing positions to identify its closest approach to walls.
- **Other instruments:** checks cover interference between telescopes, their movement areas and neighbouring piers.
- **Roof closure:** compare the parked telescope against the available clearance below the roof.
- **Automatic recommendations:** adjust wall and pier dimensions toward the visibility targets and roof-clearance requirements, with suggested fixes where necessary.

Choose minimum sky altitudes separately toward the **celestial equator**, **celestial pole**, and **east/west**. The dedicated **Visible Sky** view makes structural obstructions easy to understand.

![Visible-sky horizon analysis showing which directions remain accessible](screenshots/04-visible-sky.png)

## 🌌 Simulate an entire observing night

Version 2.2 adds an astronomical sky map and night-planning engine. Set the observing date, geographic location and time zone, then assign a target to each pier.

Search **Messier, NGC, IC and Caldwell objects**, thousands of stars, named deep-sky objects, the Moon and planets—or enter right ascension and declination directly. Targets may also be selected on the sky map.

The sky display shows constellations, celestial objects, twilight and target tracks. Use the time slider or playback controls to step from sunset to sunrise, in **10-minute or one-hour increments**.

For every pier, a colour-coded timeline distinguishes clear tracking, structural obstruction, proximity to another telescope, collisions and targets below the horizon. Equatorial mounts can use shared or per-pier **meridian flip** timing.

![Night sky map with M31 and M42 targets and two telescope visibility timelines](screenshots/05-night-sky.png)

Enable **In 3D, plan and sections** to see the simulated telescope orientations throughout the night. The program can also export a step-by-step night observation plan.

## 🏠 Roof types and construction ideas

The building designer includes **roll-off gable, shed and flat roofs, hinged roof flaps, and domes**, with relevant parameters such as roof rise, travel direction, rails and opening percentage.

A separate **Roof Ideas** studio illustrates preliminary rail, wheel and support concepts and includes a planning checklist. These are concepts only, not load-rated engineered details.

![Roof Ideas studio presenting preliminary roll-off roof rail concepts](screenshots/06-roof-ideas.png)

## 🧰 Views and exports

| View | What it shows |
| --- | --- |
| **3D Model** | Interactive building, roof, telescope and pier geometry |
| **Sections** | Vertical cuts and technical clearances |
| **Floor Plan** | Building layout, pier positions and swing envelopes |
| **Visible Sky** | Horizon restrictions caused by the structure |
| **Sky Map** | Celestial targets, observing conditions and tracking paths |
| **Roof Ideas** | Preliminary rail and support concepts |

| Output | Use |
| --- | --- |
| **JSON plan** | Save a configuration and open it again later |
| **SVG drawing** | Export a scalable observatory drawing sheet |
| **PNG image** | Save an image of the 3D design |
| **HRZ horizon** | Export a custom horizon profile for compatible software such as N.I.N.A. |
| **Text night plan** | Export a step-by-step observing timeline |

Your current settings can also be remembered between sessions when browser storage is available.

## 🚀 Download and run

### Windows (64-bit)

1. Open the **Releases** section of this GitHub repository.
2. Download **`ObziMetria_3D_v2.2_Windows.exe`**, or the Windows ZIP package.
3. If you downloaded the ZIP, extract it first.
4. Start the `.exe`. If Microsoft Edge is installed, the program opens in a dedicated Edge app window; otherwise it opens in your default browser.

**Requirements:** Windows 10 or 11 (64-bit), a modern installed browser, and WebGL-capable graphics hardware for the 3D view. No separate installation or internet connection is required. The Windows launcher does **not** bundle its own browser engine.

**Windows security note:** The current Windows executable is not digitally signed, so SmartScreen may show a warning. This build has not been fully tested on a Windows computer; testing before wider distribution is recommended.

### Original single-file HTML edition

The original application is available as **`ObziMetria_3D_v2.2.html`**. Open it in a modern browser with JavaScript and WebGL support. All essential application code and astronomical catalogues are bundled into the HTML file, allowing offline use.

## 🆕 What's new in v2.2?

Compared with the original v1.0 roll-off observatory concept, the current version introduces:

- Northern and Southern Hemisphere support, plus building orientation relative to true north.
- Full-aperture horizon and physical telescope swing analysis.
- More mount classes, custom mount geometry, additional roof types and doors.
- Automated dimension recommendations and approximate material quantities.
- Celestial-pole startup pointing and switchable 3D labels.
- Up to six separately configurable telescope piers with contact checks.
- A searchable astronomical target catalogue and interactive night-sky map.
- Sunset-to-sunrise target simulation, obstruction timelines and meridian flip modelling.
- Expanded drawing, horizon and observation-plan export options.

## ⚠️ Important limitations

**ObziMetria 3D is a preliminary geometry and planning tool—not a certified construction or engineering design package.** Physical clearances depend on the exact dimensions of your equipment. Library mount dimensions are representative and should be replaced with measurements for critical decisions.

Rails, roof structure, wind and snow loads, foundations, waterproofing and all structural connections require separate engineering verification. Astronomical positions are suitable for planning (approximately one-arcminute accuracy according to the v2.2 documentation), **not precision mount pointing or telescope control**.

## 👨‍💻 Creator and data credits

**ObziMetria 3D was created by Mákszem Albert.** The application retains its original visual identity and creator contact information.

Astronomical data credits:

- **OpenNGC** — NGC/IC objects, Messier references and common names (**CC BY-SA 4.0**).
- **Yale Bright Star Catalogue** — Stellar data (**public domain**).
- **d3-celestial** — Constellation lines and names (**BSD 3-Clause**).
- **Three.js** — 3D rendering library (**MIT License**).

These credits describe incorporated data and dependencies; they do not imply that the ObziMetria application itself is distributed under those same licenses.

---

**ObziMetria 3D v2.2 — Design smarter. Check the clearances. Understand your sky.**
