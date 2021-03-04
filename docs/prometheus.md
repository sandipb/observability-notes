# Prometheus

## Basics

- [How does a Prometheus Counter work?](https://www.robustperception.io/how-does-a-prometheus-counter-work)
  Also, a video on the same:
  <iframe width="560" height="315" src="https://www.youtube.com/embed/67Ulrq6DxwA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Configuration

- [Life of a label](https://www.robustperception.io/life-of-a-label): How do labels get created and modified between scrape and storage.
- [Extracting labels from legacy metric names](https://www.robustperception.io/extracting-labels-from-legacy-metric-names): Useful for converting non-Prometheus aware metrics to metrics with label metadata.
- [Deleting time series from Prometheus](https://www.robustperception.io/deleting-time-series-from-prometheus). Also, the [official API docs](https://prometheus.io/docs/prometheus/latest/querying/api/#clean-tombstones) mentions the _clean tombstones_ api.
## Promql

- [Using `irate()` vs `rate()`](https://www.robustperception.io/irate-graphs-are-better-graphs): TLDR - Prefer `irate()` for more responsive graphs, and `rate()` for lower-noise alerting.
- [Understanding Machine CPU usage](https://www.robustperception.io/understanding-machine-cpu-usage) is a good primer on calculating CPU usage

## Other

- [openmetrics.io](https://openmetrics.io/): A standardized version of the [Prometheus exposition format](https://github.com/prometheus/docs/blob/master/content/docs/instrumenting/exposition_formats.md). Unlike Prometheus, it supports both plain text and protocol buffers.
