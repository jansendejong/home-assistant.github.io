---
layout: page
title: "London Underground"
description: "Display the current status of London underground & overground lines within Home Assistant."
date: 2017-07-15 18:45
sidebar: true
comments: false
sharing: true
footer: true
logo: london_underground.png
ha_category: Transport
ha_iot_class: "Cloud Polling"
ha_release: 0.49
---


The `london_underground` sensor will display the status of London underground lines, as well as the Overground, DLR and Tfl rail.


```yaml
# Example configuration.yaml entry
sensor:
  - platform: london_underground
    line:
      - Bakerloo
      - Central
      - Circle
      - District
      - DLR
      - Hammersmith & City
      - Jubilee
      - London Overground
      - Metropolitan
      - Northern
      - Piccadilly
      - TfL Rail
      - Victoria
      - Waterloo & City
```

Configuration variables:

- **line** (*Required*): Enter the name of at least one line.

Powered by TfL Open Data [TFL](https://api.tfl.gov.uk/).
