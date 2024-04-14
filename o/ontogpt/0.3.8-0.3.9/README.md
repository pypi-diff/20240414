# Comparing `tmp/ontogpt-0.3.8.tar.gz` & `tmp/ontogpt-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.3.8.tar", max compression
+gzip compressed data, was "ontogpt-0.3.9.tar", max compression
```

## Comparing `ontogpt-0.3.8.tar` & `ontogpt-0.3.9.tar`

### file list

```diff
@@ -1,205 +1,206 @@
--rw-r--r--   0        0        0     1571 2024-02-08 21:34:29.995931 ontogpt-0.3.8/LICENSE
--rw-r--r--   0        0        0     3838 2024-02-08 21:34:29.995931 ontogpt-0.3.8/README.md
--rw-r--r--   0        0        0     2805 2024-02-08 21:34:30.131930 ontogpt-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      657 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    48558 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/cli.py
--rw-r--r--   0        0        0      695 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     2593 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/gpt4all_client.py
--rw-r--r--   0        0        0     1701 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/hfhub_client.py
--rw-r--r--   0        0        0     7174 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0    20754 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1133 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0      684 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/conf/synonymizer-conf.yaml
--rw-r--r--   0        0        0       81 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5339 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0     3740 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/embedding_similarity_engine.py
--rw-r--r--   0        0        0     2298 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/generic_engine.py
--rw-r--r--   0        0        0    19297 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    24796 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0    11975 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/mapping_engine.py
--rw-r--r--   0        0        0     5268 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/pheno_engine.py
--rw-r--r--   0        0        0    11323 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/reasoner_engine.py
--rw-r--r--   0        0        0     1047 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    25186 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      725 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.131930 ontogpt-0.3.8/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    11906 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0    15495 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ctd/eval_ctd_ner.py
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2160 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    11455 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0     3469 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6329 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     9451 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1602 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/10338374.txt
--rw-r--r--   0        0        0      811 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/17653185.txt
--rw-r--r--   0        0        0     1516 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/18253950.txt
--rw-r--r--   0        0        0     1617 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/24104886.txt
--rw-r--r--   0        0        0     1968 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/28846760.txt
--rw-r--r--   0        0        0     1324 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/29285689.txt
--rw-r--r--   0        0        0      990 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/29441064.txt
--rw-r--r--   0        0        0     1539 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/31767987.txt
--rw-r--r--   0        0        0      744 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/PMC4961083.txt
--rw-r--r--   0        0        0     1439 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/PMC6386158.txt
--rw-r--r--   0        0        0     1001 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/PMC7003169.txt
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rwxr-xr-x   0        0        0       95 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0     1595 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/10338374_smoking.txt
--rw-r--r--   0        0        0     1447 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review.txt
--rw-r--r--   0        0        0     1191 2024-02-08 21:34:30.135930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.txt
--rw-r--r--   0        0        0     4791 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.yaml
--rw-r--r--   0        0        0     1529 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/kidney/test.txt
--rw-r--r--   0        0        0      913 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/kidney/test2.txt
--rw-r--r--   0        0        0     3584 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/kidney/test3.txt
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/__init__.py
--rw-r--r--   0        0        0    12890 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/eval_maxo.py
--rw-r--r--   0        0        0     1158 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_12958596.yaml
--rw-r--r--   0        0        0     1011 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301368.yaml
--rw-r--r--   0        0        0     1156 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301450.yaml
--rw-r--r--   0        0        0     2478 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301519.yaml
--rw-r--r--   0        0        0     1351 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301527.yaml
--rw-r--r--   0        0        0     1113 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301572.yaml
--rw-r--r--   0        0        0     2022 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301644.yaml
--rw-r--r--   0        0        0     2204 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301675.yaml
--rw-r--r--   0        0        0     1246 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301765.yaml
--rw-r--r--   0        0        0     1401 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_2063868.yaml
--rw-r--r--   0        0        0     1404 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_26110198.yaml
--rw-r--r--   0        0        0      902 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_27077170.yaml
--rw-r--r--   0        0        0     2642 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_28406602.yaml
--rw-r--r--   0        0        0     2006 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_29478819.yaml
--rw-r--r--   0        0        0     1279 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_30488337.yaml
--rw-r--r--   0        0        0     1417 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_36977302.yaml
--rw-r--r--   0        0        0     1715 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_9543069.yaml
--rw-r--r--   0        0        0      985 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0     4949 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/csv_wrapper.py
--rw-r--r--   0        0        0      540 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     5036 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3562 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2487 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1760 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0     1617 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/template_loader.py
--rw-r--r--   0        0        0     1756 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0    11155 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/models.yaml
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/ontex/__init__.py
--rw-r--r--   0        0        0    68726 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/ontex/extractor.py
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/__init__.py
--rw-r--r--   0        0        0      159 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/enrichment/__init__.py
--rw-r--r--   0        0        0     1257 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
--rw-r--r--   0        0        0     1016 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
--rw-r--r--   0        0        0      993 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
--rw-r--r--   0        0        0      994 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
--rw-r--r--   0        0        0      995 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
--rw-r--r--   0        0        0      152 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/mapping/__init__.py
--rw-r--r--   0        0        0     2424 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/mapping/eval-mapping.jinja2
--rw-r--r--   0        0        0      158 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/phenopacket/__init__.py
--rw-r--r--   0        0        0      637 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/phenopacket/phenopacket.jinja2
--rw-r--r--   0        0        0      127 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/qa/__init__.py
--rw-r--r--   0        0        0       31 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/qa/generic.jinja2
--rw-r--r--   0        0        0      150 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/reasoning/__init__.py
--rw-r--r--   0        0        0     1471 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/reasoning/reasoning.jinja2
--rw-r--r--   0        0        0      560 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/prompts/similarity/connections.jinja2
--rw-r--r--   0        0        0       67 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0     6733 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2303 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     5344 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/biotic_interaction.py
--rw-r--r--   0        0        0     2128 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/biotic_interaction.yaml
--rw-r--r--   0        0        0    10727 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/cell_type.py
--rw-r--r--   0        0        0     8011 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/cell_type.yaml
--rw-r--r--   0        0        0     2957 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/class_enrichment.py
--rw-r--r--   0        0        0     3192 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/class_enrichment.yaml
--rw-r--r--   0        0        0     8322 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/composite_disease.py
--rw-r--r--   0        0        0     4732 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/composite_disease.yaml
--rw-r--r--   0        0        0     4260 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3920 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     7590 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6713 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     6325 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/ctd_ner.py
--rw-r--r--   0        0        0     5194 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/ctd_ner.yaml
--rw-r--r--   0        0        0    62750 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/data_sheets_schema.py
--rw-r--r--   0        0        0    43069 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/data_sheets_schema.yaml
--rw-r--r--   0        0        0     6362 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/datasheet.py
--rw-r--r--   0        0        0     2567 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/datasheet.yaml
--rw-r--r--   0        0        0     5764 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/desiccation.py
--rw-r--r--   0        0        0     1763 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/desiccation.yaml
--rw-r--r--   0        0        0     9250 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/diagnostic_procedure.py
--rw-r--r--   0        0        0     4811 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/diagnostic_procedure.yaml
--rw-r--r--   0        0        0    11000 2024-02-08 21:34:30.139930 ontogpt-0.3.8/src/ontogpt/templates/dietitian_notes.py
--rw-r--r--   0        0        0    10950 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/dietitian_notes.yaml
--rw-r--r--   0        0        0     6087 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1927 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     4938 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/emapa_simple.py
--rw-r--r--   0        0        0     1169 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/emapa_simple.yaml
--rw-r--r--   0        0        0     6334 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/environmental_metadata.py
--rw-r--r--   0        0        0     2726 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/environmental_metadata.yaml
--rw-r--r--   0        0        0     6710 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     3256 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     5234 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/figure.py
--rw-r--r--   0        0        0     1464 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/figure.yaml
--rw-r--r--   0        0        0     5405 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1635 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     4501 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/genesummary.py
--rw-r--r--   0        0        0     1117 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/genesummary.yaml
--rw-r--r--   0        0        0     4949 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/go_simple.py
--rw-r--r--   0        0        0     1059 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/go_simple.yaml
--rw-r--r--   0        0        0     6059 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/go_terms.py
--rw-r--r--   0        0        0     3448 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/go_terms.yaml
--rw-r--r--   0        0        0     6450 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/go_terms_relational.py
--rw-r--r--   0        0        0     3182 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/go_terms_relational.yaml
--rw-r--r--   0        0        0     8714 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     5208 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     7188 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     5060 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/human_phenotype.py
--rw-r--r--   0        0        0     1251 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/human_phenotype.yaml
--rw-r--r--   0        0        0     8788 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     8218 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ibd_literature.py
--rw-r--r--   0        0        0     4727 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ibd_literature.yaml
--rw-r--r--   0        0        0     5035 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/kidney.py
--rw-r--r--   0        0        0     1068 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/kidney.yaml
--rw-r--r--   0        0        0     7960 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/maxo.py
--rw-r--r--   0        0        0     4692 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/maxo.yaml
--rw-r--r--   0        0        0     6733 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3256 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5939 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7816 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     4924 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/mondo_simple.py
--rw-r--r--   0        0        0     1050 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/mondo_simple.yaml
--rw-r--r--   0        0        0     5293 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/nmdc_schema_data.py
--rw-r--r--   0        0        0     1618 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/nmdc_schema_data.yaml
--rw-r--r--   0        0        0     5725 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     6743 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ontology_issue.py
--rw-r--r--   0        0        0     3383 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/ontology_issue.yaml
--rw-r--r--   0        0        0     5538 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1730 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7893 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3545 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7733 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5967 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     5800 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/traits.py
--rw-r--r--   0        0        0     3502 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/traits.yaml
--rw-r--r--   0        0        0     8331 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4604 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/utils/__init__.py
--rw-r--r--   0        0        0      573 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/utils/model_utils.py
--rw-r--r--   0        0        0      283 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/utils/parse_utils.py
--rw-r--r--   0        0        0        0 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2045 2024-02-08 21:34:30.143930 ontogpt-0.3.8/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 ontogpt-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1571 2024-03-20 16:41:46.453765 ontogpt-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3838 2024-03-20 16:41:46.453765 ontogpt-0.3.9/README.md
+-rw-r--r--   0        0        0     2695 2024-03-20 16:41:46.589763 ontogpt-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      657 2024-03-20 16:41:46.589763 ontogpt-0.3.9/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    49633 2024-03-20 16:41:46.589763 ontogpt-0.3.9/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      695 2024-03-20 16:41:46.589763 ontogpt-0.3.9/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     2775 2024-03-20 16:41:46.589763 ontogpt-0.3.9/src/ontogpt/clients/gpt4all_client.py
+-rw-r--r--   0        0        0     1701 2024-03-20 16:41:46.589763 ontogpt-0.3.9/src/ontogpt/clients/hfhub_client.py
+-rw-r--r--   0        0        0     8347 2024-03-20 16:41:46.589763 ontogpt-0.3.9/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0    20754 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1133 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5339 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3740 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0     2298 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/generic_engine.py
+-rw-r--r--   0        0        0    19245 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    25155 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0    11975 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/mapping_engine.py
+-rw-r--r--   0        0        0     7007 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/pheno_engine.py
+-rw-r--r--   0        0        0    11323 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/reasoner_engine.py
+-rw-r--r--   0        0        0     1047 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    25186 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      725 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    11906 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0    15495 2024-03-20 16:41:46.593762 ontogpt-0.3.9/src/ontogpt/evaluation/ctd/eval_ctd_ner.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2160 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    11455 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0     3469 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6329 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     9451 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1602 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/10338374.txt
+-rw-r--r--   0        0        0      811 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/17653185.txt
+-rw-r--r--   0        0        0     1516 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/18253950.txt
+-rw-r--r--   0        0        0     1617 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/24104886.txt
+-rw-r--r--   0        0        0     1968 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/28846760.txt
+-rw-r--r--   0        0        0     1324 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/29285689.txt
+-rw-r--r--   0        0        0      990 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/29441064.txt
+-rw-r--r--   0        0        0     1539 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/31767987.txt
+-rw-r--r--   0        0        0      744 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/PMC4961083.txt
+-rw-r--r--   0        0        0     1439 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/PMC6386158.txt
+-rw-r--r--   0        0        0     1001 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/PMC7003169.txt
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rwxr-xr-x   0        0        0       95 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0     1595 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/10338374_smoking.txt
+-rw-r--r--   0        0        0     1447 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review.txt
+-rw-r--r--   0        0        0     1191 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.txt
+-rw-r--r--   0        0        0     4791 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.yaml
+-rw-r--r--   0        0        0     1529 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/kidney/test.txt
+-rw-r--r--   0        0        0      913 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/kidney/test2.txt
+-rw-r--r--   0        0        0     3584 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/kidney/test3.txt
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/__init__.py
+-rw-r--r--   0        0        0    12890 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/eval_maxo.py
+-rw-r--r--   0        0        0     1158 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_12958596.yaml
+-rw-r--r--   0        0        0     1011 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301368.yaml
+-rw-r--r--   0        0        0     1156 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301450.yaml
+-rw-r--r--   0        0        0     2478 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301519.yaml
+-rw-r--r--   0        0        0     1351 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301527.yaml
+-rw-r--r--   0        0        0     1113 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301572.yaml
+-rw-r--r--   0        0        0     2022 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301644.yaml
+-rw-r--r--   0        0        0     2204 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301675.yaml
+-rw-r--r--   0        0        0     1246 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301765.yaml
+-rw-r--r--   0        0        0     1401 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_2063868.yaml
+-rw-r--r--   0        0        0     1404 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_26110198.yaml
+-rw-r--r--   0        0        0      902 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_27077170.yaml
+-rw-r--r--   0        0        0     2642 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_28406602.yaml
+-rw-r--r--   0        0        0     2006 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_29478819.yaml
+-rw-r--r--   0        0        0     1279 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_30488337.yaml
+-rw-r--r--   0        0        0     1417 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_36977302.yaml
+-rw-r--r--   0        0        0     1715 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_9543069.yaml
+-rw-r--r--   0        0        0      985 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0     4961 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/csv_wrapper.py
+-rw-r--r--   0        0        0      540 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     5036 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3562 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2487 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1760 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0     1617 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/template_loader.py
+-rw-r--r--   0        0        0     1756 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0    11723 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/models.yaml
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/ontex/__init__.py
+-rw-r--r--   0        0        0    68726 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/ontex/extractor.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1257 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0     1016 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      993 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
+-rw-r--r--   0        0        0      994 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
+-rw-r--r--   0        0        0      995 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
+-rw-r--r--   0        0        0      152 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/mapping/__init__.py
+-rw-r--r--   0        0        0     2424 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/mapping/eval-mapping.jinja2
+-rw-r--r--   0        0        0      158 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/phenopacket/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/phenopacket/phenopacket.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/qa/__init__.py
+-rw-r--r--   0        0        0       31 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/qa/generic.jinja2
+-rw-r--r--   0        0        0      150 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/reasoning/__init__.py
+-rw-r--r--   0        0        0     1471 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/reasoning/reasoning.jinja2
+-rw-r--r--   0        0        0      560 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0       67 2024-03-20 16:41:46.597762 ontogpt-0.3.9/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0     6733 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2354 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     5344 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/biotic_interaction.py
+-rw-r--r--   0        0        0     2179 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/biotic_interaction.yaml
+-rw-r--r--   0        0        0    10727 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/cell_type.py
+-rw-r--r--   0        0        0     8062 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/cell_type.yaml
+-rw-r--r--   0        0        0     2957 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3243 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     8322 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/composite_disease.py
+-rw-r--r--   0        0        0     4783 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/composite_disease.yaml
+-rw-r--r--   0        0        0     4260 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3971 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     7590 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6764 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     6325 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ctd_ner.py
+-rw-r--r--   0        0        0     5245 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ctd_ner.yaml
+-rw-r--r--   0        0        0    62750 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/data_sheets_schema.py
+-rw-r--r--   0        0        0    43120 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/data_sheets_schema.yaml
+-rw-r--r--   0        0        0     6328 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/datasheet.py
+-rw-r--r--   0        0        0     2618 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/datasheet.yaml
+-rw-r--r--   0        0        0     5722 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/desiccation.py
+-rw-r--r--   0        0        0     1814 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/desiccation.yaml
+-rw-r--r--   0        0        0     9250 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/diagnostic_procedure.py
+-rw-r--r--   0        0        0     4862 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/diagnostic_procedure.yaml
+-rw-r--r--   0        0        0    15718 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/dietitian_notes.py
+-rw-r--r--   0        0        0    16478 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/dietitian_notes.yaml
+-rw-r--r--   0        0        0     6087 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1978 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     4938 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/emapa_simple.py
+-rw-r--r--   0        0        0     1220 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/emapa_simple.yaml
+-rw-r--r--   0        0        0     6334 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/environmental_metadata.py
+-rw-r--r--   0        0        0     2777 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/environmental_metadata.yaml
+-rw-r--r--   0        0        0     6710 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     3307 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     5200 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/figure.py
+-rw-r--r--   0        0        0     1515 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/figure.yaml
+-rw-r--r--   0        0        0     5405 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1686 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     4501 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/genesummary.py
+-rw-r--r--   0        0        0     1168 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/genesummary.yaml
+-rw-r--r--   0        0        0     4915 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/go_simple.py
+-rw-r--r--   0        0        0     1110 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/go_simple.yaml
+-rw-r--r--   0        0        0     6017 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/go_terms.py
+-rw-r--r--   0        0        0     3499 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/go_terms.yaml
+-rw-r--r--   0        0        0     6404 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/go_terms_relational.py
+-rw-r--r--   0        0        0     3233 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/go_terms_relational.yaml
+-rw-r--r--   0        0        0     8714 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     5259 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     7150 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2418 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     5060 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/human_phenotype.py
+-rw-r--r--   0        0        0     1302 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/human_phenotype.yaml
+-rw-r--r--   0        0        0     8710 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4920 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     8156 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ibd_literature.py
+-rw-r--r--   0        0        0     4778 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ibd_literature.yaml
+-rw-r--r--   0        0        0     4997 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/kidney.py
+-rw-r--r--   0        0        0     1119 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/kidney.yaml
+-rw-r--r--   0        0        0     7960 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/maxo.py
+-rw-r--r--   0        0        0     4743 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/maxo.yaml
+-rw-r--r--   0        0        0     6733 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3307 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5901 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1684 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7746 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3961 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     4924 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/mondo_simple.py
+-rw-r--r--   0        0        0     1101 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/mondo_simple.yaml
+-rw-r--r--   0        0        0     5255 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/nmdc_schema_data.py
+-rw-r--r--   0        0        0     1669 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/nmdc_schema_data.yaml
+-rw-r--r--   0        0        0     5687 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2737 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     6701 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ontology_issue.py
+-rw-r--r--   0        0        0     3434 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/ontology_issue.yaml
+-rw-r--r--   0        0        0     5538 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1781 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7893 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3596 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7667 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     6018 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     5766 2024-03-20 16:41:46.601762 ontogpt-0.3.9/src/ontogpt/templates/traits.py
+-rw-r--r--   0        0        0     3553 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/templates/traits.yaml
+-rw-r--r--   0        0        0     8331 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4655 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     2114 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/utils/azure_settings.py
+-rw-r--r--   0        0        0      573 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/utils/model_utils.py
+-rw-r--r--   0        0        0      283 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/utils/parse_utils.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0     1137 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2045 2024-03-20 16:41:46.605762 ontogpt-0.3.9/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0     6241 1970-01-01 00:00:00.000000 ontogpt-0.3.9/PKG-INFO
```

### Comparing `ontogpt-0.3.8/LICENSE` & `ontogpt-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/README.md` & `ontogpt-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/pyproject.toml` & `ontogpt-0.3.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.3.8"
+version = "0.3.9"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>", "J. Harry Caufield <jhc@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 "ruamel.yaml" = ">=0.17.31"
 Jinja2 = {version = ">=3.1.2", optional = true}
 aiohttp = ">=3.8.4"
