+++
draft = false
date = "2019-12-23T12:09:32+02:00"
publishdate = "2019-12-23T12:09:32+02:00"

title = "Emoji Support"
description = "Guide to emoji usage in Hugo"
summary = "Emoji can be enabled in a Hugo project in a number of ways."

tags = [
    "emoji",
]

keywords = ['hugo', 'emoji', 'example']

[author]
    name = "Asur"
    homepage = "/"

[image]
    src = "/images/share-banner.png"    

[twitter]
    site = "@asurbernardo"

[sitemap]
    changefreq = "monthly"
    priority = 0.5
    filename = "sitemap.xml"

+++

{{< under-title >}}

# Emoji support

{{< adsense
    width="320"
    height="320"
    layout="fixed"
    slot="123456789" >}}

    
{{% post-it type="info" title="Info! 💬" %}}
80 days around the world, we’ll find a pot of gold just sitting where the rainbow’s ending. Time — we’ll fight against the time, and we’ll fly on the white wings of the wind.
{{% / post-it %}}


Emoji can be enabled in a Hugo project in a number of ways.

The [`emojify`](https://gohugo.io/functions/emojify/) function can be called directly in templates or [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

To enable emoji globally, set `enableEmoji` to `true` in your site’s [configuration](https://gohugo.io/getting-started/configuration/) and then you can type emoji shorthand codes directly in content files; e.g.


<!-- <p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br> -->

:bug:

:zap:

The [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) is a useful reference for emoji shorthand codes.

***

**N.B.** The above steps enable Unicode Standard emoji characters and sequences in Hugo, however the rendering of these glyphs depends on the browser and the platform. To style the emoji you can either use a third party emoji font or a font stack; e.g.

{{< highlight html >}}
.emoji {
font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
}
{{< /highlight >}}

{{< css.inline >}}
<style>
.emojify {
	font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
	font-size: 2rem;
	vertical-align: middle;
}
@media screen and (max-width:650px) {
    .nowrap {
	display: block;
	margin: 25px 0;
}
}
</style>
{{< /css.inline >}}