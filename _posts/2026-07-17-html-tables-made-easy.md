---
layout: post
title: "HTML Tables Made Easy: Create Professional Tables Step by Step"
date: 2026-07-17
author: Chayank

categories:
  - html

tags:
  - html
  - beginner
  - html-tables
  - web-development
  - coding

image: https://plus.unsplash.com/premium_photo-1661877737564-3dfd7282efcb?q=80&w=900&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D

excerpt: "Learn HTML tables from scratch with simple explanations, real-life examples, and hands-on practice."
---
# HTML Tables Made Easy: Create Professional Tables Step by Step

Welcome back! 👋

If you've been following this HTML series from the beginning, you've already come a long way.

In **Part 1**, you learned the fundamentals of HTML and built your first webpage.

In **Part 2**, you discovered how to make your webpages easier to read using text formatting, lists, and links.

In **Part 3**, you learned how to add beautiful images and understood the difference between relative and absolute file paths.

Now it's time to learn something you'll see almost everywhere on the internet—**HTML Tables**.

At first, tables might sound boring, but they're actually one of the easiest and most useful HTML elements to learn.

Think about the websites you visit every day.

A shopping website displays product prices.

A school's website shows examination results.

A cricket website displays scorecards.

A railway website lists train schedules.

A college website publishes timetables.

What do all of these have in common?

They organize information into **rows and columns**.

That's exactly what HTML tables are designed to do.

By the end of this chapter, you'll be able to create professional-looking tables for your own websites and understand when—and when not—to use them.

Let's get started!

---

# What Is an HTML Table?

An HTML table is used to display information in a structured format.

Instead of writing everything as paragraphs, we arrange the data into rows and columns, making it much easier to read.

Here's a simple example.

| Name    | Age | City    |
| ------- | --: | ------- |
| Chayank |  18 | Jodhpur |
| Rahul   |  19 | Jaipur  |
| Priya   |  18 | Delhi   |

Even without any explanation, it's easy to understand who is from which city and how old they are.

That's the power of tables.

---

# Where Are HTML Tables Used?

You might be surprised to know how often tables appear on websites.

Some common examples include:

* School and college timetables
* Examination results
* Product comparison tables
* Price lists
* Cricket and football scorecards
* Employee records
* Flight and train schedules
* Restaurant menus
* Monthly budgets

Whenever information is arranged neatly into rows and columns, chances are you're looking at a table.

---

# Understanding the Structure of a Table

Before writing any code, let's understand how a table is organized.

Imagine a notebook.

It has horizontal rows and vertical columns.

Each box where a row and column meet is called a **cell**.

HTML tables work exactly the same way.

Every table contains:

* One table
* Multiple rows
* Multiple cells inside each row

Once you understand this idea, creating tables becomes much easier.

---

# The `<table>` Tag

Every HTML table begins with the `<table>` tag.

Think of it as a container that holds everything related to the table.

```html
<table>

</table>
```

Without this tag, the browser doesn't know you're trying to create a table.

---

# The `<tr>` Tag (Table Row)

Inside the table, we create rows using the `<tr>` tag.

The letters **tr** stand for **Table Row**.

Example:

```html
<table>
    <tr>

    </tr>
</table>
```

This creates one empty row.

Want another row?

Simply add another `<tr>`.

```html
<table>

    <tr>

    </tr>

    <tr>

    </tr>

</table>
```

Now your table has two rows.

Think of `<tr>` as drawing one horizontal line in your table.

---

# The `<td>` Tag (Table Data)

Rows alone don't display any information.

Each row needs cells.

That's where the `<td>` tag comes in.

The letters **td** stand for **Table Data**.

Let's place some information inside a row.

```html
<table>

<tr>

<td>Chayank</td>

<td>18</td>

<td>Jodhpur</td>

</tr>

</table>
```

### Browser Output

| Chayank | 18 | Jodhpur |

Congratulations!

You've just created your first HTML table.

Although it looks very simple right now, you've already learned the three most important tags used in tables:

* `<table>`
* `<tr>`
* `<td>`

Almost every HTML table is built using these tags.

---

# Adding More Rows

Let's make our table slightly bigger.

```html
<table>

<tr>
<td>Chayank</td>
<td>18</td>
<td>Jodhpur</td>
</tr>

<tr>
<td>Rahul</td>
<td>19</td>
<td>Jaipur</td>
</tr>

<tr>
<td>Priya</td>
<td>18</td>
<td>Delhi</td>
</tr>

</table>
```

### Browser Output

| Chayank | 18 | Jodhpur |
| Rahul | 19 | Jaipur |
| Priya | 18 | Delhi |

Notice something?

The browser understands that every `<tr>` is a new row, while every `<td>` becomes a new column.

