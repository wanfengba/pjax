# pjax

导入js文件

再把
  var pjax = new Pjax({
        elements: 'a[href]:not([href^="#"])',
        cacheBust: false,
        debug: false,
        selectors: ['title', '.wrapper']
    });
    document.addEventListener('pjax:send', function() {
        NProgress.start(); 
    });
    document.addEventListener('pjax:complete', function() {
        //NProgress
        message();
    });
    //不使用pjax情况下的调用
    (function() {
        page_next();
    })();
    
 添加到最地下
 
 要刷新的部分添加.wrapper
