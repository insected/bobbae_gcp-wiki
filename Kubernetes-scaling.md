# Cluster auto scaling

GKE's cluster autoscaler automatically resizes the number of nodes in a given node pool, based on the demands of your workloads. You don't need to manually add or remove nodes or over-provision your node pools. Instead, you specify a minimum and maximum size for the node pool, and the rest is automatic.

If resources are deleted or moved when autoscaling your cluster, your workloads might experience transient disruption. For example, if your workload consists of a controller with a single replica, that replica's Pod might be rescheduled onto a different node if its current node is deleted. Before enabling cluster autoscaler, design your workloads to tolerate potential disruption or ensure that critical Pods are not interrupted.

https://cloud.google.com/kubernetes-engine/docs/concepts/cluster-autoscaler

# Horizontal pod autoscaler 

HPA changes the shape of your Kubernetes workload by automatically increasing or decreasing the number of Pods in response to the workload's CPU or memory consumption, or in response to custom metrics reported from within Kubernetes or external metrics from sources outside of your cluster.

HPA cannot be used for workloads that cannot be scaled, such as DaemonSets.

The Horizontal Pod Autoscaler automatically scales the number of Pods in a replication controller, deployment, replica set or stateful set.

The Horizontal Pod Autoscaler is implemented as a Kubernetes API resource and a controller. The resource determines the behavior of the controller. The controller periodically adjusts the number of replicas in a replication controller or deployment to match the observed metrics such as average CPU utilisation, average memory utilisation or any other custom metric to the target specified by the user.

https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler

https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale-walkthrough/


## Autoscaling via custom metrics and HPA

You can automatically scale your Google Kubernetes Engine (GKE) workloads based on metrics available in Cloud Monitoring. 

https://cloud.google.com/kubernetes-engine/docs/tutorials/autoscaling-metrics

# Vertical pod autoscaler 

Vertical Pod Autoscaler (VPA) frees the users from necessity of setting up-to-date resource limits and requests for the containers in their pods. When configured, it will set the requests automatically based on usage and thus allow proper scheduling onto nodes so that appropriate resource amount is available for each pod. It will also maintain ratios between limits and requests that were specified in initial containers configuration.

It can both down-scale pods that are over-requesting resources, and also up-scale pods that are under-requesting resources based on their usage over time.

https://cloud.google.com/kubernetes-engine/docs/concepts/verticalpodautoscaler
