Installation
Fluent Bit must be deployed as a DaemonSet, so on that way it will be available on every node of your Kubernetes cluster. To get started run the following commands to create the namespace, service account and role setup:

1. We will first setup the required role, rolebinding, namespace and service-account/ For Kubernetes v1.21 and below

kubectl apply -f install/v1.21
For Kubernetes v1.22

kubectl apply -f install/v1.22
2. After setting up the required kubernetes objects, we can now install the fluentbit(daemonsets) and it's configuration (configmap).

kubectl apply -f ./fluentbit/

apply these two files: fluentbit-cm-2.yaml, fluentbit-ds-new.yaml
Apply these two files: fluentbit-cm-2.yaml, fluentbit-ds-new.yaml
