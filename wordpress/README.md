https://github.com/bitnami/charts/tree/main/bitnami/wordpress

Install
```
helm install my-wordpress oci://registry-1.docker.io/bitnamicharts/wordpress --namespace wordpress-namespace --create-namespace -f ./values.yaml
```

Upgrade value
```
helm upgrade -n wordpress-namespace my-wordpress oci://registry-1.docker.io/bitnamicharts/wordpress -f ./values.yaml
```
