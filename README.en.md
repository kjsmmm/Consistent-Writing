# Consistent Writing

[中文](./README.md) · [MIT License](./LICENSE)

**Revise the passage. Keep the document consistent.**

You ask AI to improve one paragraph. It gives a familiar concept a new name. A few edits later, the same term means something different, and a shorter conclusion has lost the reasoning that supported it.

Consistent Writing provides two self-contained Agent Skills for Chinese and English writing. Their core concerns are **how local edits fit the wider document, and how concepts and terminology stay clear and consistent**. Paragraph structure, defensive phrasing, and formulaic prose receive attention after the meaning is sound. Both skills also support drafting whole documents, extending sections, and shortening text.

## What should survive an edit?

| Common problem | What the skill asks AI to do |
| --- | --- |
| A stronger paragraph changes the document's claim | Check its role, scope, and connection to the wider argument |
| One concept acquires several names | Reuse established terms after checking that their meanings match |
| An impressive new label appears without explanation | Describe the meaning directly, or define a necessary new concept |
| Shortening removes the reason behind a conclusion | Preserve the evidence, conditions, distinctions, and value readers need |
| Every section sounds like the same template | Improve paragraphing and phrasing while preserving the author's voice |

## How it works

The skills use the available conversation and manuscript to establish the current writing intent and terminology. They do not require a separate brief, glossary, or state file. If an isolated excerpt lacks context that would materially change the revision, the skill asks focused questions before making dependent edits. Self-contained passages and straightforward grammar corrections can proceed directly.

The rules have a clear priority: first preserve purpose, concepts, and important information; then improve paragraph organization, remove irrelevant defensive language, and revise formulaic prose. Necessary qualifications and supported negative findings remain part of the text.

## Get started

Clone the repository, or choose **Code → Download ZIP** on the [repository page](https://github.com/kjsmmm/Consistent-Writing):

```sh
git clone https://github.com/kjsmmm/Consistent-Writing.git
```

Copy the complete folder for your writing language into your tool's skills directory and load it according to that tool's instructions. Install either skill or both. Each contains its complete rules in a single `SKILL.md`, with no scripts, packages, or external services required.

| Language | Skill folder | Invocation name |
| --- | --- | --- |
| Chinese | [clear-chinese-writing](./clear-chinese-writing/) | `$clear-chinese-writing` |
| English | [clear-english-writing](./clear-english-writing/) | `$clear-english-writing` |

Consistent Writing is the project name. Folder and invocation names remain as shown above. The installed layout should be `skills-directory/clear-english-writing/SKILL.md`, or the equivalent Chinese folder.

For tools that support `$skill-name` invocation, try:

**Revise one passage**

```text
Use $clear-english-writing to revise the following section.
Use our earlier discussion and the surrounding text to keep the purpose
and terminology consistent. Preserve the reasons behind its claims.
```

**Draft a whole document**

```text
Use $clear-english-writing to draft a proposal from these notes.
The audience is the project lead. Explain the problem, proposed approach,
and how we will evaluate the result.
```

**Shorten a draft**

```text
Use $clear-english-writing to shorten this draft to about 800 words.
Preserve the central argument, key evidence, and conditions on the conclusion.
```

For other tools, select the skill through their supported interface.

## Review the result

Check whether the revision still serves the intended purpose, whether names and definitions remain consistent, and whether the essential reasons, evidence, and qualifications are still present. The skills guide drafting and revision; results depend on the model and the context available to it.

## Feedback and contributions

[Open an issue](https://github.com/kjsmmm/Consistent-Writing/issues) with an anonymized excerpt, your request, the actual output, and the meaning you wanted to preserve. Before-and-after passages help distinguish a misunderstanding of purpose from a terminology or information-retention problem.

Pull requests are welcome. When changing shared rules, check both language versions for equivalent meaning while respecting their different writing conventions.

## License

[MIT](./LICENSE). Retain the license and copyright notice when using, modifying, or distributing the project.
