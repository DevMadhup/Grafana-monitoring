# Check CPU usage of localhost Prometheus server
  sum by(mode)(irate(node_cpu_seconds_total{mode!="idle"}[1h]))
