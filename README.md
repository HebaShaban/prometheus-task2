# prometheus-task2

# 1) How do I trigger a Prometheus alert?

# ![20139661r86QlIMyGV](https://github.com/HebaShaban/prometheus-task2/assets/128882939/adf85ddd-dbe8-4bc8-a135-a13cea87c089)

# 2) What is the difference between node exporter and mysql exporter?

# Node exporter knows how to extract metrics. Those are exposed in HTTP, eg. :9201/metrics. Prometheus queries every X seconds those HTTP endpoints (node-exporter HTTTP) and stores the metrics. It also provide another HTTP for graph/console visualization/querying.22‏/11‏/2019

# 3)what is the maximum retention period to save data in Prometheus and how to increase it?

# By default the retention is configured to 15 days. The amounts of data stored on disk depends on retention — higher retention means more data on disk. The lowest supported retention in Prometheus is 2 hours (2h)

# 4) What are the different PromQL data types available in Prometheus Expression language?

# PromQL, short for Prometheus Querying Language, is the main way to query metrics within Prometheus. You can display an expression's return either as a graph or export it using the HTTP API. PromQL uses three data types: scalars, range vectors, and instant vectors. It also uses strings, but only as literals.

# To calculate the average request duration over the last 5 minutes from a histogram in Prometheus, you can use the histogram_quantile() function in combination with the rate() function and a time range selector.

# 6) What is Thanos Prometheus?

# Thanos is an open-source project that extends Prometheus, a popular time series database. It is designed to tackle some of the challenges faced when operating Prometheus at scale, especially in highly distributed and long-term storage scenarios.

# 7) What is Promtool and how i can use it?

# Promtool is a command-line tool that is used to interact with Prometheus. It can be used to do a variety of things, including:
- Querying Prometheus data: Promtool can be used to query Prometheus data using PromQL.
- Validating Prometheus configuration: Promtool can be used to validate Prometheus configuration files.
- Generating Prometheus rules: Promtool can be used to generate Prometheus rules. This can be useful for creating alerts and notifications based on your Prometheus data.
- Testing Prometheus alerts: Promtool can be used to test Prometheus alerts.
