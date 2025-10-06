# Nikolay, [rus_Cyrl/batch0.tsv](../annot_round1/rus_Cyrl/batch0.tsv)

(Outdated, used as an example)
Almost all examples are in the correct language, 1 example is the first part in Russian and the second in Ukrainian. 

Lots of commercial ads, some contain more running texts (e.g. descriptions of hotels), some less (e.g. sound equipment).

Occasionally the first part contains traces of menus, while the second part consists of running text.

# Marta, [spa_Latn/batch0.tsv](../annot_round1/spa_Latn/batch0.tsv)

* Lang id is perfect (only one document being half Portuguese, one with a sentence in English, one with a sentence in French and one with a sentence in Italian)
* Only one porn document.
* Some boilerplate in the documents (links, copyright texts, social media links, menus...). I only marked those as artifacts when they spread across the document, making the reading annoying.
* Some truncated texts (i.e. "Read more" tags) 
* Some oversplitted sentences (i.e. doc 158 or 199)
* Some documents contain sentences repeated twice (maybe images alt text)
* Other issues not covered by the current evaluation labels  (doc number starting in 2, since 1 is the header of the tsv):
  * Glued words in docs 9, 44, 48, 70, 79 and 130
  * Clearly MT or AI generated text in docs 15, 22, 38, 42, 45, 47, 64, 65, 97, 116, 164 and 170

# Patrick, [cmn_Hans/batch0.tsv](../annot_round1/cmn_Hans/batch0.tsv)

* Lang id is perfect, only one document has slightly more English than Chinese, so labelled as 0 under "correct language"
* 2-3 porn
* Some documents are apparently news titles concatenated together, so natural/fluent at the sentence level but not "coherent".
* Some documents have a long list of items, but without text artifacts

# Ona, [cat_Latn/batch0.tsv](../annot_round1/cat_Latn/batch0.tsv)
* Lang id is perfect, atlhough a few documents may contain a single sentence in Spanish or English.
* 0 porn documents.
* Some boilerplate in the documents (links, copyright texts, social media links, menus...). I did not mark this as text artifacts, as the majority of the text is good and readable.
* Some truncated texts
* Some oversplitted sentences (i.e. doc 55 or 160)
* Other issues not covered by the current evaluation labels:
  * Glued words
  * Clearly MT or AI generated text in docs 2 ("Bons Aires" instead of "Buenos Aires"), 4 ("Friends" as "Amics", the tv show, was never actually translated to Catalan), 86 ("after test" translated as "postgust"), 95
  * Bad encoding of accent characters (doc 137): "Per grans Órees geogrÓfiques van augmentar la Uniˇ Europea (3,1%), altres pa´sos i territoris d'Europa (10,9%), i AmŔrica del Nord (1,1%). "

# Peter [jpn_Jpan/batch0.tsv](../annot_round1/jpn_Jpan/batch0.tsv)

* All Lang ID is correct
* Many of the pages have quite a few text artifacts such as full menus in between proper Japanese sentences.
* There are lots of pages with e-commerce listings for consumer products, hotels, real estate etc.
* There are also lots of pages with personal blogs. These seem very useful as they are written as long-form conversational streams of consciousness. I think this data (compared to something like news) would help make an effective chatbot.
* Other smaller items were lists of Tweets, IT how-to guides, horse racing tips, horoscopes etc.
* Some texts are truncated by ellipses, and therefore unnatural (is this intentional?).
* 1 porn item. You probably want to add オナニー (masturbation) to your porn word list as there is no context where that word does not refer to masturbation.
* There is one item where a man says that he wants to die because his girlfriend broke up with him (line 155). Is this something we want to remove?


# Bhavitvya, [hin_Deva/batch0.tsv](../annot_round1/hin_Deva/batch0.tsv)

* Lang id is perfect except for 2 instances where one of them has a lot of Chinese text and other has more English than Hindi
* No porn
* Some documents contain news snippets concatenated together, so natural/fluent at the sentence level but not "coherent".
* A lot of documents contain “report”, “share”, “follow us” etc at the end which may be part of article and not boilerplate but I have still flagged them

# Erik, [fin_Latn/batch3.tsv](../annot_round1/fin_Latn/batch3.tsv)

* Lang id is 100% perfect
* 7 porn docs
* Text artifacts are relatively common, most frequently from comment sections, e.g. "VastaaPoista" ("ReplyDelete"), navigation menus, dates and non-delimited headers. When the headers (etc.) were cleanly separated in their own lines, I did not mark the text as having artifacts
* 10 docs with unnatural text, mostly SEO word lists

# Amanda [fin_Latn/batch2.tsv](../annot_round1/fin_Latn/batch2.tsv)

* Lang id perfect except one with ~50% English and one with some mess of Finnish, Estonian(?), gibberish, and English (<- chose to put it in this category because I could not understand the text)
* 2/200 porn
* A lot of adds, however with majority flowing text. Lots of news as well with bias towards one municipality (just a feature of this batch?)
* Text artifacts: forum posts had a lot of instances ot this: ``AnswerDeleteAnswerSuch a perfect combination!``
* Minor problems with Ä and Ö: ~5 texts had problems with these characters (either missing completely or unicode replacement �)

# Pablo, [spa_Latn/batch1.tsv](../annot_round1/spa_Latn/batch1.tsv)

- Language tagging is always correct
- Boilerplates are common
- There are many documents with incomplete text caused by CSS aesthetic limitator, with "..." at the end
- No porn, only a chat with near hot commentaries
- Some undesired text from the typical list of related posts/news 

# Pablo, [ita_Latn/batch0.tsv](../annot_round1/ita_Latn/batch0.tsv)

- Language tagging is correct but there is 1 multilingual document
- 1 translated
- 3 documents with explicit porn content


# Pablo, [glg_Latn/batch0.tsv](../annot_round1/glg_Latn/batch0.tsv)

- Language detection is surprisingly always correct
- some sticked words
- 2 mixed documents spa-glg

# Pablo, [ast_Latn/batch0.tsv](../annot_round1/ast_Latn/batch0.tsv)

- There are many documents in Spanish, some colloquial Spanish documents and some village names are mistaken for Asturian.

# Maja, [hrv_Latn/batch0.tsv](../annot_round1/hrv_Latn/batch0.tsv)

* Language tagging is mostly correct, although there are snippets of other languages in some documents (e.g. disclaimers in English; Slovenian menu items under text published in Croatian)
* Incorrectly tagged documents are mostly Bosnian, occasionally Serbian (apart from grammar and vocabulary, sometimes differentiable by mentions of currency or web domains)
* Most frequent artifact: ``..( n characters skipped )..``
* Other frequent artifacts: share/comment buttons, links to unrelated news headlines
* (Note that the Artifacts tag covers a spectrum from mostly harmless and easily cleaned (share/comment/read more), to more egregious (unrelated news headlines interjected in running text))
* Roughly 1/4 of documents consists of product descriptions and lists of news headlines
* 1% porn, in the form of salacious personal ads