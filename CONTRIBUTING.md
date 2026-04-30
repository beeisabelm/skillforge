# Contributing

This curriculum gets better when practitioners share what worked. Here's how to contribute.

## What we welcome

| Contribution | Where it goes |
|---|---|
| **A new real-world scenario** you ran successfully | [scenarios/](scenarios/) |
| **A new audience adaptation** (your industry, your format) | [adaptations/](adaptations/) |
| **Updated Microsoft Learn module references** (titles change) | The relevant `tracks/*.md` |
| **A template** that worked for you | `templates/` (open a PR to create the directory if needed) |
| **A correction** (typo, broken link, outdated info) | Inline edit + PR |
| **A question / gap** that's not yet covered | Open an issue |

## What we don't accept

- **Proprietary content** — anything under NDA, internal-only, or customer-confidential
- **Personal data** — names, emails, customer identifiers, screenshots of internal tools
- **Vendor-specific scenarios that exclude alternatives** — keep examples vendor-neutral where possible
- **Marketing copy** — this is educational content, not sales material

## How to contribute

1. **Open an issue first** if your contribution is more than a typo fix. A 2-line description of what you want to add saves rework.
2. **Fork → branch → PR.** Standard GitHub flow.
3. **Use the existing structure.** Look at sibling files for tone, level of detail, and formatting.
4. **One scenario per file.** Don't bundle multiple scenarios into one PR.
5. **Cite sources.** If you reference a study, framework, or external article, link to it.

## Style

- **Plain English.** No internal jargon, no acronyms without expansion on first use.
- **Active voice.** "Run the session" not "the session is run."
- **Vendor-neutral when possible.** "AI assistant" rather than naming a product unless the product specifically matters.
- **Short paragraphs.** Three sentences max. Use bullets and tables freely.
- **Verifiable claims.** If you write "this works X% of the time," cite the source or remove the number.

## Maintainer review

Maintainers will review PRs within ~1 week. We may suggest edits for tone, structure, or scope. Major restructures may take longer or be deferred to a planning discussion.

## Quarterly link verification

Microsoft Learn module titles and URLs change. Every quarter, a maintainer or contributor walks the canonical link list at [`tracks/_module-index.md`](tracks/_module-index.md) and:

1. Opens each URL in the index. If it 404s or redirects to an unrelated page, mark `❌` and file an issue.
2. Compares the listed title against the page's current title. If retitled, update the index *first*, then update every track-file occurrence.
3. Updates the **Last verified** date for each row that's still good.
4. Re-checks any rows in the **Pending verification** section to see if a canonical URL is now available.
5. Opens a single PR with all link updates, with the title `chore: quarterly link verification — YYYY-Q#`.

The index is the single source of truth. If a track file disagrees with the index, the index wins.

## Code of conduct

Be respectful. Disagree with ideas, not people. Assume good intent. If something feels off, [open an issue](../../issues) or contact the maintainer directly.
