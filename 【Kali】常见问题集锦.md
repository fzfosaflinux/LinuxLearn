1. 没有声音
KaliLinux默认是关闭声卡的，需要手动开启声卡`pulseaudio --start`
如果需要一直这样需要修改配置温江
`systemctl -user enable pulseaudio`
或者编辑`/etc/default/pulseaudio`写入
```
PULSEAUDIO_SYSTEM_START=1
DISALLOW_MODULE_LOADING=0

```