# Cloud9 IDE

The Cloud9 IDE is an open source project started by Fabian Jakobs ([fjakobs]), Ruben Daniels ([javruben], Mike de Boer ([mikedeboer]) and Rik Arends ([rikarends]) from [ajax.org], built on top of [Node.JS].

This Integrated Development Environment aims to bring all great features from other existing IDE's and source code editors like Eclipse, Netbeans, Textmate, and many others together, bundled as plugins.
Cloud9's main focus is on Javascript development, it is able to set a new standard for client and server development integration.

And if you find that functionality is missing? Just write a plugin and patch it yourself!

Written in Javascript, for Javascripters.

## Features

  * High performance text editor with bundled syntax highlighting support for JS, HTML, CSS and mixed modes.
  * Integrated debugger for [Node.JS] applications which can started, paused and stopped from within the IDE
  * Integrated debugger for the Google Chrome browser which can started, paused and stopped from within the IDE
  * Local filesystem is exposed through [WebDAV](http://en.wikipedia.org/wiki/WebDAV) to the IDE, which makes it possible to connect to remote workspaces as well
  * Highly extensible through the plugin system
  * Bundled plugins: browser, clipboard, code (editor), console, debugger, docs, editors, filesystem, html, keybindings, newresource, noderunner, panels, refactor, richtext, save, searchreplace, settings, tree, undo

## Browser Support
We are developing on firefox and this is a development repo, other browsers might be less stable until a proper release.

## Usage

After a Git checkout of the project or download (see Installation section), the command you need to run the IDE locally is the following:

To start cloud9 and install all submodules you can use the quickstart options for your platform on the console or from your explorer/finder and opens it in your default browser:

Linux and OSX:

    $ bin/cloud9.sh

Windows:

    > bin\cloud9-win32.bat

Note you'll need a git version 1.7 or higher to use the stock shell script provided.

If you want to start it manually try:

    $ node bin/cloud9.js

This runs the IDE with itself set as the workspace. When you open the url 

    http://localhost:3000
    
in your browser, it will show the directory structure of the current workspace in a tree. Since none is provided by the startup command above, it will show the IDE directory contents as a default workspace.

You can specify your own workspace as follows:

    $ node bin/cloud9.js -w /path/to/your/awesome/workspace

And as a result the tree will display the contents of that directory.

You can specify the ip cloud9 is listening to using:

    $ node bin/cloud9.js -l 192.168.2.1

Or specify to listen to all ip's

    $ node bin/cloud9.js -l all

To see more usage information and additional command line options use.

    $ node bin/cloud9.js -h

## Installation

Via git (or downloaded tarball):

    $ git clone git://github.com/ajaxorg/cloud9.git

Via [npm](http://github.com/isaacs/npm):

    $ npm install cloud9

## Documentation

Documentation is in the making. 

## Open Source Projects Used

The Cloud9 IDE couldn't be this cool if it weren't for the wildly productive [Node.JS] community producing so many high quality software.
Main projects that we use as building blocks:

  * [async.js] by [fjakobs]
  * [jsDAV] by [mikedeboer]
  * [connect] by [senchalabs](http://github,com/senchalabs)
  * [socket.io] by [LearnBoost](http://github.com/LearnBoost)
  * [ace](http://github.com/ajaxorg/editor) by [fjakobs]
  * [apf](http://www.ajax.org) by [ajax.org]
  * and of course [Node.JS]!
  
Thanks to all developers and contributors of these projects! 

[fjakobs]: http://github.com/fjakobs
[javruben]: http://github.com/javruben
[mikedeboer]: http://github.com/mikedeboer
[ajax.org]: http://www.ajax.org/
[async.js]: http://github.com/fjakobs/async.js
[jsDAV]: http://github.com/mikedeboer/jsdav
[connect]: http://github.com/senchalabs/connect
[socket.io]: http://github.com/LearnBoost/Socket.IO-node.git
[requireJS]: http://requirejs.org/
[Node.JS]: http://nodejs.org/

## License

The GPL version 3, read it at [http://www.gnu.org/licenses/gpl.txt](http://www.gnu.org/licenses/gpl.txt)
