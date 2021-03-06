---
layout: post
title: "Accessing macOS Location Services from the command line"
category: featured
tags: [programming, Mac, Objective C, geolocation]
---
{% include JB/setup %}

I wanted to access location services data from a bash script so I threw together [osx-location](https://github.com/WIZARDISHUNGRY/osx-location).
```
$ make
$ ./location --help
--count <number>         Wait for this many responses (default: 1).
--debug                  Output helpful debugging info.
--format <format>        Set the output format (default: key-value).
--help                   Show this help.
Formats available:
              k = key-value
              j = Geo JSON
              s = SBS-1 ADS-B

$ ./location --debug
location service enabled
<+40.696969,-73.420420> +/- 65.00m (speed -1.00 mps / course -1.00) @ 6/18/13 8:43:43 PM Eastern Daylight Time
timestamp: 2013-06-19 00:43:43 +0000
latitude,longitude: 40.696969,-73.420420
altitude: 26.000000
horizontalAccuracy: 65.000000
verticalAccuracy: 10.000000
speed: -1.000000
course: -1.000000
```
