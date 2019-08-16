# Your First Progressive Web App Codelab

These are the resource files needed for the
[Your First Progressive Web App][codelab] codelab.

In this codelab, you'll  build a weather web app using Progressive Web App
techniques. Your app will:

* Use responsive design, so it works on desktop or mobile.
* Be fast & reliable, using a service worker to precache the app resources
  (HTML, CSS, JavaScript, images) needed to run, and cache the weather data
  at runtime to improve performance.
* Be installable, using a web app manifest and the `beforeinstallprompt` event
  to notify the user it's installable.


## What you'll learn

* How to create and add a web app manifest
* How to provide a simple offline experience
* How to provide a full offline experience
* How to make your app installable


## Feedback

This is a work in progress, if you find a mistake, please [file an issue][git-issue].

## License

Copyright 2019 Google, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements. See the NOTICE file distributed with this work for
additional information regarding copyright ownership. The ASF licenses this
file to you under the Apache License, Version 2.0 (the “License”); you may not
use this file except in compliance with the License. You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed
under the License is distributed on an “AS IS” BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied. See the License for the
specific language governing permissions and limitations under the License.


[codelab]: https://codelabs.developers.google.com/codelabs/your-first-pwapp/
[git-issue]: https://github.com/googlecodelabs/your-first-pwapp/issues



### Add this to `manifest.json`
`{
  "name": "Weather",
  "short_name": "Weather",
  "icons": [{
    "src": "/images/icons/icon-128x128.png",
      "sizes": "128x128",
      "type": "image/png"
    }, {
      "src": "/images/icons/icon-144x144.png",
      "sizes": "144x144",
      "type": "image/png"
    }, {
      "src": "/images/icons/icon-152x152.png",
      "sizes": "152x152",
      "type": "image/png"
    }, {
      "src": "/images/icons/icon-192x192.png",
      "sizes": "192x192",
      "type": "image/png"
    }, {
      "src": "/images/icons/icon-256x256.png",
      "sizes": "256x256",
      "type": "image/png"
    }, {
      "src": "/images/icons/icon-512x512.png",
      "sizes": "512x512",
      "type": "image/png"
    }],
  "start_url": "/index.html",
  "display": "standalone",
  "background_color": "#3E4EB8",
  "theme_color": "#2F3BA2"
}`
