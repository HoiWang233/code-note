###### 捕捉class的点击事件,并取得其内容,以id或class修改其他元素

```

$(document).ready(function() {
            // 绑定点击事件到每个产品名称
            $('.p3_o').on('click', function() {
                var productName =  $(this).find('.p3_o_t').text();

				var productImageSrc = productImages[productName] || 'images/22.png';
                // 更新右侧的产品图片和名称
				console.log(productImageSrc)
				console.log(productName)
                $('#productImage').attr('src', productImageSrc);
                $('#productName').text(productName);

                // 取消所有链接的默认行为
                return false;
            });
        });
```

###### 引入jquery的css和js, 实现滚动式页面

```
<link rel="stylesheet" href="static/css/jquery.fullpage.css">

<script src="static/js/jquery.fullpage.min.js"></script>

$(function(){

<script>

	$.fn.fullpage({

		verticalCentered: false,

		// anchors: ['page1', 'page2', 'page3', 'page4', 'page5', 'page6', 'page7', 'page8', 'page9', 'page10'],

		navigation: true,

		// navigationTooltips: ['首页', '视觉', '交互', '皮肤', '功能', '待办邮件', '联系人邮件', '科技', '连接易信', '马上体验']

	});

});
</script>
```
