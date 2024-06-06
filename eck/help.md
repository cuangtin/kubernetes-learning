#### Get elasticsearch user elastic password:
``kubectl get secret elasticsearch-es-elastic-user -o go-template='{{.data.elastic | base64decode}}'``

#### Check elasticsearch connection
``curl -k -u 'elastic:<password>' https://localhost:9200``

[Source](https://devopsvn.tech/kubernetes-practice/trien-khai-elasticsearch-len-tren-kubernetes-cloud)