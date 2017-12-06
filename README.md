# cloud-native-labs-minishift
It's possible to install the cloud native lab guides into minishift using an addon.
 1. install minishift https://github.com/minishift/minishift
 1. install the guides https://github.com/openshift-roadshow/cloud-native-guides/tree/ocp-3.6/minishift
When minishift is running you can install the guides using these commands (taken from above docs)
```sh
git clone https://github.com/openshift-roadshow/cloud-native-guides.git
minishift addons install minishift/
minishift addon apply cloud-native-labs
minishift openshift service guides -n cloud-native-labs
```
