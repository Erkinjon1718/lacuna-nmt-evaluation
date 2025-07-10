
# Lacuna-Annotated Corpus and Ontology for Uzbek-English and Turkish-English Machine Translation

## Overview

This repository presents a comprehensive, manually annotated dataset and ontology resource for the study and computational treatment of lexical lacunae—expressions and concepts unique to one language and culture that have no direct equivalents in another. The resource is intended to advance reproducible research in neural machine translation (NMT), cross-cultural semantics, and knowledge-based language processing for low-resource language pairs.

The dataset and ontology were developed as part of the research project  
**"Linguistic and Computational Solutions for Translating Lexical Lacunae in Neural Machine Translation Systems"**  
at the Tashkent State University of Uzbek Language and Literature.

## Repository Structure

- `annotated_lacuna.csv`  
  Manually annotated Uzbek-English and Turkish-English bilingual sentence pairs, each labeled for lacuna type and translation strategy.
- `lacuna_ontology.owl`  
  Domain-specific bilingual ontology, mapping lacuna expressions to conceptual categories, descriptors, and translation recommendations.
- `examples/`  
  Sample translation pairs and typical error cases for system benchmarking and demonstration.
- `docs/`  
  Detailed project methodology, annotation guidelines, publication references, and ablation study results.
- `README.md`  
  This documentation file.

## Dataset Description

### Motivation and Scope

Lexical lacunae—cultural, administrative, and conceptual units without direct translation—pose a significant challenge for both statistical and neural machine translation systems, especially in low-resource contexts. The objective of this dataset is to provide a rigorously annotated benchmark for identifying, classifying, and modeling such expressions in Turkic languages and English.

### Data Sources

The corpus is compiled from a wide range of written and spoken genres, including:

- Legal and administrative documents
- News reports and journalistic materials
- Literary texts, folklore, and conversational speech
- Educational and governmental publications

Each source was selected to maximize the representativeness and diversity of cultural and institutional terminology.

### Annotation Procedure

Three professional linguists, each fluent in Uzbek, Turkish, and English, were recruited to perform independent annotation. Annotators applied strict criteria, identifying lacunae if a lexical item or phrase:

- Has no direct semantic correspondence in the target language,
- Embodies culture-specific, religious, administrative, or historical meaning,
- Requires explanatory paraphrasing or annotation in translation.

Annotation guidelines were developed based on established theoretical models (e.g., Wierzbicka; Vinay & Darbelnet) and iteratively refined through pilot studies. Inter-annotator agreement, measured by Cohen’s Kappa, was 0.84. All disputed cases were resolved by panel adjudication. The final "gold-standard" corpus comprises 1,000 bilingual sentence pairs, with detailed metadata, lacuna types, and semantic notes. Each record was verified by at least two annotators.

For full reproducibility, the dataset may be requested for academic use and will be publicly released upon acceptance of related publications.

## Ontology Resource

The accompanying bilingual ontology was constructed in OWL format and integrates over 700 concepts derived from BabelNet, DBpedia, and custom domain-specific resources. Each ontology node is linked to:

- The source term and contextual usage,
- Conceptual classification (cultural, administrative/legal, lexical-conceptual),
- A recommended translation or explanation strategy,
- Descriptive notes and references to corpus examples.

The ontology supports integration into semantic-aware machine translation workflows, SPARQL querying, and further extension for other language pairs.

## Applications

This resource can be used for:

- Training and evaluation of lacuna-aware NMT systems,
- Systematic benchmarking of translation models for cultural and terminological adequacy,
- Development of knowledge-based translation modules,
- Research in cross-cultural semantics, lexicography, and computational linguistics.

## Example Usage

Included in the `examples/` directory are scripts and sample analyses that demonstrate:

- Querying the ontology for translation suggestions,
- Comparing baseline versus ontology-enriched NMT output,
- Evaluating translation accuracy by lacuna type.

Benchmarking results and ablation studies are provided in the `docs/` folder.

## Citation

If you use this resource in your work, please cite:

Gaybullaev, E., & Adilova, M. (2025).  
Lacuna-Annotated Corpus and Ontology for Uzbek-English and Turkish-English Machine Translation.  
Tashkent State University of Uzbek Language and Literature.

## License

This dataset and ontology are distributed under the Creative Commons Attribution 4.0 International (CC BY 4.0) License.

## Contact

For dataset access, collaboration, or further information, contact:

erkinjon.gaybullayev@gmail.com  
adilovamunojot@gmail.com

## Acknowledgments

The authors thank all annotators and colleagues at the NLP Lab, Tashkent State University of Uzbek Language and Literature, for their contributions and support.

## Project Status

- Corpus annotation and ontology compilation complete
- Documentation and scripts under active development
- Full public release planned following journal publication
