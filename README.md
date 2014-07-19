# jquery.search [![spm version](http://spmjs.io/badge/jquery.search)](http://spmjs.io/package/jquery.search)
AUTHOR WEBSITE: [http://ydr.me/](http://ydr.me/)

Simple to operate location search.

__IT IS [A spm package](http://spmjs.io/package/jquery.search).__




#USAGE
```
var $ = require('jquery');
require('jquery.search')($);


// 1、设置
// 可以继续链式
$.search().set('键', '值');
$.search().set({键值对});
$.search().push('键', '值');
$.search().pop('键', '值');
$.search().unshift('键', '值');
$.search().shift('键', '值');

// 2、获取
// 可以继续链式
$.search().get('键');
$.search().get(['键1', '键2']);
$.search().get();

// 3、删除、清空
// 可以继续链式
$.search().remove('键');
$.search().remove(['键1', '键2']);
$.search().remove();

// 4、判断
// $.search().has('键');
```



#OPTIONS
```
defaults = {
    // 是否严格模式，默认true
    // 严格模式下，将在读取后、写入前分别进行encodeURIComponent、decodeURIComponent操作
    isStrict: !0,
    // 传入search部分，为空默认为window.location.search
    search: ''
};
```


#SET OPTIONS
```
$.search.defaults;
```


