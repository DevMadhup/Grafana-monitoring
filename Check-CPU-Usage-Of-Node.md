# Check CPU usage of node connected to Prometheus server
  sum by(mode) (count_over_time(node_cpu_seconds_total{mode!="idle"}[1h]))
