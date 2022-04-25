# Op1st content writing style guide

## Overview

These guidelines help make your content more clear and consistent.
This helps your readers and your editors.

### Markdown

Documents are written in Markdown.
See the [Markdown Guide][2] for instructions on how to use this simple and versatile markup language.

For technical content, we have our own [technical markup style guide][5].

### Document naming conventions

Documentation titles are pre-fixed by the type of content if it is an FAQ or how-to type of content.
Other significant documents simply have descriptive titles.
In titles, words are always separated by a hyphen.

**Example:**
* Significant documents: glossary, style-guide
* How-to guides: how-to-request-a-repository, how-to-use-o1-clone-tool

### Organization

There are two folders in the `community-handbook` repository: `content` and `contributing`.

The `content` folder holds documentation for project users and contributors to help themselves get things done (task instructions and guides).

The `contributing` folder contains general information and how-to content for documentation and content contributors.
That is, people who write docs, blog posts, and articles for the *Operate First User and Contributor Handbook* are content contributors.

When adding to the repository, place documentation in the applicable folder.
If you are unsure which folder to use, please ask for guidance in your issue or PR to the repository.

## Format

### Headings

Use `Title Case` when referring to the full name of a document, such as, *Operate First Community Handbook*.
All other titles and headings use `Sentence case`, meaning capitalization follows the same rules as that of a normal sentence (only the first word and proper nouns are capitalized).

### Line breaks

When writing paragraphs, start each sentence on a new line.
This format will render as a normal paragraph, but makes it significantly easier to edit a document.
Without this method, edits to one sentence of a paragraph will appear as a change to the entire paragraph on GitHub.
By starting each sentence on a new line, an edit to a sentence will show up as a change to only that sentence, making it easier to review and approve new modifications to a document.

**Example:**

In Markdown:
>These two sentences are separated into two lines.<br>
This is our preferred method, as it makes it much easier to review changes to the paragraph.

Rendered:
>These two sentences are separated into two lines.
This is our preferred method, as it makes it much easier to review changes to the paragraph.

### Links

Use reference style links, as they are the easiest to read and do not clutter up the text.
They appear similar to footnotes in Markdown, but they render as hyperlinks.

**Example:**

In Markdown:

>For instructions on reference style links, click \[here]\[1]<br>
...<br>
*At the bottom of the document:*<br>
\[1]: https://www.markdownguide.org/basic-syntax/#reference-style-links


Rendered:
> For instructions on reference style links, click [here][1]

The link in the example above is called an absolute path.
Absolute paths should only be used to link to a page outside of the community handbook repository.
When linking to another document within the repository, however, we prefer to use the relative path.

**Example:**

Relative path:
>../content/how-to-request-a-repository.md<br>
In this case, the initial **..** is necessary because the style guide is located within the **contributing** folder of the community handbook repository.
Relative paths are relative to the location of the current file, so we need to move back one directory with the .. before we can specify the **content** folder and the document within it.<br>

Instead of:
>https://github.com/operate-first/community-handbook/blob/main/content/how-to-request-a-repository.md

### Templates

Our [template document][4] provides several templates for various document types: how-to, article, FAQ, and so forth.
To use the template document:
1. A writer picks one of the templates and discards the rest of the markup.
1. The templates are displayed as code blocks by indenting 4 characters; this makes the markup visible on the rendered page. To use the template, the 4 characters must be removed.

## Admonitions

These are used to highlight parts of the content that are particularly useful to the reader in some fashion.
The type of usefulness is indicated by the name and icon.

> :notebook: **Note** Use this when you want to note something, that is, call it out of the text to draw attention to it.
But the attention is a neutral one, "Simply note this fact", rather than e.g. a warning or a command.

> :bulb: **Tip** This is a note about something particularly useful.
It is informative and it may contain actions that can be taken, but choice in use of the actions is clearly voluntary and low risk.

> :construction: **Caution** This is a note cautioning the reader about something.
It may be to take caution in following an action or some other caution to consider.
This implies there is a heightened but unmeasured/unspecified risk.

> :warning: **Warning** This is a note warning the reader that something is likely of a high-risk and special attention needs to be paid.

> :rotating_light: **Danger** This is a note warning of the highest levels of risk where there is still some level of choice to not do the dangerous thing.

> :no_entry: **Do not** This is a note with a command of full-stop or do not continue.
It should be considered absolute and the danger it implies is of the highest.

## Content

### Overview

The handbook strives to be as accurate and up-to-date as possible.
It is crucial that the documentation provides clear, detailed instructions that match the actual experience of someone attempting to follow those instructions.

### Terms and Language

We believe that consistency of language is extremely important to the growth of our initiative and the health of our community.
We want to ensure that the language surrounding Operate First as a whole is clear and accessible to everyone.
To aid in this effort, we have compiled a glossary of basic terms and definitions crucial to understanding Operate First.
Please refer to this [glossary][3] for explanations of these important terms.

[1]: https://www.markdownguide.org/basic-syntax/#reference-style-links
[2]: https://www.markdownguide.org/
[3]: https://github.com/operate-first/community/blob/main/glossary.md
[4]: template-handbook-article.md
[5]: technical-markup-style-guide.md
