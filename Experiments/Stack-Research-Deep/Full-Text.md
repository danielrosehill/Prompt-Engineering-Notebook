# Deepening Stack Research - A ChatGPT Prompting Experiment

## Experiment Summary

**Model, Platform:** GPT 4o, ChatGPT, Web UI

The purpose of this prompting experiment was to probe the ability of ChatGPT to generate a more comprehensive tech evaluation list output integrating a series of steps into one long prompt. 

## Outcomes

- GPT successfully retrieved the 12 requested variables for knowledge base management tools maintaining a consistent format throughout the output.
- The prompt output successfully transitioned to the second stage, refining the "longlist" into a shortlist based upon the presence or absence of 3 "hard requirement criteria"
- The output did not succeed in the third and final stage of the prompt which requested that GPT pick a "winner" from the shortlist based upon one (rather nebulous) criteria of scability

Overall - an impresive generation. 

---

## Prompt Text (Raw)

Please provide an overview of 10 SaaS tools for building up a comprehensive knowledge base. 

For every tool that you discover, please output the following details:

- Name of the solution
- Does it have an Android app?
- Does it have a Linux desktop app? 
- Does it have a desktop app for Fedora linux?
- Is it backed by Postgres? If not, what database?
- Does it have native support for markdown?
- Details about the product
- Is it scalable and suitable for enterprise?
- What level of scale can it achieve? How many files?
- Does it allow users to backup their data? If so, how?
- Link to the project
- Price and pricing structure

At the end of the output, please provide a new section called Shortlist

In this section, include a summary of the tools which meet all of these criteria:

- Has an Android app
- Support markdown
- Offers the ability to backup data

Finally, provide a section called Top 3 GPT Recommendations

Recommend 3 solutions from the shortlist and pick whichever one you think is best and offers the best scalability

## Sample Output

### Overview of 10 SaaS Tools for Building a Knowledge Base

#### 1. **Notion**
- **Android App:** Yes
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** A versatile tool for note-taking, task management, and wiki creation.
- **Scalable:** Yes, used by teams and enterprises.
- **Scale:** Unlimited blocks (files/pages).
- **Backup:** Yes, export options in HTML, Markdown, CSV.
- **Link:** [Notion](https://www.notion.so/)
- **Price:** Free; $8/user/month for teams.]#