---

# The Problem with Our Table

Our table works...

But it doesn't look very professional.

Can you immediately tell which column contains names?

Which one shows ages?

Which one shows cities?

Not really.

That's because we haven't added **headings** yet.

Imagine reading a newspaper where none of the columns have titles.

It would be confusing.

To solve this problem, HTML provides another important tag.

---

# The `<th>` Tag (Table Header)

The `<th>` tag is used to create headings for a table.

The letters **th** stand for **Table Header**.

Instead of writing:

```html
<td>Name</td>
```

We write:

```html
<th>Name</th>
```

Let's improve our table.

```html
<table>

<tr>
<th>Name</th>
<th>Age</th>
<th>City</th>
</tr>

<tr>
<td>Chayank</td>
<td>18</td>
<td>Jodhpur</td>
</tr>

<tr>
<td>Rahul</td>
<td>19</td>
<td>Jaipur</td>
</tr>

<tr>
<td>Priya</td>
<td>18</td>
<td>Delhi</td>
</tr>

</table>
```

### Browser Output

| **Name** | **Age** | **City** |
| -------- | ------: | -------- |
| Chayank  |      18 | Jodhpur  |
| Rahul    |      19 | Jaipur   |
| Priya    |      18 | Delhi    |

Now the table is much easier to understand.

The browser automatically makes header cells **bold** and centers them, helping readers quickly identify each column.

---

# Understanding the Four Essential Table Tags

Before moving ahead, let's quickly revise the tags you've learned.

| Tag       | Purpose                              |
| --------- | ------------------------------------ |
| `<table>` | Creates the entire table             |
| `<tr>`    | Creates a table row                  |
| `<th>`    | Creates a table heading              |
| `<td>`    | Creates a table cell containing data |

These four tags are the foundation of every HTML table.

Once you're comfortable with them, creating more advanced tables becomes much easier.

---

# Mini Challenge

Before reading further, try creating a table on your own.

Your table should contain:

* Name
* Favorite Subject
* Favorite Sport

Add information for at least **three students**.

Don't worry if you make mistakes.

Every experienced web developer learned HTML by practicing, experimenting, and fixing errors.

Take five minutes to build the table yourself before continuing to the next section.

You'll be surprised how much confidence you'll gain by writing the code on your own.

---

## What's Coming Next?

Great job! 🎉

You've learned the basic structure of HTML tables and created your first table using `<table>`, `<tr>`, `<th>`, and `<td>`.

In **Part 4B**, we'll make our tables look even better by learning:

* Table borders
* `border`, `cellpadding`, and `cellspacing`
* `colspan`
* `rowspan`
* Common beginner mistakes
* A real-world timetable project

By the end of the next section, you'll be able to build tables that look organized and professional.
# Making Tables Look Better

So far, our tables work perfectly.

The browser understands our rows, columns, and data.

But there's one small problem...

They don't look very attractive.

If you run the previous examples in your browser, you'll notice that the table doesn't have visible borders. Everything looks like plain text.

Let's fix that.

---

# Adding Borders to a Table

The easiest way to make a table easier to read is by adding borders.

In older HTML tutorials, you'll often see this:

```html
<table border="1">

<tr>
<th>Name</th>
<th>Age</th>
<th>City</th>
</tr>

<tr>
<td>Chayank</td>
<td>18</td>
<td>Jodhpur</td>
</tr>

<tr>
<td>Rahul</td>
<td>19</td>
<td>Jaipur</td>
</tr>

</table>
```

### Browser Output

| Name    | Age | City    |
| ------- | --: | ------- |
| Chayank |  18 | Jodhpur |
| Rahul   |  19 | Jaipur  |

Now every cell is separated with borders, making the table much easier to understand.

> **Good to Know**
>
> Modern websites usually use **CSS** to create beautiful table borders instead of the `border` attribute.
>
> Since you haven't learned CSS yet, using `border="1"` is perfectly fine for practice.

---

# Understanding Cell Padding

Imagine sitting in a classroom where every desk is so small that your notebook barely fits.

It would feel uncomfortable.

Table cells work the same way.

Without extra space, the content touches the borders and looks crowded.

Older HTML allowed spacing using the `cellpadding` attribute.

```html
<table border="1" cellpadding="10">

<tr>
<th>Name</th>
<th>Age</th>
</tr>

<tr>
<td>Chayank</td>
<td>18</td>
</tr>

</table>
```

The number **10** means the browser leaves extra space around the text inside each cell.

This makes tables much easier to read.

---

# Understanding Cell Spacing

Now imagine moving every classroom desk slightly away from each other.

That's exactly what **cell spacing** does.

```html
<table border="1" cellspacing="8">
```

