---
theme : "white"
transition: "slide"
highlightTheme: "monokai"
slideNumber: false
title: "ILIAS Content Styles"
customTheme: "additionalstyles"
---

# Content Styles

Creating designed elements to guide attention

for a better UX

---

#### UX Designers @ Concepts and Training GmbH

Christoph Krahl

Linda Dierke

Ferdinand Engländer

---

Concepts and Training = CaT

offers ILIAS-based training management solutions for businesses (insurances, car dealers)

---

ILIAS with our extensions, modifications and skins = Cate

---

## Client feedback

---

As content grows:

---

Navigation, lists, breadcrumbs and dashboards get overwhelming

---

Users miss important information on full content pages

---

User feels lost

---

## The challenge

---

We need to guide the user through many categories and long content pages

---

**reduce and filter:**

hand-pick what is displayed at once

---

**prioritize and lead attention:**

what is most important?

---

maximize overview

---

public pages need to look on brand

---

## General solutions for better UX

Good structure

---

level 2 offers irrelevant options

![](imgs/structure_bad.svg)

---

level 2 invites discovery

![](imgs/structure_better.svg)

---

## Design teams perspective

on ILIAS / Cate

---

What you would expect:

Skin design

---

<!-- .slide: data-background="imgs/ilias_start.png" -->

---

<!-- .slide: data-background="imgs/cate_tms.png" -->

---

<!-- .slide: data-background="imgs/cate_bright.png" -->

---

<!-- .slide: data-background="imgs/cate_green.png" -->

---

A bit more adventerous:

Tools for designing content

---

<video controls muted autoplay>
    <source data-src="vids/cate_learning-module.mp4" type="video/mp4" />
</video>

---

### Content styles

usually used for small visual changes of page editor elements

---

<video controls muted autoplay>
    <source data-src="vids/standard-content-style.mp4" type="video/mp4" />
</video>

---

text, border, background color

---

Complex magazine layouts are possible with column layout

---

So...

Let's use the page editor & content styles

---

and create a toolbox {.fragment .fade-in-then-semi-out}

* for guiding attention on pages {.fragment .fade-in-then-semi-out}
* for creating home and overview pages {.fragment .fade-in-then-semi-out}

---

goal: help users find their way to the important content

---

Examples in Cate:

---

<video controls muted autoplay>
    <source data-src="vids/cate_4-image-tiles-menu.mp4" type="video/mp4" />
</video>

---

<video controls muted autoplay>
    <source data-src="vids/cate_banner-and-accordion.mp4" type="video/mp4" />
</video>

---

Content styles offer many possibilities beyond just changing a text color.

---

## Let's dive in

---

### Building a course card:

Card with an image, description text and call to action button

---

![](imgs/ilias_content-card-example.png)

---

* Possibilities and limitations of content styles {.fragment .fade-in-then-semi-out}
* How to overcome these limitations with CSS {.fragment .fade-in-then-semi-out}
* Ideas to make content building easier for designers and users {.fragment .fade-in-then-semi-out}

---

![](imgs/ilias_content-card-example.png)

---

Not to be confused with

list objects as item cards:

---

![](imgs/ilias_card-repo.png)

---

### Purpose:

Displaying a selection of courses of a sub-category {.fragment .fade-in-then-semi-out}

Recommending a course within a content body {.fragment .fade-in-then-semi-out}

---

### Step by step demonstration

1. so you can build it yourself {.fragment .fade-in-then-semi-out}

2. so you experience the issues {.fragment .fade-in-then-semi-out}

---

Content styles are created through the admin interface

Layout and Navigation > Layout > Content Styles

---

<video controls muted autoplay>
    <source data-src="vids/path-to-content-styles.mp4" type="video/mp4" />
</video>

---

### Card base

Block
* color
* margins

---

<video controls muted autoplay>
    <source data-src="vids/card-content-style-form_base.mp4" type="video/mp4" />
</video>

---

On the side

Assembling our elements inside the page editor

---

<video controls muted autoplay>
    <source data-src="vids/card-content-style-form_start-page.mp4" type="video/mp4" />
</video>

---

Adding images

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_adding-images.mp4" type="video/mp4" />
</video>

---

![](imgs/ilias_content-card-example.png)

---

### Image

Media
* 100% width
* no margins

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_image-full-width.mp4" type="video/mp4" />
</video>

---

Adding a headline

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_adding-headline.mp4" type="video/mp4" />
</video>

---

![](imgs/ilias_content-card-example.png)

---

### The inner padding

Block
* padding

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_padding.mp4" type="video/mp4" />
</video>

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_padding-page-editor.mp4" type="video/mp4" />
</video>

---

### The CTA button

Character
* text color
* margin
* background color

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_ButtonStyle.mp4" type="video/mp4" />
</video>

---

Adding the button

---

<video controls muted autoplay>
    <source data-src="vids/card-content-form_complete-button.mp4" type="video/mp4" />
</video>

---

Done!

![](imgs/ilias_content-card-example.png)

---

### Limitations & issues

---

many, many clicks

---

