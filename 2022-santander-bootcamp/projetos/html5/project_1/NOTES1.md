# HTML5 BASICS

At first, HTML didn't have semantics as clear as the 5th release in 2014. There were only divs that could only be differentiated via class names, such as

` <div class="header"></div>`

`<div class="post"></div>` 



Now, we have much more self-explanatory tags to work with:

- ```<section>``` - for general usage (a generic 'div').

- ```<header>``` - used for menus, search bars and showing logos (there can only be one per page!).

- ```<article>``` - mainly used for the most important part of the page, such as a post. May contain its own header, images, paragraphs `<p>`...

- ```<aside>``` - for secondary information still related to the article. Author's info, contact, ads...

- ```<footer>``` 



... though there are still some relevant tags that remain in use to this day.

- `<h1> to <h6>` - designated to titles
- `<a>` - links/anchors that may be useful sharing.
  - `<a href="normal.link.com/innerpage">`- this link will lead to a page on the same tab.
  - `<a href="normal.link.com" target="_blank">` - this link will open on another tab.
  - `<a href="mailto:one_em@il.com">` - will launch the device's mail app, ready to send an email to one_em@il.com.
  - `<a href="tel:(+55) 11 55555-5555">`- launches the dial app.
- `<img>`- the image tag doesn't have a closing tag.
  - `img src="path_or_link_to_img.png" alt="Description of the image, for accessibility.">`
- `<ul> or <ol>` - these are listing tags. `<ul>` shows an unordered list, while `<ol>`results on ordered ones. The items can be listed with `<li>` for both cases.

