# =========================================
#  Shadowrocket  –  Bypass-Pro-Node-Video
# =========================================
[General]
bypass-system = true
ipv6 = false
dns-server = system
skip-proxy = 192.168.0.0/16, 10.0.0.0/8, 172.16.0.0/12, localhost, *.local, captive.apple.com
tun-excluded-routes = 10.0.0.0/8, 100.64.0.0/10, 127.0.0.0/8, 169.254.0.0/16, 172.16.0.0/12, 192.0.0.0/24, 192.0.2.0/24, 192.88.99.0/24, 192.168.0.0/16, 198.18.0.0/15, 198.51.100.0/24, 203.0.113.0/24, 224.0.0.0/4, 255.255.255.255/32

# =========================================
[Rule]
# ---- BYPASS  Pro-Node-Video  ----
DOMAIN-SUFFIX,pronodevideo.com,DIRECT
DOMAIN-SUFFIX,pronode.co,DIRECT
DOMAIN-SUFFIX,pronode.app,DIRECT
DOMAIN-SUFFIX,pro-node.com,DIRECT
DOMAIN-KEYWORD,pronode,DIRECT
# ---------------------------------

# ---- CN  &  common CDN ----
DOMAIN-SUFFIX,cn,DIRECT
GEOIP,CN,DIRECT
DOMAIN-SUFFIX,baidu.com,DIRECT
DOMAIN-SUFFIX,bdstatic.com,DIRECT
DOMAIN-SUFFIX,taobao.com,DIRECT
DOMAIN-SUFFIX,alicdn.com,DIRECT
DOMAIN-SUFFIX,qq.com,DIRECT
DOMAIN-SUFFIX,163.com,DIRECT
DOMAIN-SUFFIX,126.net,DIRECT
DOMAIN-SUFFIX,127.net,DIRECT
DOMAIN-SUFFIX,sina.com,DIRECT
DOMAIN-SUFFIX,weibo.com,DIRECT
DOMAIN-SUFFIX,bilibili.com,DIRECT
DOMAIN-SUFFIX,hdslb.com,DIRECT
DOMAIN-SUFFIX,baidubcr.com,DIRECT
DOMAIN-SUFFIX,alibaba.com,DIRECT
DOMAIN-SUFFIX,alipay.com,DIRECT
DOMAIN-SUFFIX,amap.com,DIRECT
DOMAIN-SUFFIX,autonavi.com,DIRECT
DOMAIN-SUFFIX,alicdn.com,DIRECT
DOMAIN-SUFFIX,alikunlun.com,DIRECT
DOMAIN-SUFFIX,apple.com,DIRECT
DOMAIN-SUFFIX,apple-cloudkit.com,DIRECT
DOMAIN-SUFFIX,icloud.com,DIRECT
DOMAIN-SUFFIX,me.com,DIRECT
DOMAIN-SUFFIX,mzstatic.com,DIRECT
DOMAIN-SUFFIX,cdn-apple.com,DIRECT
DOMAIN-SUFFIX,microsoft.com,DIRECT
DOMAIN-SUFFIX,office365.com,DIRECT
DOMAIN-SUFFIX,officecdn-microsoft-com.akamaized.net,DIRECT
DOMAIN-SUFFIX,windows.com,DIRECT
DOMAIN-SUFFIX,windowsupdate.com,DIRECT
DOMAIN-SUFFIX,steamcontent.com,DIRECT
DOMAIN-SUFFIX,steampowered.com,DIRECT
DOMAIN-SUFFIX,steamstatic.com,DIRECT
DOMAIN-SUFFIX,steam-chat.com,DIRECT
DOMAIN-SUFFIX,nvidia.com,DIRECT
DOMAIN-SUFFIX,oracle.com,DIRECT
DOMAIN-SUFFIX,java.com,DIRECT
DOMAIN-SUFFIX,ieee.org,DIRECT
DOMAIN-SUFFIX,acm.org,DIRECT
DOMAIN-SUFFIX,aps.org,DIRECT
DOMAIN-SUFFIX,springer.com,DIRECT
DOMAIN-SUFFIX,springerlink.com,DIRECT
DOMAIN-SUFFIX,sciencedirect.com,DIRECT
DOMAIN-SUFFIX,nature.com,DIRECT
DOMAIN-SUFFIX,cell.com,DIRECT
DOMAIN-SUFFIX,pnas.org,DIRECT
DOMAIN-SUFFIX,wiley.com,DIRECT
DOMAIN-SUFFIX,oup.com,DIRECT
DOMAIN-SUFFIX,cambridge.org,DIRECT
DOMAIN-SUFFIX,oxfordartonline.com,DIRECT
DOMAIN-SUFFIX,annualreviews.org,DIRECT
DOMAIN-SUFFIX,acs.org,DIRECT
DOMAIN-SUFFIX,aip.org,DIRECT
DOMAIN-SUFFIX,asm.org,DIRECT
DOMAIN-SUFFIX,asme.org,DIRECT
DOMAIN-SUFFIX,astm.org,DIRECT
DOMAIN-SUFFIX,icevirtuallibrary.com,DIRECT
DOMAIN-SUFFIX,worldscientific.com,DIRECT
DOMAIN-SUFFIX,scopus.com,DIRECT
DOMAIN-SUFFIX,webofknowledge.com,DIRECT
DOMAIN-SUFFIX,engineeringvillage.com,DIRECT
DOMAIN-SUFFIX,emerald.com,DIRECT
DOMAIN-SUFFIX,tandfonline.com,DIRECT
DOMAIN-SUFFIX,sagepub.com,DIRECT
DOMAIN-SUFFIX,jstor.org,DIRECT
DOMAIN-SUFFIX,proquest.com,DIRECT
DOMAIN-SUFFIX,ebscohost.com,DIRECT
DOMAIN-SUFFIX,ovid.com,DIRECT
DOMAIN-SUFFIX,westlaw.com,DIRECT
DOMAIN-SUFFIX,lexisnexis.com,DIRECT
DOMAIN-SUFFIX,heinonline.org,DIRECT
DOMAIN-SUFFIX,imf.org,DIRECT
DOMAIN-SUFFIX,worldbank.org,DIRECT
DOMAIN-SUFFIX,oecd-ilibrary.org,DIRECT
DOMAIN-SUFFIX,un.org,DIRECT
DOMAIN-SUFFIX,who.int,DIRECT
DOMAIN-SUFFIX,cdc.gov,DIRECT
DOMAIN-SUFFIX,nih.gov,DIRECT
DOMAIN-SUFFIX,pubmed.gov,DIRECT
DOMAIN-SUFFIX,nejm.org,DIRECT
DOMAIN-SUFFIX,jamanetwork.com,DIRECT
DOMAIN-SUFFIX,bmj.com,DIRECT
DOMAIN-SUFFIX,thelancet.com,DIRECT
DOMAIN-SUFFIX,rxiv.org,DIRECT
DOMAIN-SUFFIX,biorxiv.org,DIRECT
DOMAIN-SUFFIX,medrxiv.org,DIRECT
DOMAIN-SUFFIX,ssrn.com,DIRECT
DOMAIN-SUFFIX,arxiv.org,DIRECT
DOMAIN-SUFFIX,researchgate.net,DIRECT
DOMAIN-SUFFIX,scholar.google.com,DIRECT
DOMAIN-SUFFIX,booksc.org,DIRECT
DOMAIN-SUFFIX,libgen.is,DIRECT
DOMAIN-SUFFIX,z-lib.io,DIRECT
DOMAIN-SUFFIX,sci-hub.se,DIRECT
DOMAIN-SUFFIX,sci-hub.st,DIRECT
DOMAIN-SUFFIX,sci-hub.ru,DIRECT
IP-CIDR,192.168.0.0/16,DIRECT
IP-CIDR,10.0.0.0/8,DIRECT
IP-CIDR,172.16.0.0/12,DIRECT
IP-CIDR,127.0.0.0/8,DIRECT
IP-CIDR,100.64.0.0/10,DIRECT
IP-CIDR,224.0.0.0/4,DIRECT
IP-CIDR,255.255.255.255/32,DIRECT

