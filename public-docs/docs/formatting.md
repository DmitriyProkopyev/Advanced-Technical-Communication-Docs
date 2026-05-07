# Formatting

Even the best designed texts are difficult to decipher when their visual presentation is **monotonous**. To ensure **readability** of your documents, apply the following formatting elements to your text:

| Formatting Elements | Use Cases                                                                                                 | Recommendations                                                                                                                               |
| ------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Callouts            | Highlight important info, warnings, or tips                                                               | Keep the callouts short (up to 4 sentences) and avoid duplicating the main text                                                               |
| Tabs                | Separate parallel variants of the same action (different OSes, platforms, or delivery methods)            | Do not use tabs for unrelated pieces of content                                                                                               |
| Code blocks         | Include multi-line code, configs, CLI outputs, etc. Use monospace inline code blocks for single commands. | Specify the language of the code block explicitly.                                                                                            |
| Tables              | Compare similar items or show structured data                                                             | Double check that your tables are responsive and readable on small screens                                                                    |
| Numbered lists      | Describe procedures that must be executed in a precise sequence                                           | Avoid nesting lists deeper than two levels                                                                                                    |
| Bullet lists        | Describe enumerations of elements that have no ordinal relations                                          | Avoid nesting lists deeper than two levels                                                                                                    |
| Image galleries     | Show related images with consistent aspect ratios                                                         | Include at most 4 to 5 images, supplement each with a short caption                                                                           |
| Mermaid diagrams    | Showcase flows, complex procedures, architectures, and interactions                                       | Keep the diagram code clean and maintainable in the repository                                                                                |
| LaTeX snippets      | Show precise mathematical notations                                                                       | Keep the equation style consistent with domain conventions                                                                                    |
| Links               | Refer to other documents or external resources                                                            | Attach the links to the words that intuitively communicate what materials the link refers to                                                  |
| Headings            | Split materials into cohesive sections                                                                    | Define and apply a consistent heading hierarchy (H1–H4), capitalization rules, and predictable section ordering within similar document types |

> [!question] Links
> To facilitate navigation of your documentation by the readers, make sure to:

> - Use only **relative** paths in Markdown, never link to absolute local paths like `C:/Users/...`.
> - Use anchor links to direct the reader's attention towards important document sections.
> - Use auto-generated tables of content with stable links.

___

## Visuals

When demonstrating complex or hard-to-describe concepts, include **visual elements** into the text. Use colors, positions, and sizes to guide the reader's attention.

> [!warning] Caution
> Be careful not to confuse your readers by visual fragmentation. Instead, pick a coherent visual theme and stick to it across all pages.

Additionally, apply these tips to ensure a smooth visual experience for your readers:

> [!tip] Tips
>
> - Store images under a **predictable** and meaningfully named path (e.g. `docs/assets/images/`) to avoid misplacing the links.
> - Use **descriptive** file names for all imported assets (e.g. `controller-flow.png` instead of `image1.png`).
> - Compress large assets to improve load time.
> - Prefer SVG format for diagrams, logos, and other images that should be scalable.