#### 2. **Confluence**
- **Android App:** Yes
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary (Atlassian's infrastructure)
- **Markdown Support:** Yes (with plugins)
- **Details:** Team collaboration and documentation tool.
- **Scalable:** Yes, used by large enterprises.
- **Scale:** Suitable for extensive documentation.
- **Backup:** Yes, export in XML or PDF.
- **Link:** [Confluence](https://www.atlassian.com/software/confluence)
- **Price:** Free for up to 10 users; starts at $5/user/month.

#### 3. **Document360**
- **Android App:** No
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** Knowledge base platform for self-service documentation.
- **Scalable:** Yes, enterprise-friendly.
- **Scale:** Handles large volumes of documents.
- **Backup:** Yes, export in HTML or PDF.
- **Link:** [Document360](https://document360.com/)
- **Price:** Starts at $99/project/month.

#### 4. **Helpjuice**
- **Android App:** No
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** Customizable knowledge base with advanced search and analytics.
- **Scalable:** Yes, enterprise-friendly.
- **Scale:** Manages extensive repositories.
- **Backup:** Yes, data export options available.
- **Link:** [Helpjuice](https://helpjuice.com/)
- **Price:** Starts at $120/month for up to 4 users.

#### 5. **Guru**
- **Android App:** Yes
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** Internal wiki tool with integrations for capturing and sharing knowledge.
- **Scalable:** Yes, suitable for medium to large enterprises.
- **Scale:** Handles large-scale knowledge bases.
- **Backup:** Yes, export options available.
- **Link:** [Guru](https://www.getguru.com/)
- **Price:** Free for small teams; $5/user/month for paid plans.

#### 6. **BookStack**
- **Android App:** No
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** MySQL/MariaDB (with Postgres support in development)
- **Markdown Support:** Yes
- **Details:** Open-source documentation platform structured like a book.
- **Scalable:** Yes, used by teams and small enterprises.
- **Scale:** Can handle a large number of pages and chapters.
- **Backup:** Yes, supports full database backups.
- **Link:** [BookStack](https://www.bookstackapp.com/)
- **Price:** Free, open-source.

#### 7. **Slite**
- **Android App:** Yes
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** Team collaboration tool focused on documentation and note-taking.
- **Scalable:** Yes, suitable for teams and small enterprises.
- **Scale:** Unlimited documents.
- **Backup:** Yes, data export available.
- **Link:** [Slite](https://slite.com/)
- **Price:** Free; $6.67/user/month for Standard.

#### 8. **Tettra**
- **Android App:** Yes
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** Knowledge management software for creating internal wikis.
- **Scalable:** Yes, used by teams and medium-sized enterprises.
- **Scale:** Handles numerous articles and pages.
- **Backup:** Yes, data export in PDF or HTML.
- **Link:** [Tettra](https://tettra.com/)
- **Price:** $8.33/user/month.

#### 9. **ProProfs Knowledge Base**
- **Android App:** No
- **Linux Desktop App:** No (Web-based)
- **Fedora Support:** No
- **Database:** Proprietary
- **Markdown Support:** Yes
- **Details:** Easy-to-use knowledge base tool for creating help centers and FAQs.
- **Scalable:** Yes, suitable for small to medium businesses.
- **Scale:** Manages up to hundreds of articles.
- **Backup:** Yes, data export available.
- **Link:** [ProProfs Knowledge Base](https://www.proprofskb.com/)
- **Price:** Starts at $49/author/month.

#### 10. **BookStack**
- **Android App:** No
- **Linux Desktop App:** Yes
- **Fedora Support:** Yes
- **Database:** MySQL/PostgreSQL
- **Markdown Support:** Yes
- **Details:** Free and open-source documentation software.
- **Scalable:** Yes, can be used by individuals to large enterprises.
- **Scale:** Unlimited storage, depending on server capacity.
- **Backup:** Yes, can backup and export content in HTML or PDF formats.
- **Link:** [BookStack](https://www.bookstackapp.com/)
- **Price:** Free (Open-source).

#### 11. **Obsidian**
- **Android App:** Yes
- **Linux Desktop App:** Yes
- **Fedora Support:** Yes
- **Database:** Markdown files (locally stored)
- **Markdown Support:** Yes
- **Details:** A note-taking and knowledge base app that works with local Markdown files.
- **Scalable:** Yes, depending on storage.
- **Scale:** Unlimited, based on local storage.
- **Backup:** Yes, supports external backups.
- **Link:** [Obsidian](https://obsidian.md/)
- **Price:** Free for personal use; $25/year for commercial use.

(Additional tools would be listed similarly, providing details as above)

### Shortlist

**Tools that meet the criteria of having an Android app, support Markdown, and offer data backup:**

1. **Notion**
2. **Confluence**
3. **Document360**
4. **Guru**
5. **Slite**
6. **Obsidian**
7. **Tettra**
8. **BookStack**

### Top 3 GPT Recommendations

#### 1. **Notion**
- **Why:** Notion is highly versatile, supports Markdown, offers extensive backup options, and scales well from small teams to large enterprises.
- **Best for:** Teams needing a multi-purpose tool for documentation, project management, and knowledge bases.

#### 2. **Obsidian**
- **Why:** Obsidian is ideal for those who prefer local control over their data, with strong Markdown support, Linux desktop apps, and extensive backup options.
- **Best for:** Individuals and teams focused on local, encrypted data management.

#### 3. **Confluence**
- **Why:** Confluence offers deep integrations with other Atlassian products, making it a strong choice for enterprises needing a robust, scalable knowledge management system.
- **Best for:** Large organizations that need tight integration with project management tools like Jira.

---

## Iterative Improvement 

The final section of the prompt is the obvious starting point for first improvements before looking more carefully at the actual findings and trying to decipher how to improve the overall usefulness of the evaluation list.

The third section is:

```
Finally, provide a section called Top 3 GPT Recommendations

Recommend 3 solutions from the shortlist and pick whichever one you think is best and offers the best scalability
```

It should be reworked to be more explicit. An idea for V2 is:

```
Finally, provide a section called Winner, Runner Up

Identify the best solution from those listed in the previous section. Judge the "best" solution by the tool with the best ability to scale. List this under a heading called "The Winner."

Next, identify the second best solution from those listed in the previous section. Use the same criteria as before to make this determination. List this under a heading called "Runner Up"

```