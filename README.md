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
- **Buttons**: the tools are in the bar along the bottom. The small buttons (Bohn Ag menu, eye menu, auto colours, my location, distance scale) are in a column on the right. Drag the **⋯** handle under them across the screen, or tap it, to move them to the left side.
- **Reopen**: the last map is kept on the device; the start screen has a one-tap button to reopen it. **Home** (in the Bohn Ag menu) goes back to the start screen.
- **Picture** (in the Bohn Ag menu) saves a picture of the map with its results. **3D view** is at the top of the eye menu.
- **Roads** and **Imagery** (eye menu): roads from NRCan's CanVec map anywhere in Canada; aerial imagery from Saskatchewan's SGIC (Saskatchewan only). They need internet the first time a map is opened with them switched on. The imagery strength slider blends the photo with the shading underneath.
- **Download area** squares are laid out true north, so their edges run along the roads and section lines.
- **Large files** are opened at lower detail on phones and tablets (every 2nd or 3rd pixel) so they fit in memory. A badge under the file name and the file information in the Bohn Ag menu show the detail used.
- **My location** (arrow button; its colour is under Colours › GPS): the first tap shows a blue dot, the second keeps the map centred on you, and the third turns it off. The first time, iPhone asks for permission. If it was refused: Settings › Privacy & Security › Location Services.
- **Pictures and drainage CSVs** open the share sheet on phones and tablets (Save to Files, Messages, Mail, etc.) and download on a PC.

## Updating
Bump `CACHE` in `sw.js` and `APP_VERSION` in `index.html` (same number) whenever you publish changes. Installed copies pick the new version up the next time they are opened with a signal. The version shows on the start screen.
