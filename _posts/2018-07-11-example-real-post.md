---
ID: 479
post_title: Example Real Post
post_name: example-real-post
post_date: 2018-07-11 16:02:43
layout: post
link: >
  http://devdevblogs.wpengine.com/blog/example-real-post
published: true
tags: [ ]
categories:
  - Updates
---

		<p>Hey all,</p>
<p>I hope you enjoyed <a href="http://blogs.msdn.com/b/vbteam/archive/2015/04/01/how-roslyn-finally-unshackled-visual-basic-from-the-tyranny-of-the-pretty-lister.aspx">yesterday’s April Fools’ Day post</a>. I thought it was a fun way to kick off an experiment I’d like to conduct and in this post I’ll tell you how you can actually try out lowercase keywords for VB on your machine right now no matter what version of VS you’re using (no joke).</p>
<p>You see, a few years back Architect-emeritus Paul Vick <a href="http://www.panopticoncentral.net/2007/07/20/lowercase-keywords/">asked a question</a>, “<em>Do PascalCased keywords make VB look more verbose than it really is?</em>” At the time I didn’t really give the question enough thought but a lot of commenters responded positively about the look (both then and yesterday) and recently I got to thinking about it again. It is true both that VB uses capitalized words far more often than in natural English text and also that programmers exposed to lots of other programming languages probably also aren’t used to so many uppercase characters. I can imagine how this could magnify the perception of VB’s verbosity so I set out to figure a way to actually test the hypothesis. What I came up with was a&nbsp;special proof-of-concept font:&nbsp;<em><strong><a href="https://github.com/AnthonyDGreen/misc/releases/tag/v0.1-alpha">Glamour</a></strong></em>. How it works it pretty simple: Visual Studio can make keywords appear any color you want. But it can <em>also</em> make keywords appear <strong>bold</strong>. I made a font where the bold version is the same as the regular version <em>but with all of the uppercase letters using the lowercase glyphs</em>. So when this font is installed and selected as the text editor font and keywords are configured to be bold Visual Studio renders them in all lowercase instead&nbsp;(An elegant hack, huh?).</p>
<p><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/00/35/13/4174.dt1.png"><img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/00/35/13/4174.dt1.png" alt="" border="0"></a></p>
<p>There are several advantages to this approach:</p>
<ul>
<li>Anyone using any version of Visual Studio can try it out.</li>
<li>It’s just a presentation thing (a glamour); it won’t cause the pretty-lister to modify an existing file nor will it affect the way the text is actually saved, so…</li>
<ul>
<li>It won’t affect anyone else on your team if they don’t want to try it or don’t like it,</li>
<li>You won’t have to undo any changes if you don’t like it,</li>
<li>If a lot of people like it they can use it without half the VB code in the world using PascalCased keywords and the other half using lowercase keywords.</li>
</ul>
</ul>
<p>Of course, if you look at your code outside of VS or copy/paste it into another program or do anything to make the code not parse as keywords (like commenting out a block of code) it’ll revert to its normal PascalCased look. But for playing around with an idea I still think this is a good enough approach to get a feel for whether you like it or not. Like I said yesterday, when I started programming in QBasic all of the keywords were in SCREAMING CAPS so it’s not like the current style is etched in stone. Who knows, maybe this is popular enough that we add an option to Visual Studio for this kind of thing (no promises!).</p>
<p>I named the font <strong><em><a href="https://github.com/AnthonyDGreen/misc/releases/tag/v0.1-alpha">Glamour</a></em></strong> (like a magical illusion spell) in recognition to its appearance-only effects. It’s entirely based off of the popular open source font <em><a href="http://levien.com/type/myfonts/inconsolata.html">Inconsolata</a></em> by <a href="http://levien.com/">Raph Levien</a> (itself influenced by the popular Microsoft font Consolas) and you can try it out right now:</p>
<ol>
<li><a href="https://github.com/AnthonyDGreen/misc/releases/tag/v0.1-alpha">Download&nbsp;<em><strong>Glamour</strong></em></a> from my GitHub repo.</li>
<li>Install it by drag/dropping the truetype font (.ttf) files in your <strong>%SystemDrive%\Windows\Fonts</strong> folder.</li>
<li>Change your text editor font in the <strong>Tools &gt; Options &gt; Fonts &amp; Colors</strong> dialog to <strong><em>Glamour</em></strong>.</li>
<li>Select “<strong>Keyword</strong>” in the “Display Items” list and check the “Bold” checkbox.</li>
<li>You’re all set. <strong>Happy coding!</strong></li>
</ol>
<p>If you’re a longtime VB user like myself who’s interested in trying something a little different, or someone used to other languages who wants to give VB a more familiar look and feel go ahead and try it out and let us know what you think.</p>
<p>Regards,</p>
<p><strong>Anthony D. Green</strong>, Program Manager, <strong>Visual Basic, C#, and F# Languages Team</strong></p>
