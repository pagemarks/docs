# ui

cursor: [<uri,>*] | auto | default | pointer | not-allowed | crosshair | move | e-resize | ne-resize | nw-resize | n-resieze | se-resize | sw-resize | s-resize | w-resize | text | wait | help | progress | inherit

uri后必须更有一个逗号和某个通用关键字.可以设置多个url,浏览器会逐个查看,找到可用即停止.有video source味道.


outline:
outline-width/color/style
	不占用布局空间,不能设置单边.

::selection

::use-select:none | text | toggle | element | elements | all

resize: both | none | horizontal | vertical

-webkit-touch-callout: none 取消系统长按弹出层.如copy

-webkit-overflow-scroll: auto | touch 滑动滚动效果
	auto: 手指移开即停止
	Touch: 物理弹性效果

-webkit-tap-highlight-color: rgba(0,0,0,0) 点击元素遮罩色

-webkit/moz-appearance: none | button | button-bevel | checkbox | default-button | listbox | listitem | media-fullscreen-button | media-mute-button | media-play-button | radio | searchfield | 

pointer-events: none
事件穿透,如水印不影响选择复制

tab-size: int;
