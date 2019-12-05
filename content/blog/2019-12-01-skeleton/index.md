---
slug: post-template
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
- Software Peer Review
- R
- community
# delete the line below
# if you have no preferred image
# for Twitter cards
twitterImg: /blog/2019/06/04/post-template/name-of-image.png
output: 
  html_document:
    keep_md: true
---

Everywhere in this template (YAML, chunk below), you should change "post-template" to the slug of your post, and "2019-06-04" to the publication date.

This template will generate both an .html and an .md. Please don't include the html in your pull request to roweb2.

The chunk below ensures your plots will be inserted in the same folder as your Rmd so you can submit the bundle (.Rmd, .md, images) to roweb2.



The figure paths in the resulting Markdown will already be valid so you won't need to edit the Markdown file.

Introduction including outline of the post.

### First awesome section

I like Hugo[^1]. Yes, that is how you add a footnote.

#### First awesome subsection of the first awesome section

Below is an image, for instance your package logo, or a cute puppy picture. Here's how to use a Hugo shortcode to include it. You must use the exact same syntax as below i.e. with the html preserve comments and percent signs, otherwise the knitting will break the syntax. You can use [all options documented for the figure shortcode](https://gohugo.io/content-management/shortcodes/#figure).

<!--html_preserve--> {{% figure src = "name-of-image.png" width = "200" alt = "this is the alternative text" %}}
<!--/html_preserve-->

Here's how to introduce the same image but centered and bigger. Notice ` width = "400"` and `class = "center"`.

<!--html_preserve--> {{% figure src = "name-of-image.png" width = "400" alt = "this is the alternative text" class = "center" %}}
<!--/html_preserve-->

And here's how you'd pull it to the right. Notice `class = "pull-right"`.

<!--html_preserve--> {{% figure src = "name-of-image.png" width = "200" alt = "this is the alternative text" class = "pull-right" %}}
<!--/html_preserve-->

Below is another image, a plot generated by a code chunk, so you might see how to add alternative text and other options in this case. You can also use [all options documented for the figure shortcode](https://gohugo.io/content-management/shortcodes/#figure) except for `src` that will be created automatically when knitting.


```r
plot(1:10)
```

{{<figure src="chunkname-1.png" alt="alternative text please make it informative" title="title of the image" caption="this is what this image shows, write it here or in the paragraph after the image as you prefer" width="300">}}

Once this file is knitted the plot above will be inserted with the correct syntax.

#### Second awesome subsection

Here's how to use a Hugo shortcode to embed a tweet. We recommend the use of [Hugo shortcodes](https://gohugo.io/content-management/shortcodes/) to include tweets, Vimeo or Youtube videos, gists, etc. Again, use the exact same syntax as below i.e. with the html preserve comments and percent signs, otherwise the knitting will break the syntax.

<!--html_preserve--> {{% tweet 1138216112808529920 %}}
<!--/html_preserve-->

### Conclusion

Have fun writing your blog post!

Here's how to add the footnote text for your reference above.

[^1]: Hugo! https://gohugo.io/