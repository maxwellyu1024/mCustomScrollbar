## How to use it

After files inclusion, call mCustomScrollbar function on the element you want to add custom scrollbars. The example below adds scrollbars to elements with class name content

```javascript
(function($){
	$(window).load(function(){
		$(".content").mCustomScrollbar();
	});
})(jQuery);
```

Your **``.content``** element(s) (or any other element you’re attaching the custom scrollbar) should have a typical styling of an overflowed block, e.g. a **``height``** (or **``max-height`**) value, **``overflow: auto``** (or hidden) and its content should be long enough to require a scrollbar.

To add a **horizontal scrollbar**, style your element accordingly (give it a width value and a wide enough content) and set the **``horizontalScroll``** option parameter of mCustomScrollbar to **``true``**

```javascript
$(".content").mCustomScrollbar({
    horizontalScroll:true
});
```

jquery.mCustomScrollbar.css contains few ready-to-use scrollbar themes that you can apply easily on your scrollbars by setting the **``theme``** option parameter to the [theme name you want](http://manos.malihu.gr/tuts/custom-scrollbar-plugin/scrollbar_themes_demo.html)

```javasc
$(".content").mCustomScrollbar({
    theme:"light"
});
```

[Detailed usage guide](http://manos.malihu.gr/jquery-custom-content-scroller/)