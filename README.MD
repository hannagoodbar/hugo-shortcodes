## Hugo shortcodes

### Ordinal abbreviations: ordinalabbreviations.html

As of Hugo v0.49.2, numeric ordinal abbreviations, such as 1st or 2nd, are not supported: [source](https://gohugo.io/functions/format/).

The ordinalabbreviation shortcode adds support for calendar day ordinals, for days from 1 to 31. It uses the HTML ```sup``` and ```small``` tags to emulate superscripted ordinals.

It accepts one parameter, ```day```. If it is passed a day outside the range of 1-31, the ```th``` ordinal is added.

``` html
{{< ordabbr day="2" >}}
```

Results in ```2nd```.
