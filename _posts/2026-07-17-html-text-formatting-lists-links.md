---

layout: post
title: "HTML Text Formatting, Lists and Links: Make Your Webpages Beautiful"
date: 2026-07-17
author: Chayank
categories: html
tags:
  - html
  - beginner
  - tutorial
  - web-development

  image: https://images.unsplash.com/photo-1498050108023-c5249f4df085
  excerpt: "Learn how to format text, create lists, and add links in HTML with simple explanations and real-world examples. Perfect for absolute beginners."

---

# HTML Text Formatting, Lists & Links: Make Your Webpages Beautiful

Welcome back! 👋

If you've completed **Part 1** of this series, congratulations! You've already learned what HTML is, how websites work behind the scenes, and how to create your very first webpage.

But let's be honest...

A webpage with only plain text isn't very exciting.

Imagine opening a news website where every word looks exactly the same. No bold headings, no clickable links, no bullet points, and no organized content. It would be confusing and difficult to read.

This is where HTML becomes much more interesting.

In this chapter, you'll learn how to make your webpages look organized, readable, and professional using some of the most commonly used HTML tags.

By the end of this tutorial, you'll know how to:

* Format text using bold, italic, and other useful tags.
* Create numbered and bullet lists.
* Add clickable links to websites and webpages.
* Build webpages that are easier for visitors to read.
* Avoid common beginner mistakes.

So, open your code editor, and let's continue your HTML journey!

---

# Why Text Formatting Is Important

Have you ever noticed that books, newspapers, and websites don't display all text in the same style?

That's because our brains naturally look for important information.

For example:

* Titles are usually larger.
* Important words are often **bold**.
* Some sentences are *italicized* for emphasis.
* Instructions are shown as bullet points.
* Sections are separated using lines.

Without formatting, every webpage would look like one long paragraph, making it difficult to understand.

HTML provides several tags that help us organize and emphasize our content.

Let's learn them one by one.

---

# Making Text Bold

Sometimes you want certain words to stand out.

For example:

> **Warning:** Do not share your password with anyone.

Notice how the word **Warning** immediately catches your attention?

HTML allows us to do this using the `<strong>` tag.

```html
<p><strong>Warning:</strong> Never share your password with anyone.</p>
```

### Output

**Warning:** Never share your password with anyone.

### Why Use `<strong>` Instead of `<b>`?

HTML actually provides two tags that make text appear bold:

```html
<b>Bold Text</b>

<strong>Important Text</strong>
```

Both look similar in the browser, but they don't mean the same thing.

The `<b>` tag only changes the appearance of the text.

The `<strong>` tag tells browsers, screen readers, and search engines that the text is important.

That's why professional developers usually prefer `<strong>`.

> **Best Practice:** Use `<strong>` whenever the text carries important meaning.

---

# Writing Text in Italics

Sometimes you don't want text to be bold—you simply want to emphasize it.

Imagine reading this sentence:

> I am *really* excited to learn HTML.

The word **really** stands out without being bold.

HTML provides the `<em>` tag for this purpose.

```html
<p>I am <em>really</em> excited to learn HTML.</p>
```

### Output

I am *really* excited to learn HTML.

Just like bold text, HTML also has another tag:

```html
<i>Italic Text</i>

<em>Emphasized Text</em>
```

The `<i>` tag changes only the appearance.

The `<em>` tag adds meaning by indicating emphasis.

Whenever you're writing content that should have emphasis—not just a different style—use `<em>`.

---

# Underlining Text

HTML also allows you to underline text.

```html
<p>This is <u>underlined text</u>.</p>
```

### Output

This is <u>underlined text</u>.

However, there's something important you should know.

On most websites, underlined text usually represents a clickable link.

If you underline ordinary text, visitors might think it's clickable when it isn't.

For this reason, modern websites rarely use the `<u>` tag unless there's a specific reason.

> **Pro Tip:** Avoid underlining normal text. Reserve underlines for links or special situations.

---

# Highlighting Important Information

Imagine you're studying from a textbook.

Whenever you find an important definition, you use a yellow highlighter.

HTML lets you do the same with the `<mark>` tag.

```html
<p>HTML is <mark>the foundation of every webpage</mark>.</p>
```

### Output

HTML is <mark>the foundation of every webpage</mark>.

This is useful for:

* Important notes
* Search results
* Key definitions
* Highlighting keywords

Try using it whenever you want readers to immediately notice something important.

---

# Making Text Smaller

Sometimes not every piece of information needs the same attention.

For example:

* Copyright notices
* Terms and conditions
* Footnotes
* Image credits

For these situations, HTML provides the `<small>` tag.

```html
<p>This is normal text.</p>

<p><small>This is smaller text.</small></p>
```

