# Providers 文件注释
# Private rules
  - "RULE-SET,CustomDNS,🌍 国外媒体"
  - "RULE-SET,CustomDevice,🎯 全球直连" PS：即直连
  - "RULE-SET,CustomAuto,♻️ 自动选择"
  - "RULE-SET,CustomManual,🔰 节点选择"
  - "RULE-SET,CustomUS,🇺🇲 美国节点"
  - "RULE-SET,CustomHK,🇭🇰 香港节点"
  - "RULE-SET,CustomJP,🇯🇵 日本节点"
  - "RULE-SET,CustomSG,🇸🇬 狮城节点"


# rule

# 规则
##- PROCESS-NAME,curl,DIRECT #匹配路由自身进程(curl直连)
##- DOMAIN-SUFFIX,google.com,Proxy #匹配域名后缀(交由Proxy代理服务器组)
##- DOMAIN-KEYWORD,google,Proxy #匹配域名关键字(交由Proxy代理服务器组)
##- DOMAIN,google.com,Proxy #匹配域名(交由Proxy代理服务器组)
##- DOMAIN-SUFFIX,ad.com,REJECT #匹配域名后缀(拒绝)
##- IP-CIDR,127.0.0.0/8,DIRECT #匹配数据目标IP(直连)
##- SRC-IP-CIDR,192.168.1.201/32,DIRECT #匹配数据发起IP(直连)
##- DST-PORT,80,DIRECT #匹配数据目标端口(直连)
##- SRC-PORT,7777,DIRECT #匹配数据源端口(直连)
