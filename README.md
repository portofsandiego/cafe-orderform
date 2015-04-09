# cafe-orderform
The Coast Cafe food and beverage menu.

Details
---

This site uses out-of-the-box [Twitter Bootstrap](http://getbootstrap.com/ "Twitter Bootstrap") framework components, including media carousels, dropdown menus, sticky navbars, list-groups, and modals. Glyph icons are included using Bootstrap and [Font Awesome](http://fortawesome.github.io/Font-Awesome/ "Font Awesome"). CSS3 is straight-forward and does not currently use a Sass preprocessor. jQuery is included locally.

Installation
---

It is strongly recommended that designers use this guide or risk garbage output, unmaintainable code, and a flurry of other potential problems.

The framework of the website and workflow require [Yeoman](http://yeoman.io/ "Yeoman, the world's scaffolding tool for modern webapps"), [Grunt](http://gruntjs.com/ "Grunt, the JavaScript Task Runner"), and [Bower](http://bower.io/ "Bower, a package manager for the web"). These open source tools are freely available for any design platform (Windows/Mac/Linux). Bower requires [Node with npm](http://nodejs.org/ "Node.js, a fast, scalable web design platform built upon Google Chrome's JavaScript runtime engine"), and all source should be managed under [Git](http://git-scm.com/ "Git, a free and open source distributed version control system").

1.  Using a shell, first install Node.js with [npm](https://www.npmjs.com/ "npm, a package manager for everything"). On a Mac with [Homebrew](http://brew.sh/ "Homebrew, the missing package manager for OS X"), this can be done quite easily: `brew install node`
2.  Install Yeoman and the other prerequisites: `npm install -g yo bower grunt-cli gulp` The `-g` flag installs item globally which is essential to avoid scope issues.
3.  Install the base Yeoman generator for this project: `npm install -g generator-webapp` which is a generic project framework that can contain base technologies like Bootstrap, jQuery, Modernizr, and HTML5 Boilerplate.
4.  Clone or fork this Git repository onto your local system and change directory into the project folder.
5.  All dependencies should be included but to be safe, run `bower install --save`

Editing
---

1.  Run the Grunt watch system which will monitor all code changes and compile anything of importance automatically: `grunt serve`
2.  Grunt will open a browser window with a live-reloading —yes, live-reloading version of the project at `http://localhost:9000` Anytime you save changes, the browser will automatically reload the content.

**Make all your design and content changes in the `/app` folder. Do not change the paths for anything that is contained within the build/bower blocks.** Please use Bootstrap conventions as this project makes extensive use of the framework.

3.  When you are happy with your changes/updates, commit your code into Git and push to GitHub. Edit and commit often to keep your changes well documented for other teams.

Deploying
---

1.  If Grunt is still running its watch, stop the process with a `Ctrl-C` Then run `grunt` which will compile, minify, and optimize all the source code from `/app` into `/dist` Please note that the distribution folder is referenced in the `.gitignore` file and should not be committed to the Git repository.
2.  Copy all the files from the `/dist` folder into your production webserver and enjoy!
