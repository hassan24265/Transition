Overview
This directory manages the WIS2 Transition Guide. This document provides technical guidance on transitioning from GTS to WIS2.

Dependencies
Documentation is managed with https://asciidoctor.org[Asciidoctor]

Link checking is managed with asciidoc-link-check.

PDF generation is managed with asciidoctor-pdf.

Building the document
# create HTML (single page)
asciidoctor --trace -o wis2-transition-guide.html index.adoc
# create PDF
asciidoctor --trace -r asciidoctor-pdf --trace -b pdf -o wis2-transition-guide.pdf index.adoc
# create Word document
asciidoctor --trace --backend docbook --out-file - index.adoc | pandoc --from docbook --to docx --output wis2-transition-guide.docx



https://asciidoctor.org - automatic!

https://asciidoctor.org[Asciidoctor]

devel@discuss.example.org

mailto:devel@discuss.example.org[Discuss]

mailto:join@discuss.example.org[Subscribe,Subscribe me,I want to join!]
