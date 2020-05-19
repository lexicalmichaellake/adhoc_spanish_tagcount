# adhoc_spanish_tagcount

After fixtagging your Spanish documents, they are no longer readable by the original Spanish TagCount program because Tagcount seems to execute steps in this order:

a. read files tagged by the Spanish Tagger program.

b. assign syntactic and semantic tags in field 7 based on patterns in fields 2-6 (e.g., _vcomm_ (communication verb), _serpsvagntlss_ (agentless ser passive)).

c. count the resulting field 7 tags and output them to a spreadsheet.

TagCount does not recognize Field 7 tags immediately upon opening a text file. Doing so would be tantamount to tossing a book into a paper mill rather than woodchips. 
As such, I recommend using the files in this folder as custom dictionary files in conjunction with SiNLP (Simple Natural Language Processing) to carry out the tag counting : https://www.linguisticanalysistools.org/sinlp.html

(However, for now, you will need to normalize the scores to occurrences per thousand words to make the frequency counts comparable with other Biber tagger studies)
