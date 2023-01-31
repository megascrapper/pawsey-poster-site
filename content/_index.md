---
blurb: Internet of Things and smart buildings are all the rage nowadays. While these systems can improve comfort and efficiency, many of these smart systems were built with very little regard to privacy. We are developing an anomaly detection system in time series building IoT data. Also, we identified its privacy threats and propose ways we can mitigate those threats.
description: "By Akbar Fadiansyah -- Supervised by Dr Chehara Pathmabandu"
greeting: ""
image_stretch: true
image_url: stretch.webp
paige:
    titleclass: display-1 fw-bold text-center
title: Anomaly Detection for Privacy Preserving Time Series Building IoT Data
bibFile: /assets/references.json
---

<div class="container">
    <div class="row justify-content-center">
        <div class="col-8 text-center d-grid gap-2">
            <a class="btn btn-primary" href="/pawsey-poster.pdf">View poster</a>
            <a class="btn btn-secondary" href="/poster-references">Poster references</a>
        </div>
    </div>
</div>

&nbsp;
{{< load-plotly >}}

## Background and motivation

Internet of Things (IoT) are becoming increasingly popular as part of building automation system. Most IoT devices currently on the market have limited processing power in order to reduce their cost and power consumption. This usually results in IoT devices offloading their required data processing to the cloud. However, this raises serious privacy concerns as private and sensitive information may be transmitted to the cloud, which has the potential to be leaked or misused. For example, a malicious actor who has the raw sensor data can infer that a building is empty if a power consumption is unusually low for the given time of the day. {{< cite "http://zotero.org/groups/4911682/items/KSN4SY5M" >}}

## Research questions

1. What privacy threats are present in IoT-oriented commercial buildings?
2. How can we reveal activity patterns, anomalous behaviours and other sensitive information from time series data collected by IoT sensors in commercial buildings?
3. What is an appropriate framework to minimise revealing sensitive information in time series IoT data without impacting its functionalities?

## Research methodology

- We conducted a **review of the literature** on commercial IoT privacy, and developed a threat model (RQ1)
- We're **developing an anomaly detection system** for time series building IoT data (RQ2)
  - The idea is that anomalous or unusual readings from IoT sensors may present privacy risks, and thus needs be removed before being sent to the cloud
- We’re also **proposing a framework to mitigate privacy threats** in commercial IoT systems (RQ3)

## Related work

## Threat model

## Dataset and sensor selection

{{< plotly json="/plots/pir_seasonal_hourly_hm.json" height="450px" >}}

{{< plotly json="/plots/co2_seasonal_hourly_hm.json" height="450px" >}}

{{< plotly json="/plots/temp_seasonal_hourly_hm.json" height="450px" >}}

## Model

## Results

## Discussion

## A privacy-preserving IoT architecture

## Future work

## References

{{< bibliography cited >}}
