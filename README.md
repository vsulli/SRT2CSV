# SRT2CSV
Read in a .srt file, clean the data, and export to a .csv file for upload to ANKI. 
This script currently only supports Spanish & German fully, but the spaCy library and PyMultiDictionary offer support for various other languages. 

## USAGE
(1) The original .srt file includes the subtitle number, the start and end times, and other features such as tags that will need to be removed. 
<img src=“Screenshots/1_es_demo_srt_pt1.PNG”/>
[es_srt](Screenshots/1_es_demo_srt_pt1.PNG)

## NOTES / LIMITATIONS

- Notepad++ convert ANSI to UTF-8 for special characters
- Seems to need to be UTF-8 BOM in order to preserve special characters
- Hinglish doesn't have an official language code


## FUTURE IMPROVEMENTS
- Adding a category tag for each sentence
- Creating word clouds (for categories such as family & friends, outside & sports, cooking, etc.)
- Change educalingo dictionary to web scraping an actual dictionary for better definitions and articles for nouns?
- Add article & plural of noun - create new function that finds it based on language (key = lang & gender, value = der, die, das or el, la, etc.)
- Extend the verb definition to include tense -> go deeper into spaCy lemmatization