# ---- FINAL FALL-THROUGH ----
FINAL,PROXY

# =========================================
[Host]
localhost = 127.0.0.1

# =========================================
[URL Rewrite]
^http://(www\.)?g\.cn https://www.google.com 302
^http://(www\.)?google\.cn https://www.google.com 302

# =========================================
[Script]
# ---------------  MITM cracks  ---------------
Alightmotion = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/refs/heads/main/alight-motion.json,pattern=^https://us-central1-alight-creative\.cloudfunctions\.net/getAccountStatusAndLicenses,max-size=131072,requires-body=true,timeout=10,enable=true
PicsArt = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/refs/heads/main/picart.json,pattern=^https://api\.picsart\.com/gw-v2/shop/subscription/apple/purchases,max-size=131072,requires-body=true,timeout=10,enable=true
VSCO = type=http-request,pattern=^https?://api\.revenuecat\.com/v\d/subscribers/,script-path=https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/File/vsco.js
VSCO1 = type=http-response,pattern=^https?://api\.revenuecat\.com/v\d/subscribers/,requires-body=1,script-path=https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/File/vsco.js
KineMaster = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/refs/heads/main/Kinemaster.json,pattern=^https://api-account\.kinemasters\.com/v2/user/subscribe,max-size=131072,requires-body=true,timeout=10,enable=true
SandboxPixelArt = type=http-response,script-path=https://N9dev-dev.github.io/SL/scripts/SandBox.js,pattern=https://api.sandbox.love/accounts/current,max-size=131072,requires-body=true,timeout=10,enable=true
VivaCut = type=http-response,script-path=https://N9dev-dev.github.io/SL/scripts/VivaCut.js,pattern=https://N9dev-dev.github.io/SL/scripts/VivaCut.js,max-size=131072,requires-body=true,timeout=10,enable=true
funimate = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/Funimate.json,pattern=^https://api\.funimate\.com/users/me,max-size=131072,requires-body=true,timeout=10,enable=true
Photomath = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/Photomath.json,pattern=^https://lapi\.photomath\.net/v4/me,max-size=131072,requires-body=true,timeout=10,enable=true
Photoshop = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/Photoshop.json,pattern=^https://lcs-mobile-cops\.adobe\.io/mobile_profile,max-size=131072,requires-body=true,timeout=10,enable=true
LightRoom = type=http-response,pattern=^https://photos\.adobe\.io/v2/accounts*,requires-body=1,script-path=https://raw.githubusercontent.com/litieyin/AD_VIP/main/Script/lightroom.js
Djay = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/djay.json,pattern=^https://app\.algoriddim\.com/api/v1/validate-receipt,max-size=131072,requires-body=true,timeout=10,enable=true
Vllo = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/vllo.json,pattern=^https://buy\.itunes\.apple\.com/verifyReceipt,max-size=131072,requires-body=true,timeout=10,enable=true
vizmato = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/vizmato.json,pattern=^https://web\.vizmato\.com/itunesreceipt_v5\.php,max-size=131072,requires-body=true,timeout=10,enable=true
reface = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/reface.json,pattern=^https://api\.reface\.video/api/reface/v1/iosSubscription,requires-body=true,timeout=10,enable=true
mojo = type=http-response,script-path=https://raw.githubusercontent.com/iSteal-it/script/main/mojo.json,pattern=^https?:
