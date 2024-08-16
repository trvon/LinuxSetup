# Useful error resolutions

- Using both LXD and Docker?
[ref](https://discuss.linuxcontainers.org/t/lxd-losts-iptables-rules-with-docker/15045)

```
sudo iptables -I DOCKER-USER -i lxdbr0 -j ACCEPT
sudo iptables -I DOCKER-USER -o lxdbr0 -j ACCEPT
```
