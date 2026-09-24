# Providers 文件注释
# Private rules
  - Custom_Reject.yaml 🍃 净化环境
  - Custom_Direct.yaml 🎯 全球直连
  - Custom_Private.yaml 🎯 全球直连 // 仅包含域名
  - Custom_IP.yaml 🎯 全球直连 // 仅包含IP
  - Custom_Proxy.yaml 🌍 全球代理
  - Custom_Manual.yaml 🔰 节点选择

  - Custom_DNS.yaml 🌍 全球代理 // PS：不使用
  - CustomAuto.yaml ♻️ 自动选择 // 已删除

  - Custom_US.yaml 🇺🇲 美国节点
  - Custom_HK.yaml 🇭🇰 香港节点
  - Custom_JP.yaml 🇯🇵 日本节点
  - Custom_SG.yaml 🇸🇬 狮城节点


# rule

# 规则格式
  - PROCESS-NAME,curl,DIRECT #匹配路由自身进程(curl直连)
  - DOMAIN-SUFFIX,google.com,Proxy #匹配域名后缀(交由Proxy代理服务器组)
  - DOMAIN-KEYWORD,google,Proxy #匹配域名关键字(交由Proxy代理服务器组)
  - DOMAIN,google.com,Proxy #匹配域名(交由Proxy代理服务器组)
  - DOMAIN-SUFFIX,ad.com,REJECT #匹配域名后缀(拒绝)
  - IP-CIDR,127.0.0.0/8,DIRECT #匹配数据目标IP(直连)
  - SRC-IP-CIDR,192.168.1.201/32,DIRECT #匹配数据发起IP(直连)
  - DST-PORT,80,DIRECT #匹配数据目标端口(直连)
  - SRC-PORT,7777,DIRECT #匹配数据源端口(直连)
