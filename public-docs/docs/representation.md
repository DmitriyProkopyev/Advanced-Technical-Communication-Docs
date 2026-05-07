# Representation

The way in which text is represented often has **greater effect** than the meaning of the text. Below is a concise guide on fine-tuning the right representation for your documentation.

## Context Selection

Any good decision is only good in **some contexts** and not in others. Before writing any documentation, define your context by answering these questions:

- Who are your readers?
- What is **the goal** of your readers?
- How proficient are the readers in the field?
- In which situations will the readers need to read the documentation?
- What artifact types are you documenting (UI label, error message, CLI help, inline comment, tutorial, or API reference)?

> [!info] Adapting to the context
> The general advice for adapting your documents to the context is:
> 
> - Use the abstraction level your readers need to achieve their goal, i.e. differentiate between relevant and irrelevant information **from the perspective** of the goal of your reader.
> - Adjust the terminology to the proficiency level of the readers.
> - Write for exactly the use cases your readers will experience.

___

## Terminology & Semiotics

Once the context is clear, proceed to standardize the terminology of the documentation. Specifically:

1. List all key domain terms and check that each term has a single, consistent meaning.

> [!warning] Ambiguity
> Ensure each signifier (label) points unambiguously to one signified (meaning) concept. If a label is reused with different meanings, treat it as a **defect** and rename or clarify.
   
2. Maintain or update a controlled vocabulary so that every important term used in the document is defined once and reused consistently.

> [!example] Visual intuition
> For icons and UI symbols, validate that the visual sign (e.g., gear, question mark) matches common user expectations in this domain. If the visual representation is inconsistent or mismatches the user intuition, change and unify it.

___

## Structure

Then, define the documentation structure. Nearly always your readers only need a small fraction of the information presented. The more intuituve the structure of the documents is, the easier it will be for them to find the right document subset.

1. Design a URL structure that the readers will **easily understand**. Mirror this structure in your documents.
2. Group the content into files and directories by use case or reader type.
3. Make sure the homepage contains an up-to-date "entry map" to the rest of the documentation.
4. Make sure the pages are linked in an **intuitive** manner, supplementing the content of some pages with other pages.

___

## Communicative Function & Speech Acts

Then, select the right communicative function:

| Communicative Function | Use cases                                                     | Example                                           |
| ---------------------- | ------------------------------------------------------------- | ------------------------------------------------- |
| Referential            | To inform the reciever                                        | "The rate limit for this endpoint is 100 RPM."    |
| Conative               | To influence the receiver into an action                      | "Report the bug immediately."                     |
| Metalingual            | To refine the language/terminology/semantics in communication | "What exactly do you refer to by 'prerequisite'?" |
| Phatic                 | To maintain contact with the receiver                         | "Hello, how are you?"                             |

> [!tip] Choice
> Choose the dominant communicative function for **every paragraph** of the text. Referential and conative functions typically dominate in a well written documentation.

Revise your text or make the first draft of it after this step.

___

## Silence, Gaps & Edge States

It is often easier to cut the excessive than to add the missing. Before proceeding to improve the text, make sure you did not miss anything important. Evaluate this checklist:

- Review the actions that lead to **empty states** (empty lists, disabled buttons, no output, timeouts). Ensure the absense of messages/documents does not confuse the user.
- Review the edge cases that lead to unusual behavior. Ensure this behaviour does not confuse the user.
- Review the disabled or unavailable actions. Ensure their unavailability is clearly explained and does not confuse the user.

___

## Relevance & Information Value

Then, proceed to cut the excessive complexity from the text. Specifically:

- Simplify or remove the text when the cognitive effort required by it is **not justified** by the benefit it gives the reader.
- Scan for long, multi‑clause sentences and split them into shorter sentences or bullet points.
- Remove or relocate low‑value, high‑effort content (overly abstract explanations, implementation trivia) to advanced or appendix sections, keeping core flows focused on **immediate user goals**.
- Add scaffolding and examples for novices, compress wording and avoid over‑explaining basics for experts.
- Separate instructions by OS, role, or context instead of mixing them in one paragraph.   
- Use [visual scaffolding](formatting.md): numbered steps for procedures, bullet points for options, code blocks for commands, tables for parameter lists, and consistent formatting for repeated patterns.

___

## Speech-Act Audit

Finally, review the text for clarity, focus your attention on these aspects:

- Locution: Is the **literal wording** precise and unambiguous for this context?
- Illocution: Is your **intended force** clear (command, warning, reassurance, explanation)?
- Perlocution: Will a typical reader **actually take** the intended action or come away with the intended understanding, or are they likely to hesitate, ignore, or misinterpret?

> [!danger] Locales
> Keep text translation‑ready. Avoid idioms and culture‑specific references, as they will lose their meaning in other locales.
