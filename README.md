# NLP2024
for my NLP examn at cogsci

the code can take an input text, tokenise it and using three different models output versions of the text without angliscisms. The text must be in danish.  Some  false positives are present in the anglisicms depending on your text which can be filtered out, as seen in the code. 
some code was not used in the final paper, but kept in here in case i want to return to it (such as visualisations and an attempt at importing a norwegian language model). As mentioned in the paper, the models do not perform well on this task. 

The files must be run in the following order:
- loanwords_cleaning (imports and cleans the anglisicms, document not included here as it was obtained privately from Henrik Gottlieb
- import_danish_text (imports the chosen text, cleans it and saves as a global csv file)
- matching_loans_to_danish (takes the loanwords and text and finds matches between them, saves this file)
- importing_language_models (imports three language models and for each loanword finds the word with the closests cosine distance, which is then inserted into a new version of the original sentence. both sentences are compared in terms of cosine distance and the average performance across the document is found.
  there are also some attempts at visualisations as well as an attempt at using a norwegian language model.)

the models can be downloaded from the following links:
- https://loar.kb.dk/items/33396585-6918-4cf0-8f76-723594766f37/full
- http://vectors.nlpl.eu/repository/
- https://fasttext.cc/docs/en/crawl-vectors.html

The twitter data can be downloaded from this link:
https://danlp-alexandra.readthedocs.io/en/latest/
