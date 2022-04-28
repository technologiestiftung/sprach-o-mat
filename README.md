# Sprach-O-Mat

This tool performs a diagnosis of the level of complexity of German texts. 
It is available here: [https://evelynebrie.shinyapps.io/Sprach-O-Mat/](https://evelynebrie.shinyapps.io/Sprach-O-Mat/)
This is a prototype under construction.

The Tool provides 4 different diagnostics:

1) Sprachniveau (language level): allows the user to identity the words that are not encompassed in language levels A1, A2 or B1 (default: B1)
2) Wortlänge (word length): allows the user to identify words containing more letters than a self-defined limit (default: 10 letters)
3) Satzlänge (sentence length): allows the user to identify sentences containing more words than a self-defined limit (default: 30 words)
4) Kommatas (commas): allows the user to identify sentences containing more commas than a self-defined limit (default: 3 commas)

**CONTENT:**

- SOP_code.Rmd: A RMarkdown application for the Sprach-O-Mat Shiny App (ui and server)

- dictionary_a1a2b1_onlystems.csv: A csv file with all the vocabulary terms from the Goethe Institut based on the PDF documents in the "Dictionaries" folders. These were converted to csv using pdftools::pdf_ocr_text. There are three columns: a unique ID column referring to the original location of the word stem in the PDF documents, a "level" column indicating the language level of the stem, a "stem" column containing the stem of the word

- Dictionaries: PDF files from the Goethe Institut. Goethe-Zertifikat_A1_Wortliste.pdf (Words list A1), Goethe-Zertifikat_A2_Wortliste.pdf (Words list A2), Goethe-Zertifikat_B1_Wortliste.pdf (Words list B1). These are openly available here: https://www.sprachenzentrum.fu-berlin.de/slz/sprachen-links/deutsch/wortschatz/index.html

