# Awesome PMM

A curated list of awesome Percona Monitoring and Management (PMM) free and open-source software, libraries and resources. 

Percona Monitoring and Management (PMM) is a single pane of glass to help manage complex database environments in public, private or on-premises environments.

Designed to help DBAs and developers gain deep insight into their applications and databases, PMM is used by thousands of organizations around the globe to manage complex database environments.

## Content

- [Resources](#resources)
	- [Videos](#videos)
- [Dashboards](#dashboards)
    - [Resources](#resources-1)
    - [Community Dashboards](#community-dashboards)
- [Exporters](#exporters)
	- [Resources](#resources-2)
	- [Percona](#percona)
	- [Community Exporters](#community-exporters)

## Resources

- [Official website](https://www.percona.com/software/database-tools/percona-monitoring-and-management) - Landing page
- [Demo](https://pmmdemo.percona.com/graph/) - pmmdemo.percona.com.
- [Jira](https://jira.percona.com/projects/PMM/issues/) - issue tracker. Use the JIRA to report a bug.
- [Blog](https://www.percona.com/blog/tag/pmm/) - news, cases, lessons, webinars and articles.
- [Forum](https://www.percona.com/forums/questions-discussions/percona-monitoring-and-management) - the best place for non-Customers looking for free PMM Help.
- [User manual](https://learn.percona.com/download-percona-monitoring-and-management-pmm-manual-2-0) - Download PDF. Operations Manual is 200 pages of easily referenced documentation in PDF format.
- [Documentation](https://www.percona.com/doc/percona-monitoring-and-management/2.x/index.html) - excellent online documentation. How to install, configure and use.
- [Download](https://www.percona.com/downloads/pmm2/) - download Percona Monitoring and Management
- [Installation](https://www.percona.com/doc/percona-monitoring-and-management/2.x/install/index-server.html) - Percona Monitoring and Management (PMM) employs a client/server model. You must download and install both the client and server applications. 
- [GitHub](https://github.com/percona/pmm/tree/PMM-2.0) - the main repository. You can find links to other PMM repositories.
- [Docker](https://hub.docker.com/r/percona/pmm-server) - Docker images of PMM Server.


### Videos

- [What is new in PMM2?](https://www.youtube.com/watch?v=Tlxo2BMf9-c) – by Michael Coburn (Percona). [Official website](https://www.percona.com/resources/videos/whats-new-pmm2).
- [Monitoring MongoDB with Percona Monitoring and Management (PMM)](https://www.youtube.com/watch?v=FqdSs9H7mBM) – by Doug Duncan (Percona), Adamo Tonete (Percona). [Official website](https://www.percona.com/resources/videos/automate-pmm-deployment-ansible).
- [Automate PMM Deployment with Ansible](https://www.youtube.com/watch?v=OjKcSQOzNeQ) – by Max Bubenick (Percona). [Official website](https://www.percona.com/resources/videos/automate-pmm-deployment-ansible).

## Dashboards 

PMM Server uses Grafana Dashboards.

### Resources

- [Grafana Dashboards by Percona](https://github.com/percona/grafana-dashboards) - This is a set of Grafana dashboards for database and system monitoring using Prometheus datasource.
- [Grafana Marketplace](https://grafana.com/grafana/dashboards?search=PMM) – community built dashboards.

### Community dashboards

- [MySQL InnoDB Mutex](https://grafana.com/grafana/dashboards/9892) - by Daniel Guzman-Burgos. [Configuration article](https://www.percona.com/blog/2019/03/12/pmms-custom-queries-in-action-adding-a-graph-for-innodb-mutex-waits/).
- [System Processes Metrics](https://grafana.com/grafana/dashboards/8378) - by chaudhryfaisal. Show Linux Process information as captured by [process-exporter](https://github.com/ncabatoff/process-exporter).
- [Clickhouse Grafana Dashboard](https://grafana.com/grafana/dashboards/882) – by Yegor Andreenko for [Clickhouse Exporter for Prometheus](https://github.com/percona-lab/clickhouse_exporter).
- [MySQL InnoDB Cluster] Group Replication (https://grafana.com/grafana/dashboards/10006) - by Valentin Traen. [Custom Queries example](https://github.com/valentinmysql/MySQL-PMM-innodb_cluster_monitoring)

## Exporters

PMM Client uses Prometheus exporters. Applications store their metrics in arbitrary formats, and Prometheus exporters collect them and produce (or export to) a consistent format of key-value pairs.

### Resources

- [Official Percona Exporters](https://github.com/percona/pmm/tree/PMM-2.0#pmm-client) - Percona has developed Prometheus exporters for popular open-source databases.
- [Prometheus exporters](https://prometheus.io/docs/instrumenting/exporters/) - you can plug in Prometheus exporters for technologies not directly provided by Percona.
- [Examples of use](https://www.percona.com/blog/2018/02/12/percona-monitoring-management-pmm-support-external-monitoring-services-yes/) - Does Percona Monitoring and Management (PMM) Support External Monitoring Services? Yes It Does!
- [Textfile collector](https://www.percona.com/blog/2018/08/28/extend-metrics-for-percona-monitoring-and-management-without-modifying-code/) -  Expose statistics read from local disk. How to extend the list of available metrics without modifying the node_exporter code. It’s based on the textfile collector.

### Percona
- [Percona Node Exporter](https://github.com/percona/node_exporter) - Prometheus exporter for hardware and OS metrics exposed by \*NIX kernels, written in Go with pluggable metric collectors.
- [Percona MySQL Exporter](https://github.com/percona/mysqld_exporter) - Prometheus exporter for MySQL server metrics.
- [Percona MongoDB Exporter](https://github.com/percona/mongodb_exporter) - Based on [MongoDB Exporter](https://github.com/dcu/mongodb_exporter) by [David Cuadrado](https://github.com/dcu)
- [PostgreSQL Server Exporter](https://github.com/percona/postgres_exporter) - Prometheus exporter for PostgreSQL server metrics.
- [Percona ProxySQL Exporter](https://github.com/percona/proxysql_exporter) - Prometheus exporter for ProxySQL performance data.
- [Percona RDS Exporter](https://github.com/percona/rds_exporter) - An AWS RDS exporter for Prometheus. It gets metrics from both basic CloudWatch Metrics and RDS Enhanced Monitoring via CloudWatch Logs.

### Community Exporters

- [Clickhouse Exporter for Prometheus](https://github.com/percona-lab/clickhouse_exporter) – by Yegor Andreenko. [Clickhouse Grafana Dashboard](https://grafana.com/grafana/dashboards/882) could be a start for inspiration.
- [Redis Metrics Exporter](https://github.com/oliver006/redis_exporter) – Prometheus exporter for Redis metrics. Instructions in the section "Example 2: Adding a Redis Monitoring Service" in the [article](https://www.percona.com/blog/2018/02/12/percona-monitoring-management-pmm-support-external-monitoring-services-yes/).

## Configuration Management

PMM Server & Client can be managed using various configuration management frameworks.

### Ansible

- [PMM Client]() - by @michaelcoburn
- [PMM Server]() - by @michaelcoburn