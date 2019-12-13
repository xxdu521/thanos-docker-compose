
1，Run  docker-compose up -d  

2, Check  
  #compactor_1
  #prometheus1_1
  #sidecar1_1
  #sidecar2_1
  #storer_1
  #prometheus2_1
  #domain_exporter_1
  #grafana_1
  #traefik_1
  #minio_1
  #querier_1
  #alertmanager1_1
  
3, Access
  http://localhost:8080 traefik dashboard
  http://localhost:9000 minio (minio/password)
  http://localhost:9091 prometheus
  http://localhost:19192 thanos query
  http://localhost:3000 grafana (prometheus_url http://localhost:19192)
  
4, Remark
  Storer_1 startup, requires manually creating test buckets in minio
