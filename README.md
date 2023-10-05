#!name=SearchKing
#!desc=SearchKing

[URL Rewrite]

# zh    xxx (知乎)
^https:\/\/www\.google\.com\/search\?q=zh\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=zh, 302
# wb    xxx (微博)
^https:\/\/www\.google\.com\/search\?q=wb\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=wb, 302
# p    xxx (pdd)
^https:\/\/www\.google\.com\/search\?q=p\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=p, 302
#x    xxx (小红书)
^https:\/\/www\.google\.com\/search\?q=x\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=x, 302
# b xxx (哔哩哔哩)
^https:\/\/www\.google\.com\/search\?q=b\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=b, 302
# jd  xxx (京东)
^https:\/\/www\.google\.com\/search\?q=jd\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=jd, 302
# tb  xxx (淘宝)
^https:\/\/www\.google\.com\/search\?q=tb\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=tb, 302
# yt  xxx (YouTube)
^https:\/\/www\.google\.com\/search\?q=yt\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=yt, 302
# s    xxx （App Store)
^https:\/\/www\.google\.com\/search\?q=s\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=s, 302
# d    xxx (抖音)
^https:\/\/www\.google\.com\/search\?q=d\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=d, 302
# t    xxx (欧陆词典)
^https:\/\/www\.google\.com\/search\?q=t\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=t, 302
# dp    xxx (大众点评)
^https:\/\/www\.google\.com\/search\?q=dp\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=dp, 302
# tw    xxx (Twitter)
^https:\/\/www\.google\.com\/search\?q=tw\+ shortcuts://x-callback-url/run-shortcut?name=URL%20Rewrite&input=text&text=tw, 302



#网页版本
# yd  xxx (有道词典)
^https:\/\/www\.google\.com\/search\?q=yd\+([^&]+).+ http://dict.youdao.com/search?q=$1 302
# tc xxx (Google 译至中)
^https:\/\/www\.google\.com\/search\?q=tc\+([^&]+).+ https://translate.google.com/#view=home&op=translate&sl=auto&tl=zh-CN&text=$1 302
# te xxx (Google 译至英)
^https:\/\/www\.google\.com\/search\?q=te\+([^&]+).+ https://translate.google.com/#view=home&op=translate&sl=auto&tl=en&text=$1 302
# ph  xxx (PornHub)
^https:\/\/www\.google\.com\/search\?q=ph\+([^&]+).+ https://cn.pornhub.com/video/search?search=$1 302
# bd  xxx (百度搜索)
^https:\/\/www\.google\.com\/search\?q=bd\+([^&]+).+ https://www.baidu.com/s?wd=$1 302
# by  xxx (必应)
^https:\/\/www\.google\.com\/search\?q=by\+([^&]+).+ https://www.bing.com/search?q=$1 302
# gh    xxx (GitHub)
^https:\/\/www\.google\.com\/search\?q=gh\+([^&]+).+ https://github.com/search?q=$1 302


# cn  (切换至中国区)
^https:\/\/www\.google\.com\/search\?q=cn&.+ https://itunes.apple.com/WebObjects/MZStore.woa/wa/resetAndRedirect?dsf=143465&mt=8&url=/WebObjects/MZStore.woa/wa/viewSoftware?mt=8&id=1108187390&cc=cn&urlDesc= 302
# us  (切换至美国区)
^https:\/\/www\.google\.com\/search\?q=us&.+ https://itunes.apple.com/WebObjects/MZStore.woa/wa/resetAndRedirect?dsf=143441&mt=8&url=/WebObjects/MZStore.woa/wa/viewSoftware?mt=8&id=1108187390&cc=us&urlDesc= 302

[MITM]

hostname = %APPEND% www.google.com
