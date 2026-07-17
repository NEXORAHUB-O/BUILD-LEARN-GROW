---

layout: post
title: "HTML Part 2: Text Formatting, Lists & Links – Build Better Webpages"
date: 2026-07-17
author: Chayank
categories: html
tags:

* html
* beginner
* tutorial
* web-development
* coding
  image: https://images.unsplash.com/photo-1516321318423-f06f85e504b3
  excerpt: "Learn how to format text, create lists, and add links in HTML. This beginner-friendly guide explains everything with simple examples and hands-on practice."

---

# HTML Part 2: Text Formatting, Lists & Links

Welcome back! 👋

If you've completed **Part 1**, congratulations—you've already taken your first step into web development. You learned what HTML is, how a webpage is structured, and created your very first webpage.

Now it's time to make your webpage more useful and professional.

Imagine reading a webpage where every sentence looks exactly the same—no bold text, no headings, no links, no organized lists. It would be boring and difficult to read.

In this chapter, you'll learn how to:

* Make important text stand out
* Organize information with lists
* Connect pages using links
* Build webpages that are easy to read

Let's begin!

---

# Why Text Formatting Matters

Think about your favorite website.

Do they make important words **bold**?

Do they *highlight* certain terms?

Do they use organized bullet points?

Of course they do!

Formatting helps visitors quickly understand what's important.

HTML gives us special tags for this purpose.

---

# Bold Text

To make text bold, use the `<b>` tag.

```html
<p>This is <b>bold</b> text.</p>
```

Output:

This is **bold** text.

### Better Option: `<strong>`

Instead of `<b>`, professionals often use `<strong>`.

```html
<p>This is <strong>very important</strong>.</p>
```

Why?

Because `<strong>` tells browsers and search engines that the text is important, not just bold.

**Tip:** Use `<strong>` whenever the text is important.

---

# Italic Text

Use the `<i>` tag.

```html
<p>I am learning <i>HTML</i>.</p>
```

Output:

I am learning *HTML*.

### Better Option: `<em>`

```html
<p>I am <em>really excited</em> to learn HTML.</p>
```

`<em>` means emphasis and is preferred over `<i>` in most situations.

---

# Underlined Text

```html
<p>This is <u>underlined</u>.</p>
```

Although it works, avoid underlining normal text because users usually think underlined text is a link.

---

# Highlight Text

Want to highlight something like a marker?

Use:

```html
<p>HTML is <mark>very easy</mark> to learn.</p>
```

Output:

HTML is <mark>very easy</mark> to learn.

This is useful for important notes.

---

# Small Text

```html
<p>This is normal text.</p>
<p><small>This is smaller text.</small></p>
```

You'll often see this in footnotes or copyright sections.

---

# Superscript & Subscript

### Superscript

```html
<p>x<sup>2</sup></p>
```

Output:

x²

### Subscript

```html
<p>H<sub>2</sub>O</p>
```

Output:

H₂O

Very useful in mathematics and chemistry.

---

# Horizontal Line

Need to separate two sections?

Use:

```html
<hr>
```

This creates a horizontal line across the page.

---

# Line Break

Normally HTML ignores extra Enter presses.

To move to the next line without starting a new paragraph:

```html
<br>
```

Example:

```html
Hello<br>
Welcome<br>
to HTML.
```

---

# Lists in HTML

Lists make information clean and easy to understand.

There are three types of lists.

## 1. Unordered List

Used when order doesn't matter.

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

Output:

* HTML
* CSS
* JavaScript

---

## 2. Ordered List

Used when order matters.

```html
<ol>
    <li>Wake up</li>
    <li>Study HTML</li>
    <li>Practice</li>
</ol>
```

Output:

1. Wake up
2. Study HTML
3. Practice

---

## 3. Description List

Perfect for definitions.

```html
<dl>
    <dt>HTML</dt>
    <dd>Language used to create webpages.</dd>

    <dt>CSS</dt>
    <dd>Used to style webpages.</dd>
</dl>
```

---

# Hyperlinks

Links are one of the most important features of the web.

Without links, websites couldn't connect to each other.

The anchor tag is:

```html
<a></a>
```

---

## Basic Link

```html
<a href="https://google.com">Visit Google</a>
```

When clicked, it opens Google.

---

## Open in New Tab

```html
<a href="https://google.com" target="_blank">
Visit Google
</a>
```

`target="_blank"` opens the link in a new tab.

---

## Link to Another Page

Suppose your project looks like this:

```
project/

index.html

about.html

contact.html
```

To open the About page:

```html
<a href="about.html">About Us</a>
```

Simple!

---

## Email Link

```html
<a href="mailto:example@email.com">
Send Email
</a>
```

Clicking this opens the user's email application.

---

## Telephone Link

```html
<a href="tel:+911234567890">
Call Us
</a>
```

Very useful on mobile websites.

---

# Combining Everything

Let's create a small webpage.

```html
<!DOCTYPE html>
<html>

<head>
    <title>My Learning Page</title>
</head>

<body>

<h1>Learning HTML</h1>

<p>
Welcome to my first website.
I am learning <strong>HTML</strong>.
</p>

<hr>

<h2>Things I Will Learn</h2>

<ul>
<li>HTML</li>
<li>CSS</li>
<li>JavaScript</li>
</ul>

<h2>Useful Link</h2>

<a href="https://developer.mozilla.org" target="_blank">
Learn More About HTML
</a>

</body>

</html>
```

This small webpage already looks much better than a plain page!

---

# Common Beginner Mistakes

❌ Forgetting to close tags.

```html
<p>Hello
```

✅ Correct

```html
<p>Hello</p>
```

---

❌ Writing the URL outside `href`.

```html
<a>google.com</a>
```

✅ Correct

```html
<a href="https://google.com">
Google
</a>
```

---

❌ Mixing ordered and unordered lists accidentally.

Always decide whether the order matters before choosing `<ol>` or `<ul>`.

---

# Mini Challenge

Create a webpage that contains:

* Your name as a heading
* A short paragraph about yourself
* Three hobbies using an unordered list
* Three goals using an ordered list
* A link to your favorite website
* One important sentence using `<strong>`
* One emphasized sentence using `<em>`
* A horizontal line using `<hr>`

Try it yourself before checking the answer.

---

# Key Takeaways

✔ Use `<strong>` for important text.

✔ Use `<em>` for emphasis.

✔ Use `<ul>` for bullet lists.

✔ Use `<ol>` for numbered lists.

✔ Use `<a>` to create hyperlinks.

✔ Use `<hr>` to separate sections.

✔ Use `<br>` for a line break.

---

# Practice Questions

### Easy

1. Which tag is used to create hyperlinks?
2. What is the difference between `<strong>` and `<b>`?
3. Which tag creates a numbered list?
4. Which tag creates bullet points?
5. What does `target="_blank"` do?

### Intermediate

1. Create a webpage with your top five favorite movies.
2. Make each movie name a clickable link to its Wikipedia page.
3. Add a heading and separate sections using `<hr>`.

---

# What's Next?

In **Part 3**, we'll learn about:

* Adding images to webpages
* Understanding file paths
* Absolute vs Relative paths
* Organizing project folders
* Creating a simple portfolio webpage with images

You're getting closer to building real websites. Keep practicing—even 20 minutes a day can make a huge difference!

Happy coding! 🚀
