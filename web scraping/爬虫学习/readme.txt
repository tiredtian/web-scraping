问题：爬取网站上的数据，有些网站数据包含在原始的html网页中，有些网站数据是利用ajax请求动态加载的。直接模拟请求并不能获得网站数据
解决：可以利用requests库模拟ajax请求获取数据，分析网站中的xhr-ajax请求，模拟爬取数据。
问题：许多网站为了反爬虫，ajax接口中包含越来越多的加密参数，难以通过分析模拟出ajax请求
解决：使用selenium模拟浏览器行为，可见即可爬
