# App Store Device Redirect page
Simple single-page HTML + Vanilla JavaScript App Store redirect page based on user agent.
Can be used as template for individual implementations.

## Demo
https://webksde.github.io/app-store-device-redirect/index.html

## Functionality
Provides a static HTML page to redirect users to the app store of their device.
The detection is based on the userAgent:
`var userAgent = navigator.userAgent || navigator.vendor || window.opera;`



## Supported stores & userAgents
- Android ("android")
- Apple ("iPad|iPhone|iPod")
