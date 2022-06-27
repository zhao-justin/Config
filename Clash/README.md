<!--
 * @Author: Harahi zjc6650681@gmail.com
 * @Date: 2022-06-27 11:24:56
 * @LastEditors: Harahi zjc6650681@gmail.com
 * @LastEditTime: 2022-06-27 13:38:34
 * @FilePath: /Clash/README.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# CFW config

My CFW config(TUN Mode) for windows/macos.

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
        # windows
        - 198.18.0.2:53
        # macos
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
