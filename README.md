# Requirements for Yi Text Layout

[简体中文](README.zh-Hans.md)

## Abstract

This document summarizes text composition requirements in the Yi writing system. One of the goals of the task force is to describe issues for Yi layout, another is to describe correspondences with existing standards (such as Unicode), as well as to encourage vendors to implement relevant features correctly.

## Introduction

The Yi people are the sixth largest ethnic minority group in China, with a population of nearly ten million. The Yi script is one of the oldest writing systems still in use among China's ethnic minorities. It is the primary carrier of Yi literature, history, and cultural knowledge, and is central to Yi cultural identity. Supporting the Yi script in digital text layout is therefore important for preserving and promoting Yi culture in the digital age.

Modern Yi is a syllabic script. In modern standardized Nuosu orthography, each syllable is represented by a Yi character and words may contain one or more syllables separated by spaces. The script has no case distinction and does not use cursive joining. Yi content is often mixed with European numerals, Latin text, and Chinese text.

Early Yi was logographic. Over time, a large number of syllabic symbols were incorporated, transforming it into a logo-syllabic script that is primarily logographic but supplemented by phonetic elements. The currently prevalent Liangshan Standard Yi script is purely syllabic, whereas Yunnan Standard Yi script remains logo-syllabic.

## Text direction

### Writing mode

The 1975 *Standardization Scheme for Yi Script* rotated traditional Yi glyphs 90 degrees clockwise, changing them from a "horizontal" posture to an upright, "vertical" one and changing the writing direction from vertical to horizontal.

Modern Yi text MUST support horizontal, left-to-right layout. The default inline progression is left to right and the block progression is top to bottom.

Historical material may use vertical writing mode. Implementations SHOULD support Yi in vertical writing mode, but the preferred text direction and punctuation orientation need validation with source material.

### Bidirectional text

Classical Yi characters are generally written horizontally or vertically from left to right in Yunnan, Guizhou, and Guangxi, while in Sichuan they are written horizontally or vertically from right to left. The new standard Yi script is written horizontally from left to right.

## Glyph shaping and positioning

### Fonts and font styles

TBD

### Context-based shaping and positioning

Yi syllables MUST NOT be joined, ligated, reordered, or substituted according to neighboring Yi syllables.

### Cursive text

Yi MUST be treated as non-cursive text.

## Typographic units

### Characters and encoding

Unicode officially included the Liangshan Standard Yi script in version 3.0. The encoding range for Yi syllables is U+A000–U+A48C, comprising 1,164 syllables (syllables with diacritics are encoded individually and cannot be decomposed into a base syllable plus a combining diacritic) and one syllable iteration mark (U+A015 ꀕ, erroneously named "YI SYLLABLE WU"). The encoding range for Yi radicals is U+A490–U+A4CF, comprising 55 radicals.

In 2007, China submitted a proposal to encode the Yunnan Standard Yi script, but it has not yet been included in Unicode, nor has a code block been allocated for it.

### Grapheme, word segmentation, and selection

Grapheme segmentation algorithms MUST segment each Yi syllable as one grapheme cluster.

## Punctuation and inline features

### Phrase and section boundaries

Traditional Yi script has no standard punctuation marks. The standardized modern Yi script utilizes the punctuation marks in Chinese.

### Emphasis and highlighting

TBD

### Inline notes and annotations

TBD

### Other text decoration and inline features

TBD

## Lines and paragraphs

### Line breaking

TBD

### Hyphenation

User agents MUST NOT insert a hyphen between Yi syllables.

### Text alignment and justification

The default alignment for horizontal Yi prose MUST be left.

### Text spacing

TBD

### Lists, counters, and initials

TBD

## Layout and pages

### General page layout and progression

TBD

### Grids and tables

TBD

### Footnotes and endnotes

TBD

### Page headers and footers

TBD

### Forms and user interaction

TBD

## Open questions

* Which Yi varieties besides modern Nuosu require distinct word-segmentation, punctuation, or number-format rules?
* Does vertical-writing exist in contemporary or historical Yi publications?
* Any emphasis marks and annotation styles?
* …
