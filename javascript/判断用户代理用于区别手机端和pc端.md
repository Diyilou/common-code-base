###业务需求中，可能需要针对pc端和手机端（安卓和苹果）做不同的处理，这个时候可以使用先面的代码做判断：
---
<pre>
var userAgentJudge = function() {

    if (/(iPhone|iPad|iPod|iOS)/i.test(navigator.userAgent)) {
        //苹果手机端
        return '3';
    } else if (/(Android)/i.test(navigator.userAgent)) {
        //安卓手机端
        return '4';
    } else {
        //pc端
        return '5';
    }
};
</pre>
