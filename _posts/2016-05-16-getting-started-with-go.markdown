---
layout: post
title:  "Golang and time series databases - an explorative journey"
date:   2016-05-16 18:55:07
categories: go influxdb smappee rest tsdb
tags: go influxdb smappee rest tsdb tutorial
---
Lately I've been reading and hearing a lot about time series databases, which seem to blossom up in various solutions. These types of databases are a nice fit to actually start using these in a small project, I've been nursing the last months in my head.

I live in a home with numerous "smart home" devices like [netatmo weather-station][netatmo], [smappee energy-monitor][smappee], [Danfoss Living][danfoss], [Elgato Eve Energy][elgato]. One thing that strikes me over and over again, is the diversity in how these appliances expose their data. Some of them sure has nice looking apps and web ui's while other really lack this usability. One thing most of them have in common, is the exposure of some good APIs.
Data-points from all these devices are actually just plain time series, which can give hours of fun if accessible in an easy way.
This leads me to the small project I will start out in a 3 part blog series; collecting and visualizing time series using a time series database.

As I'm doing this on a hobby basis, it's important to me that I besides having fun also develop my personal skill set. Therefore I will move into a new language, namely [Golang][golang] and try out new products like [influxdb][influxdb].

The series will be diveded into the before mentioned parts.

1. [Golang][golang] and REST calls
  * Learning Golang in this post and getting to know how to communicate with REST endpoints.
2. Setting up [influxdb][influxdb] and exploring API
  * Installation, configuration, API exploration and visualisation tools
3. Integrating [smappee-data][smappee] into [influxdb][influxdb]
  * Finalising the solution and running it on my home server


The final result should be an automated integration from [smappee][smappee] to [influxdb][influxdb] and a simple dashboard in a visualisation tool to show the historis energy usage.

Part 1 will be online in the coming weeks, as I get to learn [golang][golang] and experiment with it.


[netatmo]:      https://www.netatmo.com/en-US/product/weather-station
[smappee]:   http://www.smappee.com/be_en/energy-monitor
[elgato]: https://www.elgato.com/en/eve/eve-energy
[danfoss]: http://homeowners.danfoss.dk/products/link/home/
[golang]: https://golang.org
[inluxdb]: https://influxdata.com/time-series-platform/influxdb/
