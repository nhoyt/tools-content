Ten to fifteen years ago (2005 to 2010), the web accessibility community generally agreed that the best approach for making web content more accessible was to focus on educating and increasing awareness of accessibility among web developers, as they were the gatekeepers regarding what was published on the web. If we can inform and educate web developers of accessibility best practices, the thinking went, then a significant portion of the content they were responsible for would be accessible.

## CMSs and Accessibility Checkers

And then along came content management systems. Their wide adoption in subsequent years has been driven by the fact that content authors no longer needed to be versed in HTML markup. The CMS provides a WYSIWYG editor that allows authors to create and publish new web pages as needed. The possibilities for web content being published with accessibility problems grew by orders of magnitude.

Not to worry, some product designers reasoned. We will simply build accessibility checkers that can be invoked by authors when they are ready to publish content. We can even make the accessibility checking step part of the CMS workflow. However, the logical point at which to invoke such a checker is at the end of the process of creating a web page, or after making extensive edits to an existing page.

What happens then? The checker compiles a list of problems, usually in document order, that you, the author, are asked to process one by one, "fixing" each problem as it is highlighted.

The problem with this approach, in presenting you with a list of problems at the end of the editing process, relates to both workflow and the format of the list.

First is the element of surprise, leading you to realize that the problems in the list were hidden until now, and to perhaps say to yourself "I thought I was done, but the editor is telling me that I'm not!"

Secondly, in going through the list, it is likely that you will move in a seemingly random fashion from one type of problem to another type, and then back to the first type again, then to a third type, and so on. This randomness is not conducive to learning more about accessibility.

In summary, this can be labeled the _reactive_ approach to accessible authoring.

## The A11yFirst project

In contrast to the accessibility checker approach, A11yFirst comprises a number of modifications to the WYSIWYG editor in CMSs that take a _proactive_ approach. These are implemented as plugins for CKEditor, the default editor in the current version of Drupal:

* A11yFirst Heading / Paragraph
* A11yFirst Character Style
* A11yFirst Link
* A11yFirst Image
* A11yFirst Help
