# reveal.rb

Presentations using reveal.js, preprocessing using rake-pipeline.

## Cloning

This repository bundles the latest reveal.js as a git submodule.
After a fresh clone, you need to checkout reveal.js using

    git submodule init
    git submodule update

## Usage

Add your reveal.js presentations to the `source` dir. 
Append '.haml' to the name for preprocessing.

Put static files in the `public` folder, e.g. images.

To write out everything to the `build` directory:

    bundle exec rakep build

To run locally:

    bundle exec rakep server

To update reveal.js:

    git pull --recurse-submodules
