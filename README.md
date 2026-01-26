# Bibliography

This repository hosts the BibTeX library for my research and publications. It is automatically synchronized with my Zotero library to ensure the latest citations are always available for LaTeX and Markdown workflows.

## Contents

* `references.bib`: The primary BibTeX file containing all top-level items from the Zotero library.

## Automation Details

This repository is **auto-generated**. Manual changes to the `.bib` file should be avoided as they will be overwritten during the next synchronization cycle.

- **Source:** [Zotero](https://www.zotero.org/)
- **Sync Frequency:** Daily via Cron Job 
- **Generator:** Zotero Web API (BibTeX Export)

## Usage

### Linking to LaTeX/Overleaf
You can pull this bibliography directly into your LaTeX projects using the raw GitHub URL:
`https://raw.githubusercontent.com/jcpru/references/main/references.bib`

## Citations

This repository uses a custom key generation algorithm implemented via a cloud-based Python sync script. This ensures consistency regardless of how items are added to the Zotero library.

### Key Format
The citation keys follow the pattern:  
`[first_author_lowercase][year][first_word_of_title_lowercase]`

**Example:**
* **Author:** Abidi, Nawras
* **Year:** 2020
* **Title:** Revisiting the Active Sites...
* **Generated Key:** `abidi2020revisiting`

### Duplicate Handling
In the event of multiple entries sharing the same author, year, and title-start, the script automatically appends an alphabetical suffix (`a`, `b`, `c`, etc.) to maintain unique keys within the `.bib` file.

> [!IMPORTANT]
> Since keys are generated during the sync process on the VPS, the citation keys seen here may differ from the default keys shown in the Zotero web interface or desktop client. Always refer to `references.bib` in this repository for the definitive key.

---
*Maintained by jcpru*
