# laws-and-regulations

The **EU AI Act**, the **GDPR** and the Commission's **guidelines on AI Act Article 5**, split into one file per article, recital, annex or guideline section, so an AI agent (or a person) can open exactly the rule it needs instead of the whole text.

Every file carries its citation, its chapter, its size, and whether the 2026 amendment changed it. Each ends with links to what it cites, what cites it, and which review areas use it. Nothing is paraphrased: the text is the source text, split and linked.

It also holds a hand-written guide for checking a product requirements document (PRD) against these laws: which rules reach it, what it breaks, what it misses, what depends on facts it doesn't give.

This is a reading aid, not legal advice. The consolidated AI Act text has no legal effect; the Official Journal versions do.

## What's in it

**AI Act**: Regulation (EU) 2024/1689, EUR-Lex consolidated text of 27.07.2026, including amendment M1 (Regulation (EU) 2026/1744). Changed wording is marked `▼M1`. No recitals. **GDPR**: Regulation (EU) 2016/679 as published in 2016, all articles and all 173 recitals, without later corrections. **Art 5 guidelines**: Commission guidelines C(2025) 5052, not binding, written before M1.

Cite as `AI Act Art 26(1)`, `GDPR Art 6(1)(f)`, `GDPR Recital 71`, `Art 5 Guidelines para 243`.

## Check a PRD

Start at [review-map/CONTEXT.md](review-map/CONTEXT.md). It reads the PRD once, screens it for scope and for banned practices, picks the review areas that apply, answers each from the article files (never from memory), and writes a report: scope, findings marked **breaks**, **missing** or **decide**, and what wasn't checked. [timeline.md](review-map/timeline.md) says when each rule starts to apply; [not-covered.md](review-map/not-covered.md) says what this library leaves out.

## Rebuild

```
python3 _system/build.py
```

Rebuilds `ai-act/`, `gdpr/`, `guidelines-art5/` and `_index/` from the three texts in `_sources/`. It checks that every source line landed in exactly one file, word for word, and that every link resolves. To update a law, replace its file in `_sources/` and rerun.

## Layout

```
laws-and-regulations/
├─ CLAUDE.md          read order for an agent: where to go for which task
├─ ai-act/            one file per article and annex, by chapter, with a list file
├─ gdpr/              one file per article and recital, by chapter
├─ guidelines-art5/   the Art 5 guidelines, one file per section
├─ _index/            definitions of defined terms, with links
├─ review-map/        the PRD check: 13 review areas, timeline, what's not covered
├─ _sources/          the three original texts, never edited
└─ _system/           build.py: splits, links and verifies everything above
```

`ai-act/`, `gdpr/`, `guidelines-art5/` and `_index/` are generated. Change `_sources/` or `build.py`, not those.
