### List of the file with their location
* grafana.ini - /etc/grafana/grafana.ini
  * grafana configuration file
* grafana.db - /var/lib/grafana/grafana.db
  * grafana database including all dashboards
* Seduce Project-1634894490446.json - Download the file from a running grafana
  by using the share button next to the dashboard title
  * The JSON description of the Home dashboard
* Energy-1634893607247.json - Download the file from a running grafana by using
  the share button next to the dashboard title
  * The JSON description of the Energy dashboard
* Temperatures-1634893648566.json - Download the file from a running grafana by
  using the share button next to the dashboard title
  * The JSON description of the Temperature dashboard
* Weather@IMT-Atlantique (Nantes)-1634893626770.json - Download the file from a
  running grafana by using the share button next to the dashboard title
  * The JSON description of the Weather dashboard

### Scripts to generate dashboard description files
* energy-dashboard.py: generate the description of the Energy dashboard by
  reading the InfluxDB database.
* seduce_rack.png: the image display in the Home dashboard page. This image is
  located to `/usr/share/grafana/public/img/`.
* seduce_rack_src.tar.gz: the GIMP source of the image `seduce_rack.png`
* temp-names.json: list of the human readable names of the temperature probes
* temperature.yaml: configuration file of the temperature probes used by the
  seduceboard project
* parse-temperature.py: generate the file `temp-names.json` from the file
  `temperature.yaml`
* temperature-dashboard.py: fill the temperature dashboard description file with
  the temperature probes
