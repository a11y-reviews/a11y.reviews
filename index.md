---
layout: default
title: Accessibility Reviews
description: Community reviews on the accessibility of tools and services.
---

A community-driven resource to both find and share information on the accessibility of tools, services, platforms, and so on.

If you have experience with a resource and how accessible it may or may not be, please contribute. Ideally, if you follow the existing format this will be much easier for others to use as well as for us to maintain.

The document is managed on GitHub and uses Markdown for contributions. If you do not use GitHub and/or Markdown, you can still submit via email (email address still needed). Please include the date of your review in the content you submit.

* this unordered seed list will be replaced by toc as unordered list
{:toc}

## Online Surveys

Tools used for polls, surveys, or questionnaires.

### SurveyMonkey

22 January 2019. Took a [Smashing Magazine survey](https://www.surveymonkey.co.uk/r/survey-smashing-team) using JAWS with Internet Explorer 11. It appears no special work needs to be done when setting up a form.

#### References

* Confirmed [no special adjustments made](https://twitter.com/indysigner/status/1087760016323563520) for the form to work with JAWS/IE11.
* Users had raised issues with TypeForm, [no issues raised since moving to SurveyMonkey](https://twitter.com/indysigner/status/1087763172436701186) in response.

#### Suggestion

A SurveyMonkey form is accessible to a JAWS / Internet Explorer 11 user. If you are using other SR/browser combinations, please add to this.

### SurveyGizmo

22 January 2019. Took a [U of Colorado survey](https://www.surveygizmo.com/s3/4724778/Universal-Design-Accessibility-Topics-in-College-Curriculum) using JAWS with Internet Explorer 11.

#### Suggestion

A SurveyGizmo form is accessible to a JAWS / Internet Explorer 11 user. If you are using another SR/browser combination, please add to this.

### Formstack

23 January 2019. Took an [IAAP survey](https://accessibilityassociation.formstack.com/forms/iaap_procurement_jta_survey) using JAWS with Internet Explorer 11.

#### References

Questions scrolled way off screen, headings were imperfect. All questions could be navigated and answered. Error messages were not inline (for radio buttons at least) and the overall error message was a very long run-on list of error text as a live region that caused JAWS to choke and stutter instead of announcing them all.

#### Suggestion

Formstack may pose problems for JAWS/IE11 users, zoom users, and mobility impaired users.

### Typeform

20 January 2019. Typeform generally does not work with screen readers across platforms. Field labels are not exposed correctly, question navigation is problematic, and answers are not consistently exposed. Color contrast is below WCAG minimums.

There is no public bug tracker to follow issues.

#### References

* [Bug reported 23 February 2016](https://twitter.com/aardrian/status/702301348381986816), screen shots attached.
* 25 February 2016, [screen shot of email response from Typeform](https://twitter.com/aardrian/status/703000834750214145) declining to give an ETA for accessibility fixes.
* 20 March 2016, [screen shot of results embed on mobile](https://twitter.com/aardrian/status/711643411242213376) showing poor contrast, mobile performance.
* 12 July 2016, [Twitter response saying accessibility is on a roadmap](https://twitter.com/typeform/status/752992486784700416).
* 5 September 2016, [Typeform offers a plain HTML fallback](https://twitter.com/typeform/status/772754674621513728), screen reader user (appropriately) dismisses it.
* 17 November 2017, [screen shot of how forms fall apart on zoom](https://twitter.com/stommepoes/status/931518521036681216).

#### Suggestion

For any organization that needs to meet WCAG 2.x, whether by law or other requirements, do not use Typeform.

### Google Forms

December 2018. Created [a form (Dutch)](https://docs.google.com/forms/d/1wCBVwPQ77lNlWLArQbrM-AH4atepsUphiffDAAfwDgc/viewform?ts=5bebf5a7&edit_requested=true) and tested with VoiceOver/Safari and Jaws/IE 11. 

#### References

* Overuse and wrong use of ARIA
* Not WCAG compliant

#### Suggestions

It is possible to fill and submit a Google Form with a screenreader but the more complex components such as linear scale and multiple choice grid can be confusing.

## Content Platforms

This can include web content management systems or other tools that allow authors to post their writing for broad consumption on the web.

### Dev.to

31 January 2019. Dev.to lets users author their content via Markdown, so they are able to use all of its structuring and semantic features (e.g. regarding headline hierarchy, quotes, images, lists). 

The overall interface contains many links without accessible names, some of them apparently only existing to enlarge the click area - see the article teaser listing. Said teaser listing also infinite scrolling.

Regarding keyboard accessibility: outline on focus is not disabled via CSS, but some elements are reachable only on hover (example: the "Follow" control inside a tag list item). Said control, again, is an anchor element with a `href="#"` but should be a button.

#### Suggestion

For any organization that needs to meet WCAG 2.x, whether by law or other requirements, do not use Dev.to.

### Medium

20 January 2019. Medium has no method to provide alternative text for images. Some authors get around this by adding a description of the image in the caption, but screen readers will often announce the file name of the image instead.

Medium does not support tables for data grids. Authors get around this by posting screen shots of tables. These screen shots also do not have alternative text.

Medium can make it difficult for some authors to identify how to structure content correctly, resulting in bullet lists that are just lines preceded by asterisks, or headings that are just bold text.

#### References

* Medium's support pages describe [how to upload an image](https://help.medium.com/hc/en-us/articles/215679797-Images), but offer no guidance on how to support screen reader users nor users who may have been unable to load the images.
* Pointer to [incorrect bullets](https://twitter.com/aardrian/status/1086639530856321024) in a Medium post.
* Pointer to [incorrect headings](https://twitter.com/aardrian/status/1083355862402506752) in a Medium post.
* Screen shot of an[incorrect table](https://twitter.com/aardrian/status/923536098734891009) in a Medium post.

#### Suggestion

For any organization whose content needs to meet WCAG 2.x, whether by law or other requirements, do not use Medium.

## Video Conferencing

### Zoom

21 January 2019. From polling blind JAWS users, Zoom works well for setting up calls and participating via audio only.

#### Suggestion

Zoom is generally accessible.
