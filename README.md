
# [Portfolio Website Project](https://www.vasudeveloper.com)
[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)

This is my current Portfolio that is build from scratch using typescript, html, and css. Click on the heading above to browse the page.


## Optimizations

Optimizations for Performance improvements is given the maximum attention to reduce the rendering time on first paint.

Here's something I did to improve the loading time of the page:

 - Used facade technique for iframes of YouTube Videos.
 - Used Imagekit CDN for profile image and loaded them using on the go transformation.
 - Used the following technique to load googleFonts:

    ```html
    <link rel="stylesheet" href="link_to_google_font&display=swap" media="print" onload="this.media='all'">
    <noscript>
        <link type="text/css" rel="stylesheet" href="link_to_google_font&display=swap">
    </noscript>
    ```
 - The usage of media="print" makes sure that page doesn't get blocked during critical rendering process and once the load completes, it replaces the media to 'all' for the effect to happen.
 - Before any optimization
   ![Before Optimization LightHouse Portfolio](https://user-images.githubusercontent.com/56103269/130655708-7812e8f4-6732-4358-a375-d8f47294daa7.png)
 - After optimization on mobile
   ![After Optimization LightHouse Portfolio - version 4](https://user-images.githubusercontent.com/56103269/130655800-0863e05f-9d37-4827-a6d0-6754289c8f7a.png)
 - After optimization on desktop
  ![After Optimization Desktop LightHouse Portfolio - version 4](https://user-images.githubusercontent.com/56103269/130655818-b4793d84-9b43-4e76-822f-a885a0bfaef3.png)

  
## Authors

- [@vasudeveloper001](https://www.github.com/vasudeveloper001)

  
