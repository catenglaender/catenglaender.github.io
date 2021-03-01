---
theme : "white"
transition: "slide"
highlightTheme: "monokai"
slideNumber: false
title: "ILIAS Content Styles"
---

# Content Styles

Creating designed elements to guide attention

for a better UX

---

Christoph Krahl

Linda Dierke

Ferdinand Engländer

#### UX Designers @ Concepts and Training GmbH

---

## Client feedback

about ILIAS

---

As content grows:

Overwhelming lists and navigations

---

User feels lost

---

## New approach

---

Let's use the page editor

---

and instead of building content pages

---

let's create home and overview pages

---

so admins can create custom simplified navigations

---

(image: menu of content cards with color overlay)

---

(image: accordeon)

---

Hghlighted sections and call to actions in content pages

---

(image: content cards offering different courses)

---

### Advantages

---

Important elements stand out clearly

---

Information overflow minimized

in favor of a drill down UX

---

### Realization

---

Content styles offer many possibilities beyond just changing a text color.

---

Navigation and overview pages

with carefully designed content elements

help users find their way.

---

## Content of this presentation

---

* Possibilities and limitations of content styles {.fragment .fade-in-then-semi-out}
* How to overcome these limitations with CSS {.fragment .fade-in-then-semi-out}
* Ideas to make content building easier for designers and users {.fragment .fade-in-then-semi-out}

---

## Possibilities & Limitations

---

### Practical example:

Course card with description text and call to action button

---

(image: the final result of the course card)

---

### Purpose:

Displaying a selection of courses of a sub-category {.fragment .fade-in-then-semi-out}

Recommending a course within a content body {.fragment .fade-in-then-semi-out}

---

Content styles are created through the admin interface

Layout and Navigation > Layout > Content Styles

---

On the side

Assembling our elements inside the page editor

---

### Card base

Block
* color
* margins

---

(image or live demonstration)

---

### Image

Media
* 100% width
* no margins

---

(image or live demonstration)

---

### The inner padding

Block
* padding

---

(image or live demonstration)

---

### The CTA button

Character
* text color
* background color

---

(image or live demonstration)

---

Done!

---

### Issues with this workflow

---

many, many clicks

---

long, confusing form

---

disjointed from the editor (on purpose)

---

no overview of how these elements come together

---

actually not that accessible - CSS knowledge required

---

designer: frustrated and limited by the form

user: intimidated, no WYSIWYG feedback

---

very hard to do anything beyond color or size changes

---

This is impossible with just the form:

---

(image: banner image in wall of text calling for an event registration)

---

## Overcoming the limitations with CSS

---

Styling the CSS instead of form parameters

---

### Step 1:

Creating the content styles without adding any settings

---

Name of the style appears in the editor dropdowns

---

### Step 2:

Setting the style with LESS/CSS code

---

Importing our content-styles.less in our skin

---

Compiling a delos.css that includes our additions

---

### Same visual result

---

designer: can style to his hearts content

user: can be offered a library of complex content styles

---

### Advantages of CSS approach

---

Settings of all elements at one glance

---

no clicking around and scrolling through a form

---

Use of less variables like @brand-primary

---

new possibilities like hover states for our "button"

---

### Issues with CSS approach

---

requires file access to the server and a custom skin setup

---

not closer to a WYSIWYG experience

---

offering a design toolbox

ended up in excessive nesting

---

Content cards build for Cate:

(image)

---

fancy additions:

* same height in every column
* spacing between content and CTA

---

All controlled by individual blocks

---

Inside page editor:

One block per setting

(image)

---

Code of the content cards:

One div per setting

(image)

---

This is how it's done in webdesign:

Fewer divs with multiple classes

(image)

---

## Who are content styles for?

---

Defined by admins / designers

use at your own risk is "ok"

---

Used in the page editor by users

should be self explanatory and fool proof

---

How do we enpower users

to create more complex layouts

on brand without confusion?

---

## A small suggestion

---

Allow choosing multiple style names

---

1. Create one block
2. Add from a selection of predefined content styles: color + padding + border + shadow

---

### Advantages

---

Avoids nesting chaos

---

less clicks inside page editor

---

User still only has a access to carefully selected on-brand options

---

## Outlook

CaT is looking into implementing this

adding to the core if it's deemed a worthy addition

---

## Vision beyond this

There are powerful page builders out there...

Wordpress: Elementor, Divi, Gutenberg

---

Get inspiration, but innovate on a small and practical level

---

Should contents styles and page editor grow closer together?

library of nested block templates?

---

Why?

Because ILIAS pages are not just a canvas for text

---

design options for pages enpower authors to

simplify navigation and create unique user journeys

---

Thank you :)

## Any questions?