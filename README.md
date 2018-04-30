# [FORKED] Node Google Search Crawler

This is a fork of `node-g-search` package to use in the #hackathonglobo2018 project (https://github.com/pamepeixinho/backend-hackathon-globo-2018 and https://github.com/pamepeixinho/pwa-hackathon-globo-2018).

## Change

The main change here is pass the data of the publication too when make the google's search.

## Installation

	npm install --save node-g-search

## How to use it ?

Just put this 11 lines and run `node MYFILE.js` and you're going to see the results

```js
const g = require('node-g-search');

g.search("memes trump")
    .then((d) => {
	if(d.data)
	   for (var i = 0; i < d.data.length; i++) {
		console.log(d.data[i].title);
		console.log(d.data[i].href);
		console.log(d.data[i].des);
		console.log(d.data[i].date);
	    }
});
```

