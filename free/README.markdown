# Lemmagen free lexicons

## About

Files located in `lexicons` directory are prebuilt lexicons for the [elasticsearch-analysis-lemmagen plugin](https://github.com/vhyza/elasticsearch-analysis-lemmagen) which provides lemmatizer as [elasticsearch token filter](https://www.elastic.co/guide/en/elasticsearch/reference/current/analysis-tokenfilters.html). Lexicons have been built using [jLemmagen](https://bitbucket.org/hlavki/jlemmagen) from [MULTEXT-East free lexicons 4.0](https://www.clarin.si/repository/xmlui/handle/11356/1041).

## Supported languages

| Language            | Filename     |
|:--------------------|:-------------|
| Bulgarian           | bg.lem       |
| Czech               | cs.lem       |
| English             | en.lem       |
| Estonian            | et.lem       |
| French              | fr.lem       |
| Hungarian           | hu.lem       |
| Romanian            | ro.lem       |
| Slovak              | sk.lem       |
| Resian (sl dialect) | sl-rozaj.lem |
| Slovene             | sl.lem       |
| Ukrainian           | uk.lem       |

## Usage

For [elasticsearch-analysis-lemmagen plugin](https://github.com/vhyza/elasticsearch-analysis-lemmagen) installation see plugin [repository](https://github.com/vhyza/elasticsearch-analysis-lemmagen).

After plugin installation, place lexicon into elasticsearch `config/lemmagen` directory (in case `lemmagen` directory is missing, create it). Example:

```bash
cd elasticsearch
mkdir config/lemmagen
cd config/lemmagen
wget https://github.com/vhyza/lemmagen-lexicons/raw/master/free/lexicons/en.lem
```

## License

This lexicons are distributed with the same [Creative Commons - Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) license as the [MULTEXT-East free lexicons 4.0](https://www.clarin.si/repository/xmlui/handle/11356/1041) source files from which lexicons were generated.
