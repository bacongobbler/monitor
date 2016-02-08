# Deis Monitor

## Description
This repository aims to contain all the necessary components for a production quality monitoring solution that runs on top of the kubernetes cluster scheduler. It provides the [TICK](https://influxdata.com/time-series-platform/) stack which is produced by the influxdata team.

## Current State
Currently this repo provides only 2 components (influxdb and telegraf). Telegraf is the metrics collection agent that runs using the daemon set API. For more infomation please read [this](telegraf/README.md).

Also provided is an influxdb container which only runs 1 instance of the database. It also does not write any data to the host filesystem so it is not a durable system right now. For more information please read [this](influxdb/README.md)


