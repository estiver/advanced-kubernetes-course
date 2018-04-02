# kube authentication resources

Add oidc setup to kops cluster:

```
spec:
  kubeAPIServer:
    oidcIssuerURL: https://ehh.auth0.com/
    oidcClientID: N5q8k0yugbneBN3A9iS3RsVOcTSOz8S3
    oidcUsernameClaim: sub
```

Create UI:

```
kubectl create -f https://raw.githubusercontent.com/kubernetes/kops/master/addons/kubernetes-dashboard/v1.6.3.yaml
```

