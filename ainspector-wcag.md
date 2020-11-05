AInspector WCAG is an [open source](https://opensource.org/osd-annotated) add-on for the Firefox browser that, when activated, automatically analyzes the page loaded in the active tab for compliance with accessibility requirements defined by the [World Wide Web Consortium (W3C)](https://www.w3.org/), and for proper use of accessibility features defined by the current HTML Standard (previously known as HTML5).

## Web Accessibility Standards

Each evaluation rule that AInspector WCAG uses is based on one or more of the requirements and features from the following widely-accepted standards:

* [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/TR/WCAG/) Success Criteria
* [Accessible Rich Internet Applications (WAI-ARIA)](https://www.w3.org/TR/wai-aria/)
* [WAI-ARIA Authoring Practices](https://www.w3.org/TR/wai-aria-practices/) Techniques
* [HTML Standard](https://html.spec.whatwg.org/multipage/)

## Evaluation Rules

AInspector WCAG produces evaluation results that are structurally identical to those produced by [FAE](/tools/fae/). This is because it utilizes the same [Evaluation Library](/tools/evaluation-library), which comprises a set of over 120 evaluation rules.

The rules in the Evaluation Library are organized into categories with which most web developers are familiar, including headings, lists, forms, tables, etc.

## Why Use AInspector WCAG?

[FAE](/tools/fae) is used for evaluating entire websites, while AInspector WCAG is for evaluating a single web page. However, AInspector WCAG does offer advantages and features not present in FAE. AInspector WCAG:

* evaluates pages that are behind a firewall if you are logged into the site with Firefox;
* allows you to evaluate dynamic content (for example, content that only appears after selecting a button or other widget on the page) via its timer-activated re-evaluation feature;
* selectively highlights elements on the page according to the evaluation result types you specify.

## Resources

* Visit the [Mozilla Add-ons page](https://addons.mozilla.org/en-US/firefox/addon/ainspector-wcag/) to install the latest version of AInspector WCAG directly into Firefox.

* See the [full documentation for AInspector WCAG](http://docs.ainspector.org) for more information.
