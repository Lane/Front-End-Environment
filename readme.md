# What is this?

This is a base vagrant box with npm and grunt tasks preconfigured that will:

  - Serve files from the `/build` directory
    - auto refresh when there are html, css, or js changes (via [reload](https://www.npmjs.org/package/reload))
  - Watch `/src/less/style.less` for changes 
    - compile into css file in `/build/css` 
  - Watch `.js` files for changes 
    - concatenate vendor scripts in `/src/js/vendor`
    - concatenate author scripts in `/src/js`
    - uglify
    - copy to `/build/js`
  - Watch `.html` files for changes
    - copy to `/build` when modified

## Getting Started

  - Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
  - Install [Vagrant](http://www.vagrantup.com/downloads.html)

Once you have VirtualBox and Vagrant installed, clone this repository.  Go into the "tools" folder and run `mac-start.command` (Mac/Linux) or `win-start.bat` (Windows).

Running the start command will download the development environment and run it on your machine.  The initial download / setup will only happen the first time.

Once the initial setup is complete, you should be able to navigate to `http://localhost:3333/` and see a "Hello World!" message.

You can now modify any of the less, js, or html files and see a live preview in your browser.