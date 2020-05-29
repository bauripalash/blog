+++
draft = false
date = "2019-12-23T12:09:32+02:00"
publishdate = "2019-12-23T12:09:32+02:00"

title = "Markdown Syntax Guide2"
description = "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
summary = "This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme."

tags = [
    "markdown",
    "amperage"
]

[amp]
    elements = ["amp-mathml" , "amp-anim" , "amp-audio" , "amp-video" , "amp-soundcloud" , "amp-facebook" , "amp-instagram"  , "amp-youtube" , "amp-twitter" , "amp-reddit" , "amp-pinterest"]

keywords = ['hugo', 'markdown', 'example']

[image]
    src = "/images/share-banner.png"  

[author]
    name = "Asur"
    homepage = "/"

[twitter]
    site = "@asurbernardo"

[sitemap]
    changefreq = "monthly"
    priority = 0.5
    filename = "sitemap.xml"
+++

{{< under-title >}}

<!-- {{<pinterest url="https://www.pinterest.com/pin/99360735500167749/">}} -->


<!-- {{<twitter tweet="885634330868850689">}} -->


<!-- {{< yt video="eQWTLTmr6AE" width="480"
  height="270"  >}} -->

<!-- {{<math>}}
\[f(a) = \frac{1}{2\pi i} \oint\frac{f(z)}{z-a}dz\]
{{</math>}} -->


<!-- {{< ig id="B__33wSF0LE" height="500" width="500" caption="true">}} -->

<!-- {{< iframe sandbox="allow-scripts allow-same-origin" src="https://palashbauri.in" height="500" width="500">}} -->

<!-- {{< fb href="https://www.facebook.com/ParksCanada/posts/1712989015384373" height="500" width="600" locale="bn_IN">}}

{{< fb href="https://www.facebook.com/nasaearth/videos/10155187938052139" type="video" height="500" width="500" locale="bn_IN" >}}

{{< fb "https://www.facebook.com/zuck/posts/10102735452532991?comment_id=1070233703036185" "comment" "100" >}} -->

<!-- {{< adsense slot="123456" >}}


{{< gif
    alt="Amperage GIF demo"
    src="/images/my.gif"
    width="1367"
    height="1112"
    layout="responsive"
    >}}

{{< gif "/images/my.gif" >}} 

![](/images/my.gif)

-->

<!-- ![](https://upload.wikimedia.org/wikipedia/commons/6/6a/Koala-ag1.jpg "Wallpapesr") -->


{{<img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/Koala-ag1.jpg" width="1000" height="600" layout="responsive" caption="koala">}}

<!--


{{< audio src="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" mp3="https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" ogg="//sample.ogg.fallback.ogg" loop="true" muted="true" >}}   

{{< audio "https://ia801402.us.archive.org/16/items/EDIS-SRP-0197-06/EDIS-SRP-0197-06.mp3" >}} -->

<!-- {{< video
    src="/images/test.webm"
    poster="/images/koala-cover.jpg"
    width="480"
    height="270"
    layout="responsive"
    controls="true"
    autoplay="true"
    muted="true"
    loop="true"
    source="" >}} -->

         
<!-- {{< soundcloud  playlist="331919427" height="450">}} -->



## Headings

{{% toc %}}


<!-- ![Hello World](/images/share-banner.png "Caption") -->


{{% post-it title="Warning! 🚨" %}}
Hong Kong Phooey, number one super guy. **Hong Kong Phooey**, quicker than the human eye. He’s got style, *a groovy style*, and a car that just won’t stop.
{{% / post-it %}}


The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1
## H2
### H3
#### H4
##### H5
###### H6

<h4> Hello H@</h4>

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.</p>
> — <cite>Rob Pike[^1]</cite>


[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### Inline Markdown within tables

| Inline&nbsp;&nbsp;&nbsp;     | Markdown&nbsp;&nbsp;&nbsp;  | In&nbsp;&nbsp;&nbsp;                | Table      |
| ---------- | --------- | ----------------- | ---------- |
| *italics*  | **bold**  | ~~strikethrough~~&nbsp;&nbsp;&nbsp; | `code`     |

## Code Blocks

#### Code block with backticks

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Example HTML5 Document</title>
    </head>
    <body>
        <p>Test</p>
    </body>
</html>
```

#### Code block with Hugo's internal highlight shortcode

{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Example HTML5 Document</title>
    </head>
    <body>
        <p>Test</p>
    </body>
</html>
{{< /highlight >}}

{{< highlight python >}}

import os

for i in range(10):
    print(i)

def pal():
    print("hello")

{{< /highlight >}}




## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Item
  * First Sub-item
  * Second Sub-item

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.
