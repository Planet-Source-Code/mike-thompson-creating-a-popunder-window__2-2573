<div align="center">

## Creating a popunder window


</div>

### Description

My article shows you how to create a popunder window using scripting.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mike Thompson](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mike-thompson.md)
**Level**          |Intermediate
**User Rating**    |5.0 (20 globes from 4 users)
**Compatibility**  |
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mike-thompson-creating-a-popunder-window__2-2573/archive/master.zip)





### Source Code

<h3>Creating a popunder window</h3>
<p>I feel guilty writing this tutorial, but as the saying goes, &quot;give the
people what they want&quot;, or to be more precise, developers. A lot of
developers would like to know how to implement popunder windows on their site as
a way to broadcast advertising. Yes it's annoying for the visitor, but proven
quite effective in getting attention.</p>
<p>Creating a popunder window is very simple, by using Javascript. Basically one
would use the same method for creating a popup window, but then
&quot;unfocus&quot; it. Here is the code in full force:</p>
<pre>&lt;script&gt;
win2=window.open(&quot;http://www.msn.com&quot;)
win2.blur()
window.focus()
&lt;/script&gt;</pre>
<p>That's it! I open a window by invoking &quot;window.open()&quot;, blur it,
then redirect the focus to the main window instead. Translation- the popup
window becomes a popunder instead.</p>
<p>You can even customize the pop under window so certain standard features are
removed, like the toolbar, or configure the window's size. Here's an example of
each:</p>
<pre>&lt;script&gt;
win2=window.open(&quot;http://www.msn.com&quot;,&quot;&quot;,toolbar=0)
win2.blur()
window.focus()
&lt;/script&gt;</pre>
<pre>&lt;script&gt;
win2=window.open(&quot;http://www.msn.com&quot;,&quot;&quot;,&quot;width=500,height=250&quot;)
win2.blur()
window.focus()
&lt;/script&gt;</pre>
<p>You've probably seen more sophisticated popunder scripts that control the
&quot;frequency&quot; of the popunder, such as popping up only once per browser
session. Instead of reinventing the wheel, I'll simply point you to a nice
example of this on JavaScript Kit: <a href="http://javascriptkit.com/script/script2/popunder.shtml">http://javascriptkit.com/script/script2/popunder.shtml</a></p>
<p>Have fun with popping under your windows.</p>

