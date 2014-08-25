---
title: embedding climbs
tags: bloggers
---
#### from any climb page 
![button location on climb page]({{site.url}}/img/features/embed.gif)

The code you get might look complex, but it offers two clean results! Here's a quick rundown of the feature: 

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

----------------------------
### Help, troubleshooting, etc.

#### Different Names?
The inline text will show the climb name by default, but finding and replacing the name in the embed code will let you use whatever text you want. 

If you're not familiar with HTML but want alternate text, just make sure you don't delete the `>` or `<`. In other words, only replace the _exact_ name. 

#### My blog isn't showing what it's supposed to?
There are a lot of potential causes here:

1. Your blog doesn't allow HTML in the 

