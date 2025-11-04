# AI Agent Instructions: Research and Format Project Entries

## Overview

Your task is to research and format AI agent project entries in the README.md file. You will process unprocessed items (bullet points with URLs) and convert them into formatted table entries.

## Table Format

Each section should have a table with the following columns:

```markdown
| Project | Description | Open-Source | GitHub | Runtime | Released |
|---------|-------------|-------------|--------|---------|----------|
```

### Column Specifications

**Project:**
- Format: `**[Project Name](URL)**`
- Make the link bold
- If there's a parent organization different from the project name, add it in parentheses: `**[Project Name](URL)** (by Organization)`
- **CRITICAL:** Pay special attention to the exact spelling of project names, including:
  - Capitalization (e.g., "Superdesign" not "SuperDesign", "TRAE" not "Trae")
  - Spaces vs. hyphens (e.g., "Project Name" vs. "Project-Name")
  - Special characters or styling
- **To verify official spelling, check IN THIS ORDER:**
  1. **Primary source (official website):**
     - Copyright notice at the bottom (e.g., "©2025 TRAE. All rights reserved.")
     - Legal documents (Terms of Service, Privacy Policy, About pages)
     - Logo and branding as displayed on the official site
  2. Secondary sources (news articles) - use only if primary source is unclear
  - **NEVER** rely solely on how journalists or bloggers spell the name
  - Primary sources are ALWAYS more authoritative than secondary sources

**Description:**
- If the unprocessed item has text after the URL (e.g., `- https://example.com: foo bar baz`), use that text as the description
- Only fix obvious typos if present
- If the unprocessed item has only a URL, create a single short sentence description
- Maximum length: 80 characters (if possible)
- Avoid buzzwords like "AI-powered", "revolutionary", "cutting-edge"
- Avoid qualitative adjectives like "fast", "powerful", "best", "professional", "amazing"
- Keep it factual and concise
- End with a period

**Open-Source:**
- Use ✅ for open-source projects
- Use ❌ for closed-source projects

**GitHub:**
- If open-source with a GitHub repository: `[user/repo](https://github.com/user/repo) (⭐️ ~Xk)`
- Format: Shorten URL to `user/repo` in the link text
- Add star count in format: `(⭐️ ~X.Xk)` for thousands, `(⭐️ ~X)` for under 1k
- Round to one decimal place for thousands (e.g., 5214 → ~5.2k, 847 → ~800, 12543 → ~12.5k)
- If no repository: ❌

**Runtime:**
- Use emoji icons based on where/how the project runs:
  - 💻 CLI: Command-line interface tool (runs in terminal)
  - 🖥️ Binary: Standalone application to install locally (e.g., desktop IDE or editor)
  - 🧩 Plugin: Extension or plugin for existing software (e.g., IDE extensions, editor plugins)
  - 🌍 Web: Web-based application (accessed through a browser)
- If a project supports multiple runtimes, include all applicable emoji icons (e.g., `💻 CLI, 🌍 Web`)

**Released:**
- Format: `[Mon YYYY](source-url)`
- Example: `[Oct 2025](https://news.ycombinator.com/item?id=12345)`
- Link to a reliable source documenting the release date
- **Finding approximate dates is better than "Unknown"**:
  - Look for Product Hunt launch pages (e.g., producthunt.com/products/[name]/launches)
  - Look for Hacker News launch posts (e.g., "Show HN" or "Launch HN" posts on news.ycombinator.com)
  - Articles dated shortly after launch often indicate launch timeframe
  - Multiple sources saying "recently launched" around the same time period
  - Even if you can't find the exact date, finding the month/year is acceptable
  - Being off by a few days or even one month is better than "Unknown"
- Only use `Unknown` (no link) if truly no evidence of launch timeframe can be found after exhaustive research

## Research Requirements

For each unprocessed item, research the following:

