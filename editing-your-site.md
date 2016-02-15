---
layout: post
title: How to edit your Jekyll site and make posts
excerpt: "Edit your site and make posts "
modified: 2016-02-15 11:00:29 
tags: [intro, beginner, jekyll, tutorial]
comments: true
---

This article will cover the basics on how to edit the features of your site and make new posts. To do this, you will need a text editor. Here are some examples: 
* [Atom](https://atom.io)
* [Sublime Text](https://www.sublimetext.com)
* [Notepad++](https://notepad-plus-plus.org)

## Editing the configuration of your Jekyll site
The _config.yml file stores data about you and your site, such as your contact information and your site's title and URL.

<pre><code>
# Site wide configuration

title:            Todd Stoffer
locale:           en_US
url:

. . .

# Site owner
owner:
  name: Todd Stoffer
  avatar: bio-photo.jpg
  bio: "Hi I'm Todd, I am a librarian."
  email: tdstoffe@ncsu.edu
  
</pre></code>

You can edit this file by opening it in a text editor, editing the information, and then saving it into the repository folder, replacing the older version of the file. You will then need to commit the changes to your github repository so that the changes will show up on your Jekyll site. 


## Adding a photo to your site

In the _config.yml file, you can add a photo that will be featured on the home page. In the site owner section, change "bio-photo.jpg" to your own image name. Make sure to add the new image to the images folder as well.

<pre><code>
# Site owner
owner:
  name: Todd Stoffer
  avatar: bio-photo.jpg
</code></pre>


## Adding posts

All you have to do to add a new post is to create a file and drop it into the _posts folder. 

Each post must have a header that tells Jekyll how to display your page. The header looks like this:

<pre><code>
---
layout: post
title: Your Title
excerpt: "Edit your site and make posts "
modified: 2016-02-15 11:00:29 
tags: [intro, beginner, jekyll, tutorial]
comments: true
---
</code></pre>

Make sure to use the three dashes at the top and bottom of the header. Then you can write your post below the dashes. 

## Editing accent colors on your page

The color_options.scss file is the place where you can edit the accent bar top and bottom colors on your site. The default colors are indicated by hex code #CC0000. Change the hex codes next to $highlightcolor to your desired colors. For more hex codes, see [here](http://www.w3schools.com/colors/colors_picker.asp). 

<pre><code>
/* Top Color */
$highlightcolor  : #CC0000;
$highlight-color : $highlightcolor;

/*Bottom Color*/
$lowlightcolor  : #CC0000;
$lowlight-color : $lowlightcolor;
</code></pre>

