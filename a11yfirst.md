Ten to fifteen years ago (2005 to 2010), the web accessibility community generally agreed that the best approach for making web content more accessible was to focus on educating and increasing awareness of accessibility among web developers, as they were the gatekeepers regarding what was published on the web. If we can inform and educate web developers of accessibility best practices, the thinking went, then a significant portion of the content they were responsible for would be accessible.

## CMSs and Accessibility Checkers

And then along came content management systems. Their wide adoption in subsequent years has been driven by the fact that content authors no longer needed to be versed in HTML markup. The CMS provides a WYSIWYG editor that allows authors to create and publish new web pages as needed. The possibilities for web content being published with accessibility problems grew by orders of magnitude.

Not to worry, some product designers reasoned. We will simply build accessibility checkers that can be invoked by authors when they are ready to publish content. We can even make the accessibility checking step part of the CMS workflow. However, the logical point at which to invoke such a checker is at the end of the process of creating a web page, or after making extensive edits to an existing page.

What happens then? The checker compiles a list of problems, usually in document order, that you, the author, are asked to process one by one, "fixing" each problem as it is highlighted.

The problem with this approach, in presenting you with a list of problems at the end of the editing process, relates to both workflow and the format of the list.

First is the element of surprise, leading you to realize that the problems in the list were hidden until now, and to perhaps say to yourself "I thought I was done, but the editor is telling me that I'm not!"

Secondly, in going through the list, it is likely that you will move in a seemingly random fashion from one type of problem to another type, and then back to the first type again, then to a third type, and so on. This randomness is not conducive to learning more about accessibility.

In summary, this can be labeled the _reactive_ approach to accessible authoring.

## The A11yFirst Project

In contrast to the accessibility checker approach, the A11yFirst Project takes a _proactive_ approach to accessible authoring. It comprises the following modifications to CKEditor, the embedded HTML editor used in CMSs such as Drupal, implemented as installable plugins.

* A11yFirst Heading / Paragraph
* A11yFirst Character Style
* A11yFirst Link
* A11yFirst Image
* A11yFirst Help

Each of these plugins is described in more detail below.

### A11yFirst Heading / Paragraph

This plugin adds the Heading / Paragraph menu button to the editor toolbar, which supports authors in the proper use of headings and other block-level paragraph formats within web documents.

It is a replacement for the Format plugin, and is intended to be used in conjunction with the A11yFirst Character Style plugin.

The Heading / Paragraph menu button includes the following features:

* Headings are made prominent by appearing first in the Heading / Paragraph menu.
* Only heading levels that result in proper nesting are enabled in the menu (based on cursor position).
* The heading menu items indicate the typical usage for various heading levels, for example:
    *  H1 - Document title
    *  H2 - Section title
    *  H3 - Subsection title
* The distraction of styling the heading menu items with different font sizes is avoided. All are styled the same, which reinforces their use as structural elements rather than for their visual effect.

### A11yFirst Character Style

This plugin adds the Character Style menu button to the editor toolbar, which enables you to add and remove inline character styling to the text content of your web document.

This plugin is a replacement for the Styles Combo plugin, and is intended to be used in conjunction with the A11yFirst Heading / Paragraph plugin.

The Character Style plugin applies an inline styling element to selected text or, if no text is selected, toggles on the selected character style until the author switches to a different style or a new line is inserted.

### A11yFirst Link

This plugin adds the A11yFirst Link button to the editor toolbar. It provides authors with features for ensuring that the display text of a link is accessible for people with disabilities.

It is a replacement for the standard Link plugin.

The A11yFirst Link plugin has all the features of the standard Link plugin, but adds additional validation of the link display text to check for common accessibility issues.

For example, the plugin checks for display text that does not describe the target of the link, e.g "click here", "more", etc.

It prompts the author when a URL is used as the display text, as they are typically not very descriptive of the link target. However, they are allowed through a confirm dialog box, which warns the user of the accessibility problems of using the URL.

In general, this plugin helps authors understand the importance of display text in describing the target of a link as accurately and succinctly as possible.

#### Display Text validation features

* Does not allow empty Display Text
* Does not default to using the URL as the Display Text
* Warns when a URL is used as the Display Text
* Detects the use of ‘click here,’ ‘more’ et al.

### A11yFirst Image

This plugin adds the A11yFirst Image button to the editor toolbar. It provides authors with additional features for ensuring image accessibility for people with disabilities.

It is a replacement for the standard Image and Enhanced Image plugins.

The A11yFirst Image plugin is a modification of the Enhanced Image (image2) plugin to include important accessibility features for validating Alternative Text and allowing the author to identify the location within the document of a longer description of the image.

People with visual impairments need descriptions of informative images to understand the purpose of the image. Each informative image must at least have Alternative Text and may require a longer description, especially if the image is a chart or graph.

Alternative Text should be succinct and should not include redundant or irrelevant information (e.g. "image of .."). An image that is purely decorative should have empty Alternative Text, but since this is rare the plugin requires the author to confirm that the image is purely decorative.

A complex informative image should have a long description in the page, adjacent to the image. The plugin provides a way for the author to provide a reference to the location of the long description in the page, which can provide a more semantically meaningful description. For example, a table may be provided that includes the data used to generate a chart or graph.

A11yFirst Image includes the following features:

#### Alternative Text Validation

The following conditions for Alternative Text are checked:

* Empty
* More than 100 char. in length
* Starts with the phrases ‘image of,’ ‘photo of’ et al.
* Includes file name or size
* For a decorative image, allows the user to confirm that Alternative Text is not required

#### Identifying Long Description

A select box allows the author to indicate if a longer description of the image exists in the document, and if so, its location (i.e. before, after or before and after the location of the image in the document).

### A11yFirst Help

This plugin adds the A11yFirst Help menu button to the editor toolbar, which launches a dialog box that provides explanatory text on topics that help authors understand the accessibility issues of editing web documents.

It compliments and provides specific information on the use of the full suite of A11yFirst plugins: Heading / Paragraph, Character Style, A11yFirst Image and A11yFirst Link.

#### Overview

Each of the A11yFirst plugins embodies a new approach to authoring accessible web documents. Rather than relying upon a reactive model that detects problems after they exist, the A11yFirst approach is proactive. It enables authors to create content that is accessible during the authoring process, by providing feedback and validation on a feature-by-feature basis.

For example, once an author becomes familiar with the requirements for, say, adding images to documents, it becomes second nature to provide alternative text when the image is added, and to consider whether the image needs a longer description in the document.

#### Features

The A11yFirst Help dialog box contains the following information:

* How to get started using A11yFirst for CKEditor and why accessibility is important
* How to work with the A11yFirst features, as well as a few of the standard features included in CKEditor that are important for accessibility
* The purpose of, and contributors to, the A11yFirst Project

## Resources

Visit the following [CKEditor Plugins](https://ckeditor.com/cke4/addons/plugins/all) pages to download and install the A11yFirst plugins:

* [A11yFirst Heading / Paragraph](https://ckeditor.com/cke4/addon/a11yheading)
* [A11yFirst Character Style](https://ckeditor.com/cke4/addon/a11ystylescombo)
* [A11yFirst Link](https://ckeditor.com/cke4/addon/a11ylink)
* [A11yFirst Image](https://ckeditor.com/cke4/addon/a11yimage)
* [A11yFirst Help](https://ckeditor.com/cke4/addon/a11yfirsthelp)
