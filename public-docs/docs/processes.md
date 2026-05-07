# Internal Processes

The products or services any documentation is meant to explain tend to constantly change. To explain them well, the documentation must also change. To uphold the documentation quality standards throughout changes, certain **processes** need to be put in place.

Below is a concise and **actionable** guide to set up these processes.

## Documentation guidelines

First, define the scope, expectations, standards, and guidelines for your project/service documentation.

> [!question] Decision Factors
> Evaluate the following questions:
> 
> - Does the documentation scope cover many products or product locales?
> - Is the documentation scope under the effect of any regulatory constraints?
> - Is the cost of error high in your domain?

If you mostly answered "yes", then develop **your own** style guide and keep it tightly integrated into your tooling (linters, templates, CI). Otherwise, borrow a **public guide** that matches your desired tone and voice, then incrementally record only the rules you actually use, until growth justifies a custom guide.

___

## Process Design

Next, design and document the process of documentation development, tie it to the stages of your product/service SDLC. Answer the following questions to define the relevant procedures:

1. Who is responsible for gathering **accurate** information about the product or service?

    1.1. Who or what will the **accurate** information about product or service changes come from?

    1.2. Who has the **final** authority in case of information accuracy disagreements?

2. Who will draft the initial documentation changes?

    2.1. If several authors will work together, how will they collaborate?

3. Who or what will review the drafts and give feedback?

    3.1. Where are the documentation guidelines defined?

    3.2. Which documentation guidelines should be specified?

    3.3. Who **owns the terminology** and has the final authority in case of diagreements related to it?

    3.4. Who **owns** the voice and tone **standards** and has the final authority in case of disagreements related to them?

    3.5. Who has the final authority to decide whether to **release** the changes?

4. How will any review disagreements be reflected in the documentation guidelines?

5. How will the drafts be revised in case of rejection?
6. How will the changes be released in case of approval?

    6.1. Will the release (deployment) process be automatic or manual?
    
    6.2. Who is responsible for timely and seamless releases?
    
7. Will the product/service and documentation changes require a changelog?

    7.1. Who is responsible for writing, reviewing, and releasing the changelog?

> [!success] Recommended Rules
> Consider following these rules for greater transparency:
> 
> - Use meaningful, **searchable**, and specific commit messages that describe documentation increments.
> - Create issues for planned work and changes, use meaningful, searchable, and specific issue names.
> - When resolving issues, work in **branches** named after the issues.

___

## Workspace Setup

Next, follow this checklist to prepare a documentation workspace:

1. Choose one **SSG** (Static Site Generator) to use for all connected documentations.
2. Create a dedicated documentation repository or a directory in your project repository for all future documentation.
3. Add `index.md` file at the **root** of your documentation directory to serve as a homepage.
4. Fill the homepage with necessary metadata: service name, short project description, target audience, links to key sections.
5. Design a URL structure that is **intuitively navigable** for your readers.
6. Explicitly configure navigation in your SSG config instead of relying on auto navigation build.
7. Set the `site_url` (or your SSG equivalent) explicitly to ensure correct canonical URLs and sitemap generation.
8. Automate **re-deployment** to a static host upon content updates.
9. Add explicit front matter (YAML metadata), a sitemap, and SEO meta tags for proper indexing by search engines.
10. Ensure users have a single stable public URL for all documentation.

> [!tip] Shannon-Weaver stages
> Identify the source, encoder, channel, decoder, destination, and noise in your documentation pipeline. This will help you identify the weak points **in advance**.
