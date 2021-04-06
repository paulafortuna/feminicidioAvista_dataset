![name](https://github.com/paulafortuna/images/blob/main/title_dataset.png)

This dataset was collected in the ["Feminicidio À Vista"](https://github.com/paulafortuna/feminicidioAvista) project and served as base for this [website](https://feminicidioavista.herokuapp.com/). 

Regarding this dataset it contains news crawled from 2001 to 2020 in several newspapers and matching different keywords. Later a step of manually annotation step was conducted by 
the repository owner. 


The dataset columns are:

- _id	- automatic id given by pandas dataframe
- pos_processed_news - id in the pos_processed_news mongodb table
- news_table_id	- id in the news_table mongodb table
- id - id in the keywords_news mongodb table
- arquivo_hash -	Arquivo.pt retrieved hash
- news_link	- Arquivo.pt retrieved page link
- news_site_date - News site retrieved date 	
- news_site_title	- News site retrieved news title 	
- news_site_authors -	News site retrieved authors 	
- news_site_text - News site retrieved news text 		
- search_newspaper - newspaper that published the news	
- title_len	- number of words in the title
- arquivo_date - Arquivo.pt retrieved date
- feminicidio -	boolean (true/false) indicating if news title or text contains at least one feminicide related word
- violencia_domestica -	boolean (true/false) indicating if news title or text contains at least one domestic violence related word
- violencia_sexual - boolean (true/false) indicating if news title or text contains at least one sexual violence related word
- assedio_sexual - boolean (true/false) indicating if news title or text contains at least one sexual harassment related word
- mulheres_assassinadas -	boolean (true/false) indicating if news title or text contains at least one murdered women related word
- search_keywords	- boolean (true/false) indicating if keywords were confirmed in the news
- title_countains_keyword	- boolean (true/false) indicating if news contain at least one keyword
- feminicidio_case - 0 indicates that news is not feminicide case, 1 indicated that it is feminicide case. This value was manually annotated.

* The keyword list corresponding to feminicidio, violencia_domestica, violencia_sexual, assedio_sexual, mulheres_assassinadas can be found in this [file](https://github.com/paulafortuna/feminicidioAvista/blob/main/crawling/Variables.py).


The dataset newspapers are:
- Publico - http://www.publico.pt
- Expresso - http://expresso.pt/
- Diario de Notícias - http://www.dn.pt/
- Correio da Manhã - http://www.cmjornal.pt/
- Sol (old)- http://www.sol.pt/
- Sol - http://sol.sapo.pt/ 
- Visão - https://visao.sapo.pt/
- Jornal de Notĩcias - https://www.jn.pt/


The used keywords for retrieving pages from Arquivo.pt are:

violencia domestica; violação; feminicidio; feminicidios; femicidio; femicidios; violações; assassinada; assassinadas; mulher assassinada; mulheres assassinadas; assassina mulher; assassinam mulher; assassina mulheres; assassinam mulheres; assassina companheira; assassina esposa; assassinam companheira; assassinam esposa; mata mulher; matam mulher; mata mulheres; matam mulheres; mata namorada; matam namorada; mata esposa; matam esposa; mata companheira; matam companheira; namorado mata; marido mata; companheiro mata; namorado assassina; marido assassina; companheiro assassina; filho mata mae; filhos matam mae; mata sogra; filho assassina mae; filhos assassinam mae; assassina sogra; assassinou mulher; assassinaram mulher; assassinou mulheres; assassinaram mulheres; assassinou companheira; assassinou esposa; assassinaram companheira; assassinaram esposa; matou mulher; mataram mulher; matou mulheres; mataram mulheres; matou namorada; mataram namorada; matou esposa; mataram esposa; matou companheira; mataram companheira; namorado matou; marido matou; companheiro matou; namorado assassinou; marido assassinou; companheiro assassinou; filho matou mae; filhos mataram mae; matou sogra; filho assassinou mae; filhos assassinaram mae; assassinou sogra; matou mae; mataram mae; mata mae; matam mae; mulher; mulheres
