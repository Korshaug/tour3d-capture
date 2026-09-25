# tour3d-capture

The capture page for tour3d: photograph a room for a 3D tour with a phone.

**https://korshaug.github.io/tour3d-capture/**

It opens the camera, shows a dot where each photo of the pattern goes, and takes
the photo when the phone is held still on it; it says when a spot is covered,
counts down the minute's pause between spots, and saves the room as one ZIP to
drop into the tour3d app. Where the phone does not report its orientation it
falls back to a ring-by-ring shot list; where the browser cannot open the camera,
to the camera-app steps.

Nothing leaves the phone: the photos stay in the browser until you save them.
The page is one self-contained file, built from the tour3d repository
(`viewer/capture.html`, `viewer/src/capture/`) with
`npm run build && node tools/build-single-file.mjs --page capture`, and copied
here as `index.html`. Kept out of search results (`noindex`) on purpose: it is a
tool reached by its link.