### 1. Project Name
- Official name of the project
- **Verify exact spelling from primary sources:**
  - Check copyright notice on official website (e.g., "©2025 TRAE. All rights reserved.")
  - Check legal documents (Terms of Service, Privacy Policy)
  - Look at logo and branding on official site
  - Do NOT rely solely on secondary sources (news articles, blog posts)
- Verify capitalization, spaces, and hyphens
- Parent organization (only if different from project name)

### 2. Runtime
- Determine where/how the project runs:
  - **💻 CLI:** Runs in a terminal/command line
  - **🖥️ Binary:** Standalone desktop application to install locally (e.g., IDE, editor)
  - **🧩 Plugin:** Extension for existing software (e.g., VS Code extension, browser plugin)
  - **🌍 Web:** Web-based service accessed through a browser
- If the project supports multiple runtimes, list all applicable types

### 3. Open-Source Status
- Is the code publicly available?
- Check for GitHub, GitLab, or other public repositories

### 4. GitHub Repository
- If open-source, find the GitHub repository URL
- Get the current star count
- Format as `user/repo` with star count

### 5. Release Date
- **CRITICAL:** Take extra care when researching release dates
- **Priority: Find at least the month/year** - this is better than "Unknown"
- Sources to check (in order of reliability):
  1. Official launch announcements (company blog, press releases)
  2. Product Hunt launch page (producthunt.com/products/[name]/launches)
  3. Hacker News launch posts (search for "Show HN" or "Launch HN" on news.ycombinator.com)
  4. Wikipedia with cited sources
  5. News articles dated shortly after launch
  6. Multiple sources mentioning "recently launched" around the same timeframe
- **Inferring approximate dates is acceptable:**
  - An article from October 2025 about a "newly launched" product → likely Oct 2025
  - Multiple sources in early November saying "launched a few days ago" → likely late Oct or early Nov 2025
  - Being off by a few days or even one month is acceptable
- Do NOT use company founding dates unless explicitly stated as the release date
- Link to the most specific source you found (Product Hunt page > Hacker News post > news article > general reference)
- Only use `Unknown` if absolutely no evidence of launch timeframe exists after exhaustive research

### 6. Description
- If text exists after the URL in the bullet point, use it (with typo fixes only)
- If no text exists, create a concise single-sentence description
- Avoid marketing language and qualitative adjectives
- Be factual and neutral

## Research Process

1. **Use WebSearch** to find information about the project
2. **Use WebFetch** to visit the project's official website:
   - **Check copyright notice** for official spelling (e.g., "©2025 TRAE. All rights reserved.")
   - Check Terms of Service / Privacy Policy for official company name
   - Look at logo and branding
3. **Verify release dates** carefully:
   - Check Product Hunt launch page first (producthunt.com/products/[name]/launches)
   - Check Hacker News for launch posts (search for "Show HN" or "Launch HN")
   - Check Wikipedia with cited sources
   - Look for official blog posts or announcements
   - Search for "launched" or "released" in news articles
   - Look at article publication dates - articles about "newly launched" products indicate timeframe
   - Multiple sources saying "recently launched" around same time indicate approximate launch date
   - Finding month/year is better than saying "Unknown"
4. **Check GitHub** for repository details and star counts

## Updating Existing Entries

For existing table entries with GitHub repositories:

1. Visit each GitHub repository URL
2. Get the current star count
3. Update the star count in the format `(⭐️ ~X.Xk)` or `(⭐️ ~X)` (rounded to one decimal place for thousands)
4. ONLY update the GitHub star count. Do NOT change any other fields (project name, description, type, release date, etc.)

## Handling Mixed Processed and Unprocessed Items

A section may contain:
- **Only unprocessed items** (bullet list): Create a new table
- **Only processed items** (table): Update star counts and "Last updated" date
- **Both processed and unprocessed items** (table + bullet list): Add new rows to the existing table

