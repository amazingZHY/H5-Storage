## H5的几种存储  
1. localstorage  
待补充  
2. sessionStorage  
待补充  
3. Application Cache  
待补充  
4. Web Storage  
(目前得到支持最广泛的HTML5本地存储规范：IE 8+、FF 3.5+、Safari 4+、Chrome 4+、Opera 10.5+，以及iPhone 2+和Android 2+都已经支持Web Storage）要判断你的浏览器是否支持Web Storage，可以使用下面这个函数：
代码
    function supports_html5_storage() {
    try {
    return 'localStorage' in window && window['localStorage'] !== null;
    } catch (e) {
    return false;
    }
    }
Web SQL Database
Web SQL Database是一个已经废弃的规范，但是鉴于除了IE和Firefox，其他浏览器都已经实现了Web SQL Database，并且它还具有一些HTML5 Storage所不具有的特性，所以还是值得了解一下的。
IndexedDB
相比其他两个规范，目前只有Firefox实现了IndexedDB（顺便提一下，Mozilla表示它们永远不会去实现Web SQL Database），不过Google已经表示正在考虑在Chrome中加入IndexDB支持。
