# Real-Time Anomaly Detection 

![](images/dashboard-gif.gif)



## Platform Architecture

![](images/architecture-square-grey-background-monitoring-block.png)

Our Platform is built using the following tools:
- [JupyterLab](https://jupyter.org/) - An extensible environment for interactive and reproducible computing, based on the Jupyter Notebook and Architecture.
- [FastAPI](https://fastapi.tiangolo.com/) - FastAPI is a Web framework for developing RESTful APIs in Python.
- [Caddy](https://caddyserver.com/) - The Caddy web server is an extensible, cross-platform, open-source web server written in Go. The name "Caddy" refers both to a helper for tedious tasks, and a way to organize multiple parts into a simplified system.
- [Prometheus](https://prometheus.io/) - Prometheus is a free software application used for event monitoring and alerting. 
- [Grafana](https://grafana.com/) - Grafana is a multi-platform open source analytics and interactive visualization web application. It provides charts, graphs, and alerts for the web when connected to supported data sources.


## Makefile Documentation

| Target        | Utility                                                          |
|:--------------|:-----------------------------------------------------------------|
| help          | Lists all targets in this Makefile along with their descriptions |
| run-jupyter   | Build and Run a Jupyter Lab Container                            |
| build-api     | Build the Prediction API Docker Image                            |
| run-api       | Build and Run a Prediction API Container                         |
| run-platform  | Build and Run the entire Platform                                |
| run-all       | Run the Platform and the Jupyter Lab Container                   |
| stop-jupyter  | Kill and Delete the Jupyter Lab Container                        |
| stop-api      | Kill and Delete the Prediction API Container                     |
| stop-all      | Stop the Platform and the Jupyter Lab Container                  |
| remove-all    | Remove all the Docker images we've created                       |
| test-platform | Create Python Virtual Environment, run the tester script and visualize output in Grafana |
| remove-env    | Delete the Python Virtual Environment created for testing        |


