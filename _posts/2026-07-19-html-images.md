---

layout: post
title: "HTML Images for Beginners: Add Beautiful Images to Your Web Pages"
date: 2026-07-20
author: Chayank
categories: web-development
tags:

* html
* html tutorial
* images
* img tag
* web development
* beginners
  image: https://images.unsplash.com/photo-1498050108023-c5249f4df085
  excerpt: "Learn how to add images to your HTML webpages with the img tag. Understand image paths, resizing, alt text, responsive images, and common beginner mistakes through practical examples."

---

# HTML Images for Beginners: Add Beautiful Images to Your Web Pages

Welcome back! 👋

So far in this HTML series, you've learned how to create webpages, use different HTML elements, organize content with lists, and connect pages using links. Now it's time to make your website look more attractive by adding **images**.

Think about your favorite website. Whether it's YouTube, Amazon, Instagram, or a personal blog, every great website uses images to grab attention, explain ideas, and create a better experience for visitors.

Imagine opening an online shopping website where every product is represented only by text. It would be difficult to understand what you're buying, and honestly, it wouldn't be very exciting! Images make websites feel alive.

In this tutorial, you'll learn everything you need to know about adding images in HTML. We'll start with the basics and gradually explore resizing images, image paths, alternative text, responsive images, and best practices.

By the end of this guide, you'll be able to confidently add images to your own website.

---

# Why Are Images Important?

Images do much more than make a webpage look beautiful.

They help you:

* Explain ideas quickly.
* Make blog posts more engaging.
* Showcase products.
* Improve user experience.
* Break up long blocks of text.
* Keep visitors interested for longer.

A webpage filled with only text can feel overwhelming. Adding relevant images makes your content easier and more enjoyable to read.

---

# The HTML `<img>` Tag

In HTML, images are added using the **`<img>`** tag.

Here's the simplest example:

```html
<img src="cat.jpg" alt="A cute cat">
```

Unlike most HTML elements, the `<img>` tag doesn't have a closing tag. It's a self-closing element that simply tells the browser which image to display.

Let's understand the two most important attributes:

* **`src`** – Specifies the location of the image.
* **`alt`** – Provides a description of the image if it can't be displayed. It's also important for accessibility and SEO.

---

# Your First Image

Suppose you have this project structure:

```
project/
│
├── index.html
└── cat.jpg
```

Now add the following code to your HTML file:

```html
<img src="cat.jpg" alt="Cute Cat">
```

Save the file and open it in your browser. If the image is in the correct location, it will appear on your webpage.

Congratulations! 🎉 You've just displayed your first image.

---

# Understanding Image Paths

One of the biggest challenges for beginners is using the correct image path.

### Image in the Same Folder

```
project/
│
├── index.html
└── logo.png
```

```html
<img src="logo.png" alt="Website Logo">
```

---

### Image Inside a Folder

```
project/
│
├── index.html
└── images/
    └── logo.png
```

```html
<img src="images/logo.png" alt="Website Logo">
```

---

### Going Back One Folder

```
project/
│
├── index.html
└── pages/
    └── about.html
```

If the image is next to `index.html`, then inside `about.html`:

```html
<img src="../logo.png" alt="Website Logo">
```

Understanding paths now will save you hours of debugging later.

---

# Changing Image Size

Images often appear too large or too small.

You can resize them using the `width` and `height` attributes.

```html
<img src="mountain.jpg" alt="Mountain" width="400">
```

Or:

```html
<img src="mountain.jpg" alt="Mountain" width="400" height="250">
```

If you only specify the width, the browser automatically adjusts the height to maintain the image's proportions.

---

# Adding Alternative Text

The `alt` attribute is more important than many beginners realize.

```html
<img src="flower.jpg" alt="A red rose in a garden">
```

Alternative text is used when:

* The image fails to load.
* Someone uses a screen reader.
* Search engines understand your content.

Always write meaningful descriptions instead of generic text like "image" or "photo."

---

# Using Images from the Internet

You don't always need to download images. You can use an image URL directly.

```html
<img src="https://example.com/image.jpg" alt="Example Image">
```

However, for your own projects, it's usually better to store important images locally so you have full control over them.

---

# Making an Image Clickable

You can combine what you learned in Part 5 with images.

```html
<a href="https://www.google.com">
    <img src="logo.png" alt="Google Logo">
</a>
```

Now clicking the image opens the website.

---

# Responsive Images

People visit websites on laptops, tablets, and phones.

A fixed-size image may look great on a computer but too large on a mobile device.

A simple responsive image uses CSS:

```html
<img src="nature.jpg" alt="Beautiful Nature" style="max-width:100%; height:auto;">
```

This allows the image to shrink automatically on smaller screens.

---

# Common Beginner Mistakes

Here are some mistakes you'll probably encounter—and how to fix them:

### Wrong File Name

❌

```html
<img src="Photo.jpg">
```

If your file is actually named `photo.jpg`, the image won't load on many web servers.

---

### Wrong Folder Path

Always double-check where your image is stored and update the `src` path accordingly.

---

### Forgetting the `alt` Attribute

Even if the image displays correctly, always include meaningful alternative text.

---

### Stretching Images

Avoid setting both width and height to values that distort the image.

Instead, adjust only one dimension or use CSS to maintain proportions.

---

# Practice Exercise

Create a webpage that includes:

* A heading
* Three different images
* One local image
* One online image
* One clickable image
* Different image sizes
* Meaningful `alt` text for every image

---

# Mini Project

Build a simple photo gallery.

Ideas:

* Your favorite places
* Animals
* Cars
* Technology
* Nature

Add a title below each image and make the gallery easy to browse.

---

# Key Takeaways

Before moving on, remember these important points:

* Images are added using the `<img>` tag.
* The `src` attribute tells the browser where the image is located.
* The `alt` attribute improves accessibility and SEO.
* Learn image paths carefully—they're one of the most common sources of errors.
* Responsive images make your website look better on all devices.

---

# What's Next?

In **Part 7**, we'll explore **HTML Tables**.

You'll learn how to:

* Create tables
* Add rows and columns
* Merge cells
* Style tables
* Build professional-looking data tables

By then, your webpages will be able to display information in a clean and organized way.

Happy coding, and see you in Part 7! 🚀
