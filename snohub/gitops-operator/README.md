# Deploy Openshift GitOps 1.18 on OCP 4.19 

oc create ns openshift-gitops-operator 

oc label namespace openshift-gitops-operator openshift.io/cluster-monitoring=true 

oc apply -f gitops-og.yaml 

oc apply -f gitops-sub.yaml 

