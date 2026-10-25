# Terrain Analysis Tool

Bohn Ag Consulting. LiDAR elevation, drainage, slope and water analysis that runs entirely on the device. One app for iPhone, iPad and PC, in portrait or landscape.

## Install on iPhone or iPad
1. Open the app link in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open **Terrain** from the home screen. Once it has opened, it works offline.

## Use on a PC
- Open the app link in **Chrome** or **Edge**. To keep it like a program, use the browser's **Install app** button in the address bar. It then opens in its own window and works offline.
- Or open `index.html` straight from a folder on the computer. This works without internet too, except for **Download area**.

## Getting elevation files
- **Download area**: a square (1–20 km on a side, 1, 2 or 5 m detail, bare ground or surface) from the government HRDEM service, either around **My location** or anywhere you **Pick on map**: pan the map (search for a town, postal code or "lat, long") until the red square covers the area. Yellow shading shows where LiDAR exists.
- **Open file**: elevation files (`.tif`, or a `.zip` containing them) from Files, Downloads, or a folder. On a PC you can also drag them onto the window. Select several tiles to join them.

### Files from Google Drive
The Google Drive app treats a `.tif` as a picture: **Download** saves it to Photos, which ruins it. Instead:
- In Drive, tap **⋯** on the file → **Open in** → **Save to Files**, then open it from Files; or
- keep the elevation files **zipped** in Drive (Clip Zip Ship downloads already are). A `.zip` stays a normal file, and the app opens the `.tif` inside it directly.

## Good to know
- **Buttons**: the tools are in the bar along the bottom. The small buttons (Bohn Ag menu, my location, eye menu, map layers, auto colours, distance scale) are in a column on the right. To have them on the left, use **Buttons** in the eye menu. The › at the end of the tool bar hides it (and the open tool's panel) when you only need the map, e.g. tracking yourself; the tool bar button at the bottom of the side bar brings it back.
- **Reopen**: the last map is kept on the device; the start screen has a one-tap button to reopen it. **Home** (in the Bohn Ag menu) goes back to the start screen.
- **Picture** (in the Bohn Ag menu) saves a picture of the map with its results. **3D view** is at the top of the eye menu.
- **Map layers** (layers button): one main layer at a time: Hillshade or Elevation (the LiDAR alone), Satellite (Saskatchewan aerial photo, SGIC) or Soil (SKSIS soil survey: zone, ag class, texture, salinity, pH or irrigation potential, with its legend). Below them, sub layers that go on top of any of those: Roads (NRCan CanVec, all of Canada), Townships and Sections (SKSIS, Saskatchewan; with their numbers). Satellite and soil strength are in the eye menu.
- **Start screen layers** (the row under the buttons): which layers come down with the elevation when a map opens. Untick them all in the field to download only the elevation; a layer left off can still be loaded later from the layers menu. Ticked layers are kept for the map, so they work without signal once loaded.
- **Tools**: once a tool has what it needs (a point tapped, a profile finished, a drainage outlet, a pour point, an outline closed) its setup panel steps aside and the results show. Tap the tool again for its controls. **Point** also shows the quarter section and the soil classes there (from the downloaded layers, offline too) and, with signal, the soils, landscape and stones.
- **Download area** squares are laid out true north, so their edges run along the roads and section lines.
- **Turning the map**: twist with two fingers (Alt + mouse wheel on a PC). A compass appears under the distance scale while north is not up; tap it to turn north back up. **Rotation lock** in the eye menu keeps north up; it is on to start with, so turn it off to twist the map or have the GPS turn it heading-up.
- **Large files** are opened at lower detail on phones and tablets (every 2nd or 3rd pixel) so they fit in memory. A badge under the file name and the file information in the Bohn Ag menu show the detail used.
- **My location** (arrow button; its colour is under Colours › GPS): the first tap shows a blue dot, the second keeps the map centred on you and turned so the way you are going is up, and the third turns it off. The dot glides between GPS fixes; the Point tool shows the fix rate (updates per second). The first time, iPhone asks for permission. If it was refused: Settings › Privacy & Security › Location Services.
- **Pictures and drainage CSVs** open the share sheet on phones and tablets (Save to Files, Messages, Mail, etc.) and download on a PC.

## Updating
Bump `CACHE` in `sw.js` and `APP_VERSION` in `index.html` (same number) whenever you publish changes. Installed copies pick the new version up the next time they are opened with a signal. The version shows on the start screen.
