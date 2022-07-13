#### Commands

```bash
# This Helm Package deploys 2 deployment components for 2 subdomains following ingress.
# lables & selector labels are Immutable - They cannot be changed, so Hardcoded in yaml files.

### Pre-requsities
# Supply your own Subdomains 1 and 2 as per your requirements in values.yaml

# Under /etc/hosts file, include the following inputs For Local-DNS Resolution:
# 127.0.0.1       localhost
# 192.168.49.2    analytics.cloudopsmeta.com
# 192.168.49.2    shopping.cloudopsmeta.com
# 192.168.49.2    azure.cloudopsmeta.com
# 192.168.49.2    devops.cloudopsmeta.com


### COMMANDS
# helm install <ChartName> .      
# helm list
# helm upgrade <NewChart> .
# helm history <RunningChart>
# helm rollback <RunningChart> <REVISION-No>
# helm delete <Chartname>

# Enable INGRESS using Commnad -------------->> $ minikube addons enable ingress
# For minikube there will be only 1 node, others pass "nodeSelector" and assign label to any node before
# deploying the Package.


```
</br>
