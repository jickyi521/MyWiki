---
title: "clipSubview"
date: 2014-07-29 14:33
---

UIImage View 里android 有个 ScaleType.CENTER_CROP 对应于 iOS 下面的 Aspect Fill
不过需要将 clipSubViews 选中，否则绘制图片的布局将会撑大原有的frame。



