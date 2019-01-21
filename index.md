---
layout: default
title: a11y.reviews
description: Community reviews on the accessibility of tools and services.
---

A community-driven resource to both find and share information on the accessibility of tools, services, platforms, and so on.

If you have experience with a resource and how accessible it may or may not be, please contribute. Ideally, if you follow the existing format this will be much easier for others to use as well as for us to maintain.

The document is managed on GitHub and uses Markdown for contributions. If you do not use GitHub and/or Markdown, you can still submit via email (email address needed). At launch, this has been seeded with one review to demonstrate the format.

* this unordered seed list will be replaced by toc as unordered list
{:toc}

## Online Surveys

Tools used for polls, surveys, or questionnaires.

### Typeform

Typeform generally does not work with screen readers across platforms. Field labels are not exposed correctly, question navigation is problematic, and answers are not consistently exposed. Color contrast is below WCAG minimums.

There is no public bug tracker to follow issues.

#### Evidence

* [Bug reported 23 February 2016](https://twitter.com/aardrian/status/702301348381986816), screen shots attached.
* 25 February 2016, [screen shot of email response from Typeform](https://twitter.com/aardrian/status/703000834750214145) declining to give an ETA for accessibility fixes.
* 20 March 2016, [screen shot of results embed on mobile](https://twitter.com/aardrian/status/711643411242213376) showing poor contrast, mobile performance.
* 12 July 2016, [Twitter response saying accessibility is on a roadmap](https://twitter.com/typeform/status/752992486784700416).
* 5 September 2016, [Typeform offers a plain HTML fallback](https://twitter.com/typeform/status/772754674621513728), screen reader user (appropriately) dismisses it.
* 17 November 2017, [screen shot of how forms fall apart on zoom](https://twitter.com/stommepoes/status/931518521036681216).

#### Verdict

For any organization that needs to meet WCAG 2.x, whether by law or other requirements, do not use Typeform.

## Content Platforms

This can include web content management systems or other tools that allow authors to post their writing for broad consumption on the web.

### Medium

Medium has no method to provide alternative text for images. Some authors get around this by adding a description of the image in the caption, but screen readers will often announce the file name of the image instead.

Medium does not support tables for data grids. Authors get around this by posting screen shots of tables. These screen shots also do not have alternative text.

Medium can make it difficult for some authors to identify how to structure content correctly, resulting in bullet lists that are just lines preceded by asterisks, or headings that are just bold text.

#### Evidence

* Medium's support pages describe [how to upload an image](https://help.medium.com/hc/en-us/articles/215679797-Images), but offer no guidance on how to support screen reader users nor users who may have been unable to load the images.
* Pointer to [incorrect bullets](https://twitter.com/aardrian/status/1086639530856321024) in a Medium post.
* Pointer to [incorrect headings](https://twitter.com/aardrian/status/1083355862402506752) in a Medium post.
* Screen shot of an[incorrect table](https://twitter.com/aardrian/status/923536098734891009) in a Medium post.

#### Verdict

For any organization whose content needs to meet WCAG 2.x, whether by law or other requirements, do not use Medium.
