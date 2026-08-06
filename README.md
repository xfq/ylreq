# Requirements for Yi Text Layout

## Abstract

This document summarizes text composition requirements in the Yi writing system. One of the goals of the task force is to describe issues for Yi layout, another is to describe correspondences with existing standards (such as Unicode), as well as to encourage vendors to implement relevant features correctly.

## Introduction

Modern Yi is a syllabic script. In modern standardized Nuosu orthography, each syllable is represented by a Yi syllable character and words may contain one or more syllables separated by spaces. The script has no case distinction and does not use cursive joining. Yi content is commonly mixed with European numerals, Latin text, Chinese text, and punctuation.

Early Yi was logographic. Over time, a large number of syllabic symbols were incorporated, transforming it into a logo-syllabic script that is primarily logographic but supplemented by phonetic elements. The currently prevalent Liangshan Standard Yi script is purely syllabic, whereas Yunnan Standard Yi script remains logo-syllabic.

## Text direction

### Writing mode

Modern Yi text MUST support horizontal, left-to-right layout. The default inline progression is left to right and the block progression is top to bottom.

Historical and traditional material may use vertical writing mode. Implementations SHOULD support Yi in vertical writing mode, but the preferred column order and punctuation orientation need validation with source material.

### Bidirectional text

Classical Yi characters are generally written horizontally or vertically from left to right in Yunnan, Guizhou, and Guangxi, while in Sichuan they are written horizontally or vertically from right to left. The new standard Yi script is written horizontally from left to right.

## Glyph shaping and positioning

### Fonts and font styles

TBD

### Context-based shaping and positioning

One encoded Yi syllable character MUST map to one visible syllable glyph. Yi syllables MUST NOT be joined, ligated, reordered, or substituted according to neighboring Yi syllables.

### Cursive text

Yi MUST be treated as non-cursive text.

## Typographic units

### Characters and encoding

Unicode officially included the Liangshan Standard Yi script in version 3.0. The encoding range for Yi syllables is U+A000–U+A48C, comprising 1,164 syllables (syllables with diacritics are encoded individually and cannot be decomposed into a base syllable plus a combining diacritic) and one syllable iteration mark (U+A015 ꀕ, erroneously named "YI SYLLABLE WU"). The encoding range for Yi radicals is U+A490–U+A4CF, comprising 55 radicals.

In 2007, China submitted a proposal to encode the Yunnan Standard Yi script, but it has not yet been included in Unicode, nor has a code block been allocated for it.

### Grapheme, word segmentation, and selection

Grapheme segmentation MUST expose each Yi syllable as one grapheme cluster.

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
* Which vertical-writing conventions are still used in contemporary or historical Yi publications?
* Which emphasis marks and annotation styles are preferred?
