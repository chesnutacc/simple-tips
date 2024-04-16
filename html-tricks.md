# HTML Tricks

> ⚠️ __Important__
> 
> __This guide is not meant to be any kind of definitive or comprehensive resource for HTML (or anything else).__
>
> Any information found anywhere in this repository is almost certainly __meant for something *very* specific__ and is likely __*extremely* oversimplified__.

## HTML Tage & Elements for Dummies

Because I want to keep this as easy and user friendly as I possibly can, I'm going to oversimplify things as much as I possibly can.

At its core, __HTML__ is built entirely with two main components: __Tags__ and __Elements__.

1. __Tags__: The *"Self-Contained"* Building Blocks of HTML.
2. __Elements:__ The foundation for basically all content on an HTML web page.

Below is a simple diagram that illustrates the differnt parts of an __HTML Element__:


<img src="./img/DO_Elements-Diag.png"
    alt="HTML Elements (image from DigitalOcean)"
/>
Image taken from the *[What is an HTML Tag?](https://www.digitalocean.com/community/tutorials/what-is-an-html-tag#)* tutorial by *[DigitalOcean](https://digitalocean.com)*.
 



### HTML Tags

Tags are usually referred to as the *Building Blocks of HTML*, and that's exactly what they are. Everything in HTML is made of tags. Everything.


#### What does an *HTML Tag* look like?

All HTML Tags have at least 3 parts:

1. The "opening" arrow `<` to start the tag
    - Also known as the "less-than" symbol.
2. The tag name itself, like `br` for "line break" (see below).
3. The "closing" arrow, `>` or `/>`.
    - Also known as the "greater-than" symbol.
    - Both are correct, but the forward-slash `/` isn't necessary.

See the Tag Example below for how the Line Break tag uses just these three components.

##### Tag Example: Line Breaks (New Line)
```html
<br />
<br/>
<br>
```

All 3 of those examples above are valid, but I prefer to use the first one because it makes my HTML code a little easier to read. 


#### Attributes

So, what about HTML tags that have more than those 3 components? Well, those additional components are called __[Attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)__. On a basic level, attributes always follow this format:

```html
<tag attribute="value">
```

There can be many attributes, typically separated by spaces or new lines.

However, because this guide is meant for people who don't have any experience (or interest) in web development, there's really only one tag you might use that requires the use of attributes: The __Image Tag__ `<img>`.

The `<img>` tag requires at least one attribute to indicate the source of the image, otherwise it will just load a blank image placeholder.

Here's a very basic example of how I used the `src` and `alt` attributes of the `<img>` tag to post the "HTML Elements Diagram" above:

```html
<img src="./img/DO_Elements-Diag.png"
     alt="HTML Elements (image from DigitalOcean)"
/>
```

For more information about how to use the __HTML Image Tag__, see Mozilla's official documentation [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img).



<br />

### HTML Elements

How are Elements different from Tags? Elements are made of `<Open>` and `</Close>` tags.

No, it's nothing like a door opening and closing. Think of it more along the lines of __Beginning__ and __Ending__.

One of the more commonly used HTML elements is the __[Paragraph Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)__, which is also shown in the diagram above.

```html
<p>
  This is a paragraph.
</p>
```

But because this isn't a guide to web development, let's move on to something more useful to casual users looking for some neat tricks.



<br /><br />

## Creating Embedded Hyperlinks

Adding and creating __Hyperlinks__ has become so universally streamlined and automated that, at this point, people just expect hyperlinks from any URL they paste into a text field, or send in a message.


And that's exactly how it should be, because 99.9% of the time, that's exactly how it works in pretty much everything. Universal defaults are (usually) a wonderful thing. It helps people do things without needing to be very knowledgeable on the subject.


#### Question: What if it doesn't automatically work?

So, what happens when you paste a URL and it doesn't automatically become blue text that can magically take you to where you want to go?

Well, if you're using a blog or something that has a little support for HTML, you're asking that question in the right place. Otherwise, maybe try asking that question on Google or something.

For those of you looking for an HTML solution, here are the basics...


### Hyperlink Basic Format

> ℹ️ __Note__
>
> This is meant to help average users take advantage of certain systems or platforms that offer **limited HTML support**, like some blogs.

> ℹ️ __Note__
>
> For more information about the HTML Anchor `<a>` Element, please refer to Mozilla's official [Anchor Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) documentation.

To create a hyperlink using HTML, we're going to use the __Anchor Element__, which is just `<a...></a>`.

```html
<a href="URL">DISPLAY TEXT</a>
```


<br /><br />

---

> ⚠️ This guide is still a work in progress. ⚠️





