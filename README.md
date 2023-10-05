#!url=http://script.hub/file/_start_/https://raw.githubusercontent.com/ddgksf2013/Rewrite/master/Html/Q-Search.conf/_end_/Q-Search.sgmodule?type=qx-rewrite&target=shadowrocket-module
#!name=Search
#!desc=Search

[URL Rewrite]

^https?://duckduckgo.com/search\?q=zh\+ zhihu://search?q= 302



[MITM]

hostname = %APPEND% duckduckgo.com
