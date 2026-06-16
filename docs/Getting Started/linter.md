# Linter
## An AI-powered tool for checking page content against your own style guide.

The Linter automates content validation by checking documentation against your company’s style guide and established writing standards. It streamlines the manual review process writers typically perform with external tools.

You can configure custom rules to enforce code formatting, word choice, and adherence to internal style and best practices. Whether your documentation includes custom HTML or extensive code samples, the Linter ensures consistency across all your docs.

[keep the plan table]

## How the Linter works

The Linter is an AI-assisted style guide enforcer that works in a two-step process.

First, it takes your style rules and transforms them into a rubric of individual assessment tasks. This means you can write your rules however makes the most sense to you: a list, a narrative description, examples, or a combination of all three.

Then, it reads your documentation and checks the content against that rubric. It provides a score based on that assessment, highlights errors and warnings you've identified in your configuration, and provides suggestions for how to improve your score.

_Note: Linter is only available for Guides and API Reference pages._

## Configure with your style rules

In the dashboard for your project, go to the **Admin Tools** section and select **AI > Linter**. You can also get to the configuration page by clicking on the [icon] gear icon next to [play icon] **Run AI Linter** at the bottom of any Guide or API Reference page.

The configuration page has three sections: Style Guide, Errors, and Warnings.

- **Style Guide:** a description of your content style guide. You can include anything in this section, from voice and tone to specific word choice to code sample formatting. The rules and guidance in this section are what the Linter uses to generate your Style Guide Score.
<!-- I'm providing some subjective guidance here (include errors in style guide for sure vs. include warnings if you want) as a reflection of the feature as it works as of June 2026, where the assessment doesn't include Errors in the score. I personally think Errors should be included, which is why I'm suggesting it here. I should talk to product and decide if this was a deliberate decision or not. -->
- **Errors:** style rules that _cannot_ be broken. The Errors section can be used to identify things like miscapitalization, incorrect code formatting, and placeholder text. This section should be a subset of the rules defined in the Style Guide section above so they show up as part of the overall score.
- **Warnings:** style rule violations you want to point out specifically, but don’t necessarily need to be changed. Add these rules to the Style Guide section if you want them to be included 




## Run the Linter on your docs

- explain what you see
- explain the score

## Next steps

- make changes and re-run
- "Fix" option to make changes in Agent