### 🥤 Gulp build to integrate in vue-cli
---
### 📖 Quick guide
This Gulp build can:
- Convert fonts sequentially from otf to ttf and then ttf to woff and woff2 formats
- Convert all popular types of images to WebP (optimized format without any quality loses
and with less file weight)
- Make svg sprite from several svg icons. This task is not automated and requires you to run
__*npm run svgSprive*__ task in the command line (in svgSprive.js file you can turn on or
off building an example file, which can be useful for connecting svg's to working file)
- Archive /dist folder into a zip file with compression (just run __*npm run zip*__)
---
All npm scripts can be found in the package.json file

To make this gulp build work you must put processing files into /gulp-src folder.

Your folder might be looking like this:
root
-- gulp-src
---- files
---- fonts
---- img
---- svgicons

Then, after gulp work, you can find all processed files into /src/assets folder.