<p align="center"><img width="600" src="https://user-images.githubusercontent.com/2406499/57032656-ea740e00-6c18-11e9-9c06-218dcc105fc3.png" /></p>
<p align="center">Add some pony to your badge collection!</p>


## Static Examples

![badge-pinkiepie][badge-pinkiepie]

![badge-rainbowdash][badge-rainbowdash]

![badge-twilightsparkle][badge-twilightsparkle]

![badge-applejack][badge-applejack]

![badge-derpy][badge-derpy]

![badge-octavia][badge-octavia]

![badge-luna][badge-luna]

(pixel art by [pix3m](https://deviantart.com/pix3m))

## Animated Examples

![badge-rainbowdash-gif][badge-rainbowdash-gif]

![badge-twilightsparkle-gif][badge-twilightsparkle-gif]

![badge-applejack-gif][badge-applejack-gif]

![badge-fluttershy-gif][badge-fluttershy-gif]

Note: These don't play in some versions of Firefox.

## How it works

This repo contains "serverless" functions for both [Cloudflare Workers](https://www.cloudflare.com/products/cloudflare-workers/) and [Google Cloud Functions](https://cloud.google.com/functions/). These functions act as a proxy to the popular [Shields.IO](https://shields.io/) service, allowing you to pass in a [Derpibooru](https://derpibooru.org/) image id to use as a logo on the badge. It works by fetching the image data from Derpibooru and then passing it to Shields.IO as a data uri in the `logo` parameter. Unfortunately due to url length constraints, images must be pretty small - the current functions limit images to 100px by 100px.


[badge-pinkiepie]:https://us-central1-pony-badges.cloudfunctions.net/badge/Pinkie%20Pie-Best%20Pony-F7438C.svg?style=popout&imageId=638543
[badge-rarity]:https://us-central1-pony-badges.cloudfunctions.net/badge/Rarity-Best%20Pony-6A50A7.svg?style=popout&imageId=662317
[badge-rainbowdash]:https://us-central1-pony-badges.cloudfunctions.net/badge/Rainbow%20Dash-Best%20Pony-269DCE.svg?style=popout&imageId=638547
[badge-twilightsparkle]:https://us-central1-pony-badges.cloudfunctions.net/badge/Twilight%20Sparkle-Best%20Pony-273873.svg?style=popout&imageId=638549
[badge-applejack]:https://us-central1-pony-badges.cloudfunctions.net/badge/Applejack-Best%20Pony-E59819.svg?style=popout&imageId=638528
[badge-derpy]:https://us-central1-pony-badges.cloudfunctions.net/badge/Derpy-Best%20Muffin-C1C5D3.svg?style=popout&imageId=638529
[badge-octavia]:https://us-central1-pony-badges.cloudfunctions.net/badge/Octavia-Best%20Pony-4B4B4B.svg?style=popout&imageId=638540
[badge-luna]:https://us-central1-pony-badges.cloudfunctions.net/badge/Luna-Best%20Princess-2449BE.svg?style=popout&imageId=638534

[badge-rainbowdash-gif]:https://us-central1-pony-badges.cloudfunctions.net/badge/Rainbow%20Dash-Best%20Pony-269DCE.svg?style=popout&imageId=1699633
[badge-twilightsparkle-gif]:https://us-central1-pony-badges.cloudfunctions.net/badge/Twilight%20Sparkle-Best%20Pony-273873.svg?style=popout&imageId=1379405
[badge-applejack-gif]:https://us-central1-pony-badges.cloudfunctions.net/badge/Applejack-Best%20Pony-E59819.svg?style=popout&imageId=296082
[badge-fluttershy-gif]:https://us-central1-pony-badges.cloudfunctions.net/badge/Fluttershy-Best%20Pony-E57FB1.svg?style=popout&imageId=678310

