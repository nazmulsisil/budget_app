# Steps to set up the boilerplate

### DONE

**node-sass**
<br />
*[no dependency]*
<br />
node-sass: take files <br />
from `./src/styles/sass/from_sass.scss` <br />
to `./temp/styles/from_sass.css` <br />
**notes:** completed and added script in package.json file which will automatically combine all files into a single file called "from_sass.scss" and then convert that file to regular css file named "from_sass.css", but still live-server is not detecting css file changes because css files hasnt been transported to public folder where live-server is pointing to. So gulp task will do it, or concat will do it.

**gulp** <br />
_[no-dependency]_

**post-css** <br />
_[gulp]_ <br />
gulp-post-css: takes files <br />
from `src/styles/postcss/from_postcss.css`
to `./temp/styles/from_postcss.css`
**notes:** completed postcss set up and compilation to a single file into temp folder. I used postcss nested, simple-vars, mixins, hexrgba, autoprefixer

**Take temp files and move to public folder**

**gulp-watch**

**browsersync** <br />
**notes:** Do not download version 2, that will not work with my gulp coding.

**css injection** <br />
**notes:** Completed watching for changes in css, scss, sass files and folders with gulp-watch, and inject the styles code by browsersynd.stream()

**Webpack**
**notes:** completed webpack and gulp setup to watch src/scripts/\*_/_.js, then bundle, then refresh browsersync

**babel**
**notes:** completed babel setup which auto compiles and gulp watch everything and refresh page!

### TO DO

**minimize file size and production process**