-airium = ">=0.2.5"
 beautifulsoup4 = ">=4.11.1"
 bioc = ">=2.0.post5"
 cachier = ">=2.1.0"
-class-resolver = ">=0.4.2"
 click = ">=8.1.3"
-eutils = ">=0.6.0"
 fastapi = {version = ">=0.88.0", optional = true}
 gilda = ">=1.0.0"
 gpt4 = ">=0.0.1"
-httpx = ">=0.23.3"
 huggingface_hub  = {version = ">=0.15.1", extras = ["huggingface"], optional = true}
 inflect = ">=6.0.2"
 inflection = ">=0.5.1"
-jsonlines = ">=3.1.0"
 linkml = "^1.5.7"
 linkml-owl = "^0.3.0"
 llm = ">=0.8"
 llm-gpt4all = {version = ">=0.2", extras = ["gpt4all"], optional = true}
 myst-parser = {version = ">=0.18.1", extras = ["docs"], optional = true}
 nlpcloud = ">=1.0.39"
-oaklib = ">=0.5.15"
-openai = ">=0.27.8, <1.0"
+oaklib = ">=0.5.28"
+openai = "^1.10.0"
 pydantic = ">=2.4.0"
-pystow = "^0.5.0"
-python-multipart = "^0.0.5"
 recipe-scrapers = {version = ">=14.35.0", extras = ["recipes"], optional = true}
 requests = "^2.31.0"
-requests-cache = ">=1.0.1"
+requests-cache = ">=1.2.0"
 sphinx = {version = ">=5.3.0", extras = ["docs"], optional = true}
 sphinx-autodoc-typehints = {version = ">=1.19.4", extras = ["docs"], optional = true}
 sphinx-click = {version = ">=4.3.0", extras = ["docs"], optional = true}
 sphinx-rtd-theme = {version = ">=1.0.0", extras = ["docs"], optional = true}
 streamlit = ">=1.22.0"
 textract = {version = "*", extras = ["textract"], optional = true}
-tiktoken = ">=0.3.3"
+tiktoken = ">=0.5.0"
 uvicorn = {version = ">=0.20.0", optional = true}
 wikipedia = ">=1.4.0"
 wikipedia-api = ">=0.5.8"
+dpath = "^2.1.6"
+toml = "^0.10.2"
+urllib3 = "<2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1.2"
 setuptools = ">=65.5.0"
 tox = ">=3.25.1"
 mkdocs-mermaid2-plugin = ">=0.6.0"
```

### Comparing `ontogpt-0.3.8/src/ontogpt/__init__.py` & `ontogpt-0.3.9/src/ontogpt/__init__.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/cli.py` & `ontogpt-0.3.9/src/ontogpt/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dataclasses import dataclass
 from io import BytesIO, TextIOWrapper
 from pathlib import Path
 from typing import List, Optional, Union
 
 import click
 import jsonlines
-import openai
+
 import yaml
 from oaklib import get_adapter
 from oaklib.cli import query_terms_iterator
 from oaklib.interfaces import OboGraphInterface
 from oaklib.io.streaming_csv_writer import StreamingCsvWriter
 from sssom.parsers import parse_sssom_table, to_mapping_set_document
 from sssom.util import to_mapping_set_dataframe
@@ -193,14 +193,20 @@
 )
 show_prompt_option = click.option(
     "--show-prompt/--no-show-prompt",
     default=False,
     show_default=True,
     help="If set, show all prompts passed to model through an API. Use with verbose setting.",
 )
