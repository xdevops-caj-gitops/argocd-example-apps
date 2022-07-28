# Demo

## Setup Namespace
```bash
oc new-project argocd-example
# run as cluster admin to label namespace
oc label namespace argocd-example argocd.argoproj.io/managed-by=myargocd
```

## Deploy guestbook app

Failed to deploy due to:
```text
AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 10.130.3.73. Set the 'ServerName' directive globally to suppress this message
4
(13)Permission denied: AH00072: make_sock: could not bind to address [::]:80
3
(13)Permission denied: AH00072: make_sock: could not bind to address 0.0.0.0:80
2
no listening sockets available, shutting down
1
AH00015: Unable to open logs

```