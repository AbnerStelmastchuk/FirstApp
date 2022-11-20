# Comands for running jenkins with helm
helm install jenkins . --namespace <yourNamespace>

# If u set up in localhost, use:
kubectl --namespace <yourNamespace> port-forward svc/jenkins 8081:8081

# 1. Get your 'admin' user password by running:
  kubectl exec --namespace firstwebapp -it svc/jenkins -c jenkins -- /bin/cat /run/secrets/additional/chart-admin-password && echo OR
  kubectl exec --namespace firstwebapp -it svc/jenkins -c jenkins -- /bin/cat /run/secrets/additional/chart-admin-password

 
login: admin

pass: tNtHnCuopOjwGJhS7q9mbL