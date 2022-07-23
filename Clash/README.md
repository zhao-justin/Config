# CFW config

My CFW config(TUN Mode) for Windows/MacOS.

# Guide

1. Install Service Mode.
2. Turn on Mixin.
3. Restart CFW && Enjoy.

**Notice: Do not Turn on _System Proxy_.**

## Windows/MacOS switch

[cfw-settings.yaml](https://github.com/harahi/Config/blob/main/Clash/cfw-settings.yaml)
```yaml
# TUN Mode
    tun:
      enable: true
      stack: system #gvisor system 
      dns-hijack:
        # Windows
        - any:53
        # MacOS
        # - 8.8.8.8
        # - 1.1.1.1
        # - 223.5.5.5
        # - 1.12.12.12
      auto-route: true
      # 自动检查网络端口,如果设备有多网口或虚拟网卡,建议使用interface-name
      auto-detect-interface: true
      # interface-name: en0
```

## Credit

- [clash](https://github.com/Dreamacro/clash)
- [clash_for_windows_pkg](https://github.com/Fndroid/clash_for_windows_pkg) and [wiki](https://docs.cfw.lbyczf.com/)
- [OpenClash](https://github.com/vernesong/OpenClash/)
- [clash-tap-tun](https://github.com/kjfx/clash-tap-tun)
- [clash-rules](https://github.com/Loyalsoldier/clash-rules)
- [Rules](https://github.com/zzcabc/Rules)
