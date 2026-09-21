---
layout: page
title: "StilleMap"
description: "Urban noise digital twin."
img: /assets/img/logo_stillemap.jpg
importance: 6
category: fun
---

StilleMap (pronounceed /ˈʃtɪləmæp/)

[GitHub repository](https://github.com/akaliutau/stillemap)

We have forecasts for rain, heat, and air quality, but miss one of the most pervasive, invisible pollutants affecting our health: urban noise.
While powerful open-source acoustic engines already exist — like the [NoiseModelling](https://github.com/Universite-Gustave-Eiffel/NoiseModelling) tool from Université Gustave Eiffel  — translating raw, fragmented city data into a working, live noise map has always been painfully complex.

So we built StilleMap: an autonomous digital twin for urban noise. 

Most urban datasets were not designed to measure noise directly.
StilleMap combines **proxy signals** collected for completely different purposes.

One address. One click. And the entire, complex modelling pipeline spins up automatically.

StilleMap unites everything: the location, the local road networks and surrounding building geometry, official Department for Transport historical observations, anchoring the traffic data directly onto the local streets.

But cities are dynamic, so is StilleMap. It analyzes the visual feed from the nearest live TfL traffic camera to evaluate vehicle mix, congestion, and apparent speed. 
All visual insights are translated then into enriched inputs for NoiseModelling.

With the live context locked in, StilleMap compiles the full acoustic scene and then hands the data off to the NoiseModelling engine to run a precise, industry-standard acoustic simulation.

The result is a high-resolution, street-level noise heatmap where you can inspect individual receivers, isolate specific road sources, and compare the historical baseline against the live, real-world traffic scenario.

StilleMap is a new kind of urban intelligence, used to decode the invisible, ambient forces shaping our environment and making our cities a better place to live.

--


