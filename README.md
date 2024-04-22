## Project Title: Monitoring Python Web App Total Request Count and CPU Usage with Alerting using Prometheus and Grafana

## Objective:
The objective of this project is to implement monitoring for a Python web application using Prometheus and Grafana, focusing on tracking the total request count and CPU usage of the hosting node. Additionally, we'll set up an alerting mechanism to notify when CPU usage exceeds a certain threshold. Monitoring these metrics will provide insights into the application's usage patterns and resource utilization, facilitating proactive troubleshooting and optimization.

## Project Steps:

 1)  Set Up Python Web Application: Develop a Python web application using a framework like Flask or Django. This application will serve as the target for monitoring.
 2) Instrument Total Request Count Metric: Instrument the Python web application to track the total request count. Implement logic to increment a counter for each incoming request to the application.
 3) Integrate Prometheus with Python Web Application: Use Prometheus client libraries (such as prometheus-client for Python) to expose the total request count metric endpoint in your application code. Register a custom metric for tracking the total request count.
 4) Monitor CPU Usage of Hosting Node: Set up node-exporter to collect system-level metrics, including CPU usage, from the hosting node. Configure Prometheus to scrape metrics from node-exporter to monitor CPU usage.
 5) Configure Prometheus Alerting Rule: Define an alerting rule in Prometheus configuration to trigger an alert when CPU usage exceeds a certain threshold.
 6) Visualize Metrics with Grafana: Install Grafana and configure it to connect with Prometheus as a data source. Create a dashboard in Grafana to visualize the total request count and CPU usage metrics over time. Customize the dashboard to display both metrics graphically and side by side for comparison.
 7) Testing and Monitoring: Test the Python web application by generating various requests and observe the total request count metric in Grafana. Monitor the hosting node's CPU usage in real-time to understand resource utilization. Identify any anomalies or performance issues through monitoring. When CPU usage exceeds the defined threshold, Prometheus will trigger an alert, and Grafana can be configured to receive and display these alerts.

### Project Deliverables:
 1) Python web application with integrated Prometheus metrics tracking total request count.
 2) Node-exporter configured to collect CPU usage metrics from the hosting node.
 3) Configured Prometheus server scraping metrics from the Python web application and node-exporter.
 4) Grafana dashboard visualizing the total request count and CPU usage metrics over time.
 5) Alerting rule in Prometheus to trigger alerts for high CPU usage.
 6) Documentation outlining the setup process, configuration steps, and usage instructions for monitoring the Python web application's total request count and hosting node's CPU usage with alerting using Prometheus and Grafana.

## Port open in Security Group
1) 9090 - Prometheus
2) 5000 - Python flask app running
3) 3000 - Grafana
4) 9100 - node_exporter = this port add in Prometheus.yml file
