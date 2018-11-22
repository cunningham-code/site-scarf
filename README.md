# Site Scarf
Site Scarf is a way to convert your favorite website into a web app.

[This site scarf is for an awesome time tracker called Toggl you should now go try.](https://www.toggl.com/)

------

#### (1) What to add your HTML Headers

```html
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="msapplication-TileColor" content="#e20405">
<meta name="theme-color" content="#ffffff">
<meta content="yes" name="apple-mobile-web-app-capable">
<meta content="black" name="apple-mobile-web-app-status-bar-style">
```

Alright, so what does this code mean? Well, the first three lines give the website a favicon and apple home screen icon.

`<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">`
`<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">`
`<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">`

The fourth line adds a manifest file (we'll get to that next!)

`<link rel="manifest" href="/site.webmanifest">`

The fifth line sets the backgorund on windows when you add a website to the user's home screen

`<meta name="msapplication-TileColor" content="#e20405">`

The sixth line sets the color of the URL bar in chrome.

`<meta name="theme-color" content="#ffffff"></meta>`

The seventh and eighth makes the website act like a website when a user pins it to their home screen.

`<meta content="yes" name="apple-mobile-web-app-capable">`

`<meta content="black" name="apple-mobile-web-app-status-bar-style">`



------

### (2) Let's make that site.webmanifest

```
{
    "name": "Toggl",
    "short_name": "Toggl",
    "icons": [
        {
            "src": "/android-chrome-192x192.png",
            "sizes": "192x192",
            "type": "image/png"
        }
    ],
    "theme_color": "#ffffff",
    "background_color": "#ffffff",
    "display": "standalone"
}
```

This file is a lot more self explanitory. Just make sure to include "display": "standalone".

------

### (3) Let's make Edge happy.

It s file called browserconfig.html.

```
<?xml version="1.0" encoding="utf-8"?>
<browserconfig>
    <msapplication>
        <tile>
            <square150x150logo src="/mstile-150x150.png"/>
            <TileColor>#e20405</TileColor>
        </tile>
    </msapplication>
</browserconfig>
```

Pretty clear too, this just lets you pin a website to your homescreen with Edge.

------

### (4) And now, the images.

Open your photo editor of your choice, and replace all of the files in the folder.

android-chrome-192x192.png

apple-touch-icon.png

favicon-16x16.png

favicon-32x32.png

favicon.ico

launch-640x1136.png

launch-750x1294.png

launch-1125x2436.png

launch-1242x2148.png

launch-1536x2048.png

launch-1668x2224.png

launch-2048x2732.png

mstile-150x150.png

------

### And, that's it.

Whether you are making a website, updating your website, or giving a website in your workflow the code it needs, good luck! Would love to see additions to this.

