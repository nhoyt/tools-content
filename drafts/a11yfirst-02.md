Ten to fifteen years ago (2005 to 2010), the web accessibility community generally agreed that the best approach for making web content more accessible was to focus on educating and increasing awareness of accessibility among web developers, as they were the gatekeepers regarding what was published on the web. If we can inform and educate web developers of accessibility best practices, the thinking went, then a significant portion of the content they were responsible for would be accessible.

## CMSs and Accessibility Checkers

And then along came content management systems. Their wide adoption in subsequent years has been driven by the fact that content authors no longer needed to be versed in HTML markup. The CMS provides a WYSIWYG editor that allows authors to create and publish new web pages as needed. The possibilities for web content being published with accessibility problems grew by orders of magnitude.

Not to worry, some product designers reasoned. We will simply build accessibility checkers that can be invoked by authors when they are ready to publish content. We can even make the accessibility checking step part of the CMS workflow. However, the logical point at which to invoke such a checker is at the end of the process of creating a web page, or after making extensive edits to an existing page.

What happens then? The checker compiles a list of problems, usually in document order, that you, the author, can process one by one, "fixing" each problem as it is highlighted.

The problem with this approach, in presenting you with a list of problems at the end of the editing process, is in what this communicates to the author. Namely, that (1) each problem likely has a simple fix, and (2) you can save this step until the end. Implicit in both of these messages is that accessibility must not be that important.

About ten years ago, developers at the Illinois Dept. of Human Services built
