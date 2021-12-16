# HornMT 

The `HornMT` repository contains data and the associated metadata for the project [Machine Translation Benchmark Dataset for Languages in the Horn of Africa](https://lesan.ai/benchmark). The goal is to create a multi-way parallel corpus that will serve as a benchmark to accelerate progress in machine translation research and production systems for languages in the Horn of Africa.


## Supported Languages

 Language      | ISO 639-3 code
 ------------- | -------------
Afar	| aaf
Amharic	| amh
English	| eng
Oromo	| orm
Somali	| som
Tigrinya	| tir


## Content

`data/` contains one text file per language and each file contains news snippets in the same order for each language.

```
data
├── aar.txt
├── amh.txt
├── eng.txt
├── orm.txt
├── som.txt
└── tir.txt
```

`metadata.tsv` contains tab separated data describing each news snippet. The metadata contains the following fields.

- **Scope** - describes whether the news is global or local. It takes two values: Global news and Local news.
- **Category** - News category covering the following 12 topics
  - Art and Culture
  - Business and Economy
  - Conflicts and Attacks
  - Disaster and Accidents
  - Entertainment
  - Environment
  - Health
  - International Relations
  - Law and Crime
  - Politics
  - Science and Technology
  - Sport
- **Source** - List of one or more URLs from which the news content is extracted or based on. 
- **Domain** - TLD corresponding to the URL(s) in Source.
- **Date** - The publication date of the source article. The format is yyyy-mm-dd.

## Other formats

All the data and associated metadata together in one file is also available in other file formats.

`HornMT.xlsx` - data and associated metadata in xlsx format.

`HornMT.json` - data and associated metadata in json format.

Below is an example row.

```json
{
   "data":{
      "eng":"The World Meteorological Organisation reports that the ozone layer is damaged to its worst extent ever in the Arctic.",
      "aaf":"Baad Metrolojih Eglali Areketekeh Addal Ozonih qelu faxe waktik lafetle calat biyakisem xayose.",
      "amh":"የአለማ የአየር ንብረት ድርጅት በአርክቲክ አካባቢ ያለው የኦዞን ምንጣፍ ከፍተኛ ጉዳት እንደደረሰበት አስታወቀ፡፡",
      "orm":"Dhaabbanni Meetiroolojii Addunyaa baqqaanni oozonii Arkiitik keessatti gara sadarkaa isa hamaa haga ammaatti akka miidhame gabaase.",
      "som":"Ururka Saadaasha Hawada Adduunka ayaa ku warramaya in lakabka ozoneka ee Ka koreeya dhulka baraflayda uu waxyeelladii abid ugu darnaa soo gaadhay.",
      "tir":"ውድብ ሜትሮሎጂ ዓለም ኣብ ኣርክቲክ ዝርከብ ናሕሲ ኦዞን ኣዝዩ ብዝኸፍአ ደረጃ ከምዝተጎድአ ሓቢሩ፡፡"
   },
   "metadata":{
      "scope":"Global",
      "category":"Science and Technology",
      "source":"https://www.independent.co.uk/environment/climate-change/ozone-layer-damaged-by-unusually-harsh-winter-2263653.html",
      "domain":"www.independent.co.uk",
      "date":"2011-04-05"
   }
}
```

## Team

### Afar 

Mohammed Deresa and team 


### Amharic

Tigist Taye

Selamawit Hailemariam

Wako Tilahun

### Oromo

Gemechis Melkamu

Galata Girmaye

### Somali 

Abdiselam Mohamed and team 

### Tigrinya 

Berhanu Abadi Weldegiorgis

Michael Minassie

Nureddin Mohammedshiek


### Project Leaders 

Abel Aregawi <abel@lesan.ai>

Gebrekirstos G. Gebremeskel <gebrekirstos.gebremeskel@ru.nl>

Asmelash Teka Hadgu <asme@lesan.ai>
 
## License

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
