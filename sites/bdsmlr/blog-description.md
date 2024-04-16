> ⚠️ __WARNING__ ⚠️
>
> Due to the explicit nature of the website this fix is about, I recommend reaching out via Session if you have questions. If anyone posts issues/comments that violate GitHub's policies, they will be deleted and blocked without warnings or second chances.


# BDSMLR Blog Descriptions

For those of you who are familiar with the site, you are probably very familiar with their poor web design and lack of maintenance. So when users started posting their Session ID's in their blog description, it wasn't surprising to discover those *very* long ID's were causing the mobile version of the site to break.

Fortunately, BDSMLR has a limited amount of HTML support for their blog descriptions. Now, keep in mind that this "HTML support" is almost certainly __not intentional__. More likely, it's a lucky byproduct of bad/lazy coding. Still, this allows us to implement some of our own fixes that the developers are too lazy to do themselves.

There are other issues with the site's "Blog Description" feature, like how it removes any new lines so you can't have multiple paragraphs, and there are fixes for some of those issues too. But let's start with the Session ID issue.


## Session ID Fix

Long story short, when you're viewing a specific blog on BDSMLR, the site uses an "infinite scrolling" content loading method. This method relies on the position of your screen to initiate and load additional content. However, when a very long, uninterrupted string of characters (like a Session ID or website URL) force the mobile page beyond the width its designed for, this system breaks.

Without getting too complicated, the core issue behind the Session ID issue is the lack of "word wrapping" in the site's style rules. To fix this, you can use the HTML Span Element to enable word wrapping so that the Session ID's continue on another line without actually breaking the ID for when you copy/paste it.


### Basic Template

```html
<span style="word-wrap: break-word;">
DESCRIPTION GOES HERE.

<br /><br />
This will come out as a separate paragraph (as if you pressed Enter twice).

<br /><br />
Session ID:
<br />
SESSION ID GOES HERE.
</span>
```

If you want to start from scratch and only copy the span element, you can copy the following code block:

```html
<span style="word-wrap: break-word;">

</span>
```


## Multiple Paragraphs

As you might have seen in the template above for the Session ID fix, you can create multiple paragraphs in your blog description using the HTML Line Break tag. Make sure you use two of them to add a blank line between each paragraph, if that's what you're going for.

Here's an example...

### What you set:
```html
First paragraph.

<br /><br />
Second Paragraph.
```

### How it renders:
```
First paragraph.

Second Paragraph.
```
