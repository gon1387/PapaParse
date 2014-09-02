BabyParse
=========

I needed a really fast and reliable CSV parser. [PapaParse.com](http://papaparse.com) is the best one I've come across yet but it's designed for web sites and uses several features exclusive to browsers.

So I extracted the actual parser and made it Node/AMD compatible, so that I could drop it into server-side projects. The code hasn't been touched other than that. It seems pretty decent. In the project I'm working on now it was an order of magnitude quicker than the thicket of regex hacks it replaced.

Don't thank me, thank [@mholt6](https://twitter.com/mholt6). (Thanks Matt!)



Usage
-----

```js
// pass in the contents of a csv file
parsed = Baby.parse( csv );

// voila
rows = parsed.data;
```

See the [documentation for Papa Parse](http://papaparse.com/docs.html) since it's the same in Baby Parse, but realize that a few features (like downloading, file reading, and worker threads) are unavailble in Baby Parse.


License
-------

The original PapaParse is MIT licensed. So is BabyParse.
