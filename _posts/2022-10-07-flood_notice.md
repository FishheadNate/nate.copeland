---
layout: post
title: "Flood Notion iOS"
author: "Nathan Copeland"
categories: samples
tags: [sample]
image: padus_v2_1.png
---

![Simulator Screen Recording - iPhone 14 Pro - 2022-10-06 at 14 30 40](https://user-images.githubusercontent.com/22895187/194402589-4bbc945a-f5f1-4570-becb-5f4135057580.gif)

### Coverage Area:

Initial coverage is limited to Ozark Mountains, with plans to expand it to the entire US and Puerto Rico.

<iframe src="https://api.mapbox.com/styles/v1/copeys/cl627pe2o000e14s6xk8ht4ft.html?title=view&access_token=pk.eyJ1IjoiY29wZXlzIiwiYSI6ImNsNHI3c3NnZTB5d3ozYnF6a2hrYmdjazEifQ.3EuBe1AnQ3k3BrO6SfESVg&zoomwheel=true&fresh=true#6/36.224/-93.408" title="Colorado USFS and BLM Lands" style="border:none; min-width: 320px; max-width:820px; width:100%; height:620px "></iframe>

### Objectives

1. Build a clean, easy to digest rendering of the stream flow data published by the National Weather Service (NWS) Advanced Hydrologic Prediction Service (AHPS).
2. Expend my comprehension of Swift and UX/UI design


### Background

The original planning focused on addressing a need within my extended family for a simple, easy to navigate method for interacting with the NWS AHPS that could be utilized by everyone.

After chatting with some friends about a Swift app they were tinkering with to teach their kids math, I decided to dust off my comprehension of Swift and challenged myself to build a 100% Swift based app to address this need. Midway through, I decided to make it an [open-source project](https://github.com/FishheadNate/FloodNotice-iOS).

Several different databases and services were sourced to collect stream gage locations, stream flows, flood stage thresholds, along with geospatial relations amount the stream gages.

The location of stream gage stations, current observations, and the forecast are sourced from the NWS AHPS. A crosswalk JSON from NWS is used to build relations between the NWS site identities and United States Geological Survey (USGS) gage identities. Which was required to query the Hydro Network-Linked Data Index (NLDI) to source neighboring stream gage stations.
