## cloud-init

cloud-init file used by ESXi in home-lab

### Create ISO file

```
# linux
$ genisoimage -output k8s-worker.iso -volid cidata -joliet -rock meta-data user-data network-config

# macos
$ hdiutil makehybrid -o k8s-worker.iso -hfs -joliet -iso -default-volume-name cidata k8s-worker/
```
