# My-portfolio

### Who

I'm Cassidy. I'm a engineer and I've been teaching myself HTML, CSS, and other web development and scripting for over 15 years.
And I want to teach you now.
Because you're good looking.
And because it's useful.

### What

In this tutorial, we'll start from the very beginning.  You don't need to know anything about HTML and CSS or anything about code to start.  I'll include some tutorial files for you to play with and check out.

### When

Now.  Or whenever.  I'm not planning on taking this down anytime soon.  But you are only limited by your own schedule.  Or set free by it.  Whatever.

### Where

On a computer.  Here.

### Why

Because this stuff is important.  Whether you're a business person formatting your emails, an aspiring web designer wanting to get your feet wet, or just someone who is interested and hasn't tried any sort of coding, scripting, or programming before, **HTML and CSS are an essential part** of your learning curve.

## Table of Contents
	* Editors
	* Tag Structure
	* Text Structure
	* Links
	* Other tags
		* Images
		* Line Breaks
		* Tables
	* Making Things Gorgeous The Wrong Way
		* Colors
		* Width and Height
		* Borders
		* Text Styles
	* The `<head>` tag
	* Putting it all together so far
		* Classes
		* ID
			* HTML5 and CSS3
			* How To Meet Losers (Get it? HTML Jokes are the best...)        
 * [Final Project!](https://github.com/Sneha-create/My-portfolio)
 * And now, the end is near

## HTML Time. Let's Go.

### Editors

So the first thing you'll need is an editor to edit your jazz.  There's tons of options out there.

 * Notepad/TextEdit (that's right, the stupid thing that comes on your computer) - This is about as basic as you can get.  It's totally okay if you want to use this, but I recommend one of the editors below just so you can see code highlighting (which will help you out later on).  But, if you want to be a purist, this'll work just fine.
 * [Sublime Text 3](https://www.sublimetext.com/3) - This is a pretty popular option, and for good reason.  Very clean interface.  Once you can navigate it (learning curve isn't that big), it's pretty dreamy. Like your face.


### HTML Tag Structure

Here is a barebones HTML page, about as simple as you can get.  You can open it up in the **1 - Structure** folder in the file part1.html.  If you were to open the file in your favorite browser (which you can do, go ahead), you'll see a plain webpage with the title "My Website" and the words, "Hello, World!" written on the page.

```html
<!doctype html>
<html>
	<head>
		<title>
			My Website
		</title>
	</head>
	<body>
		Hello, World!	
	</body>
</html>
```

So, what are we looking at here?
HTML, short for *HyperText Markup Language*, consists of these things called tags, which are words written between `<` and `>` characters, like `<sometag>`.  All tags (with just a few exceptions that we'll talk about later) have a matching closing tag, which has the same name as the opening tag, except that it contains `/` after the first `<`, like `</sometag>`. 

For example, `<html>` is one tag and the closing tag for it is `</html>`, same with `<head>` and `</head>` and `<body>` and `</body>`, and so on.  You get it.
The opening and closing tags together are an *element* (which also includes everything written in it).  For example, `<title>My Website</title>` is one element.  The text inside an element, in the title case, `My Website`, is called the *content* of an element.

Tags organize your page and tell the browser what your page consists of.  There's tons of tags out there, some that you may never use.  
Here's some lists of tags if you really care to see all of them at this point:
 * [HTML Dog Tag List](http://www.htmldog.com/reference/htmltags/)
 * [W3Schools Tag List](http://www.w3schools.com/tags/default.asp)
 * [Quackit HTML Tag List](http://www.quackit.com/html/tags/)

So, if you look at our example, you can also put tags inside other tags (like we did with the `<title>` tags inside the `<head>` tags).  This is called *nesting* elements.
In this case, we would say that the `<head>` *contains* the `<title>`.  Sometimes when you have a lot of nested tags, it's hard to keep track, so you have to format your code with spacing, as shown.  Typically, inner tags are spaced more than their outer tags (just as `<title>` is indented further than `<head>`).

Let's take a look again at part1.html in the **1 - Structure** folder.  You'll notice that the first line has `<!doctype html>`.  Every HTML document and website has to have this special tag, as it tells the browser what language we're using.  This is one of those special tags I mentioned that doesn't need a closing tag.

On the second line, you can see a `<html>` tag.  Everything in the website is contained by this tag, and the last line of your entire document will always be `</html>`.

Inside `<html>`, there are two elements: `<head>`and `<body>`. Contained in `<head></head>`, we will put all kinds of information for the browser that the user doesn't necessarily need to see.  For now, we just have `<title>`. The content of `<title>` will be used for the name of the tab of the browser, and also by search engines. 

On the other side of the planet, we have `<body></body>`.  Everything visible to the user is contained in these tags.  Right now, all that consists of is "Hello, World!"  Let's change that for fun.  Replace "Hello, World!" with your own text in your favorite HTML editor, and then open the page in your browser.  Neat!

### Structuring text

Let's get juicy.  We're going to talk about some new tags for structuring your text.  Because you're not going to want just one style of text throughout your whole website, right?

Check out part2.html in the **1 - Structure** folder.  The tags that we'll be talking about here are `<h1>`, `<p>`, `<ul>`, and `<li>`.  Open the file in the browser to try and understand what the heck is going on. 

Now, let's talk about it.

First, we have `<h1>`, which adds a *heading* to our website.  Basically, a heading is just text with a bigger font.  But still.  Important. We'll soon learn how to adjust any and all font sizes, but not yet.  Just know that your headings should be in `<h1>` tags.  Also, if you have a smaller heading, or *sub-heading*, you could use `<h2>`, which is smaller than `<h1>`, but bigger than regular text.  You can keep going with more numbers until you reach `<h6>`, with each heading a bit smaller than the previous.  Try adding some subheadings underneath our current heading!

Next, we have `<p>` tags.  `<p>` adds a *paragraph* of text to our website, which are blocks of text that have some space before and after them.  Edit the text in the paragraphs given, and add your own to see what I mean!

And finally, we have `<ul>`.  `<ul>` means a bulleted list (also known as an *unordered list*), where every `<li>` is an item in that list (called a *list item*). But what if you want a numbered list?  You could change `<ul>` to `<ol>` (and don't forget its closing tag), it's that simple!  `<ol>` is an *ordered list*, which has numbers instead of bullet points, and that is truly the only difference.  Add some list items (`<li>`) to the list (make sure you stay inside the `<ul>` tags), and then change your `<ul>` tags to `<ol>`!

### Links

Links are what makes the world/Internet go 'round.  Seriously.  So, let's learn about them.

Links are made with the `<a>` tag, which stands for *anchor*.  

Open up the **2 - Tags** folder, and add this piece of code right after your heading in page1.html:

```html
<p>This paragraph <a href="http://www.lalalalalalalalalalalalalalalalalala.com/">has a totally awesome link.</a></p>
```

Open page1.html in a browser and click on it!  BEAUTIFUL.

Okay, so let's take a look at this.  First of all, you can see the `<a>` tag there contained in the paragraph.  Beautiful.
But what's that funky milk `href=`?  Well, that syntax called an *attribute*.  Attributes change the way a tag works, and are not visible to the website's user.  You only add attributes to the opening tag, not a closing tag.  Tags can have multiple attributes, for example:

```html
<tag attribute="value1" attribute2="value2">Content of tag</tag>`
```

Got it?  Good.  You're so good looking.

So, anyway, the attribute 'href' tells us where the link is going to go when the user clicks on it (and for those curious, it stands for *hyperreference*).  Try adding some more links to the page to different websites!  

Also, one thing you should note:  Links don't have to be in `<p>` tags like I put above.  You could put them in `<li>` tags in a list, `<h1>` tags for a linking header, or completely on their own!

#### Adding links to other pages in your website
Let's just say you have a fully functioning website called fakewebsite.com.  You have your homepage and your "Contact Us" page in the same directory or folder.

Normally when a beginner links to different pages on their website, they just make links that look like `<a href="http://www.fakewebsite.com/index.htmL">Home</a>` and `<a href="http://www.fakewebsite.com/contactus.htmL">Contact Us</a>`.

This is okay.  BUT, you can do better.  So, what if you change your domain name to reallyfakewebsite.com?  When you edit your HTML, you'd have to edit every single one of the links to match the new domain.  That's gross.  There is a better way.

When you make a link to a page within your own directory or folder on your website, instead of putting in the whole URL, put in something more like this:

```html
<a href="page2.html">Click here to go back to Page 2.</a>
```

Paste this line of code into page1.html.  Watch the magic happen.

Now, if you were to change your domain or location of your files, you don't have to change a thing.  Boo yah.

### Other tags

So, you can reference the links that I showed you before if you want to check out some jazzy stuff you can do with your page.  There are some other ones though that you might want to see before we move on to cooler and bigger things.

#### Images
`<img>`. Let's just say you want to put an image on your website.  This is probably a good tag to know.  
Add the following to page1.html:

```html
<img src="https://i.imgur.com/B9q0A.gif" />
```

Open up the page in a browser.  WHOA.  Image!  So, the `<img>` tag is one of those special tags.  First of all, it doesn't have a closing tag.  You just stick in a `/` at the end of the one tag and you're done.  Secondly, it also has a `src` attribute (which is short for *source*), and in the value of that attribute you put the URL of the image (similar to `href` in the anchor tag).

One attribute that might be good for you to remember for `<img>` tags is the `alt` attribute.  If you changed the code above to:

```html
<img src="https://i.imgur.com/B9q0A.gif" alt="I could have danced all night" />
```

When you load the page in the browser, the image looks the same.  But, if you roll your mouse over the image, you'll see some words appear!  WOW.  That's the `alt` attribute.  It stands for the *alternate text* for an image, and it's used when a user can't view the image for whatever reason (using a screen reader, slow connection, error in the `src` attribute, etc.).  Or, in the case of [XKCD](http://xkcd.com/), it's used to add more humor to the page (roll your mouse over all of the comics on the site, they always add another joke or two that a lot of people don't know about).

#### Line breaks
Let's just say you want to keep all your content in one paragraph `<p>`, but you still want to break it up.

That's easy.

So, there's two special tags here, `<hr>` and `<br>`.  They are *empty tags*, meaning they have no closing tag.

`<hr>` stands for *horizontal rule*, and creates a visible line break.
`<br>` is a simple line break, all it does is split your paragraph up.

Try inserting these in between some of your `<p>` tags to try it out!

#### Tables
Tables are really cool.  They can also be a bit confusing.  Open up tables.html (in the **2 - Tags**  folder) in a browser to check out the example table I made for you there.

There's several tags for tables, but the essential ones are `<table>`, `<tr>`, `<th>`, and `<td>`.  Look at tables.html in your editor.

We're going to make our own table again on this page.  You can delete the one I made for you, or just make one underneath the current one there.

So, to create a table, you start with the `<table>` tag.  Simple enough.
	
This will contain all the parts of your table.  Sometimes, tables have a `border` attribute that will equal some value for the thickness of the table's border (it's proper to have just "1" or nothing, for reasons we'll explain later).  Go ahead and add one so it looks like this:

```html
<table border="1">
</table>
```

Boom.  Let's add some more.

The next tag we're gonna check out is `<tr>`, which is for a *table row*.  Easy peasy.  So, let's add 3 `<tr>` tags to our table.

```html
<table border="1">
	<tr>
	</tr>
	<tr>
	</tr>
	<tr>
	</tr>
</table>
```

## Final Project!

Alrighty!  So you've looked at the **My-portfolio** folder a bit, but I haven't told you what that folder is for yet.

Well guess what.

It's a project. [confetti]


Thanks for reading, you beautiful specimen, you.
