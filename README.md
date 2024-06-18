# Minimal CJK support for Zotero-Pandoc workflow

This repository contains a .tex file and a .csl file that provide basic support for Chinese characters in Pandoc and LaTeX, serving as a temporary solution for specific workflow issues involving Zotero, Zotero Better BibTeX, and Pandoc. With minor modifications, the solution will work for Japanese and Korean characters.

## Background 

JurisM provides crucial support for multilingual citation where Zotero does not. However, JurisM is no longer compatible with Zotero Better BibTeX. A future update may solve this, but in the meantime this is a hack-ish workaround. 

The Minimal CJK Chicago CSL style is specifically modified to utilize data from the "original-author" and "original-title" fields found in Zotero's "Extra" field. 

## Example Usage

For a bibliography entry like:

    Title: 1945：民营企业家组党
    Author: 章, 立凡

Add the following in the Zotero "Extra" field:

    original-title: The Entrepreneurs of Society Form a Party
    original-author: <Zhang> || <Lifan>

When exported to Zotero Better BibTeX, the original and translated author names and titles will be correctly cited in documents processed with Pandoc.





