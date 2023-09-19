# Check CPU usage of localhost Prometheus server
  sum by(mode)(irate(process_cpu_seconds_total{mode!="idle"}[1h]))
