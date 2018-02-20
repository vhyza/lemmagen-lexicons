# Lemmagen NON-FREE lexicons

## About

Files located in `lexicons` directory are prebuilt lexicons for the [elasticsearch-analysis-lemmagen plugin](https://github.com/vhyza/elasticsearch-analysis-lemmagen) which provides lemmatizer as [elasticsearch token filter](https://www.elastic.co/guide/en/elasticsearch/reference/current/analysis-tokenfilters.html). Because [MULTEXT-East non-commercial lexicons 4.0](https://www.clarin.si/repository/xmlui/handle/11356/1042) source is not accessible to me, lexicons have been extracted from [jlemmagen-lang](https://bitbucket.org/hlavki/jlemmagen/src/04782dae2f5eb379a6a19bb9c067045618821395/jlemmagen-lang/src/main/resources/?at=master) library. This lexicons **can't be used commercially**.

## Supported languages

| Language            | Filename     |
|:--------------------|:-------------|
| Farsi / Persian     | fa.lem       |
| Macedonian          | mk.lem       |
| Polish              | pl.lem       |
| Russian             | ru.lem       |
| Serbian             | sr.lem       |

## Usage

For [elasticsearch-analysis-lemmagen plugin](https://github.com/vhyza/elasticsearch-analysis-lemmagen) installation see plugin [repository](https://github.com/vhyza/elasticsearch-analysis-lemmagen).

After plugin installation, place lexicon into elasticsearch `config/lemmagen` directory (in case `lemmagen` directory is missing, create it). Example:

```bash
cd elasticsearch
mkdir config/lemmagen
cd config/lemmagen
wget https://github.com/vhyza/lemmagen-lexicons/raw/master/non-free/lexicons/pl.lem
```

## License

This lexicons are distributed with the same [Creative Commons - Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) license as the [MULTEXT-East non-commercial lexicons 4.0](https://www.clarin.si/repository/xmlui/handle/11356/1042).
