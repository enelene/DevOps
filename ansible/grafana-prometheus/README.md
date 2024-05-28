role1: grafana-server
	installs grafana-server
	In the grafana configuration file, port, listen address, username, and password are changeable.
	Installs Nginx server and creates the Nginx server block for the Grafana-Server.
	Imports Node Exporters Dashboard and Prometheus datastore. 
	
role2: prometheus-alertmanager
	if Prometheus:true than installs prometheus service and cofigures configuration file.
	if alertmanager:true than installs alertmanager service and configures configuration file.
	
