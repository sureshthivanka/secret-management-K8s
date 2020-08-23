# secret-management-K8s

Create Kubernetes Secrets

Creating a Secret manually

kubectl apply -f ./create_secret_manually.yaml

Check Secrets

kubectl get secrets

View a description of a Secret

kubectl describe secrets/mysecret

kubectl get secret mysecret -o yaml


Using Secret

Using Secrets as files from a Pod

kubectl apply -f ./mount_secret_volume.yaml

Projection of Secret keys to specific paths

kubectl apply -f ./mount_secret_specific_volume.yaml

Using Secrets as environment variables

kubectl apply -f ./mount_as_environment_variables.yaml

Check Secrets on the Pod

kubectl exec mypod -it sh
