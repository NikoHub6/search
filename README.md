#!url=http://script.hub/file/_start_/https://raw.githubusercontent.com/ddgksf2013/Rewrite/master/Html/Q-Search.conf/_end_/Q-Search.sgmodule?type=qx-rewrite&target=shadowrocket-module
#!name=Search
#!desc=Search

[URL Rewrite]

^https?://www.google.cn/search\?q=zh\+ zhihu://search?q= 302

# wb    xxx (微博)
^https:\/\/duckduckgo.com\/\?q=wb\+([^&]+).+ sinaweibo://searchall?q=$1 302 
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+wb.+ sinaweibo://searchall?q=$1 302 
# p    xxx (pdd)
^https:\/\/duckduckgo.com\/\?q=p\+([^&]+).+ pinduoduo://com.xunmeng.pinduoduo/search_result.html?search_key=$1 302 
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+p.+ pinduoduo://com.xunmeng.pinduoduo/http://mobile.yangkeduo.com/search_result.html?search_key= =$1 302 
#x    xxx (小红书)
^https:\/\/duckduckgo.com\/\?q=x\+([^&]+).+ xhsdiscover://search/result?keyword=$1 302 
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+x.+ xhsdiscover://search/result?keyword=$1 302 
# bli xxx (哔哩哔哩)
^https:\/\/duckduckgo.com\/\?q=bli\+([^&]+).+ bilibili://search?keyword=$1 302
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+bli.+ bilibili://search?keyword=$1 302
# jd  xxx (京东)
^https:\/\/duckduckgo.com\/\?q=jd\+([^&]+).+ openapp.jdmobile://virtual?params={"des":"productList","keyWord":"$1","from":"search","category":"jump"} 302
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+jd.+ openapp.jdmobile://virtual?params={"des":"productList","keyWord":"$1","from":"search","category":"jump"} 302
# tb  xxx (淘宝)
^https:\/\/duckduckgo.com\/\?q=tb\+([^&]+).+ taobao://s.taobao.com?q=$1 302
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+tb.+ taobao://s.taobao.com?q=$1 302
# yt  xxx (YouTube)
^https:\/\/duckduckgo.com\/\?q=yt\+([^&]+).+ youtube://results?search_query=$1 302
^https:\/\/duckduckgo.com\/\?q=([^+]+)\+yt.+ youtube://results?search_query=$1 302

[MITM]

hostname = %APPEND% duckduckgo.com
