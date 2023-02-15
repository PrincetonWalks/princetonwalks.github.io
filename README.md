# README.md for the Recommended Systems Homepage

## SCSS

We compile SCSS with Brew's SASS. To do so:
- Install SASS with `brew install sass/sass/sass`
- While developing, you can start `SASS` in watch mode via `sass --watch styles.scss styles.css` in the folder where your CSS/SCC is (the top-level directory in this case). You can also run SASS in the top level folder by adding absolute paths to the files.

## Linting

We use black as an automated linter. To run black:
- Install with `pip install black`
- Run with `black .` in the correct directory.

# Deplying Changes

Our site is hosted in AWS S3 with a ClounFront cache. 
- You need to upload files to the S3 buckets
    - Buckets: `recommended.systems`, `www.recommended.systems`, `rsco-homepage`
    - Then you need to make sure all of the files are set to public by going into the bucket, selecting all files, and then bulk `Make Public in ACL`
- You also need to clear the CloudFront cache:
    - Cloundfront > Distributions > Invalidations  and create a new invaluation with object paths `/*` to clear the full cache
