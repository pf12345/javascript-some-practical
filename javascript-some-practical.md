#javascript 实用方法

1、使用typeof、instanceof和constructor
<pre>
<code>
var arr = [];
typeof arr;   // "object" 
arr  instanceof Array // true
arr.constructor();  //[]
</code>
</pre>

2、在特定范围里获得一个随机数

<pre>
<code>
var x = Math.floor(Math.random() * (max - min + 1)) + min;
</code>
</pre>

3、从数字数组中获得最大值和最小值

<pre>
<code>

var  arr = [5, 45 , 120 , -25 , 28 , 40 , 1225, -411]; 
var max = Math.max.apply(Math, arr); 
var min = Math.min.apply(Math, arr);
</code>
</pre>

4、判断是否能够使用flash

<pre>
<code>
judgeHasFlash = function() {
        var hasFlash = false;
        try {
            var fo = new ActiveXObject('ShockwaveFlash.ShockwaveFlash');
            if (fo) {
                hasFlash = true;
            }
        } catch (e) {
            if (navigator.mimeTypes
                    && navigator.mimeTypes['application/x-shockwave-flash'] != undefined
                    && navigator.mimeTypes['application/x-shockwave-flash'].enabledPlugin) {
                hasFlash = true;
            }
        }
        return hasFlash;
    }
</code>
</pre>
