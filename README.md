# KubernetesQuestion-
How to use the `curl` command be used in a Pod to retrieve all Pods in the `default` namespace? 

## Apply the manifest
`kubectl apply -f test.yaml`

## Access the pod
`kubectl exec -it test -- /bin/sh`

## retrieve information about all Pods in the default namespace
`curl -k https://kubernetes.default.svc/api/v1/namespaces/default/pods`
