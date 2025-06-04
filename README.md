# growthbook-proxy

Create your helm values file <https://chrismckee.co.uk/growthbook-proxy/>

```shell
helm repo add growthbook https://chrismckee.co.uk/growthbook-proxy/
helm repo update
helm upgrade --install growthbookproxy-linux growthbook/growthbook-proxy --create-namespace --namespace growthbook -f values.yaml
```
