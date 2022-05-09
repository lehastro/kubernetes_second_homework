In Minikube in namespace kube-system, there are many different pods running. Your task is to figure out who creates them, and who makes sure they are running (restores them after deletion).

kubelet

An agent that runs on each node in the cluster. It makes sure that containers are running in a Pod.
The kubelet takes a set of PodSpecs that are provided through various mechanisms and ensures that
the containers described in those PodSpecs are running and healthy. The kubelet doesn't manage
containers which were not created by Kubernetes.




Testing Canary

$ curl $(minikube ip)

and

$ curl -H "canary:always" $(minikube ip)
