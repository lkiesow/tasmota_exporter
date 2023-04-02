# tasmota\_exporter

OpenMetrics exporter for Tasmota devices.

This tool gathers data from Tasmota devices and generates an OpenMetrics
compatible report for Prometheus to be served via a web server like Nginx or
Apache.


## Configuration

Set the location of the metrics file to write to and the list of devices (and passwords) to scrape from in the `config.json` file:

```json
{
	"metrics-file": "/srv/www/metrics/tasmota",
	"devices": {
		"plug-01.example.home": "<password>",
		"plug-02.example.home": "<password>"
	}
}
```
