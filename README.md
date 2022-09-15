Please check below image link for Highly available k8s clsuter architecture
https://larrydevops.com/wp-content/uploads/2019/11/kubeadm-ha-topology-stacked-etcd-1024x550.png

As we can see from the image hear we have 3 master node under the load balancer which  actually ensure cluster high availability and if we check the worker node it will ensure application level high availability. We can add more worker, so this cluster is scalable. For make the cluster fault tolerance we must configure another K8s cluster in separate zone or region.  

Recovery we may configure the container backup with the help of container backup application.

For logging we can us flunted/logtash (as demon set) and Elasticsearch and Kibana for graphical view.  And alerting we can use Prometheus.

Now a days cloud gives us highly available using multiple zones, region concept. Also highly scalable, fault tolerant with so many features. If we consider e-commerce, telecom and ride sharing we may consider cloud. It reduces our cost. Also, its very much flexible for resource increase and decrease.
