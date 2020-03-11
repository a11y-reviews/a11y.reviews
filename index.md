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
* SurveyMonkey radio buttons are hidden in Windows High Contrast Mode (Edge, IE11, Firefox), meaning these users cannot identify the radio buttons nor their state (toggled or not). Raised as an [issue on this repo](https://github.com/a11y-reviews/a11y.reviews/issues/16).

#### Suggestion

A SurveyMonkey form is accessible to a JAWS / Internet Explorer 11 user. SurveyMonkey radio buttons are hidden to users in Windows High Contrast Mode.

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

11 March 2020. Typeform generally does not work with screen readers across platforms. Field labels are not exposed correctly, question navigation is problematic, and answers are not consistently exposed. Color contrast is below WCAG minimums.

There is no public bug tracker to follow issues.

#### References

* [Bug reported 23 February 2016](https://twitter.com/aardrian/status/702301348381986816), screen shots attached.
* 25 February 2016, [screen shot of email response from Typeform](https://twitter.com/aardrian/status/703000834750214145) declining to give an ETA for accessibility fixes.
* 20 March 2016, [screen shot of results embed on mobile](https://twitter.com/aardrian/status/711643411242213376) showing poor contrast, mobile performance.
* 12 July 2016, [Twitter response saying accessibility is on a roadmap](https://twitter.com/typeform/status/752992486784700416).
* 5 September 2016, [Typeform offers a plain HTML fallback](https://twitter.com/typeform/status/772754674621513728), screen reader user (appropriately) dismisses it.
* 17 November 2017, [screen shot of how forms fall apart on zoom](https://twitter.com/stommepoes/status/931518521036681216).
* 6 March 2020, in a [tweet response to a question on screen reader support](https://twitter.com/typeformhelp/status/1235887252867141632): "…we do not have any concrete plans in place for meeting WCAG accessibility standards, which includes support for screen reader technologies, but we are aware of the need for accessibility…"

#### Suggestion

For any organization that needs to meet WCAG 2.x, whether by law or other requirements, do not use Typeform.

### Google Forms

December 2018. Created [a form (Dutch)](https://docs.google.com/forms/d/1wCBVwPQ77lNlWLArQbrM-AH4atepsUphiffDAAfwDgc/viewform?ts=5bebf5a7&edit_requested=true) and tested with VoiceOver/Safari and Jaws/IE 11. 

#### References

* Overuse and wrong use of ARIA
* Not WCAG compliant

#### Suggestion

It is possible to fill and submit a Google Form with a screenreader but the more complex components such as linear scale and multiple choice grid can be confusing.

### GetFeedback

2 February 2019. Took a [3Play Media captioning survey](https://3playmedia.getfeedback.com/r/yBh4ET3z/69abffee-3cfc-44b8-989b-abd365d1da88) using JAWS with Internet Explorer 11.

#### References

* If the form contains a slider (such as choosing on a scale of 1 to n), it cannot be accessed with JAWS/IE11.
* If the form uses text inputs, contrast is very low and relies on float labels (placeholder-like labels that animate up when the field is focused).
* The final submit button has an accessible name different than the displayed text, which can be a problem for voice interface users.

#### Suggestion

GetFeedback will pose problems for JAWS/IE11 users, low-vision users, mobility impaired users, and dictation software users.

### Qualtrics

2 February 2019. Took the [2019 Stack Overflow Developer Survey](https://stackoverflow.az1.qualtrics.com/jfe/form/SV_1RGiufc1FCJcL6B?utm_medium=so-blog&utm_source=so-owned&utm_campaign=dev-survey-2019&award=ab757334b00549cda03f8983c2ccaf4f&site=stackoverflow.com) using JAWS with Internet Explorer 11.

#### References

* Initial screen's instructions are hidden to JAWS/IE11; arrowing around reveals nothing more than the Next button.
* Conveying required fields appears to rely on asterisk character, which is not part of the accessible name when spoken by JAWS.

#### Suggestion

Do not use Qualtrics if you expect to support screen reader users. Certainly not for WCAG 2.x compliance.

### Drupal 8 Webforms
[Drupal](https://www.drupal.org/) is an open source Content Management System (CMS) and one of the popular modules is the [Webform module](https://www.drupal.org/project/webform). Using a free service called [SimplyTest.me](https://simplytest.me/project/webform/8.x-5.x) anyone can install the Drupal Webform module online and have full access to a testing environment.  

#### References
* [Accessibility issue queue](https://www.drupal.org/project/issues/search/webform?version[]=8.x&issue_tags=Accessibility) with open & closed issues.
* [YouTube: Introduction to Webform for Drupal 8](https://www.youtube.com/watch?reload=9&v=VncMRSwjVto&feature=youtu.be)
* Documentation [Webform module for Drupal 8: DIY Accessibility](https://opencollective.com/webform/updates/webform-module-for-drupal-8-diy-accessibility)
* [Accessibility Review](https://docs.google.com/spreadsheets/d/19OJCDet7RF6pXmnSEq1-5EVvQPpU8VFFuD0ADxRtKb4/edit#gid=949844770) following the model by the UC Berkeley Web Access team.

#### Suggestion
* As with Drupal in general, user testing with Zoomtext, Dragon Naturally Speaking & other assistive technology could find improvements.
* I should be tested against WCAG 2.1 AA and possibly WCAG 2.2 AA (as should Drupal Core)

## Content Platforms

This can include web content management systems or other tools that allow authors to post their writing for broad consumption on the web.

### Google AMP Stories

4 September 2019. Reviewing the AMP Stories demo page, controls are unlabeled, most images are missing text alternatives, content is scattered between controls. Generally an unusable experience with a screen reader and problematic with a keyboard.

#### References

* [Amphora.](https://ethanmarcotte.com/wrote/amphora/) by Ethan Marcotte, 9 August 2019.
* AMP itself has accessibility issues, as outlined in [notes from the face-to-face meeting](https://github.com/ampproject/meta-ac/blob/master/meetings/2019-03-f2f.md#accessibility) of the Advisory Committee on 28 March 2019.
* In those same notes, acknowledgment there is no process for accessibility checking before a component is added, with a target date to have a process in place by 1 January 2020.

#### Suggestion

For any organization that needs to meet WCAG 2.x, whether by law or other requirements, do not use AMP Stories.

### Dev.to

31 January 2019. Dev.to lets users author their content via Markdown, so they are able to use all of its structuring and semantic features (e.g. regarding headline hierarchy, quotes, images, lists). 

The overall interface contains many links without accessible names, some of them apparently only existing to enlarge the click area - see the article teaser listing. Said teaser listing also infinite scrolling.

Regarding keyboard accessibility: outline on focus is not disabled via CSS, but some elements are reachable only on hover (example: the "Follow" control inside a tag list item). Said control, again, is an anchor element with a `href="#"` but should be a button.

#### Suggestion

For any organization that needs to meet WCAG 2.x, whether by law or other requirements, do not use Dev.to.

### Medium

4 September 2019. Medium now has a method to provide alternative text for images. Because it was only recently added, some authors got around this by adding a description of the image in the caption, but screen readers will often announce the file name of the image instead. Those Medium posts will not be updated unless the author decides to do so.

Medium does not support tables for data grids. Authors get around this by posting screen shots of tables. These screen shots also do not have alternative text.

Medium can make it difficult for some authors to identify how to structure content correctly, resulting in bullet lists that are just lines preceded by asterisks, or headings that are just bold text.

#### References

* [Medium Supports alt Text (Mostly)](https://medium.com/@aardrian/medium-supports-alt-text-mostly-d1e53d0e21cb) by Adrian Roselli, 18 July 2019.
* Medium's support pages describe [how to upload an image](https://help.medium.com/hc/en-us/articles/215679797-Images) and now offers brief instructions on how to add alternative text, but not how to write it.
* Pointer to [incorrect bullets](https://twitter.com/aardrian/status/1086639530856321024) in a Medium post.
* Pointer to [incorrect headings](https://twitter.com/aardrian/status/1083355862402506752) in a Medium post.
* Screen shot of an [incorrect table](https://twitter.com/aardrian/status/923536098734891009) in a Medium post.

#### Suggestion

For any organization whose content needs to meet WCAG 2.x, whether by law or other requirements, do not use Medium.

## Video Conferencing

### Zoom

21 January 2019. From polling blind JAWS users, Zoom works well for setting up calls and participating via audio only.

#### Suggestion

Zoom is generally accessible.

## Source Control

### Github website

3 February 2019. With one or two exceptions, the [Github website](https://github.com/) has good general accessibility and is usable with most Assistive Technologies (AT). Exceptions include horizontal scrolling at high zoom or magnification, use of browser default focus indication, and missing alt texts on non-essential images (like user contribution graphs). An overuse of aria-label with sometimes nonsensical names makes some controls a bit confusing ("Only those with link Learn more about permission levels to this repository can merge pull requests.")

#### References

[Voluntary Product Accessibility Template (VPAT) for Github](https://government.github.com/accessibility)

#### Suggestion

The Github website is inconvenient for magnification users, and for keyboard users with low vision, but is otherwise usable by most people. The Github team is responsive to issues relating to accessibility.

## Project Management Software

### Trello

November 2018. Trello is generally unusable or difficult to use for some people. 

This includes low-vision users who use browser zoom (everything is absolutely positioned and overlaps, hiding most of the content) and low-vision users using screen magnification software (mouse-users can get around and reach everything, but keyboard-users cannot rely on their focus to move their viewport around since Trello has its own "application" focus for its built-in keyboard shortcuts). 

The keyboard shortcuts are single-character keys, causing trouble for speech recognition users (at the time of testing there was no way to change these or turn them off).

Sighted keyboard users of all types aren't able to move their focus into opened popups/submenus, except for the few who have an autofocussed input inside. Focus also often seems to end up in random places after performing an action. "Star" controls only appear on mouse hover and cannot be reached with keyboard, and are not real controls but clickable spans.

Screen reader users contend with lack of structure (something they could otherwise use to supplement the difficulty of using the keyboard shortcuts for navigation), unlabelled controls or controls with title attributes only.

#### References

[Partial WCAG 2.1 mini-audit](https://stommepoes.nl/trello/trello.html).

#### Suggestion

Avoid choosing Trello for your project management unless all team members have excellent vision and can use a pointer. Having a large monitor helps. Its main strength is being a simple, straightforward and un-opinionated management tracker or even just for keeping track of TO-DO's, where teams/owners choose their own rules and decide how complex their flows will be.

## Collaboration Software

### Slack

30 May 2019. Slack’s web interface and native clients are generally accessible to skilled screen reader users.

#### Suggestion

Given Slack's history of accessibility issues, be certain to test with your users before rolling it out within an organization.

#### References

[Status Of The Accessibility Of Slack](https://marcozehe.wordpress.com/2016/01/16/status-of-the-accessibility-of-slack/)

## Widgets

### ag-Grid

9 September 2019. The ag-Grid library promises to make data tables with plenty of add-on features. It offers information on [its accessibility features and benefits](https://www.ag-grid.com/javascript-grid-accessibility/). However, controls to use the features built into columns (such as sorting, filtering, re-ordering) are inaccessible to keyboard-only and screen reader users. Further, NVDA appears to be unable to navigate out of the row that holds the column headers and into the data. Reading order is still a potential issue unless developers know to add a specific attribute to the code.

#### References

* [Keyboard inaccessible column controls #3340](https://github.com/ag-grid/ag-grid/issues/3340), which references Zendesk entries available only for paid ag-Grid users:
  * AG-2472 Context/Column Menu - Focus menu when it is invoked, and allow keyboard navigation
* [Screen reader inaccessible column controls #3341](https://github.com/ag-grid/ag-grid/issues/3341), which references Zendesk entries available only for paid ag-Grid users:
  * AG-3223: ARIA / Accessibility / Keyboard navigation allow user to use filter and filter options by navigating with keyboard
  * AG-2629: Accessibility - Allow screen readers to access the column headers to apply sort and filtering capabilities
  * AG-3253: Accessibility / navigation Allow to navigate with keyboard though the context menu when it gets opened
* [Cannot get past column headers with NVDA #3342](https://github.com/ag-grid/ag-grid/issues/3342)
* [DOM order issues with on-demand data](https://twitter.com/aardrian/status/1167047661754683397)

#### Suggestion

For any organization whose site or content needs to meet WCAG 2.x, whether by law or other requirements, do not use ag-Grid.

### React Datepicker

9 September 2019. The ReactJS Datepicker provides some [accessibility notes](https://www.npmjs.com/package/react-datepicker#accessibility) for developers who want to know how accessible the control is, however it only speaks to keyboard support — which is not conveyed to users by default. Generally the date picker lacks accessible names for controls, keyboard support, and sufficient contrast along with some generally incorrect use of table elements.

#### References

* [List of 8 WCAG violations](http://adrianroselli.com/2019/07/maybe-you-dont-need-a-date-picker.html#ReactDatePicker) as part of a larger blog post.
  * Specifically called our are failures of 1.3.1 Info and Relationships (A), 1.4.1 Use of Color (A), 1.4.11 Non-text Contrast (AA), 2.1.1 Keyboard (A), 3.3.2 Labels or Instructions (A), and 4.1.2 Name, Role, Value (A).

#### Suggestion

For any organization whose site or content needs to meet WCAG 2.x, whether by law or other requirements, do not use React Datepicker.

## Media Players

### Brightcove Player

19 September 2019. The Brightcove Player provides [accessibility notes](https://support.brightcove.com/brightcove-player-accessibility) that only addresses standard keyboard behaviors for buttons and makes no statement of WCAG compliance. It does recommend that the JAWS/ Chrome pairing should be avoided when using the player.

#### References

No bugs filed, but from a quick review:
*	1.4.11 Non-text Contrast Level AA — the focus ring is default, but controls also have a mild glow on focus.
* 2.4.1 Bypass Blocks Level A — the `<iframe>` used for the embed has no `title` attribute.
*	2.4.3 Focus Order Level A — the scrubber / timeline appears after first half of controls, visually going up then back down.
*	2.4.7 Focus Visible Level AA —	after tabbing through the controls, there are two visually hidden controls that control playback.
*	2.5.3 Label in Name Level A — the playback rate button/menu text is not part of the accessible name.
*	3.3.2 Labels or Instructions Level A — the discussed keyboard shortcuts are not exposed, such as in the closed-caption or playback rate controls.
*	4.1.2 Bypass Blocks Level A — the `<iframe>` used for the embed has no `title` attribute, same as 2.4.1.

#### Suggestion

For any organization whose video content needs to meet WCAG 2.x, whether by law or other requirements, do not use Brightcove Player.