+azure_select_option = click.option(
+    "--azure-select/--no-azure-select",
+    default=False,
+    show_default=True,
+    help="Use OpenAI model through Azure.",
+)
 
 
 @click.group()
 @click.option("-v", "--verbose", count=True)
 @click.option("-q", "--quiet")
 @click.option("--cache-db", help="Path to sqlite database to cache prompt-completion results")
 @click.option(
@@ -246,26 +252,28 @@
 @click.option(
     "--set-slot-value",
     "-S",
     multiple=True,
     help="Set slot value, e.g. --set-slot-value has_participant=protein",
 )
 @click.argument("input", required=False)
+@azure_select_option
 def extract(
     inputfile,
     template,
     target_class,
     dictionary,
     input,
     output,
     output_format,
     set_slot_value,
     use_textract,
     model,
     show_prompt,
+    azure_select,
     **kwargs,
 ):
     """Extract knowledge from text guided by schema, using SPIRES engine.
 
     Example:
 
         ontogpt extract -t gocam.GoCamAnnotations -i gocam-27929086.txt
@@ -321,14 +329,15 @@
     else:
         raise ValueError("No template specified. Use -t/--template option.")
 
     ke = SPIRESEngine(
         template_details=template_details,
         model=selectmodel["canonical_name"],
         model_source=selectmodel["provider"].lower(),
+        use_azure=azure_select,
         **kwargs,
     )
     if settings.cache_db:
         ke.client.cache_db_path = settings.cache_db
     if settings.skip_annotators:
         ke.client.skip_annotators = settings.skip_annotators
 
@@ -865,37 +874,42 @@
     "-C", "--context", required=True, help="domain e.g. anatomy, industry, health-related"
 )
 @click.argument("term")
 def synonyms(model, term, context, output, output_format, **kwargs):
     """Extract synonyms."""
     logging.info(f"Creating for {term}")
 
-    if model:
-        selectmodel = get_model_by_name(model)
-        model_source = selectmodel["provider"]
+    if not model:
+        model = DEFAULT_MODEL
 
-        if model_source != "OpenAI":
-            raise NotImplementedError("Model not yet supported for this function.")
+    selectmodel = get_model_by_name(model)
+    model_name = selectmodel["canonical_name"]
+    model_source = selectmodel["provider"]
+
+    if model_source != "OpenAI":
+        raise NotImplementedError("Model not yet supported for this function.")
 
-    ke = SynonymEngine()
-    out = str(ke.synonyms(term, context))
-    output.write(out)
+    ke = SynonymEngine(model=model_name, model_source=model_source.lower())
+    out = ke.synonyms(term, context)
+    for line in out:
+        output.write(f"{line}\n")
 
 
 @main.command()
 @output_option_txt
 @output_format_options
 @model_option
+@azure_select_option
 @click.option(
     "-C",
     "--context",
     help="domain e.g. anatomy, industry, health-related (NOT IMPLEMENTED - currently gene only)",
 )
 @click.argument("text", nargs=-1)
-def embed(text, context, output, model, output_format, **kwargs):
+def embed(text, context, output, model, output_format, azure_select, **kwargs):
     """Embed text.
 
     Not currently supported for open models.
     """
     if model:
         selectmodel = get_model_by_name(model)
         model_source = selectmodel["provider"]
@@ -904,30 +918,31 @@
             raise NotImplementedError("Model not yet supported for embeddings.")
     else:
         model = "text-embedding-ada-002"
 
     if not text:
         raise ValueError("Text must be passed")
 
-    client = OpenAIClient(model=model)
+    client = OpenAIClient(model=model, use_azure=azure_select)
     resp = client.embeddings(text)
     print(resp)
 
 
 @main.command()
 @output_option_txt
 @output_format_options
 @model_option
+@azure_select_option
 @click.option(
     "-C",
     "--context",
     help="domain e.g. anatomy, industry, health-related (NOT IMPLEMENTED - currently gene only)",
 )
 @click.argument("text", nargs=-1)
-def text_similarity(text, context, output, model, output_format, **kwargs):
+def text_similarity(text, context, output, model, output_format, azure_select, **kwargs):
     """Embed text.
 
     Not currently supported for open models.
     """
     if model:
         selectmodel = get_model_by_name(model)
         model_source = selectmodel["provider"]
@@ -944,30 +959,31 @@
         raise ValueError("Text must contain @")
     ix = text.index("@")
     text1 = " ".join(text[:ix])
     text2 = " ".join(text[ix + 1 :])
     print(text1)
     print(text2)
 
-    client = OpenAIClient(model=model)
+    client = OpenAIClient(model=model, use_azure=azure_select)
     sim = client.similarity(text1, text2, model=model)
     print(sim)
 
 
 @main.command()
 @output_option_txt
 @output_format_options
 @model_option
+@azure_select_option
 @click.option(
     "-C",
     "--context",
     help="domain e.g. anatomy, industry, health-related (NOT IMPLEMENTED - currently gene only)",
 )
 @click.argument("text", nargs=-1)
-def text_distance(text, context, output, model, output_format, **kwargs):
+def text_distance(text, context, output, model, output_format, azure_select, **kwargs):
     """Embed text and calculate euclidian distance between embeddings.
 
     Not currently supported for open models.
     """
     if model:
         selectmodel = get_model_by_name(model)
         model_source = selectmodel["provider"]
@@ -984,15 +1000,15 @@
         raise ValueError("Text must contain @")
     ix = text.index("@")
     text1 = " ".join(text[:ix])
     text2 = " ".join(text[ix + 1 :])
     print(text1)
     print(text2)
 
-    client = OpenAIClient(model=model)
+    client = OpenAIClient(model=model, use_azure=azure_select)
     sim = client.euclidian_distance(text1, text2, model=model)
     print(sim)
 
 
 @main.command()
 @output_option_txt
 @output_format_options
@@ -1135,16 +1151,26 @@
 def diagnose(
     phenopacket_files,
     model,
     output,
     **kwargs,
 ):
     """Diagnose a clinical case represented as one or more Phenopackets."""
+    if not phenopacket_files:
+        raise ValueError("No phenopacket files specified. Please provide one or more files.")
+
+    if not model:
+        model = DEFAULT_MODEL
+
+    selectmodel = get_model_by_name(model)
+    model_name = selectmodel["canonical_name"]
+    model_source = selectmodel["provider"]
+
     phenopackets = [json.load(open(f)) for f in phenopacket_files]
-    engine = PhenoEngine(model=model)
+    engine = PhenoEngine(model=model_name, model_source=model_source.lower())
     results = engine.evaluate(phenopackets)
     print(dump_minimal_yaml(results))
     write_obj_as_csv(results, output)
 
 
 @main.command()
 @inputfile_option
@@ -1305,37 +1331,38 @@
     output.write(yaml.dump(results.dict()))
 
 
 @main.command()
 def openai_models(**kwargs):
     """List OpenAI models for prompt completion."""
     ai = OpenAIClient()
-    for model in openai.Model.list():
+    for model in client.models.list():
         print(model)
 
 
 @main.command()
 @model_option
 @output_option_txt
 @output_format_options
 @show_prompt_option
+@azure_select_option
 @click.argument("input")
-def complete(model, input, output, output_format, show_prompt, **kwargs):
+def complete(model, input, output, output_format, show_prompt, azure_select, **kwargs):
     """Prompt completion."""
     if not model:
         model = DEFAULT_MODEL
     selectmodel = get_model_by_name(model)
     model_source = selectmodel["provider"]
     model_name = selectmodel["canonical_name"]
 
     text = open(input).read()
 
     # TODO: add support for other models
     if model_source == "OpenAI":
-        c = OpenAIClient(model=model_name)
+        c = OpenAIClient(model=model, use_azure=azure_select)
         results = c.complete(prompt=text, show_prompt=show_prompt)
 
     output.write(results)
 
 
 @main.command()
 @template_option
@@ -1357,20 +1384,21 @@
 
 @main.command()
 @click.option("-o", "--output", type=click.File(mode="w"), default=sys.stdout, help="Output file.")
 @output_format_options
 @model_option
 @click.option("-m", "match", help="Match string to use for filtering.")
 @click.option("-D", "database", help="Path to sqlite database.")
-def dump_completions(model, match, database, output, output_format):
+@azure_select_option
+def dump_completions(model, match, database, output, output_format, azure_select):
     """Dump cached completions."""
     if model:
         raise NotImplementedError("Caching not currently enabled for this model.")
     else:
-        client = OpenAIClient()
+        client = OpenAIClient(model=model, use_azure=azure_select)
 
     if database:
         client.cache_db_path = database
     if output_format == "jsonl":
         writer = jsonlines.Writer(output)
         for _engine, prompt, completion in client.cached_completions(match):
             writer.write(dict(engine=model, prompt=prompt, completion=completion))
@@ -1438,21 +1466,23 @@
     "-d",
     "--description",
     help="domain e.g. anatomy, industry, health-related (NOT IMPLEMENTED - currently gene only)",
 )
 @click.option(
     "--sections", multiple=True, help="sections to include e.g. medications, vital signs, etc."
 )
+@azure_select_option
 def clinical_notes(
     description,
     sections,
     output,
     model,
     show_prompt,
     output_format,
+    azure_select,
     **kwargs,
 ):
     """Create mock clinical notes.
 
     Example:
 
         ontogpt clinical-notes -d "middle-aged female patient with diabetes"
@@ -1468,15 +1498,15 @@
         model = DEFAULT_MODEL
     selectmodel = get_model_by_name(model)
     model_source = selectmodel["provider"]
     model_name = selectmodel["canonical_name"]
 
     # TODO: add support for other models
     if model_source == "OpenAI":
-        c = OpenAIClient(model=model_name)
+        c = OpenAIClient(model=model, use_azure=azure_select)
         results = c.complete(prompt=prompt, show_prompt=show_prompt)
 
     output.write(results)
 
 
 @main.command()
 def list_templates():
```

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/__init__.py` & `ontogpt-0.3.9/src/ontogpt/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/gpt4all_client.py` & `ontogpt-0.3.9/src/ontogpt/clients/gpt4all_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     # TODO: Explicitly deprecate interactive mode for local models
     interactive: Optional[bool] = None
 
     local_model: Gpt4AllModel = None
 
     def __post_init__(self):
         logging.info(f"Preparing {self.model} for local use...")
+        if self.model not in llm.get_model_aliases():
+            raise ValueError(f"Model {self.model} not found in llm.get_model_aliases()")
+        print(llm.get_model_aliases())
         self.local_model = llm.get_model(self.model)
 
     # Use this command in subsequent calls
     def chain_gpt4all_model(model, prompt_text):
         """Interact with a GPT4All model."""
         raw_output = model.prompt(prompt_text)
```

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/hfhub_client.py` & `ontogpt-0.3.9/src/ontogpt/clients/hfhub_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/openai_client.py` & `ontogpt-0.3.9/src/ontogpt/clients/openai_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,63 @@
 """OpenAI client."""
+
 import ast
 import logging
 import sqlite3
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
 from time import sleep
 from typing import Iterator, Optional, Tuple
 
 import numpy as np
-import openai
+from openai import OpenAI
+
 from oaklib.utilities.apikey_manager import get_apikey_value
+from openai import AzureOpenAI
+from ontogpt.utils.azure_settings import AZURE_MODEL, AZURE_API_VERSION, AZURE_ENDPOINT
 
 logger = logging.getLogger(__name__)
+
 NUM_RETRIES = 3
 
 
 @dataclass
 class OpenAIClient:
     # max_tokens: int = field(default_factory=lambda: 3000)
     model: str = field(default_factory=lambda: "gpt-3.5-turbo")
     cache_db_path: str = ""
     api_key: str = ""
     interactive: Optional[bool] = None
+    use_azure: Optional[bool] = None
 
     def __post_init__(self):
         if not self.api_key:
             self.api_key = get_apikey_value("openai")
-        openai.api_key = self.api_key
+
+        if self.use_azure:
+            self.model = field(default_factory=lambda: AZURE_MODEL)
+            # TODO: control client (Azure vs not) using a feature flag
+            self.client = AzureOpenAI(
+                api_version=AZURE_API_VERSION,
+                azure_endpoint=AZURE_ENDPOINT,
+                api_key=self.api_key,
+                azure_deployment=AZURE_MODEL,
+            )
+        else:
+            self.client = OpenAI(api_key=self.api_key)
 
     # TODO: Dynamically update max_tokens
-    def complete(self, prompt, max_tokens=3000, show_prompt: bool = False, **kwargs) -> str:
-        engine = self.model
+    def complete(self, prompt, max_tokens=500, show_prompt: bool = False, **kwargs) -> str:
+        # TODO: dynamically set model at call time
+        if self.use_azure:
+            engine = AZURE_MODEL
+        else:
+            engine = self.model
+
         logger.info(f"Complete: engine={engine}, prompt[{len(prompt)}]={prompt[0:100]}...")
         if show_prompt:
             logger.info(f" SENDING PROMPT:\n{prompt}")
         cur = self.db_connection()
         res = cur.execute("SELECT payload FROM cache WHERE prompt=? AND engine=?", (prompt, engine))
         payload = res.fetchone()
         if payload:
@@ -46,47 +68,56 @@
         i = 0
         while not response:
             i += 1
             logger.debug(f"Calling OpenAI API (attempt {i})...")
             try:
                 if self.interactive:
                     response = self._interactive_completion(prompt, engine, max_tokens, **kwargs)
-                elif self._must_use_chat_api():
-                    response = openai.ChatCompletion.create(
+                elif self._must_use_chat_api() and self.use_azure:
+                    response = self.client.chat.completions.create(
                         model=engine,
                         messages=[
                             {
                                 "role": "user",
                                 "content": prompt,
                             },
                         ],
                         max_tokens=max_tokens,
                         **kwargs,
                     )
+                elif self._must_use_chat_api() and not self.use_azure:
+                    response = self.client.chat.completions.create(model=engine,
+                    messages=[
+                        {
+                            "role": "user",
+                            "content": prompt,
+                        },
+                    ],
+                    max_tokens=max_tokens,
+                    **kwargs)                    
                 else:
-                    response = openai.Completion.create(
-                        engine=engine,
-                        prompt=prompt,
-                        max_tokens=max_tokens,
-                    )
+                    # TODO: remove chat api flag and eliminate references to legacy completions API
+                    raise ValueError("Unsupported mode")
                 break
             except Exception as e:
                 logger.error(f"OpenAI API connection error: {e}")
                 if i >= NUM_RETRIES:
                     raise e
                 sleep_time = 4**i
                 logger.info(f"Retrying {i} of {NUM_RETRIES} after {sleep_time} seconds...")
                 sleep(sleep_time)
 
+        #response = response.dict()
+        #print(response)
         if self.interactive:
             payload = response
         elif self._must_use_chat_api():
-            payload = response["choices"][0]["message"]["content"]
+            payload = response.choices[0].message.content
         else:
-            payload = response["choices"][0]["text"]
+            payload = response.choices[0].text
         logger.info(f"Storing payload of len: {len(payload)}")
         cur.execute(
             "INSERT INTO cache (prompt, engine, payload) VALUES (?, ?, ?)",
             (prompt, engine, payload),
         )
         cur.connection.commit()
         return payload
@@ -161,19 +192,17 @@
             "SELECT vector_as_string FROM embeddings_cache WHERE text=? AND engine=?", (text, model)
         )
         payload = res.fetchone()
         if payload:
             logger.info(f"Using cached embeddings for {model} {text[0:80]}...")
             return ast.literal_eval(payload[0])
         logger.info(f"querying OpenAI for {model} {text[0:80]}...")
-        response = openai.Embedding.create(
-            model=model,
-            input=text,
-        )
-        v = response.data[0]["embedding"]
+        response = self.client.embeddings.create(model=model,
+        input=text)
+        v = response.data[0].embedding
         logger.info(f"Storing embeddings of len: {len(v)}")
         cur.execute(
             "INSERT INTO embeddings_cache (text, engine, vector_as_string) VALUES (?, ?, ?)",
             (text, model, str(v)),
         )
         cur.connection.commit()
         return v
```

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.3.9/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/soup_client.py` & `ontogpt-0.3.9/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.3.9/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/conf/synonymizer-conf.yaml` & `ontogpt-0.3.9/src/ontogpt/conf/synonymizer-conf.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.3.9/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/embedding_similarity_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/generic_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/generic_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/halo_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 """
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set
 
-import openai
 import pydantic
 import tiktoken
 import yaml
 from linkml.utils.schema_fixer import uncamel
 from linkml_runtime.utils.formatutils import camelcase
 from oaklib.datamodels.obograph import Graph
 from oaklib.datamodels.vocabulary import IS_A
@@ -77,15 +76,14 @@
         default_factory=lambda: tiktoken.get_encoding("cl100k_base")
     )
 
     def __post_init__(self):
         self.template_class = self._get_template_class("halo.OntologyElement")
         self.client = OpenAIClient(model=self.engine)
         self.api_key = self._get_openai_api_key()
-        openai.api_key = self.api_key
 
     def seed(self, seed_ontology: Ontology):
         """Seed the engine with an initial ontology.
 
         :param seed_ontology:
         :return:
         """
```

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/knowledge_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from types import ModuleType
 from typing import Dict, Iterator, List, Optional, TextIO, Union
 from urllib.parse import quote
 
 import inflection
-import openai
 import pydantic
 import tiktoken
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model import ClassDefinition, ElementName, SlotDefinition
 from oaklib import BasicOntologyInterface, get_adapter
 from oaklib.datamodels.text_annotator import TextAnnotationConfiguration
@@ -87,17 +86,18 @@
     """
     Abstract base class for all knowledge engines.
 
     A Knowledge Engine is able to extract knowledge from text, utilizing
     knowledge sources plus LLMs
     """
 
-    template_details: tuple
+    template_details: tuple = None
     """Tuple containing loaded template details, including:
-    (LinkML class, module, python class, SchemaView object)"""
+    (LinkML class, module, python class, SchemaView object).
+    May be None because some child classes do not require a template."""
 
     template_class: ClassDefinition = None
     """LinkML Class for the template.
     This is derived from the template and does not need to be set manually."""
 
     template_pyclass = None
     """Python class for the template.
@@ -161,14 +161,17 @@
     """Cache of last text."""
 
     last_prompt: str = ""
     """Cache of last prompt used."""
 
     encoding = None
 
+    use_azure: Optional[bool] = None
+    """Use Azure API for OpenAI models, if True."""
+
     def __post_init__(self):
         if self.template_details:
             (
                 self.template_class,
                 self.template_module,
                 self.template_pyclass,
                 self.schemaview,
@@ -178,27 +181,31 @@
         if not self.model:
             self.model = DEFAULT_MODEL
         if self.mappers is None:
             logging.info("Using mappers (currently hardcoded)")
             self.mappers = [get_adapter("translator:")]
 
         self.set_up_client(model_source=self.model_source)
+        if not self.client:
+            if self.model_source:
+                raise ValueError(f"No client available for {self.model_source}")
+            else:
+                raise ValueError("No client available because model source is unknown.")
 
         # We retrieve encoding for OpenAI models
         # but tiktoken won't work for other models
         if self.model_source == "openai":
             try:
                 self.encoding = tiktoken.encoding_for_model(self.client.model)
             except KeyError:
                 self.encoding = tiktoken.encoding_for_model(DEFAULT_MODEL)
                 logger.error(f"Could not find encoding for model {self.client.model}")
 
     def set_api_key(self, key: str):
         self.api_key = key
-        openai.api_key = key
 
     def extract_from_text(
         self, text: str, cls: ClassDefinition = None, object: OBJECT = None
     ) -> ExtractionResult:
         raise NotImplementedError
 
     def extract_from_file(self, file: Union[str, Path, TextIO]) -> pydantic.BaseModel:
@@ -591,13 +598,12 @@
         """
         Select the appropriate client based on the model's source.
 
         Args: model_source (str): lowercase string indicating the source of the model,
             e.g., openai
         """
         if model_source == "openai":
-            self.client = OpenAIClient(model=self.model)
+            self.client = OpenAIClient(model=self.model, use_azure=self.use_azure)
             logging.info("Setting up OpenAI client API Key")
             self.api_key = self._get_openai_api_key()
-            openai.api_key = self.api_key
         elif model_source == "gpt4all":
             self.client = GPT4AllClient(model=self.model)
```

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/mapping_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/mapping_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/pheno_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/pheno_engine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reasoner engine."""
+
 import json
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from jinja2 import Template
@@ -56,14 +57,38 @@
         if isinstance(template_path, Path):
             template_path = str(template_path)
         if isinstance(template_path, str):
             # create a Jinja2 template object
             with open(template_path) as file:
                 template_txt = file.read()
                 template = Template(template_txt)
+        # Account for missing template fields if necessary
+        # TODO: make this its own function
+        for subject_key in ["sex", "ageAtCollection"]:
+            if subject_key not in phenopacket["subject"]:
+                logging.warning(f"Missing subject key: {subject_key}. Setting to 'UNKNOWN'.")
+                phenopacket["subject"][subject_key] = "UNKNOWN"
+            if subject_key == "ageAtCollection":
+                if "timeAtLastEncounter" in phenopacket["subject"]:
+                    if "age" in phenopacket["subject"]["timeAtLastEncounter"]:
+                        if (
+                            "iso8601duration"
+                            in phenopacket["subject"]["timeAtLastEncounter"]["age"]
+                        ):
+                            logging.warning("Found patient age in timeAtLastEncounter. Updating.")
+                            phenopacket["subject"]["ageAtCollection"] = {
+                                "age": phenopacket["subject"]["timeAtLastEncounter"]["age"][
+                                    "iso8601duration"
+                                ]
+                            }
+                else:
+                    phenopacket["subject"]["ageAtCollection"] = {"age": "UNKNOWN"}
+        if "phenotypicFeatures" not in phenopacket:
+            logging.warning(f"No phenotypicFeatures found in phenopacket {phenopacket['id']}.")
+            logging.warning("Diagnosis accuracy may be very inaccurate.")
         prompt = template.render(
             phenopacket=phenopacket,
         )
         payload = self.client.complete(prompt, max_tokens=self.completion_length)
         print(payload)
         try:
             obj = json.loads(payload)
@@ -78,19 +103,26 @@
         mondo = self.mondo
         if not isinstance(mondo, MappingProviderInterface):
             raise TypeError("Mondo adapter must implement MappingProviderInterface")
 
         results = []
         for phenopacket in phenopackets:
             dp = DiagnosisPrediction(case_id=phenopacket["id"], model=self.model)
-            validated_disease_ids = {disease["term"]["id"] for disease in phenopacket["diseases"]}
+            try:
+                validated_disease_ids = {
+                    disease["term"]["id"] for disease in phenopacket["diseases"]
+                }
+            except KeyError:
+                logger.warning(f"No diseases found in phenopacket {phenopacket['id']}")
+                validated_disease_ids = set()
             dp.validated_disease_ids = list(validated_disease_ids)
-            dp.validated_disease_labels = [
-                disease["term"]["label"] for disease in phenopacket["diseases"]
-            ]
+            if validated_disease_ids:
+                dp.validated_disease_labels = [
+                    disease["term"]["label"] for disease in phenopacket["diseases"]
+                ]
             dp.validated_mondo_disease_ids = []
             dp.validated_mondo_disease_labels = []
             for disease_id in validated_disease_ids:
                 mondo_id = mondo.normalize(disease_id, target_prefixes=["MONDO"])
                 if mondo_id:
                     dp.validated_mondo_disease_ids.append(mondo_id)
                     dp.validated_mondo_disease_labels.append(mondo.label(mondo_id))
```

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/reasoner_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/reasoner_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/resolver.py` & `ontogpt-0.3.9/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/spires_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.3.9/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.3.9/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.3.9/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ctd/eval_ctd_ner.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/ctd/eval_ctd_ner.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/10338374.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/10338374.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/17653185.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/17653185.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/18253950.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/18253950.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/24104886.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/24104886.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/28846760.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/28846760.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/29285689.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/29285689.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/29441064.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/29441064.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/31767987.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/31767987.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/PMC4961083.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/PMC4961083.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/PMC6386158.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/PMC6386158.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/Abstracts/PMC7003169.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/Abstracts/PMC7003169.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/10338374_smoking.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/10338374_smoking.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/ibd/text_data/PMC6386158_review_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/kidney/test.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/kidney/test.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/kidney/test2.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/kidney/test2.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/kidney/test3.txt` & `ontogpt-0.3.9/src/ontogpt/evaluation/kidney/test3.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/eval_maxo.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/eval_maxo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_12958596.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_12958596.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301368.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301368.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301450.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301450.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301519.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301519.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301527.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301527.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301572.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301572.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301644.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301644.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301675.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301675.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301765.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_20301765.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_2063868.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_2063868.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_26110198.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_26110198.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_27077170.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_27077170.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_28406602.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_28406602.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_29478819.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_29478819.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_30488337.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_30488337.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_36977302.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_36977302.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/maxo/test_cases/maxo_case_9543069.yaml` & `ontogpt-0.3.9/src/ontogpt/evaluation/maxo/test_cases/maxo_case_9543069.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.3.9/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/csv_wrapper.py` & `ontogpt-0.3.9/src/ontogpt/io/csv_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,29 +102,29 @@
                     continue
 
     return lines
 
 
 def write_obj_as_csv(obj: Any, file, minimize=True, index_field=None) -> None:
     if isinstance(obj, BaseModel):
-        obj = obj.dict()
+        obj = obj.model_dump()
     if isinstance(obj, list):
         rows = obj
     elif not isinstance(obj, dict):
         if not index_field:
             index_fields = [k for k, v in obj.items() if v and isinstance(v, list)]
             if len(index_fields) == 1:
                 index_field = index_fields[0]
                 logger.warning(f"Using {index_field} as index field")
         rows = obj[index_field]
     else:
         raise ValueError(f"Cannot dump {obj} as CSV")
     if isinstance(file, Path) or isinstance(file, str):
         file = open(file, "w", encoding="utf-8")
-    rows = [row.dict() if isinstance(row, BaseModel) else row for row in rows]
+    rows = [row.model_dump() if isinstance(row, BaseModel) else row for row in rows]
     writer = csv.DictWriter(file, fieldnames=rows[0].keys(), delimiter="\t")
     writer.writeheader()
     for row in rows:
 
         def _str(s):
             if s is None:
                 return ""
```

### Comparing `ontogpt-0.3.8/src/ontogpt/io/exporter.py` & `ontogpt-0.3.9/src/ontogpt/io/exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/html_exporter.py` & `ontogpt-0.3.9/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.3.9/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.3.9/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.3.9/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/template_loader.py` & `ontogpt-0.3.9/src/ontogpt/io/template_loader.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.3.9/src/ontogpt/io/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/models.yaml` & `ontogpt-0.3.9/src/ontogpt/models.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,26 @@
     creators:
       - OpenAI
     requirements:
       diskspace: "N/A"
       memory: "N/A"
     is_default: true
 
+  - name: MODEL_GPT_3_5_TURBO_0125
+    canonical_name: "gpt-3.5-turbo-0125"
+    alternative_names:
+      - "gpt3.5-0125"
+      - "openai-gpt-3.5-turbo-0125"
+    provider: OpenAI
+    creators:
+      - OpenAI
+    requirements:
+      diskspace: "N/A"
+      memory: "N/A"
+
   - name: MODEL_GPT_3_5_TURBO_16K
     canonical_name: "gpt-3.5-turbo-16k"
     alternative_names:
       - "gpt3.5-16k"
       - "chatgpt-16k"
       - "chatgpt3.5-16k"
       - "openai-gpt-3.5-turbo-16k"
@@ -51,17 +63,30 @@
     requirements:
       diskspace: "N/A"
       memory: "N/A"
 
   - name: MODEL_GPT_4_1106_PREVIEW
     canonical_name: "gpt-4-1106-preview"
     alternative_names:
+      - "gpt4turbo-1106"
+      - "gpt-4-turbo-1106"
+      - "openai-gpt-4-1106-preview"
+    provider: OpenAI
+    creators:
+      - OpenAI
+    requirements:
+      diskspace: "N/A"
+      memory: "N/A"
+
+  - name: MODEL_GPT_4_0125_PREVIEW
+    canonical_name: "gpt-4-0125-preview"
+    alternative_names:
       - "gpt4turbo"
       - "gpt-4-turbo"
-      - "openai-gpt-4-1106-preview"
+      - "openai-gpt-4-0125-preview"
     provider: OpenAI
     creators:
       - OpenAI
     requirements:
       diskspace: "N/A"
       memory: "N/A"
```

### Comparing `ontogpt-0.3.8/src/ontogpt/ontex/extractor.py` & `ontogpt-0.3.9/src/ontogpt/ontex/extractor.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/mapping/eval-mapping.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/mapping/eval-mapping.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/phenopacket/phenopacket.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/phenopacket/phenopacket.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/reasoning/reasoning.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/reasoning/reasoning.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/prompts/similarity/connections.jinja2` & `ontogpt-0.3.9/src/ontogpt/prompts/similarity/connections.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/biological_process.py` & `ontogpt-0.3.9/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/biological_process.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/biological_process
 name: biological-process-template
 title: Biological Process Template
 description: >-
   A template for GO-CAMs
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   CL: http://purl.obolibrary.org/obo/CL_
   GO: http://purl.obolibrary.org/obo/GO_
   HGNC: http://identifiers.org/hgnc/
   bp: http://w3id.org/ontogpt/biological-process-template
   linkml: https://w3id.org/linkml/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/biotic_interaction.py` & `ontogpt-0.3.9/src/ontogpt/templates/biotic_interaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/biotic_interaction.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/biotic_interaction.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/biotic_interaction
 name: biotic-interaction-template
 title: Biotic Interaction Template
 description: >-
   A template for biotic interactions
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   MESH: http://identifiers.org/mesh/
   NCBITaxon: http://purl.obolibrary.org/obo/NCBITAXON_
   RO: http://purl.obolibrary.org/obo/RO_
   bp: http://w3id.org/ontogpt/biotic-interaction-template
   col: https://www.catalogueoflife.org/data/taxon/
   gbif: https://www.gbif.org/species/
   itis: https://www.itis.gov/servlet/SingleRpt/SingleRpt?search_topic=TSN&search_value=
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/cell_type.py` & `ontogpt-0.3.9/src/ontogpt/templates/cell_type.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/cell_type.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/cell_type.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/cell_type
 name: cell_type
 title: Composite Disease
 description: >-
   A template for representing cell types
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   AUTO: http://w3id.org/ontogpt/auto/
   BFO: http://purl.obolibrary.org/obo/BFO_
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   CL: http://purl.obolibrary.org/obo/CL_
   FBbt: http://purl.obolibrary.org/obo/FBbt_
   GO: http://purl.obolibrary.org/obo/GO_
   HGNC: http://identifiers.org/hgnc/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/class_enrichment.py` & `ontogpt-0.3.9/src/ontogpt/templates/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/class_enrichment.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/class_enrichment.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 title: Class Enrichment Datamodel
 name: class-enrichment
 description: >-
   A datamodel for representing the results of class enrichment on gene sets
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   OBI: http://purl.obolibrary.org/obo/OBI_
   STATO: http://purl.obolibrary.org/obo/STATO_
   bpa: https://bioportal.bioontology.org/annotator/
   linkml: https://w3id.org/linkml/
   oa: http://www.w3.org/ns/oa#
   ontoenrich: https://w3id.org/oak/class-enrichment/
   pav: http://purl.org/pav/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/composite_disease.py` & `ontogpt-0.3.9/src/ontogpt/templates/composite_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/composite_disease.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/composite_disease.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/composite_disease
 name: composite_disease
 title: Composite Disease
 description: >-
   A template for representing composite disease concepts
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   HGNC: http://identifiers.org/hgnc/
   HP: http://purl.obolibrary.org/obo/HP_
   MAXO: http://purl.obolibrary.org/obo/MAXO_
   RO: http://purl.obolibrary.org/obo/RO_
   composite_disease: http://w3id.org/ontogpt/composite_disease/
   linkml: https://w3id.org/linkml/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/core.py` & `ontogpt-0.3.9/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/core.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/core.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 id: http://w3id.org/ontogpt/core
 name: core
 title: AI core Template
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   NCIT: http://purl.obolibrary.org/obo/NCIT_
   RO: http://purl.obolibrary.org/obo/RO_
   biolink: https://w3id.org/biolink/vocab/
   core: http://w3id.org/ontogpt/core/
   linkml: https://w3id.org/linkml/
   rdfs: http://www.w3.org/2000/01/rdf-schema#
 description: Core upper level
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ctd.py` & `ontogpt-0.3.9/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/ctd.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   Relation (CDR) Task (BC5CDR).
 see_also:
   - https://biocreative.bioinformatics.udel.edu/media/store/files/2015/BC5CDR_overview.final.pdf
   - https://academic.oup.com/database/article/doi/10.1093/database/baw068/2630414
 source: https://biocreative.bioinformatics.udel.edu/tasks/biocreative-v/track-3-cdr/
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   MESH: http://identifiers.org/mesh/
   drug: http://w3id.org/ontogpt/drug/
   linkml: https://w3id.org/linkml/
 
 default_prefix: drug
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ctd_ner.py` & `ontogpt-0.3.9/src/ontogpt/templates/ctd_ner.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ctd_ner.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/ctd_ner.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 see_also:
   - https://biocreative.bioinformatics.udel.edu/media/store/files/2015/BC5CDR_overview.final.pdf
   - https://academic.oup.com/database/article/doi/10.1093/database/baw068/2630414
 source: >-
   https://biocreative.bioinformatics.udel.edu/tasks/biocreative-v/track-3-cdr/
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   MESH: http://identifiers.org/mesh/
   ctdner: http://w3id.org/ontogpt/ctd_ner
   linkml: https://w3id.org/linkml/
 
 default_prefix: ctdner
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/data_sheets_schema.py` & `ontogpt-0.3.9/src/ontogpt/templates/data_sheets_schema.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/data_sheets_schema.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/data_sheets_schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 description: |-
   A LinkML schema for Datasheets for Datasets.
 license: MIT
 see_also:
   - https://bridge2ai.github.io/data-sheets-schema
 
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   biolink: https://w3id.org/biolink/
   csvw: http://www.w3.org/ns/csvw#
   data_sheets_schema: https://w3id.org/bridge2ai/data-sheets-schema/
   datasets: https://w3id.org/linkml/report
   dcat: http://www.w3.org/ns/dcat#
   example: https://example.org/
   formats: http://www.w3.org/ns/formats/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/datasheet.py` & `ontogpt-0.3.9/src/ontogpt/templates/datasheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,22 +44,22 @@
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Dataset(NamedEntity):
     """
     A document that contains a description of a dataset.
     """
     name: Optional[str] = Field(None, description="""The name of the dataset.""")
     subsets: Optional[List[str]] = Field(default_factory=list, description="""Semicolon-separated list of names of any subsets of the dataset.""")
@@ -68,84 +70,84 @@
     limitations: Optional[str] = Field(None, description="""Known limitations of the dataset. This should be no more than 1 sentence.""")
     warnings: Optional[str] = Field(None, description="""Warnings regarding content or application of the dataset.""")
     references: Optional[List[str]] = Field(default_factory=list, description="""Semicolon-separated list of publications describing the data or the process used to produce it.""")
     license: Optional[str] = Field(None, description="""The set of rules defining the rights of the developer and the users of the dataset, for example, BSD-3 or CC0.""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Organization(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 Dataset.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/datasheet.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/datasheet.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   as defined by the Datasheets for Datasets model
   (see https://github.com/bridge2ai/data-sheets-schema),
   itself based on Gebru et al. (2021)
   (https://cacm.acm.org/magazines/2021/12/256932-datasheets-for-datasets/abstract)
 
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   d4d: http://w3id.org/ontogpt/datasheet
 
 default_prefix: d4d
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/desiccation.py` & `ontogpt-0.3.9/src/ontogpt/templates/desiccation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,115 +44,115 @@
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class EntityContainingDocument(NamedEntity):
     
     environmental_conditions: Optional[List[str]] = Field(default_factory=list, description="""A semicolon-separated list of environmental terms.""")
     taxa: Optional[List[str]] = Field(default_factory=list, description="""A semicolon-separated list of taxonomic terms of living things.""")
     traits: Optional[List[str]] = Field(default_factory=list, description="""A semicolon-separated list of plant traits.""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class EnvironmentalCondition(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Taxon(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Trait(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 EntityContainingDocument.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/desiccation.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/desiccation.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/desiccation
 name: desiccation
 title: desiccationTemplate
 description: >-
   A template for extracting ChEBI, GO, NCBITAXON, PO, TO, PECO
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   desiccation: http://w3id.org/ontogpt/desiccation
 
 default_prefix: desiccation
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/diagnostic_procedure.py` & `ontogpt-0.3.9/src/ontogpt/templates/diagnostic_procedure.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/diagnostic_procedure.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/diagnostic_procedure.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 name: diagnostic_procedure
 title: Diagnostic Procedure Template
 description: >-
   A template for clinical diagnostic procedures and the
   phenotypes they may contribute to.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   HP: http://purl.obolibrary.org/obo/HP_
   LOINC: http://loinc.org/rdf/
   OBA: http://purl.obolibrary.org/obo/OBA_
   PATO: http://purl.obolibrary.org/obo/PATO_
   RO: http://purl.obolibrary.org/obo/RO_
   UO: http://purl.obolibrary.org/obo/UO_
   biolink: https://w3id.org/biolink/vocab/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/dietitian_notes.py` & `ontogpt-0.3.9/src/ontogpt/templates/gocam.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,41 +21,54 @@
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
     pass
 
 
+class GeneLocationEnum(str):
+    
+    
+    dummy = "dummy"
+    
+
+class GOCellComponentType(str):
+    
+    
+    dummy = "dummy"
+    
+
+class CellType(str):
+    
+    
+    dummy = "dummy"
+    
+
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
     NOT_APPLICABLE = "NOT_APPLICABLE"
     
     NOT_MENTIONED = "NOT_MENTIONED"
     
     
 
-class ClinicalObservationSet(ConfiguredBaseModel):
-    """
-    A set of sets of clinical observations.
-    """
-    observations: Optional[List[str]] = Field(default_factory=list)
-    
-    
-
-class MalnutritionObservations(ConfiguredBaseModel):
+class GoCamAnnotations(ConfiguredBaseModel):
     
-    malnutrition_presence: Optional[str] = Field(None, description="""True if the patient is malnourished, False otherwise. N/A if not provided.""")
-    malnutrition_risk: Optional[str] = Field(None, description="""True if the patient has a demonstrable risk for malnutrition, False otherwise. N/A if not provided.""")
-    severity: Optional[str] = Field(None, description="""The severity of the patient's malnutrition, if present. This may be Mild, Moderate, or Severe. In general, a patient receiving less than 50% of their estimated energy requirement for greater than 5 days is considered to have severe malnutrition. N/A if not provided.""")
-    acute_or_chronic: Optional[str] = Field(None, description="""The duration of the patient's malnutrition, if present. For pediatric patients, acute malnutrition is less than 3 months, and chronic malnutrition is greater than 3 months. This may be Acute or Chronic. N/A if not provided.""")
-    diagnosis: Optional[str] = Field(None, description="""The patient's malnutrition diagnosis, if present. This should not include modifiers like 'severe'. N/A if not provided.""")
-    etiology: Optional[str] = Field(None, description="""The cause of the patient's malnutrition, if known. This may be due to acute or chronic disease or social/behavioral factors. N/A if not provided.""")
+    genes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of genes""")
+    organisms: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of organism taxons""")
+    gene_organisms: Optional[List[GeneOrganismRelationship]] = Field(default_factory=list)
+    activities: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of molecular activities""")
+    gene_functions: Optional[List[GeneMolecularActivityRelationship]] = Field(default_factory=list, description="""semicolon-separated list of gene to molecular activity relationships""")
+    cellular_processes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of cellular processes""")
+    pathways: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of pathways""")
+    gene_gene_interactions: Optional[List[GeneGeneInteraction]] = Field(default_factory=list, description="""semicolon-separated list of gene to gene interactions""")
+    gene_localizations: Optional[List[GeneSubcellularLocalizationRelationship]] = Field(default_factory=list, description="""semicolon-separated list of genes plus their location in the cell; for example, \"gene1 / cytoplasm; gene2 / mitochondrion\"""")
     
     
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
@@ -72,82 +85,102 @@
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class ClinicalObservations(NamedEntity):
-    """
-    A set of clinical observations about a single patient at a single time.
-    """
-    is_pediatric: Optional[str] = Field(None)
-    is_preterm: Optional[str] = Field(None)
-    patient_height: Optional[QuantitativeValueWithMetric] = Field(None)
-    patient_weight: Optional[QuantitativeValueWithMetric] = Field(None)
-    head_circumference: Optional[QuantitativeValueWithMetric] = Field(None)
-    malnutrition_status: Optional[MalnutritionObservations] = Field(None)
-    diet_supplementation: Optional[List[str]] = Field(default_factory=list, description="""A semicolon-separated list of the patient's diet supplementation therapies. All acronyms should be expanded, omitting the original acronym. Relevant acronyms: PO: per os/by mouth, NPO: nil per os/nothing by mouth, TPN: total parenteral nutrition, PN: parenteral nutrition, EN: enteral nutrition, IBW: ideal body weight, UBW: usual body weight, ABW: actual body weight, D#%: dextrose percentage (e.g. D5%) for PN infusion, AA # g/kg/d: amino acid provisions (may also be in percentages) for PN infusion, SMOF # g/kg/d: soy MCT olive fish oil emulsion for PN infusion, GIR: glucose infusion rate, SBS: short bowel syndrome, LIS: low intermittent suction, BW: birth weight, EHM: exclusively human milk, RTBW: return to birth weight, Mg: magnesium, Phos: phosphorus, GI: gastrointestinal, PICC: peripherally inserted central catheter, DOL: day of life, TG: triglycerides, KUB: Kidney ureter bladder CT""")
-    nutrition_support: Optional[List[str]] = Field(default_factory=list, description="""A semicolon-separated list of the patient's nutrition support therapies, usually enteral or parenteral nutrition. All acronyms should be expanded, omitting the original acronym. Relevant acronyms: PO: per os/by mouth, NPO: nil per os/nothing by mouth, TPN: total parenteral nutrition, PN: parenteral nutrition, EN: enteral nutrition, IBW: ideal body weight, UBW: usual body weight, ABW: actual body weight, D#%: dextrose percentage (e.g. D5%) for PN infusion, AA # g/kg/d: amino acid provisions (may also be in percentages) for PN infusion, SMOF # g/kg/d: soy MCT olive fish oil emulsion for PN infusion, GIR: glucose infusion rate, SBS: short bowel syndrome, LIS: low intermittent suction, BW: birth weight, EHM: exclusively human milk, RTBW: return to birth weight, Mg: magnesium, Phos: phosphorus, GI: gastrointestinal, PICC: peripherally inserted central catheter, DOL: day of life, TG: triglycerides, KUB: Kidney ureter bladder CT""")
+class Gene(NamedEntity):
+    
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class DietSupplementation(NamedEntity):
-    """
-    A diet supplementation therapy.
-    """
+class Pathway(NamedEntity):
+    
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class NutritionSupport(NamedEntity):
-    """
-    A nutrition support therapy used to treat or prevent malnutrition.
-    """
+class CellularProcess(NamedEntity):
+    
+    id: str = Field(..., description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
+    
+    
+
+class MolecularActivity(NamedEntity):
+    
+    id: str = Field(..., description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
+    
+    
+
+class GeneLocation(NamedEntity):
+    
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class Disease(NamedEntity):
+class Organism(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class Unit(NamedEntity):
+class Molecule(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
     
 
-class QuantitativeValue(CompoundExpression):
+class GeneOrganismRelationship(CompoundExpression):
+    
+    gene: Optional[str] = Field(None)
+    organism: Optional[str] = Field(None)
+    
+    
+
+class GeneMolecularActivityRelationship(CompoundExpression):
+    
+    gene: Optional[str] = Field(None)
+    molecular_activity: Optional[str] = Field(None)
+    
+    
+
+class GeneMolecularActivityRelationship2(CompoundExpression):
+    
+    gene: Optional[str] = Field(None)
+    molecular_activity: Optional[str] = Field(None)
+    target: Optional[str] = Field(None)
+    
+    
+
+class GeneSubcellularLocalizationRelationship(CompoundExpression):
     
-    value: Optional[str] = Field(None, description="""The value of the quantity, or N/A if not provided.""")
-    unit: Optional[str] = Field(None, description="""The unit of the quantity.""")
+    gene: Optional[str] = Field(None)
+    location: Optional[str] = Field(None)
     
     
 
-class QuantitativeValueWithMetric(QuantitativeValue):
+class GeneGeneInteraction(CompoundExpression):
     
-    percentile: Optional[str] = Field(None, description="""The reported percentile of the value, as compared to a reference patient population. Always positive, on a scale from 0 to 99%. May be reported as \"X%\", \"X%ile\", or \"Xth percentile\", where X is the value. N/A if not provided.""")
-    zscore: Optional[str] = Field(None, description="""The relative standard deviation of the value, as a function of the percentile. May be positive or negative. May be reported as \"z-score\", \"Z-score\", or \"Z\", followed by the value. N/A if not provided.""")
-    value: Optional[str] = Field(None, description="""The value of the quantity, or N/A if not provided.""")
-    unit: Optional[str] = Field(None, description="""The unit of the quantity.""")
+    gene1: Optional[str] = Field(None)
+    gene2: Optional[str] = Field(None)
     
     
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
@@ -202,26 +235,30 @@
     object_text: Optional[str] = Field(None)
     
     
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
-ClinicalObservationSet.model_rebuild()
-MalnutritionObservations.model_rebuild()
+GoCamAnnotations.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
-ClinicalObservations.model_rebuild()
-DietSupplementation.model_rebuild()
-NutritionSupport.model_rebuild()
-Disease.model_rebuild()
-Unit.model_rebuild()
+Gene.model_rebuild()
+Pathway.model_rebuild()
+CellularProcess.model_rebuild()
+MolecularActivity.model_rebuild()
+GeneLocation.model_rebuild()
+Organism.model_rebuild()
+Molecule.model_rebuild()
 CompoundExpression.model_rebuild()
-QuantitativeValue.model_rebuild()
-QuantitativeValueWithMetric.model_rebuild()
+GeneOrganismRelationship.model_rebuild()
+GeneMolecularActivityRelationship.model_rebuild()
+GeneMolecularActivityRelationship2.model_rebuild()
+GeneSubcellularLocalizationRelationship.model_rebuild()
+GeneGeneInteraction.model_rebuild()
 Triple.model_rebuild()
 TextWithTriples.model_rebuild()
 TextWithEntity.model_rebuild()
 RelationshipType.model_rebuild()
 Publication.model_rebuild()
 AnnotatorResult.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/drug.py` & `ontogpt-0.3.9/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/drug.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/drug.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/drug
 name: drug
 title: Drug Template
 description: >-
   A template for Drugs and drug mechanism
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   HGNC: http://identifiers.org/hgnc/
   MESH: http://identifiers.org/mesh/
   drug: http://w3id.org/ontogpt/drug/
   linkml: https://w3id.org/linkml/
 
 default_prefix: drug
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/emapa_simple.py` & `ontogpt-0.3.9/src/ontogpt/templates/emapa_simple.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/emapa_simple.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/emapa_simple.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/emapa_simple
 name: emapa_simple
 title: Simple EMAPA Extraction Template
 description: >-
   Simple Mouse Developmental Anatomy Ontology Extraction Template
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   EMAPA: http://purl.obolibrary.org/obo/EMAPA_
   GO: http://purl.obolibrary.org/obo/GO_
   emapa_simple: http://w3id.org/ontogpt/emapa_simple
   linkml: https://w3id.org/linkml/
 
 default_prefix: emapa_simple
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/environmental_metadata.py` & `ontogpt-0.3.9/src/ontogpt/templates/environmental_metadata.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/environmental_metadata.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/environmental_metadata.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 name: environmental-metadata
 title: Environmental sample metadata
 description: >-
   A template for categorizing Environmental Data Initiative
   data entries. See https://github.com/EDIorg/EDIorg-repository-index
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   ENVO: http://purl.obolibrary.org/obo/ENVO_
   envmd: http://w3id.org/ontogpt/environmental-metadata
   linkml: https://w3id.org/linkml/
 
 default_prefix: envmd
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.3.9/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/environmental_sample.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/environmental-sample
 name: environmental-sample
 title: Environmental Sample Template
 description: >-
   A template for Environmental Samples
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   ENVO: http://purl.obolibrary.org/obo/ENVO_
   PATO: http://purl.obolibrary.org/obo/PATO_
   UO: http://purl.obolibrary.org/obo/UO_
   linkml: https://w3id.org/linkml/
   sample: http://w3id.org/ontogpt/environmental-sample/
 
 default_prefix: sample
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/figure.py` & `ontogpt-0.3.9/src/ontogpt/templates/figure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -37,108 +39,108 @@
 class FigureCaption(ConfiguredBaseModel):
     """
     A caption for a figure from a scientific paper. The caption may contain multiple subpanel descriptions.
     """
     title: Optional[str] = Field(None, description="""the overall title of the figure caption""")
     subpanel: Optional[List[SubPanel]] = Field(default_factory=list, description="""a subpanel of the figure""")
     
-        
+    
 
 class SubPanel(ConfiguredBaseModel):
     """
     A subcomponent of the overall figure caption.
     """
     id: Optional[str] = Field(None, description="""The identifier for this figure subpanel""")
     text: Optional[str] = Field(None, description="""The text associated with this figure subpanel""")
     info: Optional[str] = Field(None, description="""any information from the overall figure caption that applies to that subpanel (which may be duplicated across other subpanels).""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 FigureCaption.model_rebuild()
 SubPanel.model_rebuild()
 ExtractionResult.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/figure.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/figure.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/figure
 name: figure-template
 title: Plazi Figure Template
 description: >-
   A template for Plazi figures and sub-parts
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   fig: http://w3id.org/ontogpt/figure-template
 
 default_prefix: fig
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.3.9/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/gene_description_term.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/go_term
 name: go-term-template
 title: GO Term Template
 description: >-
   A simple GO term template for NER
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   GO: http://purl.obolibrary.org/obo/GO_
   HGNC: http://identifiers.org/hgnc/
   MESH: http://identifiers.org/mesh/
   MONDO: http://purl.obolibrary.org/obo/MONDO_
   bp: http://w3id.org/ontogpt/biological-process-template
   linkml: https://w3id.org/linkml/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/genesummary.py` & `ontogpt-0.3.9/src/ontogpt/templates/genesummary.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/genesummary.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/genesummary.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/gocam
 name: genesummary-template
 title: genesummary Template
 description: >-
   A template for genesummary
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CL: http://purl.obolibrary.org/obo/CL_
   GO: http://purl.obolibrary.org/obo/GO_
   HGNC: http://identifiers.org/hgnc/
   PR: http://purl.obolibrary.org/obo/PR_
   UniProtKB: http://purl.uniprot.org/uniprot/
   genesummary: http://w3id.org/ontogpt/genesummary/
   linkml: https://w3id.org/linkml/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/go_simple.py` & `ontogpt-0.3.9/src/ontogpt/templates/go_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,99 +44,99 @@
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class OntologyTermSet(NamedEntity):
     
     terms: Optional[List[str]] = Field(default_factory=list, description="""A semicolon-separated list of any Gene Ontology terms.""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class OntologyTerm(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 OntologyTermSet.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/go_simple.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/go_simple.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/go_simple
 name: go_simple
 title: Simple Gene Ontology Extraction Template
 description: >-
   Simple Gene Ontology Extraction Template
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   go_simple: http://w3id.org/ontogpt/go_simple
   GO: http://purl.obolibrary.org/obo/GO_
 
 default_prefix: go_simple
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/go_terms.py` & `ontogpt-0.3.9/src/ontogpt/templates/go_terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class GOBiologicalProcessType(str):
     
     
     dummy = "dummy"
     
@@ -60,117 +62,117 @@
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class BiologicalProcess(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CellularComponent(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class MolecularFunction(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class Document(TextWithEntity):
     """
     A document that contains biological or biomedical concepts.
     """
     biologicalprocesses: Optional[List[str]] = Field(default_factory=list, description="""One or more biological processes, as defined by the Gene Ontology.""")
     cellularcomponents: Optional[List[str]] = Field(default_factory=list, description="""One or more cellular components, as defined by the Gene Ontology.""")
     molecularfunctions: Optional[List[str]] = Field(default_factory=list, description="""One or more molecular functions, as defined by the Gene Ontology.""")
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 BiologicalProcess.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/go_terms.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/go_terms.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/go_terms
 name: go_terms
 title: Gene Ontology Term and CURIE Extraction
 description: >-
   A template for GO Term and ID extraction.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   go_terms: http://w3id.org/ontogpt/go_terms
 
 default_prefix: go_terms
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/go_terms_relational.py` & `ontogpt-0.3.9/src/ontogpt/templates/go_terms_relational.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,129 +44,129 @@
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Protein(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class GOTerm(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class ProteinToGORelationship(Triple):
     """
     A triple where the subject is a protein and the object is a GO term.
     """
     subject: Optional[str] = Field(None, description="""The protein participating in the relationship, for example: Klp61F, GATA binding protein 3, S-formylglutathione hydrolase""")
     predicate: Optional[str] = Field(None, description="""The relationship type, usually HAS ANNOTATION.""")
     object: Optional[str] = Field(None, description="""The Gene Ontology term participating in the relationship, for example: cytosol, plasma cell differentiation, small-subunit processome""")
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the protein.""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the GO term.""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class Document(TextWithTriples):
     """
     A document that contains biological or biomedical concepts.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[ProteinToGORelationship]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class ProteinToGOPredicate(RelationshipType):
     """
     A predicate for protein to GO term relationships.
     """
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 Protein.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/go_terms_relational.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/go_terms_relational.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 description: >-
   A template for GO Term and ID extraction,
   as relations involving specific proteins.
   Note this does not make a distinction between
   GO term types.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   go_terms_relational: http://w3id.org/ontogpt/go_terms_relational
 
 default_prefix: go_terms_relational
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/gocam.py` & `ontogpt-0.3.9/src/ontogpt/templates/ibd.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     
     NOT_APPLICABLE = "NOT_APPLICABLE"
     
     NOT_MENTIONED = "NOT_MENTIONED"
     
     
 
-class GoCamAnnotations(ConfiguredBaseModel):
+class IBDAnnotations(ConfiguredBaseModel):
     
     genes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of genes""")
     organisms: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of organism taxons""")
     gene_organisms: Optional[List[GeneOrganismRelationship]] = Field(default_factory=list)
     activities: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of molecular activities""")
     gene_functions: Optional[List[GeneMolecularActivityRelationship]] = Field(default_factory=list, description="""semicolon-separated list of gene to molecular activity relationships""")
     cellular_processes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of cellular processes""")
@@ -235,15 +235,15 @@
     object_text: Optional[str] = Field(None)
     
     
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
-GoCamAnnotations.model_rebuild()
+IBDAnnotations.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 Gene.model_rebuild()
 Pathway.model_rebuild()
 CellularProcess.model_rebuild()
 MolecularActivity.model_rebuild()
 GeneLocation.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/gocam.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/gocam
 name: gocam-template
 title: GO-CAM Template
 description: >-
   A template for GO-CAMs
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   CL: http://purl.obolibrary.org/obo/CL_
   EFO: http://www.ebi.ac.uk/efo/EFO_
   GO: http://purl.obolibrary.org/obo/GO_
   HGNC: http://identifiers.org/hgnc/
   NCBITaxon: http://purl.obolibrary.org/obo/NCBITAXON_
   PR: http://purl.obolibrary.org/obo/PR_
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/halo.py` & `ontogpt-0.3.9/src/ontogpt/templates/halo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -34,128 +36,128 @@
     
     
 
 class Ontology(ConfiguredBaseModel):
     
     elements: Optional[List[OntologyElement]] = Field(default_factory=list)
     
-        
+    
 
 class OntologyElement(ConfiguredBaseModel):
     
     name: str = Field(..., description="""the name of the entity""")
     context: Optional[str] = Field(None, description="""the ontology to which this belongs (single-valued)""")
     description: Optional[str] = Field(None, description="""a textual description of the entity (single-valued)""")
     synonyms: Optional[List[str]] = Field(default_factory=list, description="""a list of alternative names of the entity""")
     categories: Optional[List[str]] = Field(default_factory=list, description="""a list of the categories to which this entity belongs""")
     subclass_of: Optional[List[str]] = Field(default_factory=list, description="""a list of parent class (superclasses) of this entity""")
     part_of: Optional[List[str]] = Field(default_factory=list, description="""a list of things this element is part of""")
     subtypes: Optional[List[str]] = Field(default_factory=list, description="""a list of child classes (subclasses) of this entity""")
     parts: Optional[List[str]] = Field(default_factory=list, description="""a list of names of things this element has as parts (components)""")
     equivalent_to: Optional[str] = Field(None, description="""an OWL class expression with the necessary and sufficient conditions for this entity to be an instance of this class""")
     
-        
+    
 
 class Category(OntologyElement):
     
     name: str = Field(..., description="""the name of the entity""")
     context: Optional[str] = Field(None, description="""the ontology to which this belongs (single-valued)""")
     description: Optional[str] = Field(None, description="""a textual description of the entity (single-valued)""")
     synonyms: Optional[List[str]] = Field(default_factory=list, description="""a list of alternative names of the entity""")
     categories: Optional[List[str]] = Field(default_factory=list, description="""a list of the categories to which this entity belongs""")
     subclass_of: Optional[List[str]] = Field(default_factory=list, description="""a list of parent class (superclasses) of this entity""")
     part_of: Optional[List[str]] = Field(default_factory=list, description="""a list of things this element is part of""")
     subtypes: Optional[List[str]] = Field(default_factory=list, description="""a list of child classes (subclasses) of this entity""")
     parts: Optional[List[str]] = Field(default_factory=list, description="""a list of names of things this element has as parts (components)""")
     equivalent_to: Optional[str] = Field(None, description="""an OWL class expression with the necessary and sufficient conditions for this entity to be an instance of this class""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 Ontology.model_rebuild()
 OntologyElement.model_rebuild()
 Category.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/halo.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/halo.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/halo
 name: ontology-class
 title: Ontology Class Template
 description: >-
   A template for Ontology Classes
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   oc: http://w3id.org/ontogpt/ontology-class-template
   BFO: http://purl.obolibrary.org/obo/BFO_
 
 default_prefix: oc
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/human_phenotype.py` & `ontogpt-0.3.9/src/ontogpt/templates/human_phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/human_phenotype.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/human_phenotype.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/human_phenotype
 name: human_phenotype-template
 title: Human Phenotype Extraction Template
 description: >-
   A template for extracting human phenotypes to HPO terms
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   HP: http://purl.obolibrary.org/obo/HP_
   human_phenotype: http://w3id.org/ontogpt/human_phenotype
   linkml: https://w3id.org/linkml/
 
 default_prefix: human_phenotype
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ibd.py` & `ontogpt-0.3.9/src/ontogpt/templates/reaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,246 +18,198 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
-class GeneLocationEnum(str):
+class NullDataOptions(str, Enum):
     
     
-    dummy = "dummy"
+    UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
-
-class GOCellComponentType(str):
+    NOT_APPLICABLE = "NOT_APPLICABLE"
     
+    NOT_MENTIONED = "NOT_MENTIONED"
     
-    dummy = "dummy"
     
 
-class CellType(str):
+class GeneToReaction(ConfiguredBaseModel):
     
+    gene: Optional[str] = Field(None, description="""name of the gene that catalyzes the reaction""")
+    reactions: Optional[Dict[str, Reaction]] = Field(default_factory=dict, description="""semicolon separated list of reaction equations (e.g. A+B = C+D) catalyzed by the gene""")
+    organism: Optional[str] = Field(None)
     
-    dummy = "dummy"
     
 
-class NullDataOptions(str, Enum):
-    
-    
-    UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
-    
-    NOT_APPLICABLE = "NOT_APPLICABLE"
+class ReactionDocument(ConfiguredBaseModel):
     
-    NOT_MENTIONED = "NOT_MENTIONED"
-    
-    
-
-class IBDAnnotations(ConfiguredBaseModel):
+    genes: Optional[List[str]] = Field(default_factory=list, description="""semicolon separated list of genes that catalyzes the mentioned reactions""")
+    reactions: Optional[Dict[str, Reaction]] = Field(default_factory=dict, description="""semicolon separated list of reaction equations (e.g. A+B = C+D) catalyzed by the gene""")
+    gene_reaction_pairings: Optional[List[GeneReactionPairing]] = Field(default_factory=list, description="""semicolon separated list of gene to reaction pairings""")
+    organism: Optional[str] = Field(None)
+    has_evidence: Optional[List[str]] = Field(default_factory=list, description="""evidence for the reaction""")
     
-    genes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of genes""")
-    organisms: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of organism taxons""")
-    gene_organisms: Optional[List[GeneOrganismRelationship]] = Field(default_factory=list)
-    activities: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of molecular activities""")
-    gene_functions: Optional[List[GeneMolecularActivityRelationship]] = Field(default_factory=list, description="""semicolon-separated list of gene to molecular activity relationships""")
-    cellular_processes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of cellular processes""")
-    pathways: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of pathways""")
-    gene_gene_interactions: Optional[List[GeneGeneInteraction]] = Field(default_factory=list, description="""semicolon-separated list of gene to gene interactions""")
-    gene_localizations: Optional[List[GeneSubcellularLocalizationRelationship]] = Field(default_factory=list, description="""semicolon-separated list of genes plus their location in the cell; for example, \"gene1 / cytoplasm; gene2 / mitochondrion\"""")
     
-        
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class Gene(NamedEntity):
+class Reaction(NamedEntity):
     
+    label: Optional[str] = Field(None, description="""the name of the reaction""")
+    description: Optional[str] = Field(None, description="""a textual description of the reaction""")
+    synonyms: Optional[List[str]] = Field(default_factory=list, description="""alternative names of the reaction""")
+    subclass_of: Optional[str] = Field(None, description="""the category to which this biological process belongs""")
+    left_side: Optional[List[str]] = Field(default_factory=list, description="""semicolon separated list of chemical entities on the left side""")
+    right_side: Optional[List[str]] = Field(default_factory=list, description="""semicolon separated list of chemical entities on the right side""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class Pathway(NamedEntity):
+class ReactionGrouping(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class CellularProcess(NamedEntity):
+class ChemicalEntity(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class MolecularActivity(NamedEntity):
+class Evidence(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class GeneLocation(NamedEntity):
+class Gene(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Organism(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
-
-class Molecule(NamedEntity):
-    
-    id: str = Field(..., description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
-
-class GeneOrganismRelationship(CompoundExpression):
-    
-    gene: Optional[str] = Field(None)
-    organism: Optional[str] = Field(None)
-    
-        
-
-class GeneMolecularActivityRelationship(CompoundExpression):
-    
-    gene: Optional[str] = Field(None)
-    molecular_activity: Optional[str] = Field(None)
-    
-        
-
-class GeneMolecularActivityRelationship2(CompoundExpression):
-    
-    gene: Optional[str] = Field(None)
-    molecular_activity: Optional[str] = Field(None)
-    target: Optional[str] = Field(None)
     
-        
 
-class GeneSubcellularLocalizationRelationship(CompoundExpression):
-    
-    gene: Optional[str] = Field(None)
-    location: Optional[str] = Field(None)
+class GeneReactionPairing(CompoundExpression):
     
-        
-
-class GeneGeneInteraction(CompoundExpression):
+    gene: Optional[str] = Field(None, description="""name of the gene that catalyzes the reaction""")
+    reaction: Optional[str] = Field(None, description="""equation describing the reaction (e.g. A+B = C+D) catalyzed by the gene""")
     
-    gene1: Optional[str] = Field(None)
-    gene2: Optional[str] = Field(None)
     
-        
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
-IBDAnnotations.model_rebuild()
+GeneToReaction.model_rebuild()
+ReactionDocument.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
+Reaction.model_rebuild()
+ReactionGrouping.model_rebuild()
+ChemicalEntity.model_rebuild()
+Evidence.model_rebuild()
 Gene.model_rebuild()
-Pathway.model_rebuild()
-CellularProcess.model_rebuild()
-MolecularActivity.model_rebuild()
-GeneLocation.model_rebuild()
 Organism.model_rebuild()
-Molecule.model_rebuild()
 CompoundExpression.model_rebuild()
-GeneOrganismRelationship.model_rebuild()
-GeneMolecularActivityRelationship.model_rebuild()
-GeneMolecularActivityRelationship2.model_rebuild()
-GeneSubcellularLocalizationRelationship.model_rebuild()
-GeneGeneInteraction.model_rebuild()
+GeneReactionPairing.model_rebuild()
 Triple.model_rebuild()
 TextWithTriples.model_rebuild()
 TextWithEntity.model_rebuild()
 RelationshipType.model_rebuild()
 Publication.model_rebuild()
 AnnotatorResult.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/ibd.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/gocam
 name: gocam-template
 title: GO-CAM Template
 description: >-
   A template for GO-CAMs
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   gocam: http://w3id.org/ontogpt/gocam/
   GO: http://purl.obolibrary.org/obo/GO_
   CL: http://purl.obolibrary.org/obo/CL_
 
 default_prefix: gocam
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ibd_literature.py` & `ontogpt-0.3.9/src/ontogpt/templates/ibd_literature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -39,160 +41,160 @@
     genes: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of genes""")
     exposures: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of exposures""")
     gene_exposures_relationships: Optional[List[GeneExposureRelationship]] = Field(default_factory=list, description="""semicolon-separated list of gene to molecular activity relationships""")
     diseases: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of diseases""")
     cellular_process: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of cellular processes""")
     disease_cellular_process_relationships: Optional[List[DiseaseCellularProcessRelationship]] = Field(default_factory=list, description="""semicolon-separated list of disease to cellular process relationships""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Gene(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class ChemicalExposure(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class ChemicalExposureToGenePredicate(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Disease(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CellularProcess(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class DiseaseToCellularProcessPredicate(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class GeneExposureRelationship(CompoundExpression):
     
     subject: Optional[str] = Field(None, description="""The name of the exposure, such as a exposure to a chemical toxin.""")
     predicate: Optional[str] = Field(None, description="""The name of the type of relationship between a chemical exposure and a gene.""")
     object: Optional[str] = Field(None, description="""The name of the gene in the pair. This comes second in the pair.""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the chemical exposure.""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the gene.""")
     
-        
+    
 
 class DiseaseCellularProcessRelationship(CompoundExpression):
     
     subject: Optional[str] = Field(None, description="""The name of the disease.""")
     predicate: Optional[str] = Field(None, description="""The name of the type of relationship between a disease and a cellular process.""")
     object: Optional[str] = Field(None, description="""The name of the cellular process.""")
     subject_qualifier: Optional[str] = Field(None)
     object_qualifier: Optional[str] = Field(None)
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 IBDAnnotations.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ibd_literature.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/ibd_literature.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/ibd_literature
 name: ibd-literature-template
 title: IBD Literature Template
 description: >-
   A template for extracting information from IBD literature
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   ECTO: http://purl.obolibrary.org/obo/ECTO_
   ExO: http://purl.obolibrary.org/obo/ExO_
   HGNC: http://identifiers.org/hgnc/
   NCIT: http://purl.obolibrary.org/obo/NCIT_
   MONDO: http://purl.obolibrary.org/obo/MONDO_
   GO: http://purl.obolibrary.org/obo/GO_
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/kidney.py` & `ontogpt-0.3.9/src/ontogpt/templates/kidney.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -35,112 +37,112 @@
     
 
 class KidneyAnnotations(ConfiguredBaseModel):
     
     cell_type: Optional[List[str]] = Field(default_factory=list)
     gene: Optional[List[str]] = Field(default_factory=list, description="""A gene""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CellType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Gene(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 KidneyAnnotations.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/kidney.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/kidney.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/biological_process
 name: kidney-template
 title: kidney-template
 description: >-
   A template for extracting kidney info from literature
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   kidney: http://w3id.org/ontogpt/kidney-template
 
 default_prefix: kidney
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/maxo.py` & `ontogpt-0.3.9/src/ontogpt/templates/maxo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/maxo.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/maxo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 name: maxo
 title: Template for Medical Action Extraction
 description: >-
   A template for extracting relationships relevant to the
   MAXO medical action ontology.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   HP: http://purl.obolibrary.org/obo/HP_
   MAXO: http://purl.obolibrary.org/obo/MAXO_
   MONDO: http://purl.obolibrary.org/obo/MONDO_
   OBA: http://purl.obolibrary.org/obo/OBA_
   PATO: http://purl.obolibrary.org/obo/PATO_
   RO: http://purl.obolibrary.org/obo/RO_
   biolink: https://w3id.org/biolink/vocab/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.3.9/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/mendelian_disease
 name: mendelian_disease-template
 title: GO-CAM Template
 description: >-
   A template for GO-CAMs
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   HGNC: http://identifiers.org/hgnc/
   HP: http://purl.obolibrary.org/obo/HP_
   MONDO: http://purl.obolibrary.org/obo/MONDO_
   linkml: https://w3id.org/linkml/
   mendelian_disease: http://w3id.org/ontogpt/mendelian_disease/
 
 default_prefix: mendelian_disease
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.3.9/src/ontogpt/templates/metabolic_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,111 +44,111 @@
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class MetabolicProcess(NamedEntity):
     
     label: Optional[str] = Field(None, description="""the name of the metabolic process""")
     description: Optional[str] = Field(None, description="""a textual description of the metabolic process""")
     synonyms: Optional[List[str]] = Field(default_factory=list, description="""alternative names of the metabolic process""")
     subclass_of: Optional[List[str]] = Field(default_factory=list, description="""a semicolon separated list of broader metabolic processes which this is a subclass of""")
     category: Optional[str] = Field(None, description="""the category of metabolic process, e.g metabolic process, catabolic process, biosynthetic process, small molecule sensor activity""")
     inputs: Optional[List[str]] = Field(default_factory=list, description="""the inputs of the metabolic process""")
     outputs: Optional[List[str]] = Field(default_factory=list, description="""the outputs of the metabolic process""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
     
-        
+    
 
 class MetabolicProcessCategory(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class ChemicalEntity(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
 MetabolicProcess.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/metabolic_process.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/metabolic_process
 name: metabolic-process-template
 title: metabolic Process Template
 description: >-
   A template for GO-CAMs
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   bp: http://w3id.org/ontogpt/metabolic-process-template
 
 default_prefix: bp
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.3.9/src/ontogpt/templates/metagenome_study.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,168 +44,168 @@
     treatments: Optional[List[str]] = Field(default_factory=list)
     measurements: Optional[List[Measurement]] = Field(default_factory=list)
     location: Optional[List[str]] = Field(default_factory=list, description="""the sites at which the study was conducted""")
     environmental_material: Optional[List[str]] = Field(default_factory=list, description="""the environmental material that was sampled""")
     sequencing_technologies: Optional[str] = Field(None)
     organisms: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of all studied organism taxons""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Location(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class EnvironmentalMaterial(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Environment(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Variable(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Unit(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class SequencingTechnology(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Treatment(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Organism(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Measurement(CompoundExpression):
     
     value: Optional[str] = Field(None, description="""the value of the measurement""")
     unit: Optional[str] = Field(None, description="""the unit of the measurement""")
     
-        
+    
 
 class CausalRelationship(CompoundExpression):
     
     cause: Optional[str] = Field(None, description="""the variable that is the cause of the effect""")
     effect: Optional[str] = Field(None, description="""the things that is affected""")
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 Study.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/metagenome_study.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/metagenome
 name: environmental-metagenome
 title: Environmental Metagenome Template
 description: >-
   A template for Environmental Metagenome Studies
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   eg: http://w3id.org/ontogpt/environmental-metagenome/
 
 default_prefix: eg
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/mondo_simple.py` & `ontogpt-0.3.9/src/ontogpt/templates/mondo_simple.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/mondo_simple.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/mondo_simple.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/mondo_simple
 name: mondo_simple
 title: Simple MONDO Extraction Template
 description: >-
   Simple MONDO Disease Ontology Extraction Template
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   MONDO: http://purl.obolibrary.org/obo/MONDO_
   linkml: https://w3id.org/linkml/
   mondo_simple: http://w3id.org/ontogpt/emapa_simple
 
 default_prefix: mondo_simple
 default_range: string
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/nmdc_schema_data.py` & `ontogpt-0.3.9/src/ontogpt/templates/nmdc_schema_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -36,112 +38,112 @@
 
 class Dataset(ConfiguredBaseModel):
     
     packageid: Optional[str] = Field(None, description="""The internal identifier for the dataset""")
     environmental_material: Optional[List[str]] = Field(default_factory=list, description="""the environmental material that was sampled""")
     environments: Optional[List[str]] = Field(default_factory=list, description="""the environmental context in which the study was conducted""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class EnvironmentalMaterial(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Environment(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 Dataset.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/nmdc_schema_data.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/nmdc_schema_data.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 description: >-
   A template for populating nmdc-schema required slots
   from data entries. Primarily, this involves three different
   levels corresponding to ENVO terms, as well as conversion
   of NLCD values and FAO soil taxonomy classes to ENVO.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   nmdcsd: http://w3id.org/ontogpt/nmdc-schema-data
 
 default_prefix: nmdcsd
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.3.9/src/ontogpt/templates/ontology_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -36,117 +38,117 @@
 
 class LogicalDefinition(ConfiguredBaseModel):
     
     genus: Optional[List[str]] = Field(default_factory=list)
     differentiating_characteristic_relationship: Optional[str] = Field(None)
     differentiating_characteristic_parents: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class OntologyClass(NamedEntity):
     
     label: Optional[str] = Field(None, description="""the name of the main entity being defined""")
     description: Optional[str] = Field(None, description="""a textual description of the entity""")
     synonyms: Optional[List[str]] = Field(default_factory=list, description="""alternative names of the entity""")
     categories: Optional[List[str]] = Field(default_factory=list, description="""the categories to which this entity belongs.""")
     subclass_of: Optional[List[str]] = Field(default_factory=list)
     logical_definition: Optional[LogicalDefinition] = Field(None, description="""the necessary and sufficient conditions for this entity to be an instance of this class""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
     
-        
+    
 
 class Relation(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 LogicalDefinition.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/ontology_class.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/ontology_class
 name: ontology-class
 title: Ontology Class Template
 description: >-
   A template for Ontology Classes
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   oc: http://w3id.org/ontogpt/ontology-class-template
 
 default_prefix: oc
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ontology_issue.py` & `ontogpt-0.3.9/src/ontogpt/templates/ontology_issue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class ProblemType(str, Enum):
     
     
     UNKNOWN = "UNKNOWN"
     
@@ -73,122 +75,122 @@
     title: Optional[str] = Field(None, description="""the title of the issue""")
     summary: Optional[str] = Field(None, description="""a high level summary""")
     status: Optional[str] = Field(None)
     domains: Optional[List[str]] = Field(default_factory=list, description="""What part of the ontology does this pertain to.""")
     problem_list: Optional[List[OntologyProblem]] = Field(default_factory=list, description="""A list of problems stated at a high level""")
     proposed_changes: Optional[List[OntologyChange]] = Field(default_factory=list, description="""What part of the ontology does this pertain to.""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class OntologyClass(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class OntologyProblem(CompoundExpression):
     
     description: Optional[str] = Field(None, description="""A succinct description of the problem""")
     severity: Optional[str] = Field(None, description="""How severe is this problem?""")
     category: Optional[ProblemType] = Field(None, description="""What category does this problem fall into?""")
     about: Optional[List[str]] = Field(default_factory=list, description="""What terms in the ontology is this problem about?""")
     
-        
+    
 
 class OntologyChange(CompoundExpression):
     
     description: Optional[str] = Field(None, description="""A succinct description of the proposed change""")
     category: Optional[ChangeType] = Field(None, description="""What kind of change?""")
     about: Optional[List[str]] = Field(default_factory=list, description="""What terms in the ontology will this change affect?""")
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 OntologyIssue.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/ontology_issue.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/ontology_issue.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/ontology_issue
 name: ontology-issue
 title: Ontology Issue Data Model
 description: >-
   A data model for representing the contents of a GitHub issue on an ontology tracker
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   oc: http://w3id.org/ontogpt/ontology-class-template
 
 default_prefix: oc
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/phenotype.py` & `ontogpt-0.3.9/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/phenotype.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/eq
 name: eq-template
 title: EQ Template
 description: >-
   A template for Computational Phenotypes
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   PATO: http://purl.obolibrary.org/obo/PATO_
   PR: http://purl.obolibrary.org/obo/PR_
   UBERON: http://purl.obolibrary.org/obo/UBERON_
   linkml: https://w3id.org/linkml/
   phenotype: http://w3id.org/ontogpt/phenotype/
 keywords:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/reaction.py` & `ontogpt-0.3.9/src/ontogpt/templates/recipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,29 +32,22 @@
     
     NOT_APPLICABLE = "NOT_APPLICABLE"
     
     NOT_MENTIONED = "NOT_MENTIONED"
     
     
 
-class GeneToReaction(ConfiguredBaseModel):
+class Recipe(ConfiguredBaseModel):
     
-    gene: Optional[str] = Field(None, description="""name of the gene that catalyzes the reaction""")
-    reactions: Optional[Dict[str, Reaction]] = Field(default_factory=dict, description="""semicolon separated list of reaction equations (e.g. A+B = C+D) catalyzed by the gene""")
-    organism: Optional[str] = Field(None)
-    
-    
-
-class ReactionDocument(ConfiguredBaseModel):
-    
-    genes: Optional[List[str]] = Field(default_factory=list, description="""semicolon separated list of genes that catalyzes the mentioned reactions""")
-    reactions: Optional[Dict[str, Reaction]] = Field(default_factory=dict, description="""semicolon separated list of reaction equations (e.g. A+B = C+D) catalyzed by the gene""")
-    gene_reaction_pairings: Optional[List[GeneReactionPairing]] = Field(default_factory=list, description="""semicolon separated list of gene to reaction pairings""")
-    organism: Optional[str] = Field(None)
-    has_evidence: Optional[List[str]] = Field(default_factory=list, description="""evidence for the reaction""")
+    url: str = Field(...)
+    label: Optional[str] = Field(None, description="""the name of the recipe""")
+    description: Optional[str] = Field(None, description="""a brief textual description of the recipe""")
+    categories: Optional[List[str]] = Field(default_factory=list, description="""a semicolon separated list of the categories to which this recipe belongs""")
+    ingredients: Optional[List[Ingredient]] = Field(default_factory=list, description="""a semicolon separated list of the ingredients plus quantities of the recipe""")
+    steps: Optional[List[Step]] = Field(default_factory=list, description="""a semicolon separated list of the individual steps involved in this recipe""")
     
     
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
@@ -71,71 +64,82 @@
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class Reaction(NamedEntity):
+class FoodType(NamedEntity):
     
-    label: Optional[str] = Field(None, description="""the name of the reaction""")
-    description: Optional[str] = Field(None, description="""a textual description of the reaction""")
-    synonyms: Optional[List[str]] = Field(default_factory=list, description="""alternative names of the reaction""")
-    subclass_of: Optional[str] = Field(None, description="""the category to which this biological process belongs""")
-    left_side: Optional[List[str]] = Field(default_factory=list, description="""semicolon separated list of chemical entities on the left side""")
-    right_side: Optional[List[str]] = Field(default_factory=list, description="""semicolon separated list of chemical entities on the right side""")
     id: str = Field(..., description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class ReactionGrouping(NamedEntity):
+class RecipeCategory(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class ChemicalEntity(NamedEntity):
+class Action(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class Evidence(NamedEntity):
+class UtensilType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class Gene(NamedEntity):
+class Unit(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
     
 
-class Organism(NamedEntity):
+class CompoundExpression(ConfiguredBaseModel):
     
-    id: str = Field(..., description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
+    None
     
     
 
-class CompoundExpression(ConfiguredBaseModel):
+class Ingredient(CompoundExpression):
     
-    None
+    food_item: Optional[FoodItem] = Field(None, description="""the food item""")
+    amount: Optional[Quantity] = Field(None, description="""the quantity of the ingredient, e.g. 2 lbs""")
+    
+    
+
+class Quantity(CompoundExpression):
+    
+    value: Optional[str] = Field(None, description="""the value of the quantity""")
+    unit: Optional[str] = Field(None, description="""the unit of the quantity, e.g. grams, cups, etc.""")
+    
+    
+
+class Step(CompoundExpression):
+    
+    action: Optional[str] = Field(None, description="""the action taken in this step (e.g. mix, add)""")
+    inputs: Optional[List[FoodItem]] = Field(default_factory=list, description="""a semicolon separated list of the inputs of this step""")
+    outputs: Optional[List[FoodItem]] = Field(default_factory=list, description="""a semicolon separated list of the outputs of this step""")
+    utensils: Optional[List[str]] = Field(default_factory=list, description="""the kitchen utensil used in this step (e.g. pan, bowl)""")
     
     
 
-class GeneReactionPairing(CompoundExpression):
+class FoodItem(CompoundExpression):
     
-    gene: Optional[str] = Field(None, description="""name of the gene that catalyzes the reaction""")
-    reaction: Optional[str] = Field(None, description="""equation describing the reaction (e.g. A+B = C+D) catalyzed by the gene""")
+    food: Optional[str] = Field(None, description="""the food item""")
+    state: Optional[str] = Field(None, description="""the state of the food item (e.g. chopped, diced)""")
     
     
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
@@ -190,26 +194,27 @@
     object_text: Optional[str] = Field(None)
     
     
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
-GeneToReaction.model_rebuild()
-ReactionDocument.model_rebuild()
+Recipe.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
-Reaction.model_rebuild()
-ReactionGrouping.model_rebuild()
-ChemicalEntity.model_rebuild()
-Evidence.model_rebuild()
-Gene.model_rebuild()
-Organism.model_rebuild()
+FoodType.model_rebuild()
+RecipeCategory.model_rebuild()
+Action.model_rebuild()
+UtensilType.model_rebuild()
+Unit.model_rebuild()
 CompoundExpression.model_rebuild()
-GeneReactionPairing.model_rebuild()
+Ingredient.model_rebuild()
+Quantity.model_rebuild()
+Step.model_rebuild()
+FoodItem.model_rebuild()
 Triple.model_rebuild()
 TextWithTriples.model_rebuild()
 TextWithEntity.model_rebuild()
 RelationshipType.model_rebuild()
 Publication.model_rebuild()
 AnnotatorResult.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/reaction.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/reaction
 name: reaction-template
 title: reaction Template
 description: >-
   A template for reactions
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   CHEBI: http://purl.obolibrary.org/obo/CHEBI_
   ECO: http://purl.obolibrary.org/obo/ECO_
   GO: http://purl.obolibrary.org/obo/GO_
   MS: http://purl.obolibrary.org/obo/MS_
   NCBITaxon: http://purl.obolibrary.org/obo/NCBITAXON_
   OBI: http://purl.obolibrary.org/obo/OBI_
   linkml: https://w3id.org/linkml/
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/recipe.py` & `ontogpt-0.3.9/src/ontogpt/templates/treatment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,202 +18,246 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
+
+
+class NCITDrugType(str):
+    
+    
+    dummy = "dummy"
+    
+
+class NCITTreatmentType(str):
+    
+    
+    dummy = "dummy"
+    
+
+class NCITTActivityType(str):
+    
+    
+    dummy = "dummy"
+    
 
+class MAXOActionType(str):
+    
+    
+    dummy = "dummy"
+    
+
+class MESHTherapeuticType(str):
+    
+    
+    dummy = "dummy"
+    
+
+class CHEBIDrugType(str):
+    
+    
+    dummy = "dummy"
+    
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
     NOT_APPLICABLE = "NOT_APPLICABLE"
     
     NOT_MENTIONED = "NOT_MENTIONED"
     
     
 
-class Recipe(ConfiguredBaseModel):
+class DiseaseTreatmentSummary(ConfiguredBaseModel):
+    
+    disease: Optional[str] = Field(None, description="""the name of the disease that is treated.""")
+    drugs: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of named small molecule drugs""")
+    treatments: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of therapies and treatments are indicated for treating the disease.""")
+    contraindications: Optional[List[str]] = Field(default_factory=list, description="""semicolon-separated list of therapies and treatments that are contra-indicated for the disease, and should not be used, due to risk of adverse effects.""")
+    treatment_mechanisms: Optional[List[TreatmentMechanism]] = Field(default_factory=list, description="""semicolon-separated list of treatment to asterisk-separated mechanism associations""")
+    treatment_efficacies: Optional[List[TreatmentEfficacy]] = Field(default_factory=list, description="""semicolon-separated list of treatment to efficacy associations, e.g. Imatinib*effective""")
+    treatment_adverse_effects: Optional[List[TreatmentAdverseEffect]] = Field(default_factory=list, description="""semicolon-separated list of treatment to adverse effect associations, e.g. Imatinib*nausea""")
     
-    url: str = Field(...)
-    label: Optional[str] = Field(None, description="""the name of the recipe""")
-    description: Optional[str] = Field(None, description="""a brief textual description of the recipe""")
-    categories: Optional[List[str]] = Field(default_factory=list, description="""a semicolon separated list of the categories to which this recipe belongs""")
-    ingredients: Optional[List[Ingredient]] = Field(default_factory=list, description="""a semicolon separated list of the ingredients plus quantities of the recipe""")
-    steps: Optional[List[Step]] = Field(default_factory=list, description="""a semicolon separated list of the individual steps involved in this recipe""")
     
-        
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
+
+class Gene(NamedEntity):
+    
+    id: str = Field(..., description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
+    
+    
 
-class FoodType(NamedEntity):
+class Symptom(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class RecipeCategory(NamedEntity):
+class Disease(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class Action(NamedEntity):
+class AdverseEffect(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class UtensilType(NamedEntity):
+class Treatment(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class Unit(NamedEntity):
+class Mechanism(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
-class CompoundExpression(ConfiguredBaseModel):
+class Drug(NamedEntity):
+    
+    id: str = Field(..., description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-    None
     
-        
 
-class Ingredient(CompoundExpression):
+class CompoundExpression(ConfiguredBaseModel):
+    
+    None
     
-    food_item: Optional[FoodItem] = Field(None, description="""the food item""")
-    amount: Optional[Quantity] = Field(None, description="""the quantity of the ingredient, e.g. 2 lbs""")
     
-        
 
-class Quantity(CompoundExpression):
+class TreatmentMechanism(CompoundExpression):
+    
+    treatment: Optional[str] = Field(None)
+    mechanism: Optional[str] = Field(None)
     
-    value: Optional[str] = Field(None, description="""the value of the quantity""")
-    unit: Optional[str] = Field(None, description="""the unit of the quantity, e.g. grams, cups, etc.""")
     
-        
 
-class Step(CompoundExpression):
+class TreatmentAdverseEffect(CompoundExpression):
+    
+    treatment: Optional[str] = Field(None)
+    adverse_effects: Optional[List[str]] = Field(default_factory=list)
     
-    action: Optional[str] = Field(None, description="""the action taken in this step (e.g. mix, add)""")
-    inputs: Optional[List[FoodItem]] = Field(default_factory=list, description="""a semicolon separated list of the inputs of this step""")
-    outputs: Optional[List[FoodItem]] = Field(default_factory=list, description="""a semicolon separated list of the outputs of this step""")
-    utensils: Optional[List[str]] = Field(default_factory=list, description="""the kitchen utensil used in this step (e.g. pan, bowl)""")
     
-        
 
-class FoodItem(CompoundExpression):
+class TreatmentEfficacy(CompoundExpression):
+    
+    treatment: Optional[str] = Field(None)
+    efficacy: Optional[str] = Field(None)
     
-    food: Optional[str] = Field(None, description="""the food item""")
-    state: Optional[str] = Field(None, description="""the state of the food item (e.g. chopped, diced)""")
     
-        
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
-Recipe.model_rebuild()
+DiseaseTreatmentSummary.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
-FoodType.model_rebuild()
-RecipeCategory.model_rebuild()
-Action.model_rebuild()
-UtensilType.model_rebuild()
-Unit.model_rebuild()
+Gene.model_rebuild()
+Symptom.model_rebuild()
+Disease.model_rebuild()
+AdverseEffect.model_rebuild()
+Treatment.model_rebuild()
+Mechanism.model_rebuild()
+Drug.model_rebuild()
 CompoundExpression.model_rebuild()
-Ingredient.model_rebuild()
-Quantity.model_rebuild()
-Step.model_rebuild()
-FoodItem.model_rebuild()
+TreatmentMechanism.model_rebuild()
+TreatmentAdverseEffect.model_rebuild()
+TreatmentEfficacy.model_rebuild()
 Triple.model_rebuild()
 TextWithTriples.model_rebuild()
 TextWithEntity.model_rebuild()
 RelationshipType.model_rebuild()
 Publication.model_rebuild()
 AnnotatorResult.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/recipe.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: https://w3id.org/ontogpt/recipe
 name: recipe-template
 title: Food Recipe Template
 description: >-
   A template for food recipes
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   recipe: http://w3id.org/ontogpt/recipe/
   FOODON: http://purl.obolibrary.org/obo/FOODON_
   UO: http://purl.obolibrary.org/obo/UO_
   dcterms: http://purl.org/dc/terms/
   HANCESTRO: http://purl.obolibrary.org/obo/HANCESTRO_
   BFO: http://purl.obolibrary.org/obo/BFO_
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/traits.py` & `ontogpt-0.3.9/src/ontogpt/templates/traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
+
 from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, ConfigDict,  Field, field_validator
 import re
 import sys
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -17,14 +18,15 @@
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
         validate_assignment=True,
         validate_default=True,
         extra = 'forbid',
         arbitrary_types_allowed=True,
         use_enum_values = True)
+    pass
 
 
 class NullDataOptions(str, Enum):
     
     
     UNSPECIFIED_METHOD_OF_ADMINISTRATION = "UNSPECIFIED_METHOD_OF_ADMINISTRATION"
     
@@ -42,105 +44,105 @@
     cellular_traits: Optional[List[str]] = Field(default_factory=list, description="""The cellular traits for the taxon.""")
     ecological_traits: Optional[List[str]] = Field(default_factory=list, description="""The ecological traits for the taxon.""")
     reproductive_traits: Optional[List[str]] = Field(default_factory=list, description="""The reproductive traits for the taxon.""")
     survival_traits: Optional[List[str]] = Field(default_factory=list, description="""The survival traits for the taxon.""")
     phenotypic_plasticiticy_traits: Optional[List[str]] = Field(default_factory=list, description="""The phenotypic plasticiticy traits for the taxon.""")
     preferred_environments: Optional[List[str]] = Field(default_factory=list, description="""The preferred environments for the taxon.""")
     
-        
+    
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
     named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
     
-        
+    
 
 class NamedEntity(ConfiguredBaseModel):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Trait(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class CompoundExpression(ConfiguredBaseModel):
     
     None
     
-        
+    
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
     subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
     object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
     
-        
+    
 
 class TextWithTriples(ConfiguredBaseModel):
     """
     A text containing one or more relations of the Triple type.
     """
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
     
-        
+    
 
 class TextWithEntity(ConfiguredBaseModel):
     """
     A text containing one or more instances of a single type of entity.
     """
     publication: Optional[Publication] = Field(None)
     entities: Optional[List[str]] = Field(default_factory=list)
     
-        
+    
 
 class RelationshipType(NamedEntity):
     
     id: str = Field(..., description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
     
-        
+    
 
 class Publication(ConfiguredBaseModel):
     
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
     
-        
+    
 
 class AnnotatorResult(ConfiguredBaseModel):
     
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
     
-        
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 Taxon.model_rebuild()
 ExtractionResult.model_rebuild()
 NamedEntity.model_rebuild()
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/traits.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/traits.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/traits
 name: traits
 title: Traits Template
 description: >-
   A template for Traits
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   linkml: https://w3id.org/linkml/
   traits: http://w3id.org/ontogpt/traits/
 
 default_prefix: traits
 default_range: string
 
 imports:
```

### Comparing `ontogpt-0.3.8/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.3.9/src/ontogpt/templates/treatment.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 id: http://w3id.org/ontogpt/treatment
 name: treatment-template
 title: MAXO treatment Template
 description: >-
   A template for MAXO treatments
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
   HGNC: http://identifiers.org/hgnc/
   HP: http://purl.obolibrary.org/obo/HP_
   MAXO: http://purl.obolibrary.org/obo/MAXO_
   linkml: https://w3id.org/linkml/
   treatment: http://w3id.org/ontogpt/treatments/
 keywords:
   - treatments
```

### Comparing `ontogpt-0.3.8/src/ontogpt/utils/model_utils.py` & `ontogpt-0.3.9/src/ontogpt/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/webapp/html/form.html` & `ontogpt-0.3.9/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.3.9/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/src/ontogpt/webapp/main.py` & `ontogpt-0.3.9/src/ontogpt/webapp/main.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.3.8/PKG-INFO` & `ontogpt-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.3.8
+Version: 0.3.9
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -16,51 +16,47 @@
 Provides-Extra: gpt4all
 Provides-Extra: huggingface
 Provides-Extra: recipes
 Provides-Extra: textract
 Provides-Extra: web
 Requires-Dist: Jinja2 (>=3.1.2) ; extra == "web"
 Requires-Dist: aiohttp (>=3.8.4)
-Requires-Dist: airium (>=0.2.5)
 Requires-Dist: beautifulsoup4 (>=4.11.1)
 Requires-Dist: bioc (>=2.0.post5)
 Requires-Dist: cachier (>=2.1.0)
-Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: click (>=8.1.3)
-Requires-Dist: eutils (>=0.6.0)
+Requires-Dist: dpath (>=2.1.6,<3.0.0)
 Requires-Dist: fastapi (>=0.88.0) ; extra == "web"
 Requires-Dist: gilda (>=1.0.0)
 Requires-Dist: gpt4 (>=0.0.1)
-Requires-Dist: httpx (>=0.23.3)
 Requires-Dist: huggingface_hub[huggingface] (>=0.15.1) ; extra == "huggingface"
 Requires-Dist: inflect (>=6.0.2)
 Requires-Dist: inflection (>=0.5.1)
-Requires-Dist: jsonlines (>=3.1.0)
 Requires-Dist: linkml (>=1.5.7,<2.0.0)
 Requires-Dist: linkml-owl (>=0.3.0,<0.4.0)
 Requires-Dist: llm (>=0.8)
 Requires-Dist: llm-gpt4all[gpt4all] (>=0.2) ; extra == "gpt4all"
 Requires-Dist: myst-parser[docs] (>=0.18.1) ; extra == "docs"
 Requires-Dist: nlpcloud (>=1.0.39)
-Requires-Dist: oaklib (>=0.5.15)
-Requires-Dist: openai (>=0.27.8,<1.0)
+Requires-Dist: oaklib (>=0.5.28)
+Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: pydantic (>=2.4.0)
-Requires-Dist: pystow (>=0.5.0,<0.6.0)
-Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: recipe-scrapers[recipes] (>=14.35.0) ; extra == "recipes"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: requests-cache (>=1.0.1)
+Requires-Dist: requests-cache (>=1.2.0)
 Requires-Dist: ruamel.yaml (>=0.17.31)
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4) ; extra == "docs"
 Requires-Dist: sphinx-click[docs] (>=4.3.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0) ; extra == "docs"
 Requires-Dist: sphinx[docs] (>=5.3.0) ; extra == "docs"
 Requires-Dist: streamlit (>=1.22.0)
 Requires-Dist: textract[textract] ; extra == "textract"
-Requires-Dist: tiktoken (>=0.3.3)
+Requires-Dist: tiktoken (>=0.5.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: urllib3 (<2)
 Requires-Dist: uvicorn (>=0.20.0) ; extra == "web"
 Requires-Dist: wikipedia (>=1.4.0)
 Requires-Dist: wikipedia-api (>=0.5.8)
 Description-Content-Type: text/markdown
 
 # OntoGPT
```

