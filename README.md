# ia368v_dd_class_06
IA368v DD 6th class: Training T5-base for doc2query approach.

## Created notebooks for the activity

* [T5_fine_tune_for_doc2query.ipynb](T5_fine_tune_for_doc2query.ipynb): Fine-tuning T5-base for doc2query task using the MS MARCO Tiny dataset (11k).
* [explore_ms_marco_passage.ipynb](explore_ms_marco_passage.ipynb): Prepare MS MARCO Passage Development dataset to fine-tune T5-base for doc2query, attempting to have more data (~532k).
* [T5_fine_tune_for_doc2query_more_data.ipynb](T5_fine_tune_for_doc2query_more_data.ipynb): Fine-tune T5-base using the MS MARCO Passage Development dataset.
* [T5_TREC_COVID_expansion_qualitative_test_for_doc2query.ipynb](T5_TREC_COVID_expansion_qualitative_test_for_doc2query.ipynb): Documents expansion qualitative test using the T5-base model fine-tuned for doc2query task.
* [explore_trec_covid.ipynb](explore_trec_covid.ipynb): TREC COVID dataset preparation for expansion and Pyserini's BM25 processing.
* [T5_TREC_COVID_expansion_for_doc2query.ipynb](T5_TREC_COVID_expansion_for_doc2query.ipynb): TREC COVID documents expansion using the T5-base fine-tuned  for doc2query task.
* [merge_trec_covid_expansion.ipynb](merge_trec_covid_expansion.ipynb): merge the document expansion results in a single file.
* [trec_covid_BM25.ipynb](trec_covid_BM25.ipynb): TREC COVID queries test using Pyserini's BM25 implementation over the regular and doc2query-expanded TREC COVID documents.

## Final results:

|    | nDCG@10 |
|----|:---: |
| Original TREC COVID| 0.5861|
| 20-topic expansion | 0.6436 |
| 40-topic expansion | 0.6482 |

Check [here a presentation](https://docs.google.com/presentation/d/1HaYBkPOaF60kIo5wnAP5LSrbMw4Gc2A1JHAurCiH6Z0/edit?usp=share_link) commenting this exercise resolution.
