# Check free disk space on node server
sum by(mountpoint) (node_filesystem_free_bytes{})
