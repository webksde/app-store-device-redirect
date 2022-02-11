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

# Design
The design is just a random example. Change it as needed, ensure to at least set the id attributes on the app store links, for example:
~~~
<a href="https://play.google.com/store/apps/details?id=[PACKAGE-NAME]" id="g-store-link"><strong>[APP-NAME]</strong><br />in Google Play Store</a>
~~~
~~~
<a href="http://apps.apple.com/[COUNTRY]/app/[APP-NAME]/id[STORE-ID]]" id="a-store-link"><strong>[APP-NAME]</strong><br />in Apple App Store</a>`
~~~
So JavaScript can pick them up for the redirect, without having to define them twice.
