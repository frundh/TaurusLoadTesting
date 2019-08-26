# Taurus Load Testing
This repository is to load testing http endpoint using blazemeter taurus using Apache JMeter executor. It also demonstration auto generation of html reports in local machine using JMeter without using the blazemeter online reporting services. Also it explains steps to generate a unified html report if the load test is run from multiple machines to simulate distributed load testing.

## Why is this sample repository created
I had generate offline html reports after test completion in Taurus without using Blazemeter's online service. Hence created this sample repository to demonstrate the auto html report generation using Taurus.

More on this is explained in my blog at [Blazemeter Taurus load testing and offline jmeter html report](https://blogs.harishkannarao.com/2018/09/blazemeter-taurus-load-testing-and.html)

## Run
```
docker run --rm --name bzt -v ${PWD}/tests:/bzt-configs -v ${PWD}/artifacts:/tmp/artifacts blazemeter/taurus blazedemo-journey.yml html-report.yml
```