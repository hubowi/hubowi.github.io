---
layout: page
title: About
description: 活着就是改变世界
keywords: 胡博威
comments: true
menu: 关于
permalink: /about/
---

哈喽，我是胡博威！这是我的个人小天地，一个记录我各种「折腾」和「奇思妙想」的地方。

这里可能什么都有：一段刚写的代码，一次旅行的碎片，一本读得停不下来的书，或是某个半夜突然冒出来的怪点子。没什么宏大主题，就是觉得生活里这些细碎的、有趣的东西，值得被认真安放。

如果你碰巧路过，并且对其中某样东西也感兴趣，那就太好啦。欢迎随便看看，随时找我聊聊 —— 说不定，我们能一起「折腾」出点什么新东西呢。

总之，放轻松，把这里当作一个数字世界的客厅就好。很高兴你能来✨

—— 胡博威

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'hubowei.com' %}
<li>
微信：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ site.url }}/assets/images/qrcode.jpg" alt="清风" />
</li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}



