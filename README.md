### SEO
  什么是 SEO
  百度百科：
    SEO (Search Engine Optimization): 搜索引擎优化。搜索引擎优化是一种利用搜索引擎的搜索规则来提高目前网站有关搜索引擎内的自然排名的方式。SEO 是为了从搜索引擎中获得更多的免费流量，从网站结构、内容创建方案、用户互动传播、页面等角度进行合理规划，使网站更合适搜索引擎的索引原则的行为
  
  SEO 原理
    页面抓取：蜘蛛向服务器请求页面，获取页面内容
    分析入库：对获取到的内容进行分析，对优质页面进行收录
    检索排序：当用户检索关键词时，从收录的页面中按照一定的规则进行排序，并返回给用户结果
  
  SEO 优化
    页面抓取：
      如何才能吸引蜘蛛光顾我们的网站，如何才能让蜘蛛经常光顾我们的网站。这里提出一下几个优化点：
      
      1.提交页面。提交页面又分为几种不同的方式
        1.sitemap 提交。sitemap，顾名思义，就是网站地图，当蜘蛛来到我们的网站时，告诉它我们有多少页面，不同页面是按什么分类的，每个页面的地址是什么。顺着我们的指引，蜘蛛会很轻松的爬遍所有内容。另外如果你的页面分类比较多，而且数量大，建议添加 sitemap 索引文件。如果站点经常更新添加新页面，建议及时更新 sitemap 文件；
        2.主动提交。就是把你的页面直接丢给百度的接口，亲口告诉百度你有哪些页面，这是效率最高也是收录最快的方式。但是需要注意，百度对每天提交的数量是有限制的，而且反复提交重复的页面，会被降低每日限额，所以已被收录的页面不建议反复提交。收录有个时间过程，请先耐心等待；
        3.实时提交。在页面中安装百度给的提交代码，当这个页面被用户打开，便自动把这个页面提交给百度。
     
    前端需要注意哪些 SEO
      1.合理的 title、description、keywords；搜索对这三项的权重逐个减小，title 值强调重点即可，重要关键词出现不要超过 2 次，而且要靠前，不同页面 title 要有所不同；description 把页面内容高度概括，长度合适，不可过分堆砌关键词，不同页面 description 有所不同；keywords 列举出重要关键词即可。
      2.语义化的 HTML 代码，符合 W3C 规范：语义化代码让搜索引擎容易理解网页
      3.重要内容 HTML 代码放在最前面：搜索引擎抓取 HTML 顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取
      4.重要内容不要用 js 输出：爬虫不会执行 js 获取内容
      5.少用 iframe：搜索引擎不会抓取iframe中的内容
      6.非装饰性图片必须加 alt
      7.提高网站速度：网站速度是搜索引擎排序的一个重要指标
      
### web 开发中会话跟踪的方法有哪些
  1.cookie
  2.session
  3.URL 重写
  4.隐藏 input
  5.IP 地址

### img 的 title 和 alt 有什么区别
  1.title 是 global attributes 之一，用于为元素提供附加的 advisory information。通常当鼠标滑动到元素上的时候显示。
  2.alt 是 img 的特有属性，是图片内容的等价描述，用于图片无法加载时显示、读屏器阅读图片。可提高图片可访问性，除了纯装饰图片外都必须设置有意义的值，搜索引擎会重点分析。
  
### doctype 是什么，举例常见 doctype 及特点
  1.<!doctype> 声明必须处于 HTML 文档的头部，在 html 标签之前， HTML 5 中不区分大小写
  2.<!doctype> 声明不是一个 HTML 标签，是一个用于告诉浏览器当前 HTML 版本的指令
  3.现代浏览器的 html 布局引擎通过检查 doctype 决定使用兼容模式还是标准模式对文档进行渲染，一些浏览器有一个接近标准模型
  4.在 HTML 4.01 中 <!doctype> 声明指向一个 DTD，由于 HTML 4.01 基于 SGML，所以 DTD 指定了标记规则以保证浏览器正确渲染内容
  5.HTML5 不基于 SGML，所以不用指定 DITD
  
  常见 doctype
    1. HTML4.01 strict：不允许使用表现性、废弃元素（如 font）以及 frameset。声明：<!DOCTPYE HTML PUBLIC"-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    2.HTML4.01 Transitional：允许使用表现性、废弃元素（如 font），不允许使用 frameset。声明：<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd" >
    3.HTML4.01 Frameset：允许表现性元素，废弃元素以及 frameset。声明：<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd" >
    4.XHTML1.0 Strict：不允许使用表现性、废弃元素以及 frameset。文档必须是结构良好的 XML 文档。声明 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd" >
    5.XHTML1.0 Transitional：允许使用表现性、废弃元素，不允许 frameset，文档必须是结构良好的 XML 文档。声明：<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd" >
    6.XHTML1.0 Frameset：允许使用表现性、废弃元素以及 frameset，文档必须是结构良好的 XML 文档。声明：<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd" >
    7.HTML5: <!doctype html >
