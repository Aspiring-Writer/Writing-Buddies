---
title: Adding Content To W.B.
date: 2020-07-23 03:20:00 -04:00
layout: article
permalink: /adding-content-to-wb
---

This site is meant to be a community for writers of all ages to share their work and receive feedback. It would be pretty weird if I never shared with you how to take advantage of that and join the community, right? Well, that's what this article is going to do.

{% include toc.html %}

## Behind The Scenes

I used [Jekyll](https://jekyllrb.com/), a static site generator, to create the site, GitHub Pages to host it, and Siteleaf to edit the content (when I don't want to deal with GitHub :D). This is a completely free way to get a simple site up and running without a lot of hassle. It also appeals to the coder side of me since I can add in my own custom code and design everything myself. I would recommend this setup to anyone who wants to create their website, or blog, for free.

## Accessing the CMS (Siteleaf)

To post content on this site, we use the awesome, free CMS called [Siteleaf.](https://siteleaf.com/) This CMS allows you to post your content in an easy, code-free way.

To access the CMS fill out [this form](/join-us/) and I will look over your responses, approve them, and email you a link to access Siteleaf.

> **Note:** if you know how to use GitHub or do not mind learning, please create a branch and post your content that way instead. This allows more non-technical users to use the CMS without requiring me to pull out some cash and pay for more users. Thanks.

## How To Use Siteleaf

There are many videos on how to use Siteleaf, so I won't go into detail here. It is very easy to learn and you should have no problem figuring it out on your own, but here are some articles and videos that will help you out:

* [Siteleaf for Clients](https://learn.siteleaf.com/getting-started/siteleaf-for-clients/) (Just an overview of how static sites and Siteleaf work)

* [Siteleaf for Content Managers and Creators](https://www.siteleaf.com/blog/siteleaf-for-content-managers-and-creators/)

* [Publishing A New Blog Post](https://www.siteleaf.com/blog/publishing-a-new-blog-post/)

### Metadata Fields

After reading the articles above, you should have a pretty good idea of what to do to start writing your posts. The only thing I need to go over is the metadata fields that you must use for your posts.

**All of these are case sensitive!**

> **GitHub Users:** these metadata fields are just the YAML Frontmatter

#### Tags

The first metadata field that you should see on the left of Siteleaf's post editor is the TAGS field. In this field, you will put the genres of your work and any other tags you want to help categorize your post, ie. Fiction, Romance, Drama, etc. When you click on it, a dropdown menu should appear showing you the currently available options, though you are not limited to them alone. All of these are case sensitive and I would prefer if you capitalized each word just to make it look prettier on the [tags page](/tags/).

For books, please only include tags on the introductory post. The reason for this is that I don't want to fill up the tags' page with a bunch of book chapters and articles.

> **GitHub Users:**
>
>     tags:
>       - random
>       - tag

#### Categories

Under the TAGS field, you should see the CATEGORIES field. This field is very important because it determines the URL of your post. For the categories, you should choose the type of content that your post contains. For example, this post is just an article so I would use the category "articles", it is also a tutorial so I use the category "tutorials" as well. If your post is part of a book, use the category "books". If it is a poem, use the category "poetry". Starting to see the pattern?

The current categories are:

* articles

* books

* poetry

* plays

* short-stories

That is for the first category, the second category should be the book and/or series associated with your post. Some posts may have more than two categories, others just one, it really doesn't matter as long as you have less than 5.

The reason why this field cannot be anything you want is that the categories you set will show up in the URL. For example, if I created a post titled "My Cool Post" and assigned the categories "articles" and "random", the URL for that post would be aspiring-writer.github.io/araticles/random/my-cool-post. Do you see how the categories affect the URL? Whatever categories you set will be reflected in the URL between the site's name and your post's title in the exact same order you set them. They should not be changed.

> **GitHub Users:**
>
>     categories:
>       - random
>       - categories

#### Author

The next metadata field you will want to use is called "author". This is not a default field, so you will not see it in Siteleaf's editor. To create this field, scroll down to the "New metadata field" option and click it. A box should appear with the words "Field name" highlighted and bold. Just replace that text with "author" and click the next box under it (it should be a slightly beige color). In this box, you want to put the name that is associated with you. After receiving the email containing the link to Siteleaf, you should have received a follow-up email asking you to choose your author name, nickname, bio, and avatar. The nickname that you chose will be the name that you use in this author field. For example, if you chose the nickname "aspiring-writer", you would type in "aspiring-writer" into this field the exact same way. That's it, the author of your post has been set.

> **GitHub Users:**
>
>     author: author_name

#### Book / Series

This is a field that you only assign to posts that are part of a book or part of a series of posts (series are not specific to any type of work, but they are generally used for articles and stories that are part of series). You create this field just like you created the author field, click "New metadata field" and type in "book" and/or "series" (if you are using both, create two separate fields, one for "book" and one for "series"). In the box under the field name, type in the book/series. All the book's/series' names are lowercased and the words are separated by a dash, ie. "test-my-fire", "pur-ti-miro", "cloudtopia", etc.

> **GitHub Users:**
>
>     book: book-name
>     series: example-series

### Image

This is the final field you will need to insert. This field is actually a list of other fields nested under the "image" field.

There are two images for each post, a "teaser" image, and a "feature" image. Both of these are optional and if left blank, the default teaser will be used and a feature image will be excluded. The teaser image is the image that shows above the post on the site's homepage. The feature image is the image that shows up in the post itself. They can be JPG, JPEG, PNG, or GIF. The images are all stored in the [GitHub repository](https://github.com/Aspiring-Writer/Writing-Buddies/tree/master/images) in the folder "images". To upload images, just go to the GitHub repository (you can find the link at the bottom of the site), click the images folder, click the "Add file" button, and upload the files. You will need a GitHub account to upload files to the repo, but you can use Siteleaf instead. Click the little button on the left that says "Uploads". The only problem with using Siteleaf to upload the images is that it uploads them to the wrong folder. This is something I haven't figured out how to change yet since the site theme is pulling images from a specific folder and will not show up with the posts. Hopefully, I'll figure out how to change this. In the meantime, upload your images through Siteleaf and I will move the images myself so they show up in the posts.

The "image" field is created the same way as the other fields, the only difference is that you click the dropdown arrow after the "New metadata field" option and select "Object". This should insert two boxes like before, only the second box is split into two different boxes.

1. Replace "Field name" with "image",

2. Replace "Key" with "teaser", and in the blank box input the file path for the teaser image, ie "/images/example-teaser-image.jpg".

3. Next, click "New key/value pair" under the "Key" box. You should another field inserted under the "image" field with another "Key" box and a blank box.

4. Replace "Key" with "feature" and in the blank box, input the file path for the feature image (both the teaser and the feature image can be the same file).

The next steps are only needed if you are crediting the image:

1. Repeat steps 3 and 4, replacing "Key" with "credit", and inserting the name of the image's owner.

2. Repeat steps 3 and 4 again, replacing "Key" with "creditlink" and inserting the link to the image's owner (exclude https://)

> **GitHub Users:**
>
>     image:
>       teaser: example-image.jpg
>       feature: example-image.jpg
>       credit: Example People
>       creditlink: www.example.com/images

---

That's all you need to know to start adding your posts to the site! It seems like a lot, but it is worth it and you will get the hang of it pretty quickly. One last thing, if you want to add a "Table of Contents" add "{% include toc.html %}" (without the quotes) wherever you want to TOC to be. There should be an empty line preceding and following the include.

Make sure you bookmark this page for easy reference later!

Now go start writing your posts!