Instead of increasing the space **inside** cells, it increases the space **between** cells.

Again, modern websites use CSS for this, but it's useful to understand these older attributes because you'll still find them in many tutorials.

---

# Merging Columns with `colspan`

Sometimes one heading needs to cover multiple columns.

For example, imagine creating a school report card.

Instead of writing separate headings for every subject, you might want one heading called **Marks** that covers three subjects.

HTML allows this using the `colspan` attribute.

```html
<table border="1">

<tr>
<th>Name</th>
<th colspan="3">Marks</th>
</tr>

<tr>
<th></th>
<th>Math</th>
<th>Science</th>
<th>English</th>
</tr>

<tr>
<td>Chayank</td>
<td>92</td>
<td>88</td>
<td>95</td>
</tr>

</table>
```

### Browser Output

| Name    | Marks |         |         |
| ------- | ----- | ------- | ------- |
|         | Math  | Science | English |
| Chayank | 92    | 88      | 95      |

Notice how **Marks** stretches across three columns.

That's exactly what `colspan="3"` means.

---

# Merging Rows with `rowspan`

Just like columns can be merged, rows can also be combined.

Suppose you're creating a weekly timetable.

Monday has two classes taught by the same teacher.

Instead of repeating the teacher's name twice, you can merge the rows.

```html
<table border="1">

<tr>
<th>Teacher</th>
<th>Subject</th>
</tr>

<tr>
<td rowspan="2">Mr. Sharma</td>
<td>Mathematics</td>
</tr>

<tr>
<td>Physics</td>
</tr>

</table>
```

### Browser Output

| Teacher    | Subject     |
| ---------- | ----------- |
| Mr. Sharma | Mathematics |
|            | Physics     |

The teacher's name appears once while covering two rows.

That's the job of `rowspan`.

---

# When Should You Use `colspan` and `rowspan`?

These attributes are useful when creating:

* School report cards
* Examination results
* Cricket scoreboards
* Tournament brackets
* Timetables
* Product comparison tables

Whenever one heading or one piece of information belongs to multiple rows or columns, these attributes become very helpful.

---

# Common Beginner Mistakes

### 1. Forgetting to Close Tags

Incorrect:

```html
<table>
<tr>
<td>Name
<td>Age
```

Correct:

```html
<table>
<tr>
<td>Name</td>
<td>Age</td>
</tr>
</table>
```

Always close every tag properly.

---

### 2. Different Numbers of Cells

Incorrect:

```html
<tr>
<td>Chayank</td>
<td>18</td>
</tr>

<tr>
<td>Rahul</td>
<td>19</td>
<td>Jaipur</td>
</tr>
```

One row has **2 cells**, while the next has **3 cells**.

This can make the table look broken or confusing.

Try to keep every row consistent unless you're intentionally using `colspan` or `rowspan`.

---

### 3. Using Tables for Page Layout

Years ago, developers used tables to design entire webpages.

Today, that's considered bad practice.

Tables should be used **only for displaying tabular data**, not for arranging the layout of a website.

When you learn CSS, you'll discover much better tools for page layouts.

---

# Mini Project – Student Report Card

Let's put everything together.

Create a report card like this:

| Name    | Math | Science | English | Total |
| ------- | ---: | ------: | ------: | ----: |
| Chayank |   92 |      88 |      95 |   275 |
| Rahul   |   84 |      91 |      80 |   255 |
| Priya   |   95 |      94 |      97 |   286 |

Try to:

* Add table headings using `<th>`.
* Add borders.
* Use at least three rows of data.
* Calculate the total marks yourself.

This small project will help you remember table tags much better than simply reading about them.

---

## Great Progress!

Congratulations! 🎉

You've now learned:

* How to add borders to tables.
* The purpose of `cellpadding`.
* The purpose of `cellspacing`.
* How to merge columns using `colspan`.
* How to merge rows using `rowspan`.
* Common mistakes beginners should avoid.

In **Part 4C**, we'll build a complete real-world timetable project, practice everything you've learned, and finish the chapter with interview questions, practice exercises, key takeaways, and a preview of the next topic—**HTML Forms**.
# Real-World Project – Build a School Timetable

Congratulations! 🎉

You've learned all the important HTML table tags.

Now it's time to use them in a real project.

Instead of learning another new tag, let's build something that you'll actually see on many school and college websites—a **weekly timetable**.

Projects like this help you understand how different HTML tags work together.

---

## The Final Code

Type the following code into your editor instead of copying and pasting it. Writing the code yourself is one of the fastest ways to remember HTML.

