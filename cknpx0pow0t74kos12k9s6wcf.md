## Building a landing page with HTML & CSS - part 2

Welcome back.

In part 1 of this series, we took a very simple page with nothing other than a few lines of text (and some links), and added the basic HTML structure to it.

Now, let's continue building this basic landing page by further improving it.

As a reminder, the landing page can be found at the following URL: 
[https://aldercode.com/buildinpublic1/](https://aldercode.com/buildinpublic1/)

## Adding links ##

If you're completely new to HTML, I may have jumped the gun a bit by having links already included in the text right from the outset, so let's address those immediately. 

To add a link (hyperlink) to any other site, item or section, we use `<a>` tags. Additionally, we add 'href' to specify the link to follow. So, `<a>` to specify that it's a link and 'href' to list the details of that link.

Here's an example from the actual page we're building:

The landing contains the following last sentence:

"Also, please say Hi on Twitter, and let's chat: https://twitter.com/aldercode." 

*(This blogging platform is automatically excluding the 'https://' part of what you read here, but rest assured, it's there in the background.)*

Here's the HTML for that line, viewable by right-clicking on the page and selecting 'View page source':

```
<p>Also, please say Hi on Twitter, and let's chat: 
<a href="https://twitter.com/aldercode"
    target="_blank">https://twitter.com/aldercode</a>.</p>
```

Let's unpack what we're seeing:

Firstly, we see the usual opening and closing `<p>` tags to specify that this is a single paragraph.

Then, BEFORE the clickable part of the text starts we find the opening `<a>` tag, with the 'href' information (the actual link is always wrapped in quotes). That's simply specifying the actual URL to go to. 

Following that, we see `target=_blank`. This can be excluded if you'd prefer - it's by no means mandatory. If it is excluded, the link will simply open in the very same browser tab currently in use. 

In this case, I used `_blank`, meaning: Open this link in a new tab within the browser. If you want your users to not totally disappear from your site while they check out the link you're sending them to (without having to click the Back button on the browser), this is one way to achieve this.

Then, after the opening tag, we get the actual highlighted/underlined clickable text. This is followed by the closing `</a>` tag, specifying the end of the linked text.

NOTE that we can link pretty much any text we'd like to (or pretty much anything else too, but we'll get to that in due course...). There's really no need to write the actual URL as the clickable text like I did here. 

Want an example?

I could easily have rewritten that entire line as follows (and probably should have, as it looks neater...):

"Also, please say Hi on [Twitter](https://twitter.com/aldercode), and let's chat."

Now, the source code for this line looks as follows:

```
<p>Also, please say Hi on <a href="https://twitter.com/aldercode"
    target="_blank">Twitter</a>, and let's chat.</p>
```

(That definitely looks a little neater, right?)

Now, the relevant word to link, in this case 'Twitter', is the actual link to click.

So, now that we've decided that linking the relevant word or phrase looks neater, let's go and update all three links included on the landing page.

Done?

Good. Here's a screenshot of how it now looks:


![Photo of the site after correcting links](https://cdn.hashnode.com/res/hashnode/image/upload/v1618913702056/AxpI9IycN.jpeg "Site 4 pic")

And, here's the updated page source code:

```

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>

<body>
    <h1>Hello World!</h1>

    <p>Welcome to my #buildinpublic landing page.</p>

    <p>Let's turn what you see here into a simple landing page using HTML and CSS.</p>

    <p>Want to follow along? Then please follow my <a href="https://blog.aldercode.com/" target="_blank">dev blog</a> and/or sign up for my
        <a href="http://eepurl.com/hu9lUX" target="_blank">newsletter</a>.</p>

    <p>Also, please say Hi on <a href="https://twitter.com/aldercode"
        target="_blank">Twitter</a>, and let's chat</a>.</p>
</body>

</html>
```

Right, let's move on.

## Changing the page title ##

Remember in the previous post, when the page title (visible on the tab at the top of the browser window) changed to ''Document" when we added the structure? Well, I don't like that title as it doesn't really mean anything.

So, let me pop off and change that quickly by amending the `<title>` content within the HTML `<head>` section...

Was:

`<title>Document</title>`

Now:

`<title>My Website</title>`

Here's how it looks now:


![Photo of the amended tab title.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1618914386102/cpa6dfbiq.jpeg "Site 5 pic")

That's better, right?

You can call it whatever you'd like. That being said, have you noticed how devs like to joke about how many browser tabs they always seem to have open? Well, that really does happen, and not just for devs. So, you may want to keep your page title nice and short so it doesn't get squashed away into nothingness as soon as a few more tabs are opened next to ours.

---
** So, to recap: we've learned about adding links and also changing the page's title. **

And on that note, that brings us to the end of Part 2. 

Part 3, coming soon...

---
Spotted any errors or omissions? Please do let me know!

Liked the post? Then please stop by on [Twitter](https://twitter.com/aldercode) to say Hi. 

%%[ko-fi]


