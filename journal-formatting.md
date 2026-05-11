---
name: journal-formatting
description: Format academic manuscripts for journal submission. Use when the user asks to revise, format, convert, or prepare a manuscript or DOCX according to a journal's author guidelines, including requests in Chinese such as 按期刊要求改格式, 投稿格式, 修订版, 清洁版, tracked changes, comments, or preserve the original manuscript.
---

# Journal Formatting

Use this skill whenever the user asks to format a manuscript for any journal.

## Core Rules

1. Always use the latest official journal author guidelines. Browse and cite the official guideline page unless the user provides a current guideline file.
2. Preserve the original manuscript and all original submission materials. Never overwrite the source file.
3. Deliver only two main manuscript files by default:
   - a clean manuscript version
   - a manuscript version with comments and true Word tracked changes
4. The tracked-changes manuscript must contain real Word revisions. When possible, generate it by comparing the original manuscript with the formatted clean manuscript. Verify revision counts before delivery.
5. Do not change in-text citation style unless the user explicitly asks for citation formatting.
6. Do not change reference entry formatting or reference text unless the user explicitly asks for reference formatting.
7. Do not directly edit figures, tables, graphical abstracts, supplementary files, or other separate submission materials. If the journal guidelines require changes to these items, add comments in the tracked/commented manuscript instead.
8. Use comments for author-confirmation items, including corresponding author details, ethics/IRB wording, consent wording, data availability, funding, competing interests, author contributions, AI-use statements, graphical abstract requirements, table/figure requirements, and supplementary material requirements.
9. Before delivery, render and visually inspect the DOCX files when possible.
10. After the task is complete, clean up intermediate files such as scripts, render folders, comparison folders, PDFs, temporary DOCX files, and obsolete versions. Keep only the two final main manuscript files unless the user asks otherwise.

## Workflow

1. Identify the target journal and source manuscript.
2. Confirm the latest official author instructions from the journal or publisher website. If the user provides an official PDF or template and says it is the final version, use it as the primary source.
3. Read the manuscript structure before editing: title page, abstract, keywords, headings, declarations, references, tables, figures, and supplementary references.
4. Make only formatting and structure changes required by the journal and allowed by the user's rules.
5. Add comments instead of changing items that require author confirmation or separate non-main-manuscript files.
6. Save the clean manuscript as a new DOCX in the same folder as the source manuscript.
7. Create the tracked/commented manuscript by comparing the source manuscript with the clean manuscript, then add comments and ensure Track Changes is enabled.
8. Verify:
   - source manuscript unchanged
   - clean manuscript has zero revisions and zero comments
   - tracked/commented manuscript has real revisions and comments where needed
   - final files render without obvious layout problems
9. Remove intermediate artifacts and leave the two final main manuscript files.

## Default Output Names

Use clear names based on the journal, for example:

- `manuscript_<journal>_clean.docx`
- `manuscript_<journal>_comments_revisions.docx`

Use ASCII filenames when practical. If the folder already contains final files for the same journal, overwrite only those generated outputs after confirming they are not the original manuscript.

## Important Exceptions

- If the user explicitly asks to change citations or references, then apply the journal's citation/reference format and note that this was user-approved.
- If the user explicitly asks to merge tables or figures into the main manuscript, then do so for that task only.
- If the journal requires separate checklists, cover letters, graphical abstracts, highlights, or supplementary formatting, do not create or edit them by default. Add a comment in the tracked/commented manuscript or briefly tell the user unless they explicitly ask for those files.
- If a publisher requires information the manuscript does not contain, do not invent it. Add a comment asking the author to confirm or provide the missing information.
