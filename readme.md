# Usage
```
docker run -d --privileged --name us-tiktok --network thief_br --ip 192.168.88.4 
    -v /dev/mali0:/dev/mali0 -v `pwd`/GApps-arm64-12.0.0-core:/tmp \
    redroid androidboot.redroid_gpu_mode=mali androidboot.redroid_net_dns1=192.168.88.1 androidboot.redroid_net_ndns=1


docker exec -it us-tiktok sh
cd /tmp
sh update-binary
```