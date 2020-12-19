# Kubenetes Port

Pod: 
- containerPort: 只是顯示Pod的哪個Port有Service, 純資訊, 無Function. 方便後續建立 Service 知道哪個Port可以串接

Service: 
- targetPort: 串接到 pod 的 service port. 這時候前述的 containerPort就可以指出 targetPort要指到哪
- port: Service建立後的ClusterIP負責接收 request 的 port  
    在 cluster 內可用 `clusterIP:port` 去 Access Service  
    `clusterIP:port` 會再被導向 `PodIP:targetPort` (Endpoint)
- nodePort: Cluster 中每一個 Node 都會建立一個 Port 供外界 Access, `NodeIP:nodePort` 會被導向 `clusterIP:port`

###### tags: `Note`