# YMA Poster Generator

A public, browser-based poster builder for YMA branch announcements. The first version uses a fixed poster layout: users enter the information, upload a portrait, choose a street or satellite map, and export PNG or PDF.

## Run locally

Open `index.html` in a modern browser. For best results, serve the folder with a local static web server because browser security rules may restrict some features when opened as a `file://` URL.

## Deploy with GitHub Pages

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/ (root)`, then Save.
4. GitHub will publish the site at `https://enga018.github.io/yma-poster-generator/` once deployment finishes.

## Current features

- Fixed YMA-style poster layout with live preview.
- Editable branch, heading, date, member details, statistics, funeral details and closing message.
- Portrait upload and circular crop frame.
- Searchable map location using the public Nominatim geocoder.
- Street map (OpenStreetMap) and satellite imagery (Esri World Imagery) layers.
- Click or drag the map marker to position the location.
- Browser-side PNG and A4 PDF export.
- Responsive form layout for phones and desktop browsers.

## Important notes

- This is a public website with no login. Anyone with the URL can use it. The form data and uploaded portrait are processed in the browser and are not saved to a server by this application.
- Map tiles and place search are provided by third parties. Their availability, rate limits and terms apply. OpenStreetMap data requires attribution; satellite imagery carries Esri attribution. Do not bulk-geocode or send repeated automated requests to Nominatim.
- PNG/PDF export depends on third-party map tiles allowing browser canvas capture. If a provider blocks cross-origin image capture, the export may fail or omit map imagery. Test both map styles before using a poster for official publication.
- The circular YMA seal in this prototype is placeholder artwork. Replace it with the branch's authorized logo before public production use.
- No backend, analytics, accounts, or cloud storage are included in this version.

## Next improvements

1. Replace placeholder seal with the official YMA logo.
2. Tune typography and proportions against the supplied reference poster.
3. Add image positioning controls and font-size safeguards for long names/details.
4. Test map capture and export on Android Chrome and desktop browsers.
5. Consider an optional private save/history feature only if the branch needs it.

## License

No license has been assigned yet. Add a license before allowing third parties to reuse or redistribute the code.
