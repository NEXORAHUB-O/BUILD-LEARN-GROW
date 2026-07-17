---
layout: post
title: "HTML Images and File Paths for Beginners: Add Pictures to Your Website Like a Pro"
date: 2026-07-17
author: Chayank

categories:
  - html

tags:
  - html
  - beginner
  - images
  - file-paths
  - web-development

image: https://images.unsplash.com/photo-1632882765546-1ee75f53becb?q=80&w=1032&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D

excerpt: "Learn how to add images in HTML, understand relative and absolute file paths, and organize your website like a professional developer."
---

Welcome back! 👋

If you've made it this far, give yourself a pat on the back—you've already learned the building blocks of HTML.

In Part 1, you discovered what HTML is and created your first webpage.

In Part 2, you learned how to make your content look clean using text formatting, lists, and links.

Now it's time to make your website come alive.

Think about your favorite websites. Whether it's YouTube, Amazon, Instagram, or a news website, they all have one thing in common—they use images to grab your attention.

A webpage without images often feels plain and unfinished.

The good news?

Adding images in HTML is surprisingly easy once you understand how it works.

In this chapter, you'll learn:

- How to add images to a webpage.
- What the `<img>` tag does.
- The difference between relative and absolute file paths.
- Common mistakes beginners make.
- Best practices for using images on websites.

Let's get started!

---

# Why Images Matter

Imagine you're reading a travel blog about the Himalayas.

Would you rather see:

> "The mountains were beautiful."

Or would you rather see a breathtaking photo of snow-covered peaks?

Images make information easier to understand, more engaging, and far more memorable.

That's why almost every modern website relies on visuals.

HTML lets us display images using a single tag: the `<img>` tag.
## Understanding the `src` Attribute

Now that you know how to use the `<img>` tag, let's talk about the most important attribute inside it—`src`.

The `src` attribute tells the browser **where your image is located**. Think of it as giving someone directions to your house. If the directions are correct, they'll reach your house without any trouble. If they're wrong, they'll get lost.

The browser works the same way. If the path is correct, the image appears. If the path is wrong, you'll see a broken image icon or only the alternative text.

For example:

```html
<img src="images/html-logo.png" alt="HTML Logo">
```

Here, the browser looks inside the **images** folder for a file called **html-logo.png**.

---

# Relative vs Absolute File Paths

One topic that confuses almost every beginner is **file paths**. Don't worry—it's much simpler than it sounds.

A file path is simply the location of a file.

There are two types of file paths you'll use in HTML:

* Relative File Paths
* Absolute File Paths

Let's understand both with simple examples.

---

## Relative File Paths

A relative path points to a file **inside your own project**.

Imagine your project folder looks like this:

```text
MyWebsite/
│
├── index.html
├── about.html
│
└── images/
    ├── html-logo.png
    └── coding.jpg
```

Since the **images** folder is inside your project, you can access an image like this:

```html
<img src="images/html-logo.png" alt="HTML Logo">
```

The browser starts from the location of `index.html`, enters the `images` folder, and loads `html-logo.png`.

This is called a **relative path** because the browser finds the image relative to your current file.

### Why Developers Prefer Relative Paths

Professional developers almost always use relative paths for images inside their projects because:

* They work even if the website is moved to another server.
* They keep projects organized.
* They're shorter and easier to maintain.

---

## Absolute File Paths

An absolute path points to a complete web address.

For example:

```html
<img src="https://images.unsplash.com/photo-1621839673705-6617adf9e890" alt="Programming Setup">
```

Instead of loading an image from your computer, the browser downloads it directly from the internet.

Absolute paths are useful when:

* Using images hosted on another website.
* Displaying logos from trusted CDNs.
* Embedding externally hosted assets.

However, they also have disadvantages.

If the external website removes the image, changes the URL, or becomes unavailable, your image won't load.

For your own website, it's usually better to download the image and store it in your project.

---

# Organizing Your Project

As your website grows, keeping files organized becomes very important.

A common folder structure looks like this:

```text
MyWebsite/
│
├── index.html
├── about.html
├── contact.html
│
├── images/
│   ├── logo.png
│   ├── banner.jpg
│   └── profile.png
│
├── css/
│   └── style.css
│
└── js/
    └── script.js
```

Keeping images in a separate **images** folder makes your project easier to understand and maintain.

If you're using Jekyll, you'll often see a structure like this:

```text
assets/
└── images/
    ├── html-part1-cover.jpg
    ├── html-part2-cover.jpg
    └── html-part3-cover.jpg
```

This is the structure you should use for your blog series.

---

# Choosing the Right Image Format

Not all image formats are the same.

Here's a simple guide:

| Format     | Best Used For                                 |
| ---------- | --------------------------------------------- |
| JPG / JPEG | Photos and blog covers                        |
| PNG        | Images with transparent backgrounds           |
| SVG        | Logos and icons                               |
| WebP       | Modern websites because of smaller file sizes |

If you're creating blog cover images, **JPG** or **WebP** are usually the best choices.

---

# Writing Better `alt` Text

Many beginners think the `alt` attribute isn't important.

In reality, it's one of the most useful parts of the `<img>` tag.

Instead of writing:

```html
alt="image"
```

Write something meaningful:

```html
alt="Student learning HTML on a laptop"
```

Good `alt` text helps:

* Visually impaired users using screen readers.
* Search engines understand your image.
* Visitors when the image fails to load.

Always describe what the image actually shows.

---

# Common Beginner Mistakes

### Mistake 1: Wrong File Name

```html
<img src="images/logo.png">
```

But the actual file is:

```
Logo.png
```

Some servers treat uppercase and lowercase letters differently.

`logo.png` and `Logo.png` are **not always the same file**.

---

### Mistake 2: Forgetting the Image Folder

Incorrect:

```html
<img src="logo.png">
```

Correct:

```html
<img src="images/logo.png">
```

---

### Mistake 3: Forgetting the `alt` Attribute

Incorrect:

```html
<img src="coding.jpg">
```

Better:

```html
<img src="coding.jpg" alt="Student writing HTML code">
```

---

### Mistake 4: Using Huge Images

Uploading a 10 MB image may slow down your webpage.

Before adding images, resize or compress them using an image optimization tool.

Smaller images load faster and improve user experience.

---

# Quick Practice

Create a webpage that contains:

* A heading saying **My Favorite Hobby**
* A picture related to your hobby
* A meaningful `alt` description
* An image width of **400 pixels**
* A short paragraph below the image explaining why you enjoy that hobby

Try completing this without looking back at the examples. Practice is the fastest way to remember HTML.

---

## What's Coming Next?

Great job! 🎉

You now know how to add images to your webpages and understand where they come from.

In the final part of this chapter, we'll learn:

* Image width and height
* Clickable images
* Figure and figcaption
* Mini project
* Practice questions
* Key takeaways
* Common interview questions for beginners

By the end of Part 3, you'll be able to confidently use images in any HTML project.