When a table already exists:
1. Add new rows to the existing table for unprocessed items
2. Append new entries to the end of the table in the same order as they appear in the bullet list
3. Remove the bullet points after adding them to the table
4. The "🤖 Content researched by AI. Last updated YYYY-MM-DD." line already exists below the table
5. Update the date in that line to today's date

## Final Steps

After processing all items in a section:

1. Remove the processed bullet points
2. If no "🤖 Content researched by AI. Last updated YYYY-MM-DD." line exists, add it below the table
3. If the line already exists, update the date to today's date
4. Use today's date in ISO format (YYYY-MM-DD)

After processing ALL sections in the README:

1. Update ALL "Last updated" dates below tables to today's date
2. Update the top-level "Content last updated" line near the beginning of README.md (format: `_**🤖 Content last updated YYYY-MM-DD by AI.**_`) to today's date

## Example Transformations

### Example 1: New Section (Only Unprocessed Items)

**Before:**
```markdown
## General

- https://example.com/tool: helps with testing
- https://another-tool.io
```

**After:**
```markdown
## General

| Project | Description | Open-Source | GitHub | Runtime | Released |
|---------|-------------|-------------|--------|---------|----------|
| **[ExampleTool](https://example.com/tool)** | Helps with testing. | ✅ | [user/example-tool](https://github.com/user/example-tool) (⭐️ ~3.2k) | 💻 CLI | [Mar 2024](https://github.com/user/example-tool/releases) |
| **[AnotherTool](https://another-tool.io)** | Creates automated workflows for development teams. | ❌ | ❌ | 🌍 Web | [Jan 2025](https://news.ycombinator.com/item?id=12345) |

🤖 Content researched by AI. Last updated 2025-11-04.
```

### Example 2: Existing Table with New Unprocessed Items

**Before:**
```markdown
## General

| Project | Description | Open-Source | GitHub | Runtime | Released |
|---------|-------------|-------------|--------|---------|----------|
| **[ExampleTool](https://example.com/tool)** | Helps with testing. | ✅ | [user/example-tool](https://github.com/user/example-tool) (⭐️ ~3.0k) | 💻 CLI | [Mar 2024](https://github.com/user/example-tool/releases) |

🤖 Content researched by AI. Last updated 2025-10-15.

- https://newproject.com
```

**After:**
```markdown
## General

| Project | Description | Open-Source | GitHub | Runtime | Released |
|---------|-------------|-------------|--------|---------|----------|
| **[ExampleTool](https://example.com/tool)** | Helps with testing. | ✅ | [user/example-tool](https://github.com/user/example-tool) (⭐️ ~3.2k) | 💻 CLI | [Mar 2024](https://github.com/user/example-tool/releases) |
| **[NewProject](https://newproject.com)** | Manages infrastructure deployments. | ✅ | [company/newproject](https://github.com/company/newproject) (⭐️ ~1.8k) | 🖥️ Binary | [Sep 2024](https://newproject.com/blog/launch) |

🤖 Content researched by AI. Last updated 2025-11-04.
```

Note: The star count was updated from ~3.0k to ~3.2k and the date was updated to today.

## Quality Guidelines

1. **Accuracy:** All information must be verified from reliable sources
2. **Consistency:** Follow the exact format specifications
3. **Neutrality:** Avoid promotional language
4. **Completeness:** Research all required fields
5. **Verification:** Double-check release dates with reliable sources, but approximate dates (month/year) are better than "Unknown"
6. **Timeliness:** Update all "Last updated" dates to current date when processing
7. **Spelling:** ALWAYS verify exact project name spelling from primary sources (copyright notices, legal documents) - NEVER rely solely on secondary sources like news articles

## Important Notes

- Process ALL unprocessed items in the README (all sections)
- Update star counts for ALL existing GitHub repositories
- For existing items: ONLY update the GitHub star count, do NOT modify any other fields
- Update ALL "Last updated" dates to today's date (both at the top of the document and below each table)
- Update the top-level "Content last updated" line near the beginning of README.md with today's date
- Be especially careful with release date research
- Maintain consistent formatting throughout
