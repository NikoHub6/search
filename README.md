#!name=Search
#!desc=Search

[URL Rewrite]

# zh    xxx (知乎)
^https:\/\/www\.google\.com\/search\?q=zh\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# wb    xxx (微博)
^https:\/\/www\.google\.com\/search\?q=wb\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# p    xxx (pdd)
^https:\/\/www\.google\.com\/search\?q=p\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
#x    xxx (小红书)
^https:\/\/www\.google\.com\/search\?q=x\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# bli xxx (哔哩哔哩)
^https:\/\/www\.google\.com\/search\?q=bli\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# jd  xxx (京东)
^https:\/\/www\.google\.com\/search\?q=jd\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# tb  xxx (淘宝)
^https:\/\/www\.google\.com\/search\?q=tb\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# yt  xxx (YouTube)
^https:\/\/www\.google\.com\/search\?q=yt\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# s    xxx （App Store)
^https:\/\/www\.google\.com\/search\?q=s\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# d    xxx (抖音)
^https:\/\/www\.google\.com\/search\?q=d\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# t    xxx (欧陆词典)
^https:\/\/www\.google\.com\/search\?q=t\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302






#网页版本
# yd  xxx (有道词典)
^https:\/\/www\.google\.com\/search\?q=yd\+([^&]+).+ http://dict.youdao.com/search?q=$1 302
# trc xxx (Google 译至中)
^https:\/\/www\.google\.com\/search\?q=trc\+([^&]+).+ https://translate.google.com/#view=home&op=translate&sl=auto&tl=zh-CN&text=$1 302

# tre xxx (Google 译至英)
^https:\/\/www\.google\.com\/search\?q=tre\+([^&]+).+ https://translate.google.com/#view=home&op=translate&sl=auto&tl=en&text=$1 302

# wx    xxx (微信)











# yd    xxx (有道）


[MITM]

hostname = %APPEND% www.google.com
