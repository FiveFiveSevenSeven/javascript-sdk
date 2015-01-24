# ClanOfTheCloud.com Javascript client

The 'jsclient' can be used both from node.js or from a web browser. It's written in Coffee-script, then compiled to
javascript with Browserify and optionnally minified to a mere 20kB, less than 5kB after gzip compression.

Note: This client is not feature complete yet. It implements the latest (API)[http://docs.clanofthecloud.apiary.io/#].
Feel free to submit bug reports and/or pull requests.

## Set up

After cloning this repository, you can use `npm install` to grab dependencies (with node.js installed).
Coffee-script sources live in `/src` while the compiled JS is in `/lib`.

`npm run compile` will compile the Coffee-script sources to `/lib/bundle.js` and `/lib/bundle.min.js`

## Use from node.js

The package is not published on the public npmjs.org repository yet.

## Use in a Web browser

You need a single JS script, `/lib/bundle.js`, which inlines `superagent`, the only dependency.

Then you can use the Clan class as a starting point. See (/lib/example.html)[https://github.com/clanofthecloud/javascript-client/blob/master/lib/example.html]
for a basic example.