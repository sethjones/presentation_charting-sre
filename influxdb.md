# Running InfluxDB Locally

docker run -d --network=mynetwork -p 8086:8086 --name=influxdb influxdb:latest

Running in this fashion will not save the data beyond this execution of the container.  In order to persist the data you will be required to mount a volume to the container.


# Data Import

The data window is from midnight 6/13/24 minus two days.

## Influx docs
https://hub.docker.com/_/influxdb

# Notes

The organization and bucket you set during the influx db onboarding UI should be what you enter in the grafana data source configuration ui.

***If you would like to persist your data in grafana or influx between container runs, you will need to mount a volume in docker according to the container requirements.***