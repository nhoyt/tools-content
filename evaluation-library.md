Both [FAE](/tools/fae) and [AInspector WCAG for Firefox](/tools/ainspector) share the same Evaluation Library, a custom-built JavaScript engine that applies accessibility rules to elements found on web pages and produces the evaluation results.

## Accessibility Rules

The Evaluation Library currently includes over 120 web accessibility rules, which were developed over a six year period through the work of the OpenAjax Accessibility Task Force, along with feedback from users of the initial versions of FAE and AInspector WCAG.

Every rule included in the library references at least one WCAG 2.0 Level A or AA Success Criterion requirement.

## Manual Checks

A distinguishing feature of the Evaluation Library is the number of accessibility rules it includes which produce what are known as manual checks.

While most of the rules in the library produce ‘Pass’, ‘Warn’ or ‘Fail’ results (for accessibility requirements that can be programmatically analyzed), approximately one third of its rules produce only a ‘Manual Check’ result, indicating that human intervention is needed to determine compliance.

## Rulesets

The Evaluation Library includes two rulesets, selectable by the user:

* HTML5 and ARIA Techniques
* HTML4 Legacy Techniques

The recommended ruleset is ‘HTML5 and ARIA Techniques’, as it comprises the most up-to-date requirements.

## Rule Categories

The rulesets in the Evaluation Library are organized by the following rule categories or groupings:

* Landmarks
* Headings
* Styles/Content
* Images
* Links
* Tables
* Forms
* Widgets/Scripts
* Audio/Video
* Keyboard
* Timing
* Site Navigation
