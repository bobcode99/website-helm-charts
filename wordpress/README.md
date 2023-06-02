Install
```
k create ns wordpress-ns-new
k apply -f ./cm.yaml
helm install my-wordpress oci://registry-1.docker.io/bitnamicharts/wordpress --version 16.1.10 --namespace wordpress-namespace -f ./values.yaml
```

Upgrade value
```
helm upgrade -n wordpress-namespace my-wordpress oci://registry-1.docker.io/bitnamicharts/wordpress --version 16.1.10 -f ./values.yaml
```

Ref:

https://github.com/bitnami/charts/tree/main/bitnami/wordpress
https://github.com/bitnami/charts/issues/5929
https://help.servmask.com/2018/10/27/how-to-increase-maximum-upload-file-size-in-wordpress/