# 🔥 Initial Refactorization of Frontend Application (ReactJS Version)

## Changes in `frontend/public/index.html`

1. Change the `content` of `<meta>` Tag HTML Element

```html
<meta
      name="description"
      content="Phone Book Management System created using ReactJS and TypeScript"
    />
```

2. Change the `title` Tag HTML Element

```html
<title>Phone Book Management System</title>
```

## Visit Favicon Icon Manipulation Website

[Favicon Icon Generator](https://favicon.io/)

![Favicon Icon Generator Website](/documentation/images/Favicon-Icon-Generator.png)

`😎 → ICO` has been used in this project.

From the `Categories` Dropdown List, select Object to generate the Favicon Icon Image.

![Emoji To ICO Selection](/documentation/images/Emoji-ICO-Selection.png)

Scrolling down and finding out the relevant icon that matches with the context of the application is very important.

![Icon Selection](/documentation/images/Icon-Selection.png)

Click `Download` to download the Icon

![Icon Selection](/documentation/images/Download-Icon.png)

After the download has been completed, extract the files from the ZIP File.

![File Details](/documentation/images/File-Details.png)

Rename the following files : 

| Old Name | New Name | 
| -------- | -------- | 
| android-chrome192x192.png | logo192.png | 
| android-chrome512x512.png | logo512.png |

Copy <b>ALL</b> Image Files except `about.txt` and `site.webmanifest` to `frontend/public/` Directory.

## Refactorization of Files & Folders

Update the file name of the `href` Attribute to `apple-touch-icon.png` like the following:

```html
<link rel="apple-touch-icon" href="%PUBLIC_URL%/apple-touch-icon.png" />
```

Open `manifest.json` File in `frontend/public/` Directory

Update the `manifest.json` like below : 

```json
{
  "short_name": "PBMS",
  "name": "Phone Book Management System",
  "icons": [
    {
      "src": "favicon.ico",
      "sizes": "48x48",
      "type": "image/x-icon"
    },
    {
      "src": "favicon-16x16.png",
      "sizes": "16x16",
      "type": "image/png"
    },
    {
      "src": "favicon-32x32.png",
      "sizes": "32x32",
      "type": "image/png"
    },
    {
      "src": "logo192.png",
      "type": "image/png",
      "sizes": "192x192"
    },
    {
      "src": "logo512.png",
      "type": "image/png",
      "sizes": "512x512"
    }
  ],
  "start_url": ".",
  "display": "standalone",
  "theme_color": "#000000",
  "background_color": "#ffffff"
}
```

## Update `logo.svg`

1. Visit [PNG To SVG Converter](https://www.pngtosvg.com/) Website.

2. Scroll down and Click `Choose File`

![Convert PNG to SVG](/documentation/images/PNG-SVG-Converter.png)

3. Select `logo512.png`

![Select PNG File](/documentation/images/File-Selection.png)

4. Click on `Generate` by scrolling down

![Generate SVG](/documentation/images/Generate-SVG.png)

5. Download Generated SVG File

![Download Generated SVG](/documentation/images/Download-Generated-SVG.png)

6. Rename the downloaded file to `logo.svg`

7. Move the file to `frontend/src/` Directory

## Code Refactorization

1. Delete the following code block in `App.tsx` File.

![Delete Code Block of App.tsx 1](/documentation/images/Code-Refactor-1.png)

2. Rename the `<div></div>` to `<main></main>` HTML Tag Element as shown below : 
![Change DIV To MAIN HTML Tag Element](/documentation/images/Code-Refactor-2.png)