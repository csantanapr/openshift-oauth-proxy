# Configure OpenShift OAuth Proxy

This is very simple example on how to configure [OpenShift oauth-proxy](https://github.com/openshift/oauth-proxy)

Deploy the example
```bash
oc apply -f https://raw.githubusercontent.com/csantanapr/openshift-oauth-proxy/main/example.yaml
```

Open the route url
```
open $(oc get route example -o template=https://{{.spec.host}})
```
