# Day 2

## Deploying an application into OpenShift
```
oc create deployment nginx --image=nginx:latest
```

Expected output
<pre>
(jegan@tektutor.org)$ oc create deployment nginx --image=nginx:latest
Warning: would violate PodSecurity "restricted:latest": allowPrivilegeEscalation != false (container "nginx" must set securityContext.allowPrivilegeEscalation=false), unrestricted capabilities (container "nginx" must set securityContext.capabilities.drop=["ALL"]), runAsNonRoot != true (pod or container "nginx" must set securityContext.runAsNonRoot=true), seccompProfile (pod or container "nginx" must set securityContext.seccompProfile.type to "RuntimeDefault" or "Localhost")
deployment.apps/nginx created
</pre>
