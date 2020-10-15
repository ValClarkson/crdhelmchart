# crdhelmchart

This is a working example of how to create a cluster via the crd workflow
using a helm chart

create a cert directy and generate certs
```
mkdir crunchycrdcluster/cert

# this variable is the name of the cluster being created
export pgo_cluster_name=hippo
# this variable is the namespace the cluster is being deployed into
export cluster_namespace=test1

# generate a SSH public/private keypair for use by pgBackRest
ssh-keygen -t ed25519 -N '' -f "${pgo_cluster_name}-key"

```
