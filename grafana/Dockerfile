FROM grafana/grafana-oss

ADD --chown=grafana:root https://raw.githubusercontent.com/domainaware/parsedmarc/refs/heads/master/grafana/Grafana-DMARC_Reports.json-new_panel.json /var/lib/grafana/dashboards/
RUN chmod 644 /etc/grafana/provisioning

COPY grafana-provisioning/ /etc/grafana/provisioning/
