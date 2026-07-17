---
layout: post
title: "HTML Text Formatting, Lists and Links: Make Your Webpages Beautiful"
date: 2026-07-17
author: Chayank
categories:
  - html
tags:
  - html
  - beginner
  - tutorial
  - web-development
image: "/assets/images/html-part2-cover.jpg"
excerpt: "Learn HTML text formatting, lists, and links with easy explanations, real-world examples, and hands-on practice. Perfect for absolute beginners."
---

Welcome back! 👋

First of all, congratulations!

If you've completed **Part 1**, you've already taken your very first step into web development. You learned what HTML is, how a browser understands HTML code, and how to create your first webpage.

That's a big achievement because every professional web developer started exactly where you are today.

Now it's time to make your webpages look much more organized and professional.

Imagine opening a website where everything looks exactly the same.

No bold headings.

No bullet points.

No clickable links.

No sections.

Just one giant paragraph.

Would you enjoy reading it?

Probably not.

Good websites aren't only about information—they're also about presenting that information in a way that's easy to read.

That's exactly what you'll learn in this chapter.

By the end of this tutorial, you'll know how to:

- Make important words stand out.
- Organize information using lists.
- Add clickable links.
- Create webpages that are easier to read.
- Write cleaner HTML like a beginner who is learning the right way.

So grab your favorite code editor, open the webpage you created in Part 1, and let's continue our HTML journey together.

---

# Why Text Formatting Matters

Let's start with a simple question.

Suppose your teacher gives you two pages of notes.

The first page looks like this:

Programming is fun programming is creative programming is useful programming is everywhere programming helps solve problems programming allows us to create websites applications games and much more.

Now imagine the second page.

It has headings.

Important words are bold.

Key points are highlighted.

Examples are neatly arranged.

Which page would you rather study?

The second one, of course.

That's exactly why text formatting exists.

HTML gives us several tags that help organize information so visitors can quickly understand what's important.

These tags don't just make your webpage look better—they also improve accessibility and help search engines understand your content.

Let's learn them one by one.

---

# Making Text Bold

Sometimes you want readers to notice a specific word immediately.

For example:

> **Warning:** Never share your password with anyone.

Your eyes instantly focus on the word **Warning**.

That's the power of bold text.

HTML provides two different tags that make text appear bold.

The first one is:

```html
<b>Bold Text</b>
```

The second one is:

```html
<strong>Important Text</strong>
```

### Browser Output

**Bold Text**

**Important Text**

At first glance, both look exactly the same.

So why does HTML have two different tags?

The answer is simple.

The `<b>` tag only changes the appearance of the text.

It tells the browser:

> "Make this text look bold."

The `<strong>` tag does something much more useful.

It tells browsers, search engines, and screen readers:

> "This text is important."

That's why professional developers almost always prefer `<strong>` instead of `<b>`.

### Real-Life Example

Imagine you're writing an article about online safety.

```html
<p><strong>Never share your OTP with anyone.</strong></p>
```

The browser displays:

**Never share your OTP with anyone.**

Even though it looks bold, it also carries meaning, making it a better choice than `<b>`.

> **Best Practice**
>
> Use `<strong>` whenever the text is important.
>
> Reserve `<b>` for situations where you only want visual boldness.

---

# Writing Text in Italics

Now let's say you don't want to make a word bold.

You simply want to emphasize it.

For example:

> I am *really* excited to learn HTML.

The word **really** stands out without shouting at the reader.

HTML provides two tags here as well.

```html
<i>Italic Text</i>
```

and

```html
<em>Emphasized Text</em>
```

### Browser Output

*Italic Text*

*Emphasized Text*

Again, they look almost identical.

But just like `<strong>` and `<b>`, they don't mean the same thing.

`<i>` simply changes the appearance.

`<em>` tells browsers that the word has emphasis.

That's why professional developers usually choose `<em>`.

### Example

```html
<p>I am <em>really</em> enjoying HTML.</p>
```

Browser Output:

I am *really* enjoying HTML.

Notice how the sentence feels more natural.

You're guiding the reader's attention instead of simply decorating the text.

---

# Underlining Text

HTML also provides the `<u>` tag.

```html
<p>This is <u>underlined</u> text.</p>
```

### Browser Output

This is <u>underlined</u> text.

Looks nice, right?

Well... not always.

On modern websites, underlined text usually means **"Click me!"**

If you underline ordinary text, visitors may think it's a hyperlink.

That's why experienced developers rarely use `<u>` unless there's a specific reason.

> **Pro Tip**
>
> If you want something to look important, use `<strong>` or `<mark>` instead of underlining it.

---

# Highlighting Important Information

Think about studying for an exam.

Whenever you find an important definition, what do you do?

Most students grab a yellow highlighter.

HTML has its own digital highlighter called `<mark>`.

```html
<p>HTML is <mark>the foundation of every webpage</mark>.</p>
```

### Browser Output

HTML is <mark>the foundation of every webpage</mark>.

This tag is perfect for:

- Important notes
- Search results
- Definitions
- Keywords
- Exam revision content

It immediately draws the reader's attention to the highlighted text.

---

# Small Text

Not everything on a webpage needs equal importance.

Sometimes you need text that's still readable but less noticeable.

Examples include:

- Copyright notices
- Image credits
- Terms and conditions
- Footnotes

HTML provides the `<small>` tag for these situations.

```html
<p>This is normal text.</p>

<p><small>This is smaller text.</small></p>
```

### Browser Output

This is normal text.

<small>This is smaller text.</small>

You'll see this tag on almost every professional website, especially near the footer.