The browser automatically displays the second sentence in a slightly smaller size.

You'll often see this tag at the bottom of websites.

---

# Quick Recap

So far you've learned:

| Tag        | Purpose             |
| ---------- | ------------------- |
| `<strong>` | Important bold text |
| `<em>`     | Emphasized text     |
| `<u>`      | Underlined text     |
| `<mark>`   | Highlighted text    |
| `<small>`  | Smaller text        |

These tags may look simple, but you'll use them in almost every HTML project you build.
## Superscript and Subscript

Have you ever seen mathematical formulas like **x²** or chemical formulas like **H₂O**?

The small numbers above or below the text aren't typed normally—they're created using HTML tags.

### Superscript (`<sup>`)

The `<sup>` tag displays text slightly above the normal line.

```html
<p>x<sup>2</sup> + y<sup>2</sup> = z<sup>2</sup></p>
```

**Output:**

x² + y² = z²

You'll commonly use superscript for:

* Mathematical powers (x², x³)
* Ordinal numbers (1st, 2nd, 3rd)
* Footnote references

For example:

```html
<p>This is my 1<sup>st</sup> HTML project.</p>
```

---

### Subscript (`<sub>`)

The `<sub>` tag displays text slightly below the normal line.

```html
<p>H<sub>2</sub>O</p>
```

**Output:**

H₂O

Subscript is mainly used for:

* Chemical formulas
* Mathematical expressions
* Scientific notation

Another example:

```html
<p>CO<sub>2</sub> is carbon dioxide.</p>
```

---

> **Did You Know?**
>
> Without `<sup>` and `<sub>`, many scientific and mathematical expressions would be difficult to read correctly.

---

## Creating Line Breaks

When writing paragraphs, you might want to move some text onto the next line without starting a new paragraph.

That's where the `<br>` tag comes in.

```html
<p>
Hello!<br>
Welcome to my website.<br>
I am learning HTML.
</p>
```

**Output:**

Hello!
Welcome to my website.
I am learning HTML.

### When Should You Use `<br>`?

Good uses include:

* Writing poems
* Addresses
* Song lyrics
* Contact information

Example:

```html
<p>
John Doe<br>
123 Main Street<br>
New Delhi, India
</p>
```

### Don't Overuse `<br>`

Many beginners use several `<br>` tags just to create space.

```html
<p>Paragraph One</p>
<br><br><br>
<p>Paragraph Two</p>
```

This is **not** considered good practice.

Later, when you learn CSS, you'll discover much better ways to add spacing between elements.

---

## Horizontal Rules (`<hr>`)

Imagine you're reading a book.

When a new chapter begins, there's often a blank line or decorative separator.

HTML provides the `<hr>` tag to separate sections of a webpage.

```html
<hr>
```

The browser displays a horizontal line across the page.

### Example

```html
<h2>About Me</h2>

<p>
Hi! I'm learning web development.
</p>

<hr>

<h2>My Skills</h2>

<p>
HTML, CSS and JavaScript.
</p>
```

The horizontal line clearly separates the two sections.

---

## Combining Everything You've Learned

Let's create a simple webpage using the formatting tags we've covered so far.

```html
<!DOCTYPE html>
<html>

<head>
    <title>My First Formatted Page</title>
</head>

<body>

<h1>Welcome to My Website</h1>

<p>
My name is <strong>Alex</strong>.
</p>

<p>
I am <em>very excited</em> to learn web development.
</p>

<p>
Water is written as H<sub>2</sub>O.
</p>

<p>
The area of a square is x<sup>2</sup>.
</p>

<p>
<mark>Practice every day to improve your coding skills.</mark>
</p>

<hr>

<p>
Thank you for visiting!
</p>

</body>

</html>
```

Take a moment to type this code yourself instead of simply reading it.

Typing every example helps you remember HTML much faster.

---

## Mini Challenge

Now it's your turn!

Create a webpage that includes:

* Your name in a heading
* One sentence using `<strong>`
* One sentence using `<em>`
* One highlighted sentence using `<mark>`
* One example of superscript
* One example of subscript
* A horizontal line using `<hr>`
* Your address using `<br>`

Don't worry if you make mistakes—that's how every programmer learns.

---

## What You've Learned So Far

Congratulations! 🎉

You've now learned how to:

* Make important text bold using `<strong>`
* Emphasize text using `<em>`
* Underline text with `<u>`
* Highlight information using `<mark>`
* Display smaller text with `<small>`
* Write superscript using `<sup>`
* Write subscript using `<sub>`
* Move text to a new line using `<br>`
* Separate sections with `<hr>`

These formatting tags are used on almost every website you visit.

In the next section, we'll learn how to organize information using **HTML Lists**, one of the most useful features for creating clean and readable webpages.
