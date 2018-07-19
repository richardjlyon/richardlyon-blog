---
title: Tufte CSS
description: This is a test post with a long description to make certain that multiline formatting is good.
---

{{% section %}}
Tufte CSS provides tools to style web articles using the ideas demonstrated by Edward Tufte’s books and handouts. Tufte’s style is known for its simplicity, extensive use of sidenotes, tight integration of graphics with text, and carefully chosen typography.

Tufte CSS was created by [Dave Liepmann](https://www.google.com) and is now an Edward Tufte project. The original idea was cribbed from Tufte-LaTeX and R Markdown’s Tufte Handout format. We give hearty thanks to all the people who have contributed to those projects.
{{% /section %}}


{{% section %}}
## Fundamentals
### Sections and Headings

Tufte CSS uses <code>h1</code> for the document title, <code>p</code> with class subtitle for the document subtitle, h2 for section headings, and h3 for low-level headings. More specific headings are not supported. If you feel the urge to reach for a heading of level 4 or greater, consider redesigning your document:

{{% blockquote
    source="Edward Tufte, forum post, ‘Book design: advice and examples’"
    url="http://www.google.com"
%}}

Blockquote **with** url source: [It is] notable that the Feynman lectures (3 volumes) write about all of physics in 1800 pages, using only 2 levels of hierarchical headings: chapters and A-level heads in the text. It also uses the methodology of sentences which then cumulate sequentially into paragraphs, rather than the grunts of bullet points. Undergraduate Caltech physics is very complicated material, but it didn’t require an elaborate hierarchy to organize.

{{% /blockquote %}}

{{% blockquote
    source="Edward Tufte, forum post, ‘Book design: advice and examples’"
%}}

Blockquote **without** url source: [It is] notable that the Feynman lectures (3 volumes) write about all of physics in 1800 pages, using only 2 levels of hierarchical headings: chapters and A-level heads in the text. It also uses the methodology of sentences which then cumulate sequentially into paragraphs, rather than the grunts of bullet points. Undergraduate Caltech physics is very complicated material, but it didn’t require an elaborate hierarchy to organize.

{{% /blockquote %}}

{{% /section %}}

{{% section %}}

## Sidenotes: Footnotes and Marginal Notes

<span class="newthought">One of the most distinctive features</span> of Tufte’s style is his extensive use of sidenotes.{{< sidenote reference="sn-cps2017" >}} This is a sidenote. {{< /sidenote >}} Sidenotes are like footnotes, except they don’t force the reader to jump their eye to the bottom of the page, but instead display off to the side in the margin. Perhaps you have noticed their use in this document already. You are very astute.

If you want a sidenote without footnote-style numberings, then you want a margin note. {{< marginenote reference="mn-test-note" >}} This is a margin note. {{< /marginenote >}} Notice there isn’t a number preceding the note. On large screens, a margin note is just a sidenote that omits the reference number. This lessens the distracting effect taking away from the flow of the main text, but can increase the cognitive load of matching a margin note to its referent text. However, on small screens, a margin note is like a sidenote except its viewability-toggle is a symbol rather than a reference number. This document currently uses the symbol (&#8853;), but it’s up to you.

{{% /section %}}

{{% section %}}

## Figures

Tufte emphasizes tight integration of graphics with text. Data, graphs, and figures are kept with the text that discusses them. In print, this means they are not relegated to a separate page. On the web, that means readability of graphics and their accompanying text without extra clicks, tab-switching, or scrolling.

Figures should try to use the <code>figure</code> element, which by default are constrained to the main column. Don’t wrap figures in a paragraph tag. Any label or margin note goes in a regular margin note inside the figure. For example, most of the time one should introduce a figure directly into the main flow of discussion, like so:

{{% figure src="Jessica_Beal-False_Rape_Allegation.jpg" %}}From Edward Tufte, _Visual Display of Quantitative Information_, page 92.{{% /figure %}}

But tight integration of graphics with text is central to Tufte’s work even when those graphics are ancillary to the main body of a text. In many of those cases, a margin figure may be most appropriate. To place figures in the margin, just wrap an image (or whatever) in a margin note inside a p tag, as seen to the right of this paragraph.

{{% figure src="Jessica_Beal-False_Rape_Allegation.jpg" %}}From Edward Tufte, _Visual Display of Quantitative Information_, page 92.{{% /figure %}}

If you need a full-width figure, give it the fullwidth class. Make sure that’s inside an article, and it will take up (almost) the full width of the screen. This approach is demonstrated below using Edward Tufte’s English translation of the Napoleon’s March data visualization. From _Beautiful Evidence_, page 122-124.




{{% /section %}}