```html
<!DOCTYPE html>
<html>

<head>
    <title>School Timetable</title>
</head>

<body>

<h1>Class 11 Timetable</h1>

<table border="1" cellpadding="10">

<tr>
<th>Day</th>
<th>9:00 - 10:00</th>
<th>10:00 - 11:00</th>
<th>11:00 - 12:00</th>
<th>12:00 - 1:00</th>
</tr>

<tr>
<td>Monday</td>
<td>Mathematics</td>
<td>Physics</td>
<td>Chemistry</td>
<td>English</td>
</tr>

<tr>
<td>Tuesday</td>
<td>Chemistry</td>
<td>Mathematics</td>
<td>Computer Science</td>
<td>English</td>
</tr>

<tr>
<td>Wednesday</td>
<td>Physics</td>
<td>Computer Science</td>
<td>Mathematics</td>
<td>Sports</td>
</tr>

<tr>
<td>Thursday</td>
<td>English</td>
<td>Chemistry</td>
<td>Physics</td>
<td>Mathematics</td>
</tr>

<tr>
<td>Friday</td>
<td>Computer Science</td>
<td>Physics</td>
<td>English</td>
<td>Chemistry</td>
</tr>

</table>

</body>

</html>
```

### Browser Output

Your browser will display a neat timetable with days in the first column and subjects arranged across different time slots.

Even though the table is simple, it already resembles the kind of timetable you might see on a school's website.

---

# Challenge Yourself 🚀

Now it's your turn.

Try improving the timetable by:

* Adding one more day.
* Adding a Lunch Break column.
* Using `colspan` to merge the lunch break across multiple periods.
* Adding your own favorite subjects.
* Creating a timetable for your own weekly study schedule.

The more you experiment, the faster you'll become comfortable with HTML.

---

# Practice Questions

Don't skip this section.

Reading helps you understand HTML, but practice helps you remember it.

### Beginner

1. Which tag creates a table?
2. Which tag creates a row?
3. Which tag creates a table heading?
4. Which tag creates a table cell?
5. What is the difference between `<th>` and `<td>`?

---

### Intermediate

6. What does `colspan` do?
7. What does `rowspan` do?
8. Why should tables not be used for webpage layouts?
9. What is the purpose of `cellpadding`?
10. What is the difference between `cellpadding` and `cellspacing`?

Try answering these questions without looking back at the tutorial.

If you can answer most of them, you've understood the topic well.

---

# Common Interview Questions

If you're preparing for internships or beginner web development interviews, you might come across questions like these:

### What is an HTML table?

An HTML table is used to organize information into rows and columns.

---

### What are the four basic table tags?

* `<table>`
* `<tr>`
* `<th>`
* `<td>`

---

### What is the difference between `<th>` and `<td>`?

`<th>` creates header cells, while `<td>` contains normal data.

Header cells are usually bold and centered by default.

---

### What is `colspan`?

It allows one cell to span across multiple columns.

---

### What is `rowspan`?

It allows one cell to span across multiple rows.

---

# Quick Recap

Let's quickly revise everything you've learned in this chapter.

| Tag           | Purpose                    |
| ------------- | -------------------------- |
| `<table>`     | Creates the table          |
| `<tr>`        | Creates a row              |
| `<th>`        | Creates a heading cell     |
| `<td>`        | Creates a normal data cell |
| `border`      | Displays table borders     |
| `cellpadding` | Adds space inside cells    |
| `cellspacing` | Adds space between cells   |
| `colspan`     | Merges multiple columns    |
| `rowspan`     | Merges multiple rows       |

If these tags make sense to you now, you've mastered the basics of HTML tables.

---

# Key Takeaways

Before moving on, remember these important points:

* Tables are used to display **tabular data**, not to design webpage layouts.
* Every table begins with the `<table>` tag.
* Rows are created using `<tr>`.
* Headings are created using `<th>`.
* Data is placed inside `<td>`.
* `colspan` merges columns.
* `rowspan` merges rows.
* Practice by creating different types of tables, such as timetables, report cards, price lists, and scoreboards.

The more tables you build, the more confident you'll become.

---

# What's Next?

Fantastic work! 🎉

You've completed another important milestone in your HTML journey.

So far you've learned:

* HTML Basics
* Text Formatting
* Lists
* Links
* Images
* File Paths
* Tables

Your webpages are now starting to look like real websites.

But there's still one thing missing.

Right now, visitors can only **read** your webpages.

What if you wanted them to interact with your website?

For example:

* Enter their name.
* Type an email address.
* Create a password.
* Select their favorite programming language.
* Submit feedback.
* Register for an event.

That's exactly what **HTML Forms** are used for.

In **Part 5**, you'll learn how to create interactive forms from scratch and build your very first registration form.

Trust me—this is one of the most exciting parts of HTML because it's the first step toward building websites that users can actually interact with.

See you in the next chapter, and happy coding! 🚀
