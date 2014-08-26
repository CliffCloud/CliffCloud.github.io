---
title: embedding climbs
tags: bloggers
description: Include Cliffcloud climbs in any other website with a snippet of inline text that offers a dropdown or an individual panel. Updates automatically!
titleimage: '/img/features/embed.gif'
---
## Using Cliffcloud Embeds

>> ![button location on climb page]({{site.url}}/img/features/embed.gif)
>
> The code you get might look complex, but it offers two clean results! Here's a quick rundown of the feature: 

### #1 Embed Panel

This code 
{% highlight html %}
<iframe height="260px" width="400px" frameborder="0" src="http://www.cliffcloud.com/climbs/embed/53da93c602ea7300009ee2c1" seamless></iframe> 
{% endhighlight %}

gets you a slick box that looks like:

> <div><iframe height="260px" width="400px" frameborder="0" src="http://www.cliffcloud.com/climbs/embed/53da93c602ea7300009ee2c1" seamless></iframe></div>


### #2 Inline Text 

{% highlight html %}
<style>span.cc-embed{position:relative}.cc-embed .cc-embed-panel{position:absolute;display:none}.cc-embed:hover .cc-embed-panel{display:inline-block;background:#fff;padding:8px;border:2px solid #000;border-radius:5px}.cc-embed .cc-embed-text{color:#ff0}.cc-embed img{max-width:25px;max-height:25px}.cc-desc{min-width:400px}</style><span class="cc-embed"><span class="cc-embed-text"><a href="http://www.cliffcloud.com/climbs/53da93c602ea7300009ee2c1">Life is Beautiful</a></span><span class="cc-embed-panel"><iframe height="260px" width="400px" frameborder="0" src="http://www.cliffcloud.com/climbs/embed/53da93c602ea7300009ee2c1" seamless></iframe></span></span>
{% endhighlight %}

This one's a bit heavier, but it allows you to include inline text like so: 

> <div><p>in a sample blog post about <style>span.cc-embed{position:relative}.cc-embed .cc-embed-panel{position:absolute;display:none}.cc-embed:hover .cc-embed-panel{display:inline-block;background:#fff;padding:8px;border:2px solid #000;border-radius:5px}.cc-embed .cc-embed-text{color:#ff0}.cc-embed img{max-width:25px;max-height:25px}.cc-desc{min-width:400px}</style><span class="cc-embed"><span class="cc-embed-text"><a href="http://www.cliffcloud.com/climbs/53da93c602ea7300009ee2c1">Life is Beautiful</a></span><span class="cc-embed-panel"><iframe height="260px" width="400px" frameborder="0" src="http://www.cliffcloud.com/climbs/embed/53da93c602ea7300009ee2c1" seamless></iframe></span></span> you could do something fancy like mention that climb and continue talking about the rest of your trip. Then your readers don't get more than they want, but it's there for everyone that does.</p></div>

That's it, happy embeds!

----------------------------

## Help, troubleshooting, etc.

#### **I don't want to use the climb name in the text**
 * The inline text will show the climb name by default, but finding and replacing the name in the embed code will let you use whatever text you want. 

 * If you're not familiar with HTML but want alternate text, just make sure you don't delete the `>` or the `<` surrounding the climb name. In other words, only replace the _exact_ name. 

#### **My blog isn't showing what it's supposed to?**

#### Your blog might not allow HTML in the visual editing area. In this case:

>
> Find a view called **text**, **HTML**, **code**, or something similar where you see lines that start with `<p>`, `<h1>`, `<ul>`, or other bracket surrounded words
>
> Paste your embed code into that view instead of your visual editing area

#### Your blog doesn't have a code editing area?

>
> paste a plain embed box on its own line between a `<div>` and `</div>` that you add yourself. Like so:
>
>> `<div>` `<iframe height="260px" width="400px" frameborder="0" src="http://www.cliffcloud.com/climbs/embed/###climbID####" seamless></iframe>` `</div>`
>
> for inline text with a dropdown paste the code where you want it in the paragraph, and then surround _that paragraph_ with `<div><p>` at the beginning and `</p></div>` at the end. Your final product should look like: 
>
>> `<div><p>` your paragraph about climbing goes on and on until it mentions your climb and you include the inline embed code `which you might put here` and then continue talking until you close the paragraph with `</p></div>`

