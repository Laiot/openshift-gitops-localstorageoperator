## 
Deploy the Local Storage operator from the Operator Hub by creating OperatorGroup and Subscription objects.

```
argocd app create local-storage-operator --repo https://github.com/Laiot/openshift-gitops-localstorageoperator.git --path=. --dest-server=https://kubernetes.default.svc --dest-namespace=default
argocd app sync local-storage-operator
```
