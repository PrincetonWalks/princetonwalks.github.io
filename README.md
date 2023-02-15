# README.md for working with PrincetonWalks.com

## Compiling SCSS

We compile SCSS with Brew's SASS. To do so:
- Install SASS with `brew install sass/sass/sass`
- While developing, you can start `SASS` in watch mode via `sass --watch styles.scss styles.css` in the folder where your CSS/SCC is. You can also run SASS in the top level folder by adding absolute paths to the files.

## Optimizing Images

You can use https://www.websiteplanet.com/webtools/imagecompressor/ to compile images. Images are the heaviest thing on the site and will affect page performance. 

# Deploying Changes

Our site via github pages. Deploying changes to main should update the site in real time (or near real-time depending on caches).