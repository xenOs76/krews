# krews

Custom Index for Krew plugins

## How to use

```shell
❯ krew index add https://github.com/xenOs76/krews.git
accepts 2 arg(s), received 1

❯ krew index list
INDEX     URL
default   https://github.com/kubernetes-sigs/krew-index.git
netshoot  https://github.com/nilic/kubectl-netshoot.git
os76      https://github.com/xenOs76/krews.git

❯ krew search netdrill
NAME           DESCRIPTION                                         INSTALLED
os76/netdrill  kubectl-netdrill, a network troubleshooting plu...  no

❯ krew install os76/netdrill
Updated the local copy of plugin index.
Updated the local copy of plugin index "netshoot".
Updated the local copy of plugin index "os76".
Installing plugin: netdrill
Installed plugin: netdrill
\
 | Use this plugin:
 |      kubectl netdrill
 | Documentation:
 |      https://github.com/xenOs76/kubectl-netdrill
/

❯ ~/.krew/bin/kubectl-netdrill -v
kubectl-netdrill version 0.1.2
```