long, overwhelming form

---

difficult to change all colors and fonts at once

---

disjointed from the editor (on purpose)

---

no quick preview of how these elements come together

---

actually not that accessible - CSS knowledge required

---

Impossible with just the form:

* certain hover states
* :before and :after elements
* conditional changes (change text if it is inside certain blocks)

---

designer (power user): frustrated and limited by the form

user (beginner): intimidated to add styles, only a few simple default options

---

very hard to do anything beyond small changes

---

## Overcoming the limitations with CSS

---

What is actually happening in the background?

---

Form parameters are translated into CSS

---

So let's write that CSS directly

---

= we can add anything we want through the skin CSS

---

1. Creating the content styles without adding any settings

---

<video controls muted autoplay>
    <source data-src="vids/CSS_create-content-styles-name.mp4" type="video/mp4" />
</video>

---

Style names can be used in the editor

---

<video controls muted autoplay>
    <source data-src="vids/CSS_structure-no-styling-yet.mp4" type="video/mp4" />
</video>

---

2. Using the Chrome Inspector for Styling

---

<video controls muted autoplay>
    <source data-src="vids/CSS_chrome-inspector.mp4" type="video/mp4" />
</video>

---

3. Save the LESS/CSS code

---

CSS

```CSS
.ilc_section_ContentCardBase {
    background-color: #e9f8fd;
}

.ilc_section_ContentCardPadding {
    padding: 10px;
}

.ilc_text_inline_ContentCardButtonPrimary {
    background-color: #e69e1a;
    color: white;
    padding: 10px;
    border-radius: 5px;
}

.ilc_section_ContentCardBase figure.ilc_media_cont_MediaContainer {
    margin: 0;
    width: 100%;
}
```

---

LESS

preprocessor language to generate CSS

```LESS
.ilc_section_ContentCardBase {
    background-color: mix(#FFF,@brand-primary,50%);

    figure.ilc_media_cont_MediaContainer {
        margin: 0;
        width: 100%;
    }
}

.ilc_section_ContentCardPadding {
    padding: 10px;
}

.ilc_text_inline_ContentCardButtonPrimary {
    background-color: @brand-secondary;
    color: white;
    padding: 10px;
    border-radius: 5px;
}
```

---

Importing our custom-content-styles.less in our skin

```LESS
@import "less/custom-content-styles.less";
```

---

[Official guide](https://docu.ilias.de/ilias.php?ref_id=367&obj_id=75028&cmd=layout&cmdClass=illmpresentationgui&cmdNode=iv&baseClass=ilLMPresentationGUI) on how to create a skin

---

Compiling a delos.css that includes our additions

---

### Same visual result

---

### Advantages of CSS approach

---

Settings of all elements at one glance

---

no clicking around and scrolling through a form

---

Use of variables like @brand-primary

in use and defined in standard Delos skin

easy to change colors for different brands

---

new possibilities like hover states for our "button"

---

### Issues with CSS approach

---

requires file access to the server and a custom skin setup

---

adding styles is also not beginner friendly

---

### Bottom line

designer (power user): can style to their heart's content and create helpful content styles

user (beginner): can choose from this library of helpful content styles in page editor

---

We took this very far in Cate
## Full design toolbox

---

<video controls muted autoplay>
    <source data-src="vids/cate_design-toolbox.mp4" type="video/mp4" />
</video>

---

Content cards build for Cate:

![](imgs/cate_content-cards.png)

---

fancy additions:

* same height in every column
* spacing between content and CTA

---

All controlled by individual blocks

---

Inside page editor:

One block per setting

---

excessive nesting

---

![](imgs/cate_nested-colored-cards.png)

---

potential user error: Nesting blocks in the wrong order

---

Code of the content cards:

One div per setting is not good practice

---

<video controls muted autoplay>
    <source data-src="vids/cate_heavy-nesting-code.mp4" type="video/mp4" />
</video>

---

## A small suggestion

---

Feature request

[tinyurl.com/ilias-multistyle](https://tinyurl.com/ilias-multistyle)

---

Allow choosing multiple styles for one block

---

1. Create one block
2. Add from a selection of predefined content styles: color + padding + border + shadow

---

![](imgs/mockup_multi-style.png)

---

### Advantages

---

Easy to use interface

to add many different settings to a single block

---

User still only has a access to carefully selected on-brand options

---

Avoids nesting chaos

---

less clicks inside page editor

---

Maybe the possible selections are filtered

Whitelist: What looks good together?

Blacklist: What shouldn't be used together?

---

## Outlook

CaT developers are working on an implementation

---

We are suggesting to add this to the ILIAS core

---

Any additional funding, feedback, cooperation is greatly appreciated

---

Feature request: [tinyurl.com/ilias-multistyle](https://tinyurl.com/ilias-multistyle)

Link to this presentation: [tinyurl.com/il-devconf-content-styles](https://tinyurl.com/il-devconf-content-styles)

Q&A on Skype: [tinyurl.com/content-styles-skype](https://tinyurl.com/content-styles-skype)

---

Thank you :)
