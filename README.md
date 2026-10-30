# Duty Limit Check

A phone-friendly calculator that helps a cabin manager check whether the crew is inside the flight duty limit.

- Enter the sign-on date and time. Time on duty so far counts up from the phone's clock and can be overwritten.
- Enter the time still to come: delay, flight time, diversion, medical, gas-and-go, other duty.
- The top panel shows time left (or time over), projected sign-off and latest allowed sign-off.
- The duty limit defaults to 20h 30m and can be changed. Only the limit is remembered on the phone.

It is a planning aid only. The airline's rules and rostering system are the official record.

## Use it on a phone

Open the GitHub Pages address, then use the browser's Share menu and choose **Add to Home Screen**. After the first visit it works offline.

## Updating

Everything is static: `index.html`, `sw.js`, `manifest.webmanifest` and the icons. When you change a file, bump `CACHE` in `sw.js` so installed copies refresh.
