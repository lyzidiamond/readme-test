---
title: Linter
excerpt: An AI-powered tool for checking page content against your own style guide.
deprecated: false
hidden: false
metadata:
  robots: index
---

The Linter automates content validation by checking documentation against your company’s style guide and established writing standards. It streamlines the manual review process writers typically perform with external tools.

Configure custom rules to enforce code formatting, word choice, and adherence to internal style and best practices. Whether your documentation includes custom HTML or extensive code samples, the Linter ensures consistency across all your docs.

[keep the plan table]

## How the Linter works

The Linter is an AI-assisted style guide enforcer that works in a two-step process.

First, it takes your style rules and transforms them into a rubric of individual assessment tasks. This means you can write your rules however makes the most sense to you: a list, a narrative description, examples, or a combination of all three.

Then, it reads your documentation and checks the content against that rubric. It provides a score based on that assessment, highlights errors and warnings you've identified in your configuration, and provides suggestions for how to improve your score.

_Note: Linter is only available for Guides and API Reference pages._

## Configure with your style rules

In the dashboard for your project, go to the **Admin Tools** section and select **AI > Linter**. You can also get to the configuration page by clicking on the [icon] gear icon next to [play icon] **Run AI Linter** at the bottom of any Guide or API Reference page.

The configuration page has three sections: Style Guide, Errors, and Warnings.

### Style Guide

The Style Guide section is a description of your content style guide. Include everything in this section you want used in the rubric used to calculate your Style Guide Score. Write this section as paragraphs, a bulleted list, or a combination.

Examples of style guide rules to include in this section:

- Keep headings to a single line.
- Always use active voice, never passive voice.
- Every acronym should have an definition on first mention, but then can be used without. Example: on first mention, "NOAA (the National Oceanic and Atmostpheric Association)". On subsequent mentions, "NOAA" is fine.
- Use simpler words wherever possible.
- Be consistent with vocabulary. Example: don't mix "parameter" and "variable" when talking about passing values into a function. Always use "parameter".
- No more than 4 sentences per paragraph. No more than 20 words per sentence.
- Use a casual yet informative tone. Avoid exclamation points and marketing language.

These instructions can be as detailed or general as you want, but more specific guidance helps the Linter generate a more detailed rubric.

### Errors and Warnings

The Errors and Warnings sections are subsets of style guide rules that are called out specifically in their own lists when the Linter runs. Include these rules in the Style Guide section if you want them included in the Style Guide Score.

#### Errors

Errors are objective style rules that _can't_ be broken. Some examples:

- Always style the product name as "ReadMe", never "readme" or "Readme".
- Wrap all inline code elements in backticks. Bad: "run npm install -g my-package." Good: "Run `npm install -g my-package`."
- Don't allow any placeholder text. Specifically point out instances of "TODO", "FIXME", "PLACEHOLDER", or "Lorem ipsum"-style latin.

#### Warnings

Warnings are subjective style rules that _shouldn't_ be broken. Some examples:

- Use active voice, not passive voice.
- Use authoritative, second person imperative tense. Don't use third person plural ("Let's click here") or indirect, headging language ("You can click here") -- use command language ("Click here").
- Be clear and confident. Don't use hedging language. Bad example: "You might want to consider clicking here." Good example: "Click here."

<!-- I'm providing some subjective guidance here (include errors in style guide for sure vs. include warnings if you want) as a reflection of the feature as it works as of June 2026, where the assessment doesn't include Errors in the score. I personally think Errors should be included, which is why I'm suggesting it here. I should talk to product and decide if this was a deliberate decision or not. -->
<!-- Current docs say the Linter automatically detects broken links but it's not detecting them for me -- add to UI improvements/Linear. -->

## Run the Linter on your docs

In the Editor view, navigate to the page where you want to run the Linter. At the bottom of the page, select [icon] Run AI Linter. When it’s done running, there are three new icons at the bottom of the page, each corresponding to a section of the Linter configuration.

- The dialog [modal?] that shows up first shows your Style Guide Score and the rules the Linter checked for from the Style Guide section.
- The second icon shows how many errors the Linter detected as defined in the Errors section.
- The third icon shows how many warnings were detected as defined in the Warnings section.

Click the [icon] Errors or [icon] Warnings icons to see a list of the specific errors and warnings the Linter detected. Click [icon] **Fix All** to open [Agent](https://docs.readme.com/main/docs/aiagent) and automatically make changes to the docs.


## FAQ

<!-- Can keep this the same -->