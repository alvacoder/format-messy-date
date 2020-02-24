# format-messy-time

format messy human date and time strings



# example

```
var format = require('format-messy-time');
var q = process.argv.slice(2).join(' ');
console.log(parse(q));
```

output:

```
$ date; cal
Tue Apr 14 12:20:12 PDT 2015
     April 2015       
Su Mo Tu We Th Fr Sa  
          1  2  3  4  
 5  6  7  8  9 10 11  
12 13 14 15 16 17 18  
19 20 21 22 23 24 25  
26 27 28 29 30        
                      
$ node format.js last wednesday
Wed Apr 08 2015 00:00:00 GMT-0700 (PDT)
$ node format.js 9pm on the 4th of july 1988
Mon Jul 04 1988 21:00:00 GMT-0700 (PDT)
$ node format.js next friday
Fri Apr 24 2015 00:00:00 GMT-0700 (PDT)
$ node format.js this friday
Fri Apr 17 2015 00:00:00 GMT-0700 (PDT)
$ node format.js 6 am tomorrow
Wed Apr 15 2015 06:00:00 GMT-0700 (PDT)
$ node format.js in 2hrs 50 minutes
Tue Apr 14 2015 15:10:12 GMT-0700 (PDT)
$ node format.js 2.5 hours ago
Tue Apr 14 2015 09:50:12 GMT-0700 (PDT)
```

# methods

``` js
var format = require('format-messy-time')
```

## var d = format(str, opts)

format `str`, returning a Date instance `d`.

* `opts.now` - interpret `str` with respect to `opts.now`, default `Date.now()`

# install

With [npm](https://npmjs.org) do:

```
npm install format-messy-time
```

# license

MIT
