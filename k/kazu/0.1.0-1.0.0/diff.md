# Comparing `tmp/kazu-0.1.0.tar.gz` & `tmp/kazu-1.0.0.tar.gz`

## Comparing `kazu-0.1.0.tar` & `kazu-1.0.0.tar`

### file list

```diff
@@ -1,156 +1,140 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/__init__.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/config.yaml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/AbbreviationFinderStep/default.yaml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/CleanupActions/default.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/CleanupStep/default.yaml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/DictionaryEntityLinkingStep/default.yaml
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/DisambiguationStrategies/default.yaml
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/DistillationTraining/default.yaml
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/DistillationTraining/intermediatelayer.yaml
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/DistillationTraining/production.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/EntityClassDisambiguationStep/default.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ExplosionStringMatchingStep/default.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/LSWebUtils/default.yaml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/LabelStudioManager/default.yaml
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/MappingStep/default.yaml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/MergeOverlappingEntsStep/default.yaml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/Middlewares/default.yaml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/Middlewares/jwt.yaml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/PLSapbertModel/default.yaml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/Pipeline/default.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SapBertForEntityLinkingStep/default.yaml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SapBertTraining/default.yaml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SapbertStringSimilarityScorer/default.yaml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SethStep/default.yaml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SpacyNerStep/default.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SpacyPipeline/default.yaml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/StanzaPipeline/default.yaml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/StanzaStep/default.yaml
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/StringScorers/default.yaml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/SynonymGeneration/default.yaml
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/TransformersModelForTokenClassificationNerStep/default.yaml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/TransformersModelForTokenClassificationNerStep/multilabel.yaml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/cache_sizes/default.yaml
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/confidence/default.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/curations/default.yaml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/global_actions/default.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/cellosaurus.yaml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/chembl.yaml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/cl.yaml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/clo.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/go_bp.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/go_cc.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/go_mf.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/hgnc_gene_family.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/mondo.yaml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/ot_disease.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/ot_molecule.yaml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/ot_target.yaml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/stato.yaml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/indices/uberon.yaml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/cellosaurus.yaml
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/chembl.yaml
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/cl.yaml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/clo.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/go_bp.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/go_cc.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/go_mf.yaml
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/hgnc_gene_family.yaml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/mondo.yaml
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/ot_disease.yaml
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/ot_molecule.yaml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/ot_target.yaml
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/stato.yaml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ontology_parser/uberon.yaml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ray/cluster.yaml
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ray/local.yaml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/conf/ray/local_with_frontend.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/data/__init__.py
--rw-r--r--   0        0        0    32839 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/data/data.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/data/pytorch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/hf_lightning_wrappers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/annotation/__init__.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/annotation/acceptance_test.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/annotation/label_studio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/database/__init__.py
--rw-r--r--   0        0        0    12169 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/database/in_memory_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/__init__.py
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/dataprocessor.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/lightning_plugins.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/metrics.py
--rw-r--r--   0        0        0    26653 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/models.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/tiny_transformers.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/distillation/train.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/language/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/language/language_phenomena.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/language/string_similarity_scorers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/linking/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/linking/sapbert/__init__.py
--rw-r--r--   0        0        0    21762 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/linking/sapbert/train.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_matching/LICENSE
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_matching/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_matching/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_matching/assemble_pipeline.py
--rw-r--r--   0        0        0    21815 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_matching/ontology_matcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_preprocessing/__init__.py
--rw-r--r--   0        0        0    81174 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_preprocessing/base.py
--rw-r--r--   0        0        0    13202 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/modelling/ontology_preprocessing/synonym_generation.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/pipeline/__init__.py
--rw-r--r--   0        0        0     9292 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/pipeline/pipeline.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/__init__.py
--rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/document_post_processing/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/document_post_processing/abbreviation_finder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/joint_ner_and_linking/__init__.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/joint_ner_and_linking/explosion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/__init__.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/dictionary.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/entity_class_disambiguation.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/mapping_step.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/sapbert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/__init__.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/strategy_runner.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/xref_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/disambiguation/__init__.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/disambiguation/context_scoring.py
--rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/disambiguation/strategies.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/mapping_strategies/__init__.py
--rw-r--r--   0        0        0    19747 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/linking/post_processing/mapping_strategies/strategies.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/ner/__init__.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/ner/entity_post_processing.py
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/ner/hf_token_classification.py
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/ner/seth.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/ner/spacy_ner.py
--rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/ner/tokenized_word_processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/other/__init__.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/other/cleanup.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/other/merge_overlapping_ents.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/steps/other/stanza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/__init__.py
--rw-r--r--   0        0        0    18075 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/abbreviation_detector.py
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/build_and_test_model_packs.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/caching.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/constants.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/grouping.py
--rw-r--r--   0        0        0    18791 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/link_index.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/model_pack_build_logging.conf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/spacy_pipeline.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/stanza_pipeline.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/stopwatch.py
--rw-r--r--   0        0        0    21065 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/string_normalizer.py
--rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/web/__init__.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/web/jwtauth.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/web/ls_web_utils.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/web/req_id_header.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/web/routes.py
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 kazu-0.1.0/kazu/web/server.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 kazu-0.1.0/.gitignore
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 kazu-0.1.0/AUTHORS.md
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kazu-0.1.0/LICENSE
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 kazu-0.1.0/README.md
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 kazu-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11236 2020-02-02 00:00:00.000000 kazu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/annotation/__init__.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/annotation/acceptance_test.py
+-rw-r--r--   0        0        0    20783 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/annotation/label_studio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/__init__.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/config.yaml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/AbbreviationFinderStep/default.yaml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/CleanupActions/default.yaml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/CleanupActions/uri_stripping.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/CleanupStep/default.yaml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/DictionaryEntityLinkingStep/default.yaml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/DisambiguationStrategies/default.yaml
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/DistillationTraining/default.yaml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/DistillationTraining/intermediatelayer.yaml
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/DistillationTraining/production.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/EntityClassDisambiguationStep/default.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ExplosionStringMatchingStep/default.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/LSWebUtils/default.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/LabelStudioManager/default.yaml
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/MappingStep/default.yaml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/MergeOverlappingEntsStep/default.yaml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/Middlewares/default.yaml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/Middlewares/jwt.yaml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/PLSapbertModel/default.yaml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/Pipeline/default.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/SapBertTraining/default.yaml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/SapbertStringSimilarityScorer/default.yaml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/SethStep/default.yaml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/SpacyNerStep/default.yaml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/SpacyPipeline/default.yaml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/StanzaPipeline/default.yaml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/StanzaStep/default.yaml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/StringScorers/default.yaml
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/SynonymGeneration/default.yaml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/TransformersModelForTokenClassificationNerStep/default.yaml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/TransformersModelForTokenClassificationNerStep/multilabel.yaml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/cache_sizes/default.yaml
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/confidence/default.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/global_actions/default.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/cellosaurus.yaml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/chembl.yaml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/cl.yaml
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/clo.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/go_bp.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/go_cc.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/go_mf.yaml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/hgnc_gene_family.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/mondo.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/ot_disease.yaml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/ot_molecule.yaml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/ot_target.yaml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/stato.yaml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ontologies/uberon.yaml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ray/cluster.yaml
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ray/local.yaml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/conf/ray/local_with_frontend.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/data/__init__.py
+-rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/data/data.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/data/pytorch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/database/__init__.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/database/in_memory_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/__init__.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/dataprocessor.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/lightning_plugins.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/metrics.py
+-rw-r--r--   0        0        0    26611 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/models.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/tiny_transformers.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/distillation/train.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/language/__init__.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/language/language_phenomena.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/language/string_similarity_scorers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/linking/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/linking/sapbert/__init__.py
+-rw-r--r--   0        0        0    22145 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/linking/sapbert/train.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_matching/LICENSE
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_matching/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_matching/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_matching/assemble_pipeline.py
+-rw-r--r--   0        0        0    21312 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_matching/ontology_matcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_preprocessing/__init__.py
+-rw-r--r--   0        0        0    53599 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_preprocessing/base.py
+-rw-r--r--   0        0        0    49400 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_preprocessing/parsers.py
+-rw-r--r--   0        0        0    13579 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/ontology_preprocessing/synonym_generation.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/pipeline/__init__.py
+-rw-r--r--   0        0        0    13510 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/pipeline/pipeline.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/__init__.py
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/document_post_processing/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/document_post_processing/abbreviation_finder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/joint_ner_and_linking/__init__.py
+-rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/joint_ner_and_linking/explosion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/__init__.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/dictionary.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/entity_class_disambiguation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/__init__.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/mapping_step.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/strategy_runner.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/xref_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/disambiguation/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/disambiguation/context_scoring.py
+-rw-r--r--   0        0        0     9789 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/disambiguation/strategies.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/mapping_strategies/__init__.py
+-rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/linking/post_processing/mapping_strategies/strategies.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/__init__.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/entity_post_processing.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/hf_lightning_wrappers.py
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/hf_token_classification.py
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/seth.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/spacy_ner.py
+-rw-r--r--   0        0        0    16815 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/ner/tokenized_word_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/other/__init__.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/other/cleanup.py
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/other/merge_overlapping_ents.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/steps/other/stanza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/__init__.py
+-rw-r--r--   0        0        0    18395 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/abbreviation_detector.py
+-rw-r--r--   0        0        0    16823 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/build_and_test_model_packs.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/caching.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/constants.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/grouping.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/link_index.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/model_pack_build_logging.conf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/spacy_pipeline.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/stanza_pipeline.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/stopwatch.py
+-rw-r--r--   0        0        0    20979 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/string_normalizer.py
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/web/__init__.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/web/jwtauth.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/web/ls_web_utils.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/web/req_id_header.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/web/routes.py
+-rw-r--r--   0        0        0    21744 2020-02-02 00:00:00.000000 kazu-1.0.0/kazu/web/server.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 kazu-1.0.0/.gitignore
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 kazu-1.0.0/AUTHORS.md
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kazu-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 kazu-1.0.0/README.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 kazu-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 kazu-1.0.0/PKG-INFO
```

### Comparing `kazu-0.1.0/kazu/conf/config.yaml` & `kazu-1.0.0/kazu/conf/config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 defaults:
   - ray: local
-  - ontology_parser:
-      - cellosaurus
-      - chembl
-      - cl
-      - clo
-      - go_bp
-      - go_mf
-      - go_cc
-      - hgnc_gene_family
-      - mondo
+  - ontologies:
+      - ot_target
       - ot_disease
       - ot_molecule
-      - ot_target
-      - stato
-      - uberon
-  - indices:
       - cellosaurus
       - chembl
       - cl
       - clo
       - go_bp
       - go_mf
       - go_cc
       - hgnc_gene_family
       - mondo
-      - ot_disease
-      - ot_molecule
-      - ot_target
       - stato
       - uberon
   - PLSapbertModel: default
   - SpacyPipeline: default
   - StanzaPipeline: default
   - AbbreviationFinderStep: default
   - SpacyNerStep: default
   - TransformersModelForTokenClassificationNerStep: default
-  - SapBertForEntityLinkingStep: default
   - DictionaryEntityLinkingStep: default
   - SapBertTraining: default
   - Pipeline: default
   - DistillationTraining: default
   - SethStep: default
   - SynonymGeneration: default
   - ExplosionStringMatchingStep: default
@@ -54,15 +38,14 @@
   - CleanupActions: default
   - LabelStudioManager: default
   - LSWebUtils: default
   - Middlewares: default
   - EntityClassDisambiguationStep: default
   - confidence: default
   - cache_sizes: default
-  - curations: default
   - global_actions: default
   - _self_  # see https://hydra.cc/docs/1.2/upgrades/1.0_to_1.1/default_composition_order/
 
 # we set certain env vars here for things that are statically initialised
 hydra:
   job:
     env_set:
```

### Comparing `kazu-0.1.0/kazu/conf/CleanupActions/default.yaml` & `kazu-1.0.0/kazu/conf/CleanupActions/default.yaml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-EntityFilterCleanupAction:
-  _target_: kazu.steps.other.cleanup.EntityFilterCleanupAction
-  filter_fns:
-    - _target_: kazu.steps.other.cleanup.DropUnmappedEntityFilter
-      from_ent_namespaces:
-        - _target_: kazu.steps.joint_ner_and_linking.explosion.ExplosionStringMatchingStep.namespace
 MappingFilterCleanupAction:
   _target_: kazu.steps.other.cleanup.MappingFilterCleanupAction
   filter_fns:
     - _target_: kazu.steps.other.cleanup.DropMappingsByConfidenceMappingFilter
       disambiguation_ranks_to_drop:
         - _target_: kazu.data.data.DisambiguationConfidence
           _args_:
             - AMBIGUOUS
       string_match_ranks_to_drop:
         _target_: builtins.list
+EntityFilterCleanupAction:
+  _target_: kazu.steps.other.cleanup.EntityFilterCleanupAction
+  filter_fns:
+    - _target_: kazu.steps.other.cleanup.DropUnmappedEntityFilter
+      from_ent_namespaces:
+        - _target_: kazu.steps.joint_ner_and_linking.explosion.ExplosionStringMatchingStep.namespace
```

### Comparing `kazu-0.1.0/kazu/conf/DisambiguationStrategies/default.yaml` & `kazu-1.0.0/kazu/conf/DisambiguationStrategies/default.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -11,45 +11,33 @@
         _args_:
           - RESOLVED_BY_SIMILARITY
       - _target_: kazu.data.data.EquivalentIdAggregationStrategy
         _args_:
           - MERGED_AS_NON_SYMBOLIC
     scorer:
       _target_: kazu.steps.linking.post_processing.disambiguation.context_scoring.TfIdfScorer
-      path:
-        _target_: pathlib.Path
-        _args_:
-          - ${oc.env:KAZU_MODEL_PACK}/mapping_step/tfidf
 
 gene:
   - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.DefinedElsewhereInDocumentDisambiguationStrategy
     confidence: ${confidence.disambiguation_highly_likely}
   - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.TfIdfDisambiguationStrategy
     confidence: ${confidence.disambiguation_probable}
     relevant_aggregation_strategies:
       - _target_: kazu.data.data.EquivalentIdAggregationStrategy
         _args_:
           - CUSTOM
     scorer:
       _target_: kazu.steps.linking.post_processing.disambiguation.context_scoring.TfIdfScorer
-      path:
-        _target_: pathlib.Path
-        _args_:
-          - ${oc.env:KAZU_MODEL_PACK}/mapping_step/tfidf
   - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.AnnotationLevelDisambiguationStrategy
     confidence: ${confidence.disambiguation_possible}
 
 cell_line:
   - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.DefinedElsewhereInDocumentDisambiguationStrategy
     confidence: ${confidence.disambiguation_highly_likely}
   - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.TfIdfDisambiguationStrategy
     confidence: ${confidence.disambiguation_probable}
     relevant_aggregation_strategies:
       - _target_: kazu.data.data.EquivalentIdAggregationStrategy
         _args_:
           - CUSTOM
     scorer:
       _target_: kazu.steps.linking.post_processing.disambiguation.context_scoring.TfIdfScorer
-      path:
-        _target_: pathlib.Path
-        _args_:
-          - ${oc.env:KAZU_MODEL_PACK}/mapping_step/tfidf
```

### Comparing `kazu-0.1.0/kazu/conf/DistillationTraining/default.yaml` & `kazu-1.0.0/kazu/conf/DistillationTraining/default.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 monitoring:
   monitor: entity_f1
   mode: max
 training_params:
   max_epochs: 10
 save_dir: "." # save dir managed by hydra. Override here if required
 model:
-  _target_: kazu.modelling.distillation.models.SequenceTaggingDistillationForFinalLayer
+  _target_: kazu.distillation.models.SequenceTaggingDistillationForFinalLayer
   data_dir: ???
   label_list:
     - B-disease
     - B-drug
     - B-gene
     - B-mutation
     - B-species
@@ -45,15 +45,15 @@
   accumulate_grad_batches: 1
   max_epochs: ${DistillationTraining.training_params.max_epochs}
   logger:
     - _target_: pytorch_lightning.loggers.CSVLogger
       save_dir: ${DistillationTraining.save_dir}
       name: csv_log
   plugins:
-    - _target_: kazu.modelling.distillation.lightning_plugins.StudentModelCheckpointIO
+    - _target_: kazu.distillation.lightning_plugins.StudentModelCheckpointIO
       model_name_or_path: ${DistillationTraining.model.student_model_path}
   callbacks:
     - _target_: pytorch_lightning.callbacks.ModelCheckpoint
       dirpath: ${DistillationTraining.save_dir}
       filename: "student_model-{epoch:02d}-{entity_f1:.4f}-{validation_loss:.3f}-{step:05d}"
       monitor: ${DistillationTraining.monitoring.monitor}
       mode: ${DistillationTraining.monitoring.mode}
```

### Comparing `kazu-0.1.0/kazu/conf/DistillationTraining/intermediatelayer.yaml` & `kazu-1.0.0/kazu/conf/DistillationTraining/intermediatelayer.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 monitoring:
   monitor: mserror
   mode: min
 training_params:
   max_epochs: 5
 save_dir: "." # save dir managed by hydra. Override here if required
 model:
-  _target_: kazu.modelling.distillation.models.SequenceTaggingDistillationForIntermediateLayer
+  _target_: kazu.distillation.models.SequenceTaggingDistillationForIntermediateLayer
   data_dir: ???
   label_list:
     - B-disease
     - B-drug
     - B-gene
     - B-mutation
     - B-species
@@ -46,15 +46,15 @@
   max_epochs: ${DistillationTraining.training_params.max_epochs}
   strategy: "ddp"
   logger:
     - _target_: pytorch_lightning.loggers.CSVLogger
       save_dir: ${DistillationTraining.save_dir}
       name: csv_log
   plugins:
-    - _target_: kazu.modelling.distillation.lightning_plugins.StudentModelCheckpointIO
+    - _target_: kazu.distillation.lightning_plugins.StudentModelCheckpointIO
       model_name_or_path: ${DistillationTraining.model.student_model_path}
   callbacks:
     - _target_: pytorch_lightning.callbacks.ModelCheckpoint
       dirpath: ${DistillationTraining.save_dir}
       filename: "student_model_inm_layer-{epoch:02d}-{mserror:.4f}-{step:05d}"
       monitor: ${DistillationTraining.monitoring.monitor}
       mode: ${DistillationTraining.monitoring.mode}
```

### Comparing `kazu-0.1.0/kazu/conf/DistillationTraining/production.yaml` & `kazu-1.0.0/kazu/conf/DistillationTraining/production.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 monitoring:
   monitor: entity_f1
   mode: max
 training_params:
   max_epochs: 5
 save_dir: "." # save dir managed by hydra. Override here if required
 model:
-  _target_: kazu.modelling.distillation.models.SequenceTaggingDistillationForFinalLayer
+  _target_: kazu.distillation.models.SequenceTaggingDistillationForFinalLayer
   data_dir: ???
   label_list:
     - B-disease
     - B-drug
     - B-gene
     - B-mutation
     - B-species
@@ -46,15 +46,15 @@
   max_epochs: ${DistillationTraining.training_params.max_epochs}
   strategy: "ddp"
   logger:
     - _target_: pytorch_lightning.loggers.CSVLogger
       save_dir: ${DistillationTraining.save_dir}
       name: csv_log
   plugins:
-    - _target_: kazu.modelling.distillation.lightning_plugins.StudentModelCheckpointIO
+    - _target_: kazu.distillation.lightning_plugins.StudentModelCheckpointIO
       model_name_or_path: ${DistillationTraining.model.student_model_path}
   callbacks:
     - _target_: pytorch_lightning.callbacks.ModelCheckpoint
       dirpath: ${DistillationTraining.save_dir}
       filename: "student_model-{epoch:02d}-{entity_f1:.4f}-{validation_loss:.3f}-{step:05d}"
       monitor: ${DistillationTraining.monitoring.monitor}
       mode: ${DistillationTraining.monitoring.mode}
```

### Comparing `kazu-0.1.0/kazu/conf/MappingStep/default.yaml` & `kazu-1.0.0/kazu/conf/MappingStep/default.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-_target_: kazu.steps.linking.mapping_step.MappingStep
+_target_: kazu.steps.linking.post_processing.mapping_step.MappingStep
+parsers: ${oc.dict.values:ontologies.parsers}
 strategy_runner:
   _target_: kazu.steps.linking.post_processing.strategy_runner.StrategyRunner
   cross_ref_managers: ~
-  ner_namespace_processing_order:
-    - _target_: kazu.steps.ner.hf_token_classification.TransformersModelForTokenClassificationNerStep.namespace
-    - _target_: kazu.steps.joint_ner_and_linking.explosion.ExplosionStringMatchingStep.namespace
   symbolic_strategies:
 
-    TransformersModelForTokenClassificationNerStep:
-      _target_: kazu.steps.linking.post_processing.strategy_runner.NamespaceStrategyExecution
+    HIGHLY_LIKELY:
+      _target_: kazu.steps.linking.post_processing.strategy_runner.ConfidenceLevelStrategyExecution
       stop_on_success: True
       default_strategies:
         - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
           confidence: ${confidence.string_matching_highly_likely}
           disambiguation_strategies: ${DisambiguationStrategies.default}
 
         - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.SymbolMatchMappingStrategy
@@ -76,32 +74,42 @@
             confidence: ${confidence.string_matching_probable}
             disambiguation_strategies: ${DisambiguationStrategies.cell_line}
 
           - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.TermNormIsSubStringMappingStrategy
             confidence: ${confidence.string_matching_probable}
             disambiguation_strategies: ${DisambiguationStrategies.cell_line}
 
-    ExplosionStringMatchingStep:
-      _target_: kazu.steps.linking.post_processing.strategy_runner.NamespaceStrategyExecution
+    PROBABLE:
+      _target_: kazu.steps.linking.post_processing.strategy_runner.ConfidenceLevelStrategyExecution
       stop_on_success: True
       default_strategies:
-        - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.NoopMappingStrategy
-          # This is for ExplosionStringMatchingStep entities using exact string matching
+        - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
+          disambiguation_strategies: ${DisambiguationStrategies.default}
+          confidence: ${confidence.string_matching_highly_likely}
+      ent_class_strategies:
+        _target_: builtins.dict
+
+    POSSIBLE:
+      _target_: kazu.steps.linking.post_processing.strategy_runner.ConfidenceLevelStrategyExecution
+      stop_on_success: True
+      default_strategies:
+        - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
           confidence: ${confidence.string_matching_highly_likely}
+          disambiguation_essential: true
           disambiguation_strategies:
             - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.DefinedElsewhereInDocumentDisambiguationStrategy
               confidence: ${confidence.disambiguation_highly_likely}
       ent_class_strategies:
         _target_: builtins.dict
 
 
   non_symbolic_strategies:
 
-    TransformersModelForTokenClassificationNerStep:
-      _target_: kazu.steps.linking.post_processing.strategy_runner.NamespaceStrategyExecution
+    HIGHLY_LIKELY:
+      _target_: kazu.steps.linking.post_processing.strategy_runner.ConfidenceLevelStrategyExecution
       stop_on_success: True
       default_strategies:
         - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
           confidence: ${confidence.string_matching_highly_likely}
           disambiguation_strategies: ${DisambiguationStrategies.default}
 
         - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.StrongMatchMappingStrategy
@@ -144,40 +152,29 @@
           - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.SymbolMatchMappingStrategy
             confidence: ${confidence.string_matching_probable}
             disambiguation_strategies: ${DisambiguationStrategies.cell_line}
 
           - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.TermNormIsSubStringMappingStrategy
             confidence: ${confidence.string_matching_probable}
             disambiguation_strategies: ${DisambiguationStrategies.cell_line}
-    ExplosionStringMatchingStep:
-      _target_: kazu.steps.linking.post_processing.strategy_runner.NamespaceStrategyExecution
+    PROBABLE:
+      _target_: kazu.steps.linking.post_processing.strategy_runner.ConfidenceLevelStrategyExecution
       stop_on_success: True
       default_strategies:
         - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
           disambiguation_strategies: ${DisambiguationStrategies.default}
           confidence: ${confidence.string_matching_highly_likely}
       ent_class_strategies:
-        # we don't expect any value from the disambiguation strategies for these ontologies, so save the effort
-        anatomy:
-          - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
-            disambiguation_strategies: ~
-            confidence: ${confidence.string_matching_highly_likely}
-        go_bp:
-          - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
-            disambiguation_strategies: ~
-            confidence: ${confidence.string_matching_highly_likely}
-        go_cc:
-          - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
-            disambiguation_strategies: ~
-            confidence: ${confidence.string_matching_highly_likely}
-        go_mf:
-          - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
-            disambiguation_strategies: ~
-            confidence: ${confidence.string_matching_highly_likely}
-        cell_line:
-          - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
-            disambiguation_strategies: ~
-            confidence: ${confidence.string_matching_highly_likely}
-        cell_type:
-          - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
-            disambiguation_strategies: ~
-            confidence: ${confidence.string_matching_highly_likely}
+        _target_: builtins.dict
+
+    POSSIBLE:
+      _target_: kazu.steps.linking.post_processing.strategy_runner.ConfidenceLevelStrategyExecution
+      stop_on_success: True
+      default_strategies:
+        - _target_: kazu.steps.linking.post_processing.mapping_strategies.strategies.ExactMatchMappingStrategy
+          confidence: ${confidence.string_matching_highly_likely}
+          disambiguation_essential: true
+          disambiguation_strategies:
+            - _target_: kazu.steps.linking.post_processing.disambiguation.strategies.DefinedElsewhereInDocumentDisambiguationStrategy
+              confidence: ${confidence.disambiguation_highly_likely}
+      ent_class_strategies:
+        _target_: builtins.dict
```

### Comparing `kazu-0.1.0/kazu/conf/Middlewares/jwt.yaml` & `kazu-1.0.0/kazu/conf/Middlewares/jwt.yaml`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/conf/SapBertTraining/default.yaml` & `kazu-1.0.0/kazu/conf/SapBertTraining/default.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 model:
-  _target_: kazu.modelling.linking.sapbert.train.PLSapbertModel
+  _target_: kazu.linking.sapbert.train.PLSapbertModel
   model_name_or_path: ${oc.env:KAZU_MODEL_PACK}/sapbert/SapBERT-from-PubMedBERT-fulltext
   sapbert_training_params:
-    _target_: kazu.modelling.linking.sapbert.train.SapbertTrainingParams
+    _target_: kazu.linking.sapbert.train.SapbertTrainingParams
     topk: 5
     lr: 2e-5
     weight_decay: 0.01
     miner_margin: 0.2
     type_of_triplets: "all"
     train_file: ???
     train_batch_size: 256
     num_workers: 0
   sapbert_evaluation_manager:
-    _target_: kazu.modelling.linking.sapbert.train.SapbertEvaluationDataManager
+    _target_: kazu.linking.sapbert.train.SapbertEvaluationDataManager
     debug: true
     sources:
       bc5cdr-disease:
         - ???
         - ???
       mondo:
         - ???
```

### Comparing `kazu-0.1.0/kazu/conf/StringScorers/default.yaml` & `kazu-1.0.0/kazu/conf/StringScorers/default.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 gene:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
-  - _target_: kazu.modelling.language.string_similarity_scorers.EntityNounModifierStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.EntityNounModifierStringSimilarityScorer
     noun_modifier_phrases:
       - LIKE
       - SUBUNIT
       - PSEUDOGENE
       - RECEPTOR
-  - _target_: kazu.modelling.language.string_similarity_scorers.EntitySubtypeStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.EntitySubtypeStringSimilarityScorer
 drug:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
 disease:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
-  - _target_: kazu.modelling.language.string_similarity_scorers.EntitySubtypeStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.EntitySubtypeStringSimilarityScorer
 anatomy:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
 cell_line:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
 cell_type:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
 go:
-  - _target_: kazu.modelling.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
+  - _target_: kazu.language.string_similarity_scorers.NumberMatchStringSimilarityScorer
```

### Comparing `kazu-0.1.0/kazu/conf/SynonymGeneration/default.yaml` & `kazu-1.0.0/kazu/conf/SynonymGeneration/default.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 default:
-  _target_: kazu.modelling.ontology_preprocessing.synonym_generation.CombinatorialSynonymGenerator
+  _target_: kazu.ontology_preprocessing.synonym_generation.CombinatorialSynonymGenerator
   synonym_generators:
-    - _target_: kazu.modelling.ontology_preprocessing.synonym_generation.StopWordRemover
-    - _target_: kazu.modelling.ontology_preprocessing.synonym_generation.StringReplacement
+    - _target_: kazu.ontology_preprocessing.synonym_generation.StopWordRemover
+    - _target_: kazu.ontology_preprocessing.synonym_generation.NgramHyphenation
+    - _target_: kazu.ontology_preprocessing.synonym_generation.StringReplacement
       replacement_dict:
         "-":
           - " "
           - "_"
         "_":
           - " "
           - "-"
       digit_aware_replacement_dict:
         " ":
           - "-"
       include_greek: true
 gene:
-  _target_: kazu.modelling.ontology_preprocessing.synonym_generation.CombinatorialSynonymGenerator
+  _target_: kazu.ontology_preprocessing.synonym_generation.CombinatorialSynonymGenerator
   synonym_generators:
-    - _target_: kazu.modelling.ontology_preprocessing.synonym_generation.StringReplacement
+    - _target_: kazu.ontology_preprocessing.synonym_generation.NgramHyphenation
+    - _target_: kazu.ontology_preprocessing.synonym_generation.StringReplacement
       replacement_dict:
         "-":
           - " "
           - "_"
         "_":
           - " "
           - "-"
       digit_aware_replacement_dict:
         " ":
           - "-"
       include_greek: true
 chemical:
-  _target_: kazu.modelling.ontology_preprocessing.synonym_generation.CombinatorialSynonymGenerator
+  _target_: kazu.ontology_preprocessing.synonym_generation.CombinatorialSynonymGenerator
   synonym_generators:
-    - _target_: kazu.modelling.ontology_preprocessing.synonym_generation.StringReplacement
+    - _target_: kazu.ontology_preprocessing.synonym_generation.StringReplacement
       include_greek: true
```

### Comparing `kazu-0.1.0/kazu/conf/TransformersModelForTokenClassificationNerStep/default.yaml` & `kazu-1.0.0/kazu/conf/TransformersModelForTokenClassificationNerStep/default.yaml`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/conf/cache_sizes/default.yaml` & `kazu-1.0.0/kazu/conf/cache_sizes/default.yaml`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/conf/confidence/default.yaml` & `kazu-1.0.0/kazu/conf/confidence/default.yaml`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/data/data.py` & `kazu-1.0.0/kazu/data/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import dataclasses
 import json
 import uuid
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass, field
 from datetime import datetime, date
-from enum import Enum, auto
+from enum import Enum, auto, IntEnum
 from math import inf
 from typing import List, Any, Dict, Optional, Tuple, FrozenSet, Set, Iterable, Union, DefaultDict
 
+import bson
+from bson import json_util
 from numpy import ndarray, float32, float16
 
 from kazu.utils.string_normalizer import StringNormalizer
 
 IS_SUBSPAN = "is_subspan"
 # BIO schema
 ENTITY_START_SYMBOL = "B"
@@ -55,17 +57,18 @@
         </details>
     """
 
     def _generate_next_value_(name, start, count, last_values):
         return name
 
 
-class MentionConfidence(AutoNameEnum):
-    HIGHLY_LIKELY = auto()  # almost certain to be correct
-    POSSIBLE = auto()  # high degree of uncertainty
+class MentionConfidence(IntEnum):
+    HIGHLY_LIKELY = 100  # almost certain to be correct
+    PROBABLE = 50
+    POSSIBLE = 10  # high degree of uncertainty
 
 
 class StringMatchConfidence(AutoNameEnum):
     HIGHLY_LIKELY = auto()  # almost certain to be correct
     PROBABLE = auto()  # on the balance of probabilities, will be correct
     POSSIBLE = auto()  # high degree of uncertainty
 
@@ -155,14 +158,15 @@
     xref_source_parser_name: Optional[str] = None  # source parser name if mapping is an XREF
     metadata: Dict[Any, Any] = field(default_factory=dict, hash=False)  # generic metadata
 
 
 NumericMetric = Union[bool, int, float]
 
 AssociatedIdSets = FrozenSet[EquivalentIdSet]
+"""A frozen set of :class:`.EquivalentIdSet`"""
 
 
 @dataclass(frozen=True, eq=True)
 class SynonymTerm:
     """
     a SynonymTerm is a container for a single normalised synonym, and is produced by an OntologyParser implementation.
     It may be composed of multiple terms that normalise
@@ -175,14 +179,17 @@
     parser_name: str  # ontology parser name
     is_symbolic: bool  # is the term symbolic? Determined by the OntologyParser
     associated_id_sets: AssociatedIdSets
     mapping_types: FrozenSet[str] = field(hash=False)  # mapping type metadata
     aggregated_by: EquivalentIdAggregationStrategy = field(
         hash=False, compare=False
     )  # determined by the ontology parser
+    original_term: Optional[
+        str
+    ] = None  # if generated by a synonym generator, the original source synonym
 
     @property
     def is_ambiguous(self):
         return len(self.associated_id_sets) > 1
 
 
 @dataclass(frozen=True, eq=True)
@@ -560,31 +567,33 @@
 
     @classmethod
     def doc_to_json_dict(cls, doc: Document) -> Dict[str, JsonDictType]:
         return {k: DocumentJsonUtils.obj_to_dict_repr(v) for k, v in doc.__dict__.items()}
 
     @classmethod
     def obj_to_dict_repr(cls, obj: Any) -> JsonDictType:
-        if isinstance(obj, cls.atomic_types):
+        if isinstance(obj, Enum):
+            return obj.name
+        elif isinstance(obj, cls.atomic_types):
             return obj
         elif isinstance(obj, (float16, float32)):  # type: ignore[misc]
             return obj.item()
         elif isinstance(obj, cls.listlike_types):
             return [cls.obj_to_dict_repr(elem) for elem in obj]
         elif isinstance(obj, ndarray):
             return obj.tolist()
         elif dataclasses.is_dataclass(obj):
             return cls.obj_to_dict_repr(obj.__dict__)
         elif isinstance(obj, dict):
             processed_dict_pairs = (cls._preprocess_dict_pair(pair) for pair in obj.items())
             return {k: cls.obj_to_dict_repr(v) for k, v in processed_dict_pairs}
-        elif isinstance(obj, Enum):
-            return obj.name
         elif isinstance(obj, (datetime, date)):
             return obj.isoformat()
+        elif isinstance(obj, bson.ObjectId):
+            return json_util.default(obj)
         else:
             raise cls.ConversionException(f"Unknown object type: {type(obj)}")
 
     @classmethod
     def _preprocess_dict_pair(cls, kv_pair: Tuple[Any, Any]) -> Tuple[str, JsonDictType]:
         k, v = kv_pair
         if k == "offset_map":
@@ -619,91 +628,43 @@
     def empty(x) -> bool:
         return x is None or x == {} or x == []
 
 
 SimpleValue = Union[NumericMetric, str]
 
 
-class SynonymTermBehaviour(AutoNameEnum):
+class CuratedTermBehaviour(AutoNameEnum):
     #: do nothing. Useful if you want to catalogue a term as "I've looked at this but don't want to use it for NER"
     IGNORE = auto()
     #: use the term for both dictionary based NER and as a linking target.
     ADD_FOR_NER_AND_LINKING = auto()
     #: use the term only as a linking target. Note, this is not required if the term is already in the
     #: underlying ontology, as all ontology terms are included as linking targets by default
     #: (Also see DROP_SYNONYM_TERM_FOR_LINKING)
     ADD_FOR_LINKING_ONLY = auto()
     #: do not use this term as a linking target. Normally, you would use this for a term you want to remove
     #: from the underlying ontology (e.g. a 'bad' synonym). If the term does not exist, has no effect
     DROP_SYNONYM_TERM_FOR_LINKING = auto()
-    #: removes an EquivalentIdSet from the term. The EquivalentIdSet to remove is selected via being a
-    #: superset of the IDs in the associated parser_to_target_id_mappings value
-    DROP_ID_SET_FROM_SYNONYM_TERM = auto()
+    #: used if the containing Curation has source_term !=None, in which case all behaviours are inherited
+    INHERIT_FROM_SOURCE_TERM = auto()
 
 
 class ParserBehaviour(AutoNameEnum):
     #: completely remove the ids from the parser - i.e. should never used anywhere
     DROP_IDS_FROM_PARSER = auto()
 
 
-@dataclass()
-class SynonymTermAction:
-    """
-    A SynonymTermAction is an action that affects the :class:`.SynonymTerm`\\s that a parser
-    produces.
-
-    Note, the term_norm field is calculated by the :class:`kazu.modelling.ontology_preprocessing.base.OntologyParser`
-    if required, and should not be set manually.
-
-    The parser_to_target_id_mappings field should specify the parser name and a set of affected ID's if required.
-
-    See :class:`.SynonymTermBehaviour` for the type of actions that are possible.
-
-    """
-
-    behaviour: SynonymTermBehaviour
-    entity_class: str
-    parser_to_target_id_mappings: Dict[str, Set[str]] = field(default_factory=dict)
-    term_norm: str = field(init=False)
-
-    def __post_init__(self):
-        if (
-            # map not needed for ignore
-            self.behaviour is not SynonymTermBehaviour.IGNORE
-            and len(self.parser_to_target_id_mappings) == 0
-        ):
-            raise ValueError(
-                f"parser_to_target_id_mappings must be specified for behaviour {self.behaviour}"
-            )
-        if self.behaviour is not SynonymTermBehaviour.DROP_SYNONYM_TERM_FOR_LINKING:
-            # we only need to know the parser name for DROP_SYNONYM_TERM_FOR_LINKING.
-            # all others need ids
-            for key, values in self.parser_to_target_id_mappings.items():
-                if len(values) == 0:
-                    raise ValueError(f"at least one ID must be specified for key: {key}")
-
-    @classmethod
-    def from_json(cls, json_dict: Dict) -> "SynonymTermAction":
-        return cls(
-            behaviour=SynonymTermBehaviour(json_dict["behaviour"]),
-            entity_class=json_dict["entity_class"],
-            parser_to_target_id_mappings={
-                k: set(v) for k, v in json_dict["parser_to_target_id_mappings"].items()
-            },
-        )
-
-
 @dataclass(frozen=True)
 class ParserAction:
     """
-    A ParserAction changes the behaviour of a :class:`kazu.modelling.ontology_preprocessing.base.OntologyParser` in
+    A ParserAction changes the behaviour of a :class:`kazu.ontology_preprocessing.base.OntologyParser` in
     a global sense.
 
     A ParserAction overrides any default behaviour of the parser, and also any conflicts that may occur with
-    :class:`.SynonymTermAction`\\s.
+    :class:`.CuratedTerm`\\s.
 
     These actions are useful for eliminating unwanted behaviour. For example, the root of the Mondo
     ontology is http://purl.obolibrary.org/obo/HP_0000001, which has a default label of 'All'. Since this is
     such a common word, and not very useful in terms of linking, we might want a global action so that this
     ID is not used anywhere in a Kazu pipeline.
 
     The parser_to_target_id_mappings field should specify the parser name and an affected IDs if required.
@@ -764,118 +725,127 @@
     def from_json(cls, json_dict: Dict) -> "GlobalParserActions":
         return cls(
             actions=[ParserAction.from_json(x) for x in json_dict["actions"]],
         )
 
 
 @dataclass(frozen=True)
-class Curation:
+class CuratedTerm:
     """
-    A Curation is a means to modify the behaviour of a specific :class:`.SynonymTerm`.
+    A CuratedTerm is a means to modify the behaviour of a specific :class:`.SynonymTerm`.
 
-    This can affect both the behaviour of :class:`kazu.modelling.ontology_preprocessing.base.OntologyParser`,
+    This can affect both the behaviour of :class:`kazu.ontology_preprocessing.base.OntologyParser`,
     and dictionary based NER (if using the :class:`kazu.steps.joint_ner_and_linking.explosion.ExplosionStringMatchingStep`).
-    This is controlled by the list of :class:`.SynonymTermAction`\\s attached.
 
     Example 1:
 
     The string 'ALL' is highly ambiguous. It might mean several diseases, or simply 'all'. Therefore, we want
     to add a curation as follows, so that it will only be used as a linking target and not for dictionary based NER:
 
     .. code-block:: python
 
-        Curation(curated_synonym='ALL',
-             case_sensitive=True,
-             actions=[
-                SynonymTermAction(behaviour=SynonymTermBehaviour.ADD_FOR_LINKING_ONLY,
-                                  parser_to_target_id_mappings={'OPENTARGETS_DISEASE': {'MONDO:0004967'}}}, entity_class='disease'),
-            ],
-             mention_confidence=MentionConfidence.POSSIBLE)
+        CuratedTerm(
+            curated_synonym="ALL",
+            case_sensitive=True,
+            behaviour=CuratedTermBehaviour.ADD_FOR_LINKING_ONLY,
+            associated_id_sets=None,
+            mention_confidence=MentionConfidence.POSSIBLE,
+        )
 
 
     Example 2:
 
     The string 'LH' is incorrectly identified as a synonym of the PLOD1 (ENSG00000083444) gene, whereas more often than not, it's actually an abbreviation of Lutenising Hormone.
-    We therefore want to drop this reference, and add a new one to LHB (ENSG00000104826, or Lutenising Hormone Subunit Beta)
+    We therefore want to override the associated_id_sets to LHB (ENSG00000104826, or Lutenising Hormone Subunit Beta)
 
-    The Curation we therefore want is:
+    The CuratedTerm we therefore want is:
 
     .. code-block:: python
 
-        Curation(curated_synonym='LH',
-             case_sensitive=True,
-             actions=[
-                SynonymTermAction(behaviour=SynonymTermBehaviour.DROP_SYNONYM_TERM_FOR_LINKING,
-                                  parser_to_target_id_mappings={'OPENTARGETS_TARGET': set()}, entity_class='gene'),
-                SynonymTermAction(behaviour=SynonymTermBehaviour.ADD_FOR_NER_AND_LINKING,
-                                  parser_to_target_id_mappings={'OPENTARGETS_TARGET': {'ENSG00000104826'}}, entity_class='gene'),
-            ],
-             mention_confidence=MentionConfidence.POSSIBLE)
+        CuratedTerm(
+            curated_synonym="LH",
+            case_sensitive=True,
+            behaviour=CuratedTermBehaviour.ADD_FOR_LINKING_ONLY,
+            associated_id_sets=frozenset((EquivalentIdSet(("ENSG00000104826", "ENSEMBL")),)),
+            mention_confidence=MentionConfidence.POSSIBLE,
+        )
 
     Example 3:
 
-    A :class:`.SynonymTerm` has an unwanted :class:`.EquivalentIdSet` attached to it, but is otherwise good. We want to remove this set
+    A :class:`.SynonymTerm` has an alternative synonym not referenced in the underlying ontology, and we want to add it.
+    We want it to inherit all the behaviour from the original term
 
     .. code-block:: python
 
-        Curation(curated_synonym='some good synonym',
-         case_sensitive=True,
-         actions=[
-            SynonymTermAction(behaviour=SynonymTermBehaviour.DROP_ID_SET_FROM_SYNONYM_TERM,
-                              parser_to_target_id_mappings={'OPENTARGETS_TARGET': {'an id from the bad set'}}}, entity_class='gene'),
-        ],
-         mention_confidence=MentionConfidence.POSSIBLE)
-
-    Notes:
-
-    The term_norm field is calculated by the :class:`kazu.modelling.ontology_preprocessing.base.OntologyParser`
-    if required, and should not be set manually.
-
-    mention_confidence is currently non-functional, and will be expanded upon at a later date
-
-
-
+        CuratedTerm(
+            curated_synonym="breast carcinoma",
+            case_sensitive=True,
+            source_term="breast cancer",
+            behaviour=CuratedTermBehaviour.INHERIT_FROM_SOURCE_TERM,
+            mention_confidence=MentionConfidence.POSSIBLE,
+        )
     """
 
+    curated_synonym: str
     mention_confidence: MentionConfidence
-    actions: List[SynonymTermAction]
+    behaviour: CuratedTermBehaviour
     case_sensitive: bool
-    curated_synonym: str
-    #: MongoDB compatible identifier for this curation
-    _id: Dict[str, str] = field(default_factory=dict)
-    #: parser specific behaviours
-    _parser_name_to_action: DefaultDict[str, List[SynonymTermAction]] = field(
-        default_factory=lambda: defaultdict(list), init=False
-    )
+    #: If specified, will override the parser defaults for the associated :class:`.SynonymTerm`\, as long as conflicts do not occur
+    associated_id_sets: Optional[AssociatedIdSets] = None
+    _id: bson.ObjectId = field(default_factory=bson.ObjectId, compare=False)
+    #: The original term that is used as a 'seed' term for this curation.
+    #: note, this is used for NER to determine how linking is performed. If you also
+    #: want to use this curation as a linking target for non-dictionary based NER processes,
+    #: or the term is identical to the one used in the source ontology,
+    #: this should be set to None, so that a novel term_norm is calculated
+    source_term: Optional[str] = None
 
     def __post_init__(self):
         # data validation
         if not isinstance(self.curated_synonym, str):
             raise ValueError(f"curated_synonym should be a string, {self}")
-        for action in self.actions:
-            for parser_name in action.parser_to_target_id_mappings.keys():
-                self._parser_name_to_action[parser_name].append(action)
 
-    def parser_behaviour(self, parser_name: str) -> Iterable[SynonymTermAction]:
-        """
-        Generator that yields behaviours for a specific parser, based on the order they are
-        specified in.
+    def term_norm_for_linking(self, entity_class: str):
+        norm_target = self.curated_synonym if self.source_term is None else self.source_term
+        return StringNormalizer.normalize(norm_target, entity_class)
 
-        :param parser_name:
-        :return:
-        """
-        yield from self._parser_name_to_action.get(parser_name, [])
+    @classmethod
+    def from_json(cls, json_str: str) -> "CuratedTerm":
+        json_dict = json_util.loads(json_str)
+        return cls.from_dict(json_dict)
 
     @classmethod
-    def from_json(cls, json_dict: Dict) -> "Curation":
-        # we call str on json_dict["_id"] in case it's a bson ObjectId
-        if not isinstance(json_dict["_id"], dict):
-            _id = {"$oid": str(json_dict["_id"])}
+    def from_dict(cls, json_dict: Dict) -> "CuratedTerm":
+        if json_dict["associated_id_sets"] is None:
+            frozen_assoc_id_sets = None
         else:
-            _id = json_dict["_id"]
+            assoc_id_sets = set()
+            for equiv_id_set in json_dict["associated_id_sets"]:
+                ids = frozenset((idx, source) for idx, source in equiv_id_set["ids_and_source"])
+                equiv_id_set = EquivalentIdSet(ids)
+                assoc_id_sets.add(equiv_id_set)
+
+            frozen_assoc_id_sets = frozenset(assoc_id_sets)
+
         return cls(
-            mention_confidence=MentionConfidence(json_dict["mention_confidence"]),
-            actions=[SynonymTermAction.from_json(x) for x in json_dict["actions"]],
+            mention_confidence=MentionConfidence[json_dict["mention_confidence"]],
+            behaviour=CuratedTermBehaviour(json_dict["behaviour"]),
+            associated_id_sets=frozen_assoc_id_sets,
             case_sensitive=json_dict["case_sensitive"],
             curated_synonym=json_dict["curated_synonym"],
-            _id=_id,
+            source_term=json_dict["source_term"],
+            _id=json_dict.get("_id", bson.ObjectId()),
         )
+
+    def to_dict(self, preserve_structured_object_id: bool = True):
+        if preserve_structured_object_id:
+            oid = self._id
+            as_dict = DocumentJsonUtils.obj_to_dict_repr(self)
+            as_dict["_id"] = oid  # type: ignore[index,call-overload]
+        else:
+            as_dict = DocumentJsonUtils.obj_to_dict_repr(self)
+        return as_dict
+
+    def to_json(self) -> str:
+        as_json = self.to_dict(False)
+        assert isinstance(as_json, dict)
+        return json.dumps(as_json)
```

### Comparing `kazu-0.1.0/kazu/data/pytorch.py` & `kazu-1.0.0/kazu/data/pytorch.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/modelling/hf_lightning_wrappers.py` & `kazu-1.0.0/kazu/steps/ner/hf_lightning_wrappers.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/modelling/annotation/acceptance_test.py` & `kazu-1.0.0/kazu/annotation/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/modelling/annotation/label_studio.py` & `kazu-1.0.0/kazu/annotation/label_studio.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 from copy import deepcopy
 from functools import cached_property
 from typing import Dict, Tuple, Set, List, Iterable
 from xml.dom.minidom import Document as XMLDocument, DOMImplementation
 from xml.dom.minidom import Element, getDOMImplementation
 
 import requests
-from requests import HTTPError
-
 from kazu.data.data import (
     Document,
     Section,
     Entity,
     Mapping,
     StringMatchConfidence,
     CharSpan,
 )
 from kazu.utils.grouping import sort_then_group
+from requests import HTTPError
 
 logger = logging.getLogger(__name__)
 
 _TAX_NAME = "taxonomy"
 
 
 class KazuToLabelStudioConverter:
@@ -451,47 +450,56 @@
                 f"{self.url}/api/projects/{self.project_id}", headers=self.headers
             )
             if resp.status_code != 204:
                 resp.raise_for_status()
         except (requests.exceptions.HTTPError, ValueError) as e:
             logger.warning(f"failed to delete project {self.project_name}. Maybe it doesn't exist?")
             logger.exception(e)
+        if "project_id" in self.__dict__:
+            del self.project_id
 
-    def create_linking_project(self, tasks, view: LabelStudioAnnotationView):
-        payload = {
-            "title": self.project_name,
-            "label_config": view.create_main_view(tasks),
-        }
+    def create_linking_project(self):
+        payload = {"title": self.project_name}
 
         try:
             resp = requests.post(f"{self.url}/api/projects", json=payload, headers=self.headers)
             if resp.status_code != 201:
                 resp.raise_for_status()
         except requests.exceptions.HTTPError as e:
             logger.error(f"failed to create project {self.project_name}")
             raise e
 
+    def update_view(self, view: LabelStudioAnnotationView, docs: List[Document]):
+        tasks = KazuToLabelStudioConverter.convert_docs_to_tasks(docs)
+        payload = {"label_config": view.create_main_view(tasks)}
+
+        try:
+            resp = requests.patch(
+                f"{self.url}/api/projects/{self.project_id}", json=payload, headers=self.headers
+            )
+            if resp.status_code not in {200, 201}:
+                resp.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            logger.error(f"failed to update view for project {self.project_name}")
+            raise e
+
+    def update_tasks(self, docs: List[Document]):
+        tasks = KazuToLabelStudioConverter.convert_docs_to_tasks(docs)
         try:
             resp = requests.post(
                 f"{self.url}/api/projects/{self.project_id}/import",
                 json=tasks,
                 headers=self.headers,
             )
-            if resp.status_code != 201:
+            if resp.status_code not in {200, 201}:
                 resp.raise_for_status()
         except requests.exceptions.HTTPError as e:
-            logger.error(f"failed to load data for project {self.project_name}")
+            logger.error(f"failed to update tasks for project {self.project_name}")
             raise e
 
-    def import_to_ls(self, docs: List[Document]):
-        tasks = KazuToLabelStudioConverter.convert_docs_to_tasks(docs)
-        return requests.post(
-            f"{self.url}/api/projects/{self.project_id}/import", json=tasks, headers=self.headers
-        )
-
     def get_all_tasks(self):
         tasks = requests.get(
             f"{self.url}/api/tasks?page_size=1000000&project={self.project_id}",
             headers=self.headers,
         ).json()
         ids = [task["id"] for task in tasks["tasks"]]
         return self.get_tasks(ids)
```

### Comparing `kazu-0.1.0/kazu/modelling/distillation/dataprocessor.py` & `kazu-1.0.0/kazu/distillation/dataprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,23 +46,23 @@
 
 
 class SeqTagProcessor(DataProcessor):
     """Base class for data converters for sequence tagging data sets."""
 
     def get_train_examples(self, data_dir) -> List[InputExample]:
         """Gets a collection of :class:`transformers.InputExample` for the train set."""
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def get_dev_examples(self, data_dir) -> List[InputExample]:
         """Gets a collection of :class:`transformers.InputExample` for the dev set."""
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def get_aug_examples(self, data_dir) -> List[InputExample]:
         """Gets a collection of :class:`transformers.InputExample` for the aug set."""
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 class NerProcessor(SeqTagProcessor):
     def get_train_examples(self, data_dir: str) -> List[InputExample]:
         return self._create_examples(
             self._read_data(os.path.join(data_dir, "train_dev.tsv")), "train"
         )
```

### Comparing `kazu-0.1.0/kazu/modelling/distillation/lightning_plugins.py` & `kazu-1.0.0/kazu/distillation/lightning_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def load_checkpoint(
         self, path: Union[str, Path], storage_options: Optional[Any] = None
     ) -> Dict[str, Any]:
         """Not currently implemented.
 
         See :external+pytorch_lightning:meth:`CheckpointIO.load_checkpoint <lightning.pytorch.plugins.io.CheckpointIO.load_checkpoint>`
         for details of the abstract method."""
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def remove_checkpoint(
         self,
         path: Union[str, Path],
     ) -> None:
 
         os.remove(path)
```

### Comparing `kazu-0.1.0/kazu/modelling/distillation/models.py` & `kazu-1.0.0/kazu/distillation/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,17 +58,17 @@
     get_constant_schedule,
     get_linear_schedule_with_warmup,
     get_cosine_schedule_with_warmup,
     get_constant_schedule_with_warmup,
 )
 from transformers.utils import check_min_version
 
-from kazu.modelling.distillation.dataprocessor import NerProcessor
-from kazu.modelling.distillation.metrics import numeric_label_f1_score, IGNORE_IDX
-from kazu.modelling.distillation.tiny_transformers import TinyBertForSequenceTagging
+from kazu.distillation.dataprocessor import NerProcessor
+from kazu.distillation.metrics import numeric_label_f1_score, IGNORE_IDX
+from kazu.distillation.tiny_transformers import TinyBertForSequenceTagging
 
 check_min_version("4.0.0")  # at least 4.0.0... for optimerzers
 
 logger = logging.getLogger(__name__)
 
 SCHEDULES: Dict[Optional[str], Callable] = {
     None: get_constant_schedule,
@@ -93,15 +93,15 @@
         label_map: Dict[str, int],
         max_length: int,
     ):
         """
 
         :param tokenizer: typically created from AutoTokenizer.from_pretrained
         :param examples: a list of InputExample, typically created from a
-            :class:`kazu.modelling.distillation.dataprocessor.NerProcessor`
+            :class:`kazu.distillation.dataprocessor.NerProcessor`
         :param label_map: str to int mapping of labels
         :param max_length: The maximum number of tokens per instance that the model can handle.
             Inputs longer than max_length value will be truncated.
         """
         self.label_map = label_map
         self.examples = examples
         self.tokenizer = tokenizer
@@ -235,15 +235,15 @@
 
     def get_training_examples(self) -> List[InputExample]:
         """
         subclasses should implement this
 
         :return:
         """
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def get_optimizer_grouped_parameters(self, student_model):
         param_optimizer = list(student_model.named_parameters())
         size = 0
         logger.info("student_model.named_parameters :")
         for n, p in student_model.named_parameters():
             logger.info("n: {}".format(n))
```

### Comparing `kazu-0.1.0/kazu/modelling/distillation/tiny_transformers.py` & `kazu-1.0.0/kazu/distillation/tiny_transformers.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/modelling/distillation/train.py` & `kazu-1.0.0/kazu/distillation/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import hydra
 import pytorch_lightning
 import torch
 from hydra.utils import instantiate
 from omegaconf import DictConfig
 from pytorch_lightning import Trainer
 
-from kazu.modelling.distillation.models import (
+from kazu.distillation.models import (
     SequenceTaggingDistillationForFinalLayer,
     SequenceTaggingDistillationForIntermediateLayer,
 )
 from kazu.utils.constants import HYDRA_VERSION_BASE
 
 
 @hydra.main(version_base=HYDRA_VERSION_BASE, config_path="../../conf", config_name="config")
```

### Comparing `kazu-0.1.0/kazu/modelling/language/language_phenomena.py` & `kazu-1.0.0/kazu/language/language_phenomena.py`

 * *Files 19% similar despite different names*

```diff
@@ -48,7 +48,10 @@
     "\u03C5": "upsilon",
     "\u03C6": "phi",
     "\u03D5": "phi",
     "\u03C7": "chi",
     "\u03C8": "psi",
     "\u03C9": "omega",
 }
+
+DASHES = {chr(0x2212), chr(0x002D)}
+DASHES.update(chr(c) for c in range(0x2010, 0x2016))
```

### Comparing `kazu-0.1.0/kazu/modelling/language/string_similarity_scorers.py` & `kazu-1.0.0/kazu/language/string_similarity_scorers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 from cachetools import LFUCache
 from pytorch_lightning import Trainer
 from rapidfuzz import fuzz
 from torch import Tensor, cosine_similarity
 
 from kazu.data.data import NumericMetric
-from kazu.modelling.linking.sapbert.train import PLSapbertModel
+from kazu.linking.sapbert.train import PLSapbertModel
 from kazu.utils.utils import Singleton
 
 
 class StringSimilarityScorer(Protocol):
     """
     calculates a NumericMetric based on a string match or a normalised string match and a normalised term
     """
 
     def __call__(self, reference_term: str, query_term: str) -> NumericMetric:
-        ...
+        raise NotImplementedError
 
 
 class BooleanStringSimilarityScorer(StringSimilarityScorer, Protocol):
     def __call__(self, reference_term: str, query_term: str) -> bool:
-        ...
+        raise NotImplementedError
 
 
 class NumberMatchStringSimilarityScorer(BooleanStringSimilarityScorer):
     """
     checks all numbers in reference_term are represented in term_norm
     """
```

### Comparing `kazu-0.1.0/kazu/modelling/linking/sapbert/train.py` & `kazu-1.0.0/kazu/linking/sapbert/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pytorch_lightning import Trainer, LightningModule
 from pytorch_lightning.utilities.types import (
     STEP_OUTPUT,
     TRAIN_DATALOADERS,
     EVAL_DATALOADERS,
     EPOCH_OUTPUT,
 )
-from pytorch_metric_learning import miners, losses
 from torch import optim
 from torch.utils.data import DataLoader, Dataset
 from transformers import (
     AutoConfig,
     AutoTokenizer,
     AutoModel,
     BatchEncoding,
@@ -335,14 +334,22 @@
 
         self.config = AutoConfig.from_pretrained(model_name_or_path)
         self.tokeniser = AutoTokenizer.from_pretrained(model_name_or_path, config=self.config)
         self.model = AutoModel.from_pretrained(model_name_or_path, config=self.config)
         self.sapbert_evaluation_manager = sapbert_evaluation_manager
         self.sapbert_training_params = sapbert_training_params
         if sapbert_training_params is not None:
+            try:
+                from pytorch_metric_learning import miners, losses
+            except ImportError as e:
+                raise ImportError(
+                    "Running the SapBERT model training code requires pytorch_metric_learning to be installed.\n"
+                    "We recommend running 'pip install kazu[model_training]' to get all model training"
+                    " dependencies."
+                ) from e
             self.loss = losses.MultiSimilarityLoss(alpha=1, beta=60, base=0.5)
             self.miner = miners.TripletMarginMiner(
                 margin=sapbert_training_params.miner_margin,
                 type_of_triplets=sapbert_training_params.type_of_triplets,
             )
             self.ontology_embeddings = None
 
@@ -466,15 +473,15 @@
         generate new embeddings for each :attr:`SapbertEvaluationDataset.ontology_source` and query them with
         :attr:`SapbertEvaluationDataset.query_source`
 
         :param outputs:
         :return:
         """
         assert self.sapbert_evaluation_manager is not None
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def log_results(self, dataset_name, metrics):
         for key, val in metrics.items():
             if key.startswith("acc"):
                 self.log(key, value=val, rank_zero_only=True)
                 logger.info(f"{dataset_name}: {key}, {val}")
```

### Comparing `kazu-0.1.0/kazu/modelling/ontology_matching/LICENSE` & `kazu-1.0.0/kazu/ontology_matching/LICENSE`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/modelling/ontology_matching/README.md` & `kazu-1.0.0/kazu/ontology_matching/README.md`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/modelling/ontology_matching/assemble_pipeline.py` & `kazu-1.0.0/kazu/ontology_matching/assemble_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     CONCAT_QUOTES,
     ALPHA_LOWER,
     ALPHA_UPPER,
     ALPHA,
     HYPHENS,
 )
 
-from kazu.modelling.ontology_matching.ontology_matcher import OntologyMatcher, SPAN_KEY
-from kazu.modelling.ontology_preprocessing.base import OntologyParser
+from kazu.ontology_matching.ontology_matcher import OntologyMatcher, SPAN_KEY
+from kazu.ontology_preprocessing.base import OntologyParser
 from kazu.utils.utils import PathLike
 
 
 SPACY_DEFAULT_INFIXES = (
     LIST_ELLIPSES
     + LIST_ICONS
     + [
@@ -44,53 +44,44 @@
 
     infixes = custom_infixes + DEFAULT_INFIXES_MINUS_HYPHENS
     infix_re = spacy.util.compile_infix_regex(infixes)
     nlp.tokenizer.infix_finditer = infix_re.finditer
 
 
 def main(
-    output_dir: PathLike,
-    parsers: List[OntologyParser],
-    use_curations: bool = True,
-    span_key: str = SPAN_KEY,
+    output_dir: PathLike, parsers: List[OntologyParser], span_key: str = SPAN_KEY
 ) -> spacy.language.Language:
     """Generates, serializes and returns a Spacy pipeline with an
-    :class:`~kazu.modelling.ontology_matching.ontology_matcher.OntologyMatcher`.
+    :class:`~kazu.ontology_matching.ontology_matcher.OntologyMatcher`.
 
     Generates an English Spacy pipeline with a tokenizer, a sentencizer with default
     config, and an OntologyMatcher based on the input parameters. The pipeline is
     written to disk, and also returned to the caller.
 
-    If 'use_curations' is False,
-    :class:`~kazu.modelling.ontology_matching.ontology_matcher.OntologyMatcher` is built directly
+    If a parser has no curations configured, the
+    :class:`~kazu.ontology_matching.ontology_matcher.OntologyMatcher` is built directly
     from the configured synonyms from the parsers (with any associated generated synonyms). This is
     useful for trying to understand which strings are 'noisy', but not recommended for production as raw ontology
     data tends to need some curation before it can be applied.
 
-    If 'use_curations' is True, it will be built using the configured instances of :class:`~kazu.data.data.Curation`
+    If a parser has curations configured, it will be built using the configured instances of :class:`~kazu.data.data.CuratedTerm`
     associated with the parser. This is generally the recommended behaviour in production, although obviously
     requires a set of high quality curations to be effective
 
     :param output_dir: the output directory to write the pipeline into.
     :param parsers: build the pipeline using these parsers as a data source.
-    :param use_curations:
     :param span_key: the key to use within the generated Spacy Docs'
         `span attribute <https://spacy.io/api/doc#spans>`_ to store and access recognised NER
         spans.
     """
     nlp = spacy.blank("en")
     custom_tokenizer(nlp)
     nlp.add_pipe("sentencizer")
     config = {
         "span_key": span_key,
         "parser_name_to_entity_type": {parser.name: parser.entity_class for parser in parsers},
     }
     ontology_matcher = nlp.add_pipe("ontology_matcher", config=config)
     assert isinstance(ontology_matcher, OntologyMatcher)
-
-    if use_curations:
-        ontology_matcher.create_phrasematchers_using_curations(parsers)
-    else:
-        ontology_matcher.create_uncurated_lowercase_phrasematcher(parsers)
-
+    ontology_matcher.create_phrasematchers_using_curations(parsers)
     nlp.to_disk(output_dir)
     return nlp
```

### Comparing `kazu-0.1.0/kazu/modelling/ontology_matching/ontology_matcher.py` & `kazu-1.0.0/kazu/ontology_matching/ontology_matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 from dataclasses import dataclass, asdict
 from functools import partial
 from pathlib import Path
 from typing import Any, List, Dict, Union, Iterable, Tuple, Optional, Set, cast
 
 import spacy
 import srsly
+from kazu.database.in_memory_db import SynonymDatabase
 from spacy import Language
 from spacy.matcher import PhraseMatcher, Matcher
 from spacy.tokens import Span, SpanGroup, Doc, Token
 from spacy.util import SimpleFrozenList
 
-from kazu.data.data import SynonymTermBehaviour
-from kazu.modelling.ontology_preprocessing.base import (
+from kazu.data.data import CuratedTermBehaviour, CuratedTerm
+from kazu.ontology_preprocessing.base import (
     OntologyParser,
 )
 from kazu.utils.grouping import sort_then_group
 from kazu.utils.utils import PathLike
 
 GENE = "gene"
 DRUG = "drug"
 ANATOMY = "anatomy"
 DISEASE = "disease"
 CELL_LINE = "cell_line"
+CELL_TYPE = "cell_type"
 ENTITY = "entity"
 
 SPAN_KEY = "RAW_HITS"
 MATCH_ID_SEP = ":::"
 
 logger = logging.getLogger(__name__)
 
@@ -132,134 +134,127 @@
         self.cfg.labels = list(labels)
         self.set_context_matchers()
 
     def set_context_matchers(self):
         self.tp_matchers, self.fp_matchers = self._create_token_matchers()
         self.tp_coocc_dict, self.fp_coocc_dict = self._create_coocc_dicts()
 
+    def filter_curations_for_ner(
+        self, curations: Iterable[CuratedTerm], parser: OntologyParser
+    ) -> Iterable[CuratedTerm]:
+        """check curations are still represented in DB before they can be used for NER."""
+        original_terms = defaultdict(set)
+        inherited_terms = defaultdict(set)
+        syn_db = SynonymDatabase()
+        for curation in curations:
+            if curation.behaviour is CuratedTermBehaviour.ADD_FOR_NER_AND_LINKING:
+                original_terms[curation.curated_synonym].add(curation)
+            elif curation.behaviour is CuratedTermBehaviour.INHERIT_FROM_SOURCE_TERM:
+                inherited_terms[curation.source_term].add(curation)
+            else:
+                # not an ner behaviour, so move on to the next curation in the loop
+                continue
+        for curated_synonym, curation_set in original_terms.items():
+            if len(curation_set) > 1:
+                # note, this shouldn't happen, as it should be handled by the curation validation logic.
+                # however, just in case this logic changes, we'll leave this here
+                logger.warning(
+                    "multiple curations detected for %s, %s", curated_synonym, curation_set
+                )
+                term_norm = next(iter(curation_set)).term_norm_for_linking(parser.entity_class)
+                if term_norm not in syn_db.get_all(parser.name):
+                    logger.warning(
+                        "dictionary based NER needs an database entry for %s, %s, but none exists",
+                        term_norm,
+                        parser.name,
+                    )
+                    continue
+            yield from curation_set
+            yield from inherited_terms.pop(curated_synonym, set())
+        if len(inherited_terms) > 0:
+            logger.warning(
+                "The following inherited curations were unmatched to a source term, and will be ignored for NER: %s",
+                inherited_terms.values(),
+            )
+
     def create_phrasematchers_using_curations(
         self, parsers: List[OntologyParser]
     ) -> Tuple[Optional[PhraseMatcher], Optional[PhraseMatcher]]:
-        """Create Spacy `PhraseMatcher <https://spacy.io/api/phrasematcher>`_\\ s based on :class:`.Curation`\\ s.
-
-        The :class:`.Curation`\\ s are provided to the :class:`.OntologyParser`\\ s as the ``curations`` parameter
-        when they are created, which are matched to appropriate entries in the :class:`.SynonymDatabase`\\ .
+        """Create Spacy `PhraseMatcher <https://spacy.io/api/phrasematcher>`_\\ s based on :class:`.CuratedTerm`\\ s.
 
+        Curations are produced by :py:meth:`.OntologyParser.populate_databases`\\ method
         :param parsers:
         :return:
         """
-
         if self.strict_matcher is not None or self.lowercase_matcher is not None:
             logging.warning("Phrase matchers are being redefined - is this by intention?")
 
         self.set_labels(parser.entity_class for parser in parsers)
         strict_matcher = PhraseMatcher(self.nlp.vocab, attr="ORTH")
         lowercase_matcher = PhraseMatcher(self.nlp.vocab, attr="NORM")
-
+        logger.info("ontology matcher build triggered. Forcing database repopulation.")
         for parser in parsers:
-            curation_with_term_norms = parser.populate_databases(force=True)
-            if curation_with_term_norms is None:
+            parser_curations = parser.populate_databases(force=True, return_curations=True)
+            if parser_curations is None:
                 logger.warning(
                     "tried to create PhraseMatchers from Curations for parser %s, but none have been provided",
                     parser.name,
                 )
                 continue
-            if len(curation_with_term_norms) == 0:
+            if len(parser_curations) == 0:
                 logger.warning(
-                    "tried to create PhraseMatchers from Curations for parser %s, but no CurationWithTermNorms were created",
+                    "tried to create PhraseMatchers from Curations for parser %s, but no Curations were produced",
                     parser.name,
                 )
                 continue
 
-            # spacy's typing isn't smart enough to know this will have a 'pipe' attr
-            patterns = self.nlp.tokenizer.pipe(  # type: ignore[union-attr]
-                curation.curated_synonym if curation.case_sensitive
-                # we need it lowercased for the case-insensitive matcher.
-                # type ignore as curated_synonym will not be None, as only
-                # curations with a curated_synonym will be 'matched'.
-                else curation.curated_synonym.lower()  # type: ignore[union-attr]
-                for curation in curation_with_term_norms
-            )
+            curations_for_ner = set(self.filter_curations_for_ner(parser_curations, parser))
 
-            for curation, pattern in zip(curation_with_term_norms, patterns):
+            # deduplicating match id's and patterns saves memory in the spacy pipeline
+            match_ids_and_strings_cs = set()
+            match_ids_and_strings_ci = set()
+            for curation in curations_for_ner:
                 # a curation can have different term_norms for different parsers,
                 # since the string normalizer's output depends on the entity class.
                 # Also, a curation may exist in multiple SynonymTerm.terms
-                for action in curation.parser_behaviour(parser_name=parser.name):
-                    if action.behaviour is SynonymTermBehaviour.ADD_FOR_NER_AND_LINKING:
-                        match_id = parser.name + self.match_id_sep + action.term_norm
-                        if curation.case_sensitive:
-                            strict_matcher.add(match_id, [pattern])
-                        else:
-                            lowercase_matcher.add(match_id, [pattern])
+                term_norm = curation.term_norm_for_linking(parser.entity_class)
+                match_id = (
+                    parser.name
+                    + self.match_id_sep
+                    + term_norm
+                    + self.match_id_sep
+                    + str(curation.mention_confidence.value)
+                )
+                if curation.case_sensitive:
+                    match_ids_and_strings_cs.add(
+                        (
+                            match_id,
+                            curation.curated_synonym,
+                        )
+                    )
+                else:
+                    match_ids_and_strings_ci.add(
+                        (
+                            match_id,
+                            curation.curated_synonym.lower(),
+                        )
+                    )
+
+            for match_id, match_str in match_ids_and_strings_cs:
+                strict_matcher.add(match_id, [self.nlp.tokenizer(match_str)])
+            for match_id, match_str in match_ids_and_strings_ci:
+                lowercase_matcher.add(match_id, [self.nlp.tokenizer(match_str)])
 
         # only set the phrasematcher if we have any rules for them
         # this lets us skip running a phrasematcher if it has no rules when we come
         # to calling OntologyMatcher
         self.strict_matcher = strict_matcher if len(strict_matcher) != 0 else None
         self.lowercase_matcher = lowercase_matcher if len(lowercase_matcher) != 0 else None
         return self.strict_matcher, self.lowercase_matcher
 
-    def create_uncurated_lowercase_phrasematcher(
-        self, parsers: List[OntologyParser]
-    ) -> Tuple[PhraseMatcher, None]:
-        """
-        Create a lower case Spacy `PhraseMatcher <https://spacy.io/api/phrasematcher>`_ using just the synonyms in the
-        :class:`.OntologyParser`\\ s and their configured ``synonym_generator``\\ s (see
-        :meth:`.OntologyParser.__init__`\\ ).
-
-        This is intended for use primarily when first adding a parser, to then run over relevant documents and
-        create :class:`.Curation`\\ s based on the result. You could also use it if you have a very simple set
-        of terms to recognise that aren't case-sensitive and you don't intend to do any curation at all.
-
-        :param parsers:
-        :return: The lowercase PhraseMatcher and None - to match the return shape of
-            :meth:`create_phrasematchers_using_curations`\\ .
-        """
-
-        if self.strict_matcher is not None or self.lowercase_matcher is not None:
-            logging.warning("Phrase matchers are being redefined - is this by intention?")
-        self.set_labels(parser.entity_class for parser in parsers)
-        lowercase_matcher = PhraseMatcher(self.nlp.vocab, attr="NORM")
-        for parser in parsers:
-            synonym_terms = parser.generate_synonyms()
-            parser_name = parser.name
-            logging.info(
-                f"generating {sum(len(x.terms) for x in synonym_terms)} patterns for {parser_name}"
-            )
-            synonyms_and_terms = [
-                (term, synonym_term)
-                for synonym_term in synonym_terms
-                for term in synonym_term.terms
-            ]
-            # spacy's typing isn't smart enough to know this will have a 'pipe' attr
-            patterns = self.nlp.tokenizer.pipe(term for (term, _synonym_term) in synonyms_and_terms)  # type: ignore[union-attr]
-
-            for (term, synonym_term), pattern in zip(synonyms_and_terms, patterns):
-                match_id = parser_name + self.match_id_sep + synonym_term.term_norm
-                try:
-                    # if we're adding to the lowercase matcher, we don't need to add
-                    # to the exact case matcher as well, since we'll definitely get
-                    # the hit, so would just be a waste of memory and compute.
-                    lowercase_matcher.add(match_id, [pattern])
-
-                except KeyError as e:
-                    logging.warning(
-                        f"failed to add '{term}'. StringStore is {len(self.nlp.vocab.strings)} ",
-                        e,
-                    )
-
-        self.lowercase_matcher = lowercase_matcher
-
-        if len(lowercase_matcher) == 0:
-            raise RuntimeError(
-                "No rules have been added to the PhraseMatcher. Has the OntologyMatcher been given parsers with synonyms?"
-            )
-        return lowercase_matcher, None
-
     def __call__(self, doc: Doc) -> Doc:
         if self.nr_strict_rules == 0 and self.nr_lowercase_rules == 0:
             raise ValueError("there are no matcher rules configured!")
 
         # at least one phrasematcher will now be set.
         # normally, this will only be one: either a strict matcher if constructed by curated list,
         # or a lowercase matcher if constructed 'from scrach' using the parsers - currently just an
@@ -283,28 +278,23 @@
             key_func=lambda x: (
                 x[1],
                 x[2],
             ),
         ):
             data = defaultdict(set)
             for mat in matches_grp:
-                parser_name, term_norm = self.nlp.vocab.strings.as_string(mat[0]).split(
-                    self.match_id_sep, maxsplit=1
+                parser_name, term_norm, confidence = self.nlp.vocab.strings.as_string(mat[0]).split(
+                    self.match_id_sep, maxsplit=2
                 )
                 ent_class = self.parser_name_to_entity_type[parser_name]
-                data[ent_class].add(
-                    (
-                        parser_name,
-                        term_norm,
-                    )
-                )
-            for ent_class in data:
+                data[ent_class].add((parser_name, term_norm, confidence))
+            for ent_class, ent_class_data in data.items():
                 # we use a uuid here so that every span hash is unique
                 new_span = Span(doc, start, end, label=uuid.uuid4().hex)
-                new_span._.set("ontology_dict_", {ent_class: data[ent_class]})
+                new_span._.set("ontology_dict_", {ent_class: ent_class_data})
                 spans.append(new_span)
         final_spans = self.filter_by_contexts(doc, spans)
         span_group = SpanGroup(doc, name=self.span_key, spans=final_spans)
         doc.spans[self.span_key] = span_group
         return doc
 
     def filter_by_contexts(self, doc, spans):
@@ -397,38 +387,40 @@
             return False
         return False
 
     def _create_token_matchers(self):
         tp_matchers = {}
         fp_matchers = {}
         if CELL_LINE in self.labels:
-            tp_matchers[CELL_LINE] = self._create_cellline_tp_tokenmatcher()
+            tp_matchers[CELL_LINE] = self._create_cell_tp_tokenmatcher(CELL_LINE)
+        if CELL_TYPE in self.labels:
+            tp_matchers[CELL_TYPE] = self._create_cell_tp_tokenmatcher(CELL_TYPE)
 
         if ANATOMY in self.labels:
             fp_matchers[ANATOMY] = self._create_anatomy_fp_tokenmatcher()
         return tp_matchers, fp_matchers
 
-    def _create_cellline_tp_tokenmatcher(self):
-        """Define patterns where a Cell line appears and it's likely a true positive"""
+    def _create_cell_tp_tokenmatcher(self, ent_class: str):
+        """Define patterns where a Cell line or type appears and it's likely a true positive"""
         matcher = Matcher(self.nlp.vocab)
         pattern_1: List[Dict[str, Any]] = [
-            {"_": {CELL_LINE: True}},
+            {"_": {ent_class: True}},
             {"LOWER": {"IN": ["cell", "cells"]}},
         ]
         pattern_2: List[Dict[str, Any]] = [
             {"LOWER": "cell"},
             {"LOWER": "line"},
-            {"_": {CELL_LINE: True}},
+            {"_": {ent_class: True}},
         ]
         pattern_3: List[Dict[str, Any]] = [
             {"LOWER": "cell"},
             {"LOWER": "type"},
-            {"_": {CELL_LINE: True}},
+            {"_": {ent_class: True}},
         ]
-        matcher.add("Cell_line_context", [pattern_1, pattern_2, pattern_3])
+        matcher.add("Cell_context", [pattern_1, pattern_2, pattern_3])
         return matcher
 
     def _create_anatomy_fp_tokenmatcher(self):
         """Define patterns where an atanomy entity appears and it's likely a false positive"""
         matcher = Matcher(self.nlp.vocab)
         patterns: List[List[Dict[str, Any]]] = []
         if DRUG in self.labels:
```

### Comparing `kazu-0.1.0/kazu/modelling/ontology_preprocessing/synonym_generation.py` & `kazu-1.0.0/kazu/ontology_preprocessing/synonym_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,69 +5,72 @@
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from copy import deepcopy
 from typing import List, Dict, Optional, Iterable, Set
 
 from kazu.data.data import SynonymTerm, EquivalentIdAggregationStrategy
-from kazu.modelling.language.language_phenomena import GREEK_SUBS
+from kazu.language.language_phenomena import GREEK_SUBS, DASHES
 from kazu.utils.utils import PathLike
 
 import spacy
 
 logger = logging.getLogger(__name__)
 
 
 class SynonymGenerator(ABC):
     @abstractmethod
-    def call(self, synonym: SynonymTerm) -> Optional[SynonymTerm]:
+    def call(self, synonym_str: str) -> Optional[Set[str]]:
         pass
 
-    def __call__(self, synonyms: Set[SynonymTerm]) -> Set[SynonymTerm]:
+    def __call__(self, synonym_terms: Set[SynonymTerm]) -> Set[SynonymTerm]:
 
-        existing_terms = set(term for synonym in synonyms for term in synonym.terms)
+        existing_terms = set(term for synonym in synonym_terms for term in synonym.terms)
 
         result: Set[SynonymTerm] = set()
-        for synonym in synonyms:
-            generated_synonym_terms: Optional[SynonymTerm] = self.call(synonym)
-            if generated_synonym_terms:
-                new_terms = set()
-                for generated_syn in generated_synonym_terms.terms:
-                    if generated_syn in existing_terms:
-                        logger.debug(
-                            f"generated synonym '{generated_syn}' matches existing synonym {synonym} "
-                        )
-                    elif generated_syn in new_terms:
-                        logger.debug(
-                            f"generated synonym '{generated_syn}' matches another generated synonym {synonym} "
+        for synonym_term in synonym_terms:
+            for synonym_str in synonym_term.terms:
+                generated_synonym_strings = self.call(synonym_str)
+                if generated_synonym_strings:
+                    new_terms: Set[str] = set()
+                    for generated_syn in generated_synonym_strings:
+                        if generated_syn in existing_terms:
+                            logger.debug(
+                                f"generated synonym '{generated_syn}' matches existing synonym {synonym_term} "
+                            )
+                        elif generated_syn in new_terms:
+                            logger.debug(
+                                f"generated synonym '{generated_syn}' matches another generated synonym {synonym_term} "
+                            )
+                        else:
+                            new_terms.add(generated_syn)
+                    if new_terms:
+                        if synonym_term.original_term is not None:
+                            orig_term = synonym_term.original_term
+                        else:
+                            orig_term = synonym_str
+                        result.add(
+                            dataclasses.replace(
+                                synonym_term,
+                                original_term=orig_term,
+                                terms=frozenset(new_terms),
+                                aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
+                            )
                         )
-                    else:
-                        new_terms.add(generated_syn)
-                if new_terms:
-
-                    result.add(
-                        dataclasses.replace(
-                            synonym,
-                            terms=frozenset(new_terms),
-                            aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
-                        )
-                    )
 
         return result
 
 
 class CombinatorialSynonymGenerator:
     def __init__(self, synonym_generators: Iterable[SynonymGenerator]):
         self.synonym_generators: Set[SynonymGenerator] = set(synonym_generators)
 
     def __call__(self, synonyms: Set[SynonymTerm]) -> Set[SynonymTerm]:
         """
-        :meta public:
-
-        for every permutation of modifiers, generate a list of syns, then aggregate at the end
+        For every permutation of modifiers, generate a list of syns, then aggregate at the end
 
         :param synonyms: Set[SynonymTerm] to generate from
         :return: Set[SynonymTerm] of generated synonyms. Note, the field values of the generated synonyms will
             be the same as the seed synonym, apart from SynonymTerm.terms, which contains the generated synonyms
         """
         synonym_gen_permutations = itertools.permutations(self.synonym_generators)
         results = set()
@@ -90,87 +93,77 @@
 class SeparatorExpansion(SynonymGenerator):
     def __init__(self, spacy_pipeline: spacy.Language):
         self.all_stopwords = spacy_pipeline.Defaults.stop_words
         self.end_expression_brackets = r"(.*)\((.*)\)$"
         self.mid_expression_brackets = r"(.*)\(.*\)(.*)"
         self.excluded_parenthesis = ["", "non-protein coding"]
 
-    def call(self, synonym: SynonymTerm) -> Optional[SynonymTerm]:
+    def call(self, synonym_str: str) -> Optional[Set[str]]:
         bracket_results = set()
         all_group_results = set()
-        for text in synonym.terms:
-            if "(" in text and ")" in text:
-                # expand end expression brackets
-                matches = re.match(self.end_expression_brackets, text)
+        if "(" in synonym_str and ")" in synonym_str:
+            # expand end expression brackets
+            matches = re.match(self.end_expression_brackets, synonym_str)
+            if matches is not None:
+                all_groups_no_brackets = []
+                for group in matches.groups():
+                    if (
+                        group not in self.excluded_parenthesis
+                        and group.lower() not in self.all_stopwords
+                    ):
+                        bracket_results.add(group.strip())
+                        all_groups_no_brackets.append(group)
+                all_group_results.add("".join(all_groups_no_brackets))
+            else:
+                # remove mid expression  brackets
+                matches = re.match(self.mid_expression_brackets, synonym_str)
                 if matches is not None:
                     all_groups_no_brackets = []
                     for group in matches.groups():
-                        if (
-                            group not in self.excluded_parenthesis
-                            and group.lower() not in self.all_stopwords
-                        ):
-                            bracket_results.add(group.strip())
-                            all_groups_no_brackets.append(group)
-                    all_group_results.add("".join(all_groups_no_brackets))
-                else:
-                    # remove mid expression  brackets
-                    matches = re.match(self.mid_expression_brackets, text)
-                    if matches is not None:
-                        all_groups_no_brackets = []
-                        for group in matches.groups():
-                            all_groups_no_brackets.append(group.strip())
-                        all_group_results.add(" ".join(all_groups_no_brackets))
-
-            # expand slashes
-            for x in list(bracket_results):
-                if "/" in x:
-                    splits = x.split("/")
-                    for split in splits:
-                        bracket_results.add(split.strip())
-                if "," in x:
-                    splits = x.split(",")
-                    for split in splits:
-                        bracket_results.add(split.strip())
-            bracket_results.update(all_group_results)
+                        all_groups_no_brackets.append(group.strip())
+                    all_group_results.add(" ".join(all_groups_no_brackets))
+
+        # expand slashes
+        for x in list(bracket_results):
+            if "/" in x:
+                splits = x.split("/")
+                for split in splits:
+                    bracket_results.add(split.strip())
+            if "," in x:
+                splits = x.split(",")
+                for split in splits:
+                    bracket_results.add(split.strip())
+        bracket_results.update(all_group_results)
         if len(bracket_results) > 0:
-            return dataclasses.replace(
-                synonym,
-                terms=frozenset(bracket_results),
-                aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
-            )
+            return bracket_results
         else:
             return None
 
 
 class StopWordRemover(SynonymGenerator):
     """
     remove stopwords from a string
     """
 
     all_stopwords = {"of", "and", "in", "to", "with", "caused", "involved", "by", "the"}
 
     @classmethod
-    def call(cls, synonym: SynonymTerm) -> Optional[SynonymTerm]:
+    def call(cls, synonym_str: str) -> Optional[Set[str]]:
         new_terms = set()
-        for text in synonym.terms:
-            lst = []
-            detected = False
-            for token in text.split():
-                if token.lower() in cls.all_stopwords:
-                    detected = True
-                else:
-                    lst.append(token)
-            if detected:
-                new_terms.add(" ".join(lst))
+        lst = []
+        detected = False
+        for token in synonym_str.split():
+            if token.lower() in cls.all_stopwords:
+                detected = True
+            else:
+                lst.append(token)
+        if detected:
+            new_terms.add(" ".join(lst))
         if new_terms:
-            return dataclasses.replace(
-                synonym,
-                terms=frozenset(new_terms),
-                aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
-            )
+            return new_terms
         else:
             return None
 
 
 class GreekSymbolSubstitution:
 
     ALL_SUBS: Dict[str, Set[str]] = defaultdict(set)
@@ -192,129 +185,150 @@
             ALL_SUBS[greek_letter].add(lower_greek_letter)
 
     # we don't want this to have the semantics of a defaultdict for missing lookups
     ALL_SUBS = dict(ALL_SUBS)
 
 
 class StringReplacement(SynonymGenerator):
+    GREEK_VARIANT_PREFIX_SUFFIX = DASHES.union(set(" "))
+
     def __init__(
         self,
         replacement_dict: Optional[Dict[str, List[str]]] = None,
         digit_aware_replacement_dict: Optional[Dict[str, List[str]]] = None,
         include_greek: bool = True,
     ):
         self.include_greek = include_greek
         self.replacement_dict = replacement_dict
         self.digit_aware_replacement_dict = digit_aware_replacement_dict
 
-    def call(self, synonym: SynonymTerm) -> Optional[SynonymTerm]:
+    def call(self, synonym_str: str) -> Optional[Set[str]]:
         results = set()
-        for text in synonym.terms:
-            if self.replacement_dict:
-                for to_replace, replacement_list in self.replacement_dict.items():
-                    if to_replace in text:
-                        for replace_with in replacement_list:
-                            results.add(text.replace(to_replace, replace_with).strip())
-            if self.digit_aware_replacement_dict:
-                for to_replace, replacement_list in self.digit_aware_replacement_dict.items():
-                    matches = set(re.findall(to_replace + r"[0-9]+", text))
-                    for match in matches:
-                        number = match.split(to_replace)[1]
-                        for sub_in in replacement_list:
-                            new_str = text.replace(match, f"{sub_in}{number}").strip()
-                            results.add(new_str)
-
-            if self.include_greek:
-                # only strip text once initially - the greek character replacement
-                # will not introduce leading or trailing whitespace unlike the other
-                # replacements above
-                stripped_text = text.strip()
-                strings_to_substitute = {stripped_text}
-                for to_replace, replacement_set in GreekSymbolSubstitution.ALL_SUBS.items():
-                    # if it's in the original text it should be in all previous substitutions, no
-                    # need to check all of them
-                    if to_replace in text:
-                        # necessary so we don't modify strings_to_substitute while looping over it,
-                        # which throws an error
-                        outputs_this_step = set()
-                        for string_to_subsitute in strings_to_substitute:
-                            for replacement in replacement_set:
-                                single_unique_letter_substituted = string_to_subsitute.replace(
-                                    to_replace, replacement
-                                )
-                                outputs_this_step.add(single_unique_letter_substituted)
-                                results.add(single_unique_letter_substituted)
-                        strings_to_substitute.update(outputs_this_step)
+        if self.replacement_dict:
+            for to_replace, replacement_list in self.replacement_dict.items():
+                if to_replace in synonym_str:
+                    for replace_with in replacement_list:
+                        results.add(synonym_str.replace(to_replace, replace_with).strip())
+        if self.digit_aware_replacement_dict:
+            for to_replace, replacement_list in self.digit_aware_replacement_dict.items():
+                matches = set(re.findall(to_replace + r"[0-9]+", synonym_str))
+                for match in matches:
+                    number = match.split(to_replace)[1]
+                    for sub_in in replacement_list:
+                        new_str = synonym_str.replace(match, f"{sub_in}{number}").strip()
+                        results.add(new_str)
+
+        if self.include_greek:
+            self._generate_greek_subs(results, synonym_str)
 
         if len(results) > 0:
-            return dataclasses.replace(
-                synonym,
-                terms=frozenset(results),
-                aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
-            )
+            return results
         else:
             return None
 
+    def _generate_greek_subs(self, results, synonym_str):
+        # only strip text once initially - the greek character replacement
+        # will not introduce leading or trailing whitespace unlike the other
+        # replacements above
+        stripped_text = synonym_str.strip()
+        strings_to_substitute = {stripped_text}
+        for candidate, replacement_set in GreekSymbolSubstitution.ALL_SUBS.items():
+            # if it's in the original text it should be in all previous substitutions, no
+            # need to check all of them
+            for fix in self.GREEK_VARIANT_PREFIX_SUFFIX:
+                prefix = False
+                suffix = False
+                # necessary so we don't modify strings_to_substitute while looping over it,
+                # which throws an error
+                outputs_this_step = set()
+                if f"{fix}{candidate}" in synonym_str:
+                    suffix = True
+                if f"{candidate}{fix}" in synonym_str:
+                    prefix = True
+
+                for string_to_substitute in strings_to_substitute:
+                    for replacement in replacement_set:
+                        if prefix:
+                            single_unique_letter_substituted = string_to_substitute.replace(
+                                f"{candidate}{fix}", f"{replacement}{fix}"
+                            )
+                            outputs_this_step.add(single_unique_letter_substituted)
+                            results.add(single_unique_letter_substituted)
+                        if suffix:
+                            single_unique_letter_substituted = string_to_substitute.replace(
+                                f"{fix}{candidate}", f"{fix}{replacement}"
+                            )
+                            outputs_this_step.add(single_unique_letter_substituted)
+                            results.add(single_unique_letter_substituted)
+                strings_to_substitute.update(outputs_this_step)
+
 
 class SuffixReplacement(SynonymGenerator):
     """Interchange all suffixes within a provided set to produce new synonyms.
 
     Note, this is expected to be noisy, and for most of the generated synonyms not to be valid
     words. This class is present as a generation step for high recall, with curation of synonyms
-    expected later (see :ref:`curating_for_explosion`).
+    expected later.
 
     In particular, note that this also doesn't check for the longest matching suffix - e.g. for a
     synonym 'anaemia' and the suffixes 'ia', 'a' and 'ic', the new synonyms 'anaemic' and
     'amaemiic' will both be generated.
     """
 
     def __init__(self, suffixes: Iterable[str]):
         self.suffixes = set(suffixes)
 
-    def call(self, synonym: SynonymTerm) -> Optional[SynonymTerm]:
+    def call(self, synonym_str: str) -> Optional[Set[str]]:
         new_terms: Set[str] = set()
-        for term in synonym.terms:
-            for suffix in self.suffixes:
-                # Note that this will trigger twice for 'ia' since 'a' is also present.
-                # We expect this to be noisy, and then curate from this.
-                if term.endswith(suffix):
-                    term_without_suffix = term.removesuffix(suffix)
-                    new_terms.update(
-                        term_without_suffix + new_suffix
-                        for new_suffix in self.suffixes
-                        if new_suffix is not suffix
-                    )
+        for suffix in self.suffixes:
+            # Note that this will trigger twice for 'ia' since 'a' is also present.
+            # We expect this to be noisy, and then curate from this.
+            if synonym_str.endswith(suffix):
+                term_without_suffix = synonym_str.removesuffix(suffix)
+                new_terms.update(
+                    term_without_suffix + new_suffix
+                    for new_suffix in self.suffixes
+                    if new_suffix is not suffix
+                )
 
         if new_terms:
-            return dataclasses.replace(
-                synonym,
-                terms=frozenset(new_terms),
-                aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
-            )
+            return new_terms
         else:
             return None
 
 
 class SpellingVariationReplacement(SynonymGenerator):
     """Generate additional synonyms using a mapping of (known) synonyms to a list of variations."""
 
     def __init__(self, input_path: PathLike):
         with open(input_path, mode="r", encoding="utf-8") as inf:
             raw_variation_mapping: Dict[str, List[str]] = json.load(inf)
 
         # lowercase for case-insensitive comparison
         self.variation_mapping = {k.lower(): val for k, val in raw_variation_mapping.items()}
 
-    def call(self, synonym: SynonymTerm) -> Optional[SynonymTerm]:
+    def call(self, synonym_str: str) -> Optional[Set[str]]:
         new_terms = set()
-        for term in synonym.terms:
-            variations = self.variation_mapping.get(term.lower())
-            if variations is not None:
-                new_terms.update(variations)
+        variations = self.variation_mapping.get(synonym_str.lower())
+        if variations is not None:
+            new_terms.update(variations)
         if new_terms:
-            return dataclasses.replace(
-                synonym,
-                terms=frozenset(new_terms),
-                aggregated_by=EquivalentIdAggregationStrategy.CUSTOM,
-            )
+            return new_terms
         else:
             return None
+
+
+class NgramHyphenation(SynonymGenerator):
+    """Generate hyphenated variants of ngrams."""
+
+    def __init__(self, ngram: int = 2):
+        self.ngram = ngram
+
+    def call(self, synonym_str: str) -> Optional[Set[str]]:
+        parts = synonym_str.split()
+        if len(parts) != self.ngram:
+            return None
+        else:
+            new_terms = set()
+            for hyphen in DASHES:
+                new_terms.add(hyphen.join(parts))
+        return new_terms
```

### Comparing `kazu-0.1.0/kazu/pipeline/pipeline.py` & `kazu-1.0.0/kazu/steps/linking/post_processing/disambiguation/strategies.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,239 +1,267 @@
+import functools
 import logging
-import os.path
-import time
-import uuid
-from pathlib import Path
-from typing import List, Dict, Optional, Protocol
-
-import psutil
-from hydra.utils import instantiate
-from omegaconf import DictConfig
-
-from kazu.data.data import Document, PROCESSING_EXCEPTION
-from kazu.steps import Step
-from datetime import datetime
+from abc import ABC, abstractmethod
+from collections import defaultdict
+from os import getenv
+from typing import Tuple, Optional, Set, Dict, Iterable, FrozenSet
+
+import numpy as np
+
+from kazu.data.data import (
+    Document,
+    EquivalentIdSet,
+    EquivalentIdAggregationStrategy,
+    DisambiguationConfidence,
+)
+from kazu.database.in_memory_db import (
+    MetadataDatabase,
+    SynonymDatabase,
+    NormalisedSynonymStr,
+)
+from kazu.steps.linking.post_processing.disambiguation.context_scoring import TfIdfScorer
 
 logger = logging.getLogger(__name__)
 
 
-def load_steps_and_log_memory_usage(cfg: DictConfig) -> List[Step]:
+class DisambiguationStrategy(ABC):
     """
-    Loads steps based on the pipeline config, and log the memory increase after loading each step.
+    The job of a DisambiguationStrategy is to filter a Set of :class:`.EquivalentIdSet` into a
+    (hopefully) smaller set.
 
-    Note that you can instantiate the pipeline directly from the config in a way that gives the
-    same results, but this is useful for monitoring/debugging high memory usage.
+    A :meth:`prepare` method is available, which can be cached in the event of any duplicated
+    preprocessing work that may be required (see :class:`.StrategyRunner` for the complexities of
+    how MappingStrategy and DisambiguationStrategy are coordinated).
+    """
 
-    :param cfg: An OmegaConf config object for the kazu :class:`.Pipeline`\\ .
-        Normally created from hydra config files.
-    :return: The instantiated steps from the pipeline config
-    """
-    steps = []
-    for step_cfg in cfg.Pipeline.steps:
-        prev_memory = psutil.Process(os.getpid()).memory_info().rss / 1024**2
-        new_step = instantiate(step_cfg)
-        steps.append(new_step)
-        new_memory = psutil.Process(os.getpid()).memory_info().rss / 1024**2
-        mem_increase = ((new_memory - prev_memory) / prev_memory) * 100
+    def __init__(self, confidence: DisambiguationConfidence):
+        """
 
-        logger.info(
-            f"loaded {new_step.namespace()}. Memory usage now {round(new_memory,2)} MB. Increased by {round(new_memory-prev_memory,2)}MB, {round(mem_increase,2)}%"
-        )
+        :param confidence: the level of confidence that should be assigned to this strategy. This is simply a label
+            for human users, and has no bearing on the actual algorithm.
+        """
+        self.confidence = confidence
 
-    return steps
+    @abstractmethod
+    def prepare(self, document: Document):
+        """
+        perform any preprocessing required
 
+        :param document:
+        :return:
+        """
+        pass
+
+    @abstractmethod
+    def disambiguate(
+        self, id_sets: Set[EquivalentIdSet], document: Document, parser_name: str
+    ) -> Set[EquivalentIdSet]:
+        """
+        subset a set of :class:`.EquivalentIdSet`\\ .
 
-def calc_doc_size(doc: Document):
-    return sum(len(section.text) for section in doc.sections)
+        :param id_sets:
+        :param document:
+        :param parser_name:
+        :return:
+        """
+        pass
 
+    def __call__(
+        self, id_sets: Set[EquivalentIdSet], document: Document, parser_name: str
+    ) -> Set[EquivalentIdSet]:
+        self.prepare(document)
+        return self.disambiguate(id_sets, document, parser_name)
 
-def batch_metrics(docs: List[Document]):
-    lengths = []
-    ent_count = []
-    for doc in docs:
-        lengths.append(calc_doc_size(doc))
-        ent_count.append(len(doc.get_entities()))
-    return {
-        "max_length": max(lengths),
-        "mean_length": float(sum(lengths)) / float(len(docs)),
-        "max_ents": max(ent_count),
-        "mean_ents": float(sum(ent_count)) / float(len(ent_count)),
-    }
 
+class DefinedElsewhereInDocumentDisambiguationStrategy(DisambiguationStrategy):
+    """
+    1. look for entities on the document that have mappings
+    2. see if any of these mappings correspond to any ids in the :class:`.EquivalentIdSet` on each
+       hit
+    """
 
-class FailedDocsHandler(Protocol):
-    """Handle failed docs."""
+    def __init__(self, confidence: DisambiguationConfidence):
+        super().__init__(confidence)
+        self.mapped_ids: Set[Tuple[str, str, str]] = set()
 
-    def __call__(self, step_docs_map: Dict[str, List[Document]]):
+    def prepare(self, document: Document):
         """
-        :meta public:
+        note, this method can't be cached, as the state of the document may change between executions
 
-        :param step_docs_map: a dict of step namespace and the docs that failed for it
+        :param document:
         :return:
         """
-        raise NotImplementedError()
+        self.mapped_ids = set()
+        entities = document.get_entities()
+        self.mapped_ids.update(
+            (
+                mapping.parser_name,
+                mapping.source,
+                mapping.idx,
+            )
+            for ent in entities
+            for mapping in ent.mappings
+        )
 
+    def disambiguate(
+        self, id_sets: Set[EquivalentIdSet], document: Document, parser_name: str
+    ) -> Set[EquivalentIdSet]:
+        found_id_sets = set()
+        for id_set in id_sets:
+            for idx, source in id_set.ids_and_source:
+                if (
+                    parser_name,
+                    source,
+                    idx,
+                ) in self.mapped_ids:
+                    found_id_sets.add(id_set)
+                    break
+        return found_id_sets
 
-class FailedDocsLogHandler(FailedDocsHandler):
-    """Log failed docs as warnings."""
 
-    def __call__(self, step_docs_map: Dict[str, List[Document]]):
-        for step_namespace, docs in step_docs_map.items():
-            for doc in docs:
-                error_message = doc.metadata.get(PROCESSING_EXCEPTION, None)
-                if error_message is not None:
-                    logger.warning(
-                        f"processing failed for step {step_namespace}, doc: {doc.idx}, {error_message} "
-                    )
-                else:
-                    logger.warning(
-                        f"processing failed for step {step_namespace}, doc: {doc.idx}, No error mesasge found in doc metadata "
-                    )
-
-
-class FailedDocsFileHandler(FailedDocsHandler):
-    """Log failed docs to a directory along with the relevant exception."""
-
-    def __init__(self, log_dir: Path):
-        self.log_dir = log_dir
-
-    def __call__(self, step_docs_map: Dict[str, List[Document]]):
-        for step_namespace, docs in step_docs_map.items():
-            step_logging_dir = os.path.join(self.log_dir, step_namespace)
-            if not os.path.exists(step_logging_dir):
-                os.makedirs(step_logging_dir, exist_ok=True)
-
-            for doc in docs:
-                serialisable_doc = doc.json()
-                doc_id = doc.idx
-                doc_path = os.path.join(step_logging_dir, doc_id + ".json")
-                doc_error_path = os.path.join(step_logging_dir, doc_id + "_error.txt")
-                with open(doc_path, "w") as f:
-                    f.write(serialisable_doc)
-                with open(doc_error_path, "w") as f:
-                    error_message = doc.metadata.get(PROCESSING_EXCEPTION)
-                    if error_message is not None:
-                        f.write(error_message)
-                    else:
-                        logger.warning(
-                            f"No error message found for doc: {doc}. Cannot write exception to {doc_error_path}"
-                        )
+class TfIdfDisambiguationStrategy(DisambiguationStrategy):
+    """
+    1. retrieve all synonyms associated with a :class:`.EquivalentIdSet`, filter out ambiguous ones
+       and build a query matrix with the unambiguous ones.
+    2. retrieve a list of all detected entity strings from the document, regardless of source and
+       build a document representation matrix of these.
+    3. perform TFIDF on the query vs document, and sort according to most likely synonym hit from 1.
+    4. if the score is above the minimum threshold, create a mapping.
 
+    """
+
+    CONTEXT_SCORE = "context_score"
 
-class Pipeline:
     def __init__(
         self,
-        steps: List[Step],
-        failure_handler: Optional[List[FailedDocsHandler]] = None,
-        profile_steps_dir: Optional[str] = None,
-        skip_doc_len: Optional[int] = 200000,
+        confidence: DisambiguationConfidence,
+        scorer: TfIdfScorer,
+        context_threshold: float = 0.7,
+        relevant_aggregation_strategies: Optional[Iterable[EquivalentIdAggregationStrategy]] = None,
     ):
         """
-        A basic pipeline, used to help run a series of steps
 
-        :param steps: list of steps to run
-        :param failure_handler: optional list of handlers to process failed docs
-        :param profile_steps_dir: profile throughout of each step with tensorboard. path to log dir
-        """
-        self.skip_doc_len = skip_doc_len
-        self.failure_handlers = failure_handler
-        self.steps = steps
-        # documents that failed to process - a dict of [<step namespace>:List[failed docs]]
-        self.failed_docs: Dict[str, List[Document]] = {}
-        # performance tracking
-        self.init_time = datetime.now().strftime("%m_%d_%Y_%H_%M")
-        logger.info(f"pipeline initialised: {self.init_time}")
-        self.profile_steps_dir = profile_steps_dir
-        if profile_steps_dir:
-            try:
-                from torch.utils.tensorboard import SummaryWriter
-            except ImportError as e:
-                raise ImportError(
-                    "Profiling the pipeline requires tensorboard to be installed.\n"
-                    "Tensorboard is included in Kazu's dev dependencies, so this will work"
-                    " with 'pip install kazu[dev]', but you could also just do 'pip install"
-                    " tensorboard' if you don't want the other dev dependencies."
-                ) from e
-
-            idx_this_process = uuid.uuid1().hex
-            dir_and_time = f"{profile_steps_dir}_{self.init_time}_{idx_this_process}"
-            logger.info(f"profiling configured. log dir is {dir_and_time}")
-            self.summary_writer: Optional[SummaryWriter] = SummaryWriter(log_dir=dir_and_time)
-            self.call_count = 0
+        :param scorer: handles scoring of contexts
+        :param context_threshold: only consider terms above this search threshold
+        :param relevant_aggregation_strategies: Only consider these strategies when selecting synonyms from the
+            synonym database, when building a representation. If none, all strategies will be considered
+        """
+        super().__init__(confidence)
+        self.context_threshold = context_threshold
+        if relevant_aggregation_strategies is None:
+            self.relevant_aggregation_strategies = {EquivalentIdAggregationStrategy.UNAMBIGUOUS}
         else:
-            logger.info("profiling not configured")
-            self.summary_writer = None
+            self.relevant_aggregation_strategies = set(relevant_aggregation_strategies)
+        self.synonym_db = SynonymDatabase()
+        self.scorer = scorer
+        self.parser_name_to_doc_representation: Dict[str, np.ndarray] = {}
 
-    def prefilter_docs(self, docs: List[Document]):
-        docs_to_process = []
-        for doc in docs:
-            doc_size = calc_doc_size(doc)
-            if doc_size >= self.skip_doc_len:
-                doc.metadata[
-                    PROCESSING_EXCEPTION
-                ] = f"document too long: {doc_size}. max:{self.skip_doc_len}"
-                logger.warning(f"skipping doc: {doc.idx}: reason: too long")
-            else:
-                docs_to_process.append(doc)
-        return docs_to_process
-
-    def __call__(self, docs: List[Document]) -> List[Document]:
-        """
-        :meta public:
-
-        run the pipeline
-
-        :param docs: Docs to process
-        :return: processed docs
-        """
-        docs_to_process = self.prefilter_docs(docs)
-        step_times = {}
-        batch_start = time.time()
-        for step in self.steps:
-            start = time.time()
-            _processed_docs, failed_docs = step(docs_to_process)
-            step_times[step.namespace()] = round(time.time() - start, 4)
-            self.update_failed_docs(step, failed_docs)
-        batch_time = round(time.time() - batch_start, 4)
-        if self.profile_steps_dir:
-            self.profile(step_times, batch_time, batch_metrics(docs))
-        self.reset()
-
-        return docs
-
-    def profile(self, step_times: Dict, batch_time: float, batch_metrics_dict: Dict):
-        if self.summary_writer is not None:
-            self.summary_writer.add_scalars(
-                main_tag="batch_metrics",
-                tag_scalar_dict=batch_metrics_dict,
-                global_step=self.call_count,
-            )
-            self.summary_writer.add_scalars(
-                main_tag="all_steps", tag_scalar_dict=step_times, global_step=self.call_count
-            )
-            self.summary_writer.add_scalars(
-                main_tag="batch_time",
-                tag_scalar_dict={"batch": batch_time},
-                global_step=self.call_count,
-            )
-            self.summary_writer.add_scalars(
-                main_tag="memory",
-                tag_scalar_dict={"MB": psutil.Process(os.getpid()).memory_info().rss / 1024**2},
-                global_step=self.call_count,
-            )
-            for step_name, step_time in step_times.items():
-                self.summary_writer.add_scalars(
-                    main_tag=step_name,
-                    tag_scalar_dict={"time": step_time},
-                    global_step=self.call_count,
+    @functools.lru_cache(maxsize=int(getenv("KAZU_TFIDF_DISAMBIGUATION_DOCUMENT_CACHE_SIZE", 1)))
+    def prepare(self, document: Document):
+        """
+        build document representations by parser names here, and store in a dict. This method is cached so
+        we don't need to call it multiple times per document
+
+        :param document:
+        :return:
+        """
+        parser_names = frozenset(
+            term.parser_name
+            for ent in document.get_entities()
+            for term in ent.syn_term_to_synonym_terms
+        )
+        self.parser_name_to_doc_representation = self.cacheable_build_document_representation(
+            scorer=self.scorer, doc=document, parsers=parser_names
+        )
+
+    @staticmethod
+    @functools.lru_cache(maxsize=int(getenv("KAZU_TFIDF_DISAMBIGUATION_CACHE_SIZE", 20)))
+    def cacheable_build_document_representation(
+        scorer: TfIdfScorer, doc: Document, parsers: FrozenSet[str]
+    ) -> Dict[str, np.ndarray]:
+        """
+        static cached method, so we don't need to recalculate document representation between different instances
+        of this class.
+
+        :param scorer:
+        :param doc:
+        :param parsers: technically this only has to be a hashable iterable of string - but it should also be
+            unique otherwise duplicate work will be done and thrown away, so pragmatically a frozenset makes sense.
+        :return:
+        """
+        strings = " ".join(x.match_norm for x in doc.get_entities())
+        res = {}
+        for parser in parsers:
+            vectorizer = scorer.parser_to_vectorizer[parser]
+            res[parser] = vectorizer.transform([strings])
+        return res
+
+    def build_id_set_representation(
+        self,
+        parser_name: str,
+        id_sets: Set[EquivalentIdSet],
+    ) -> Dict[NormalisedSynonymStr, Set[EquivalentIdSet]]:
+        result = defaultdict(set)
+        for id_set in id_sets:
+            for idx in id_set.ids:
+
+                syns_this_id = self.synonym_db.get_syns_for_id(
+                    parser_name,
+                    idx,
+                    self.relevant_aggregation_strategies,
+                )
+                for syn in syns_this_id:
+                    result[syn].add(id_set)
+        return result
+
+    def disambiguate(
+        self, id_sets: Set[EquivalentIdSet], document: Document, parser_name: str
+    ) -> Set[EquivalentIdSet]:
+        if parser_name not in self.scorer.parser_to_vectorizer:
+            return set()
+
+        document_query_matrix = self.parser_name_to_doc_representation[parser_name]
+        id_set_representation = self.build_id_set_representation(parser_name, id_sets)
+        if len(id_set_representation) == 0:
+            return set()
+        else:
+            indexed_non_ambiguous_syns = list(id_set_representation.keys())
+            for best_syn, score in self.scorer(
+                strings=indexed_non_ambiguous_syns,
+                matrix=document_query_matrix,
+                parser=parser_name,
+            ):
+                if score >= self.context_threshold and len(id_set_representation[best_syn]) == 1:
+                    return id_set_representation[best_syn]
+            return set()
+
+
+class AnnotationLevelDisambiguationStrategy(DisambiguationStrategy):
+    """
+    certain entities are often mentioned by some colloquial name, even if it's technically incorrect. In these cases,
+    we may have an annotation_score field in the metadata_db, as a proxy of how widely studied the entity is. We
+    use this annotation score as a proxy for 'given a random mention of the entity, how likely is it that the
+    author is referring to instance x vs instance y'. Naturally, this is a pretty unsophisticated disambiguation
+    strategy, so should generally only be used as a last resort!
+    """
+
+    def prepare(self, document: Document):
+        pass
+
+    def disambiguate(
+        self, id_sets: Set[EquivalentIdSet], document: Document, parser_name: str
+    ) -> Set[EquivalentIdSet]:
+        best_score = 0
+        best_equiv_id_sets = set()
+
+        for id_set in id_sets:
+            for idx in id_set.ids:
+                score = int(
+                    MetadataDatabase().get_by_idx(parser_name, idx).get("annotation_score", 0)
                 )
-            self.call_count += 1
+                if score > best_score:
+                    best_score = score
+                    best_equiv_id_sets = {id_set}
+                elif score == best_score:
+                    best_equiv_id_sets.add(id_set)
 
-    def update_failed_docs(self, step: Step, failed_docs: List[Document]):
-        if self.failure_handlers is not None:
-            self.failed_docs[step.namespace()] = failed_docs
-
-    def reset(self):
-        if self.failure_handlers is not None:
-            for handler in self.failure_handlers:
-                handler(self.failed_docs)
-        self.failed_docs = {}
+        return best_equiv_id_sets
```

### Comparing `kazu-0.1.0/kazu/steps/__init__.py` & `kazu-1.0.0/kazu/steps/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from kazu.steps.step import Step, document_iterating_step, document_batch_step
 from kazu.steps.document_post_processing.abbreviation_finder import AbbreviationFinderStep
 from kazu.steps.joint_ner_and_linking.explosion import ExplosionStringMatchingStep
 from kazu.steps.linking.dictionary import DictionaryEntityLinkingStep
-from kazu.steps.linking.sapbert import SapBertForEntityLinkingStep
-from kazu.steps.linking.mapping_step import MappingStep
+from kazu.steps.linking.post_processing.mapping_step import MappingStep
 from kazu.steps.ner.hf_token_classification import TransformersModelForTokenClassificationNerStep
 from kazu.steps.ner.seth import SethStep
 from kazu.steps.ner.spacy_ner import SpacyNerStep
 from kazu.steps.other.cleanup import CleanupStep
 from kazu.steps.other.merge_overlapping_ents import MergeOverlappingEntsStep
 from kazu.steps.other.stanza import StanzaStep
```

### Comparing `kazu-0.1.0/kazu/steps/step.py` & `kazu-1.0.0/kazu/steps/step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import wraps
 import traceback
-from typing import Any, Callable, List, Protocol, Tuple, TypeVar
+from typing import Any, Callable, List, Protocol, Tuple, TypeVar, Iterable
 
 from kazu.data.data import Document, PROCESSING_EXCEPTION
+from kazu.ontology_preprocessing.base import OntologyParser
 
 
 class Step(Protocol):
     @classmethod
     def namespace(cls) -> str:
         """Metadata to name/describe the step, used in various places.
 
@@ -16,51 +17,70 @@
         # and @property together in most versions of python (you could in 3.9 and 3.10), and
         # it being a classmethod is quite useful.
         return cls.__name__
 
     def __call__(self, docs: List[Document]) -> Tuple[List[Document], List[Document]]:
         """Process documents and respond with processed and failed documents.
 
-        Note that many steps will be decorated by :func:`document_iterating_step` or
-        :func:`document_batch_step` which will modify the 'original' ``__call__`` function
-        signature to match the expected signature for a step, as the decorators handle the
-        exception/failed documents logic for you.
+        Note that many steps will be decorated by :func:`~.kazu.steps.step.document_iterating_step`
+        or :func:`~.kazu.steps.step.document_batch_step` which will modify the 'original'
+        ``__call__`` function signature to match the expected signature for a step, as the
+        decorators handle the exception/failed documents logic for you.
 
         :param docs:
         :return: The first element is all the provided docs (now modified by the processing), the
             second is the docs that failed to (fully) process correctly.
         """
-        raise NotImplementedError()
+        raise NotImplementedError
+
+
+class ParserDependentStep(Step):
+    """A step that depends on ontology parsers in any form.
+
+    Steps that need information from parsers should subclass this class, in order
+    for the internal databases to be correctly populated. Generally, these will be
+    steps that have anything to do with Entity Linking.
+    """
+
+    def __init__(self, parsers: Iterable[OntologyParser]):
+        """
+
+        :param parsers: parsers that this step requires
+        """
+        for parser in parsers:
+            parser.populate_databases(force=False)
 
 
 Self = TypeVar("Self")
-"""A TypeVar for the type of the class whose method is decorated with :func:`document_iterating_step`
-or :func:`document_batch_step`\\ ."""
+"""A TypeVar for the type of the class whose method is decorated with
+:func:`~.kazu.steps.step.document_iterating_step` or
+:func:`~.kazu.steps.step.document_batch_step`\\ ."""
 
 
 def document_iterating_step(
     per_doc_callable: Callable[[Self, Document], Any]
 ) -> Callable[[Self, List[Document]], Tuple[List[Document], List[Document]]]:
     """Handle a list of :class:`~kazu.data.data.Document`\\ s and add error handling.
 
     Use this to decorate a method that processes a single :class:`~kazu.data.data.Document`\\ .
     The resulting method will then iterate over a list of
     :class:`~kazu.data.data.Document`\\ s, calling the decorated function for each
     :class:`~kazu.data.data.Document`\\ . Errors are handled automatically and added to the
     ``PROCESSING_EXCEPTION`` metadata of documents, with failed docs returned as the second element
-    of the return value, as expected of the ``__call__`` method of a :class:`Step`\\ .
+    of the return value, as expected by :meth:`Step.__call__`\\ .
 
     Generally speaking, it will save effort and repetition to decorate a :class:`Step` with either
-    :func:`document_iterating_step` or :func:`document_batch_step`\\, rather than implementing the
-    error handling in the :class:`Step` itself.
-
-    Normally, :func:`document_iterating_step` would be used in preference to
-    :func:`document_batch_step`\\, unless the method involves computation which is more efficient
-    when run in a batch, such as inference with a transformer-based Machine Learning model, or
-    using spacy's `pipe <https://spacy.io/api/language/#pipe>`_ method.
+    :func:`~.kazu.steps.step.document_iterating_step` or
+    :func:`~.kazu.steps.step.document_batch_step`\\, rather than implementing the error handling in
+    the :class:`Step` itself.
+
+    Normally, :func:`~.kazu.steps.step.document_iterating_step` would be used in preference to
+    :func:`~.kazu.steps.step.document_batch_step`\\, unless the method involves computation which
+    is more efficient when run in a batch, such as inference with a transformer-based Machine
+    Learning model, or using spacy's `pipe <https://spacy.io/api/language/#pipe>`_ method.
 
     Note that this will only work for a method of a class, rather than a standalone function,
     as it expects to have to pass through 'self' as a parameter.
 
     :param per_doc_callable: A function that processes a single document, that you want to use as
         the :literal:`__call__` method of a :class:`Step`\\ . This must do its work by mutating the
         input document: the return value is ignored.
@@ -83,26 +103,27 @@
 def document_batch_step(
     batch_doc_callable: Callable[[Self, List[Document]], Any]
 ) -> Callable[[Self, List[Document]], Tuple[List[Document], List[Document]]]:
     """Add error handling to a method that processes batches of :class:`~kazu.data.data.Document`\\ s.
 
     Use this to decorate a method that processes a batch of :class:`~kazu.data.data.Document`\\ s
     at a time. The resulting method will wrap a call to the decorated function with error handling
-    which will added exceptions to the ``PROCESSING_EXCEPTION`` metadata of documents. Failed documents
-    will be returned as the second element of the return value, as expected of the ``__call__``
-    method of a :class:`Step`\\ .
+    which will add exceptions to the ``PROCESSING_EXCEPTION`` metadata of documents. Failed
+    documents will be returned as the second element of the return value, as expected by
+    :meth:`Step.__call__`\\ .
 
     Generally speaking, it will save effort and repetition to decorate a :class:`Step` with either
-    :func:`document_iterating_step` or :func:`document_batch_step`\\, rather than implementing the
-    error handling in the :class:`Step` itself.
-
-    Normally, :func:`document_iterating_step` would be used in preference to
-    :func:`document_batch_step`\\, unless the method involves computation which is more efficient
-    when run in a batch, such as inference with a transformer-based Machine Learning model, or
-    using spacy's `pipe <https://spacy.io/api/language/#pipe>`_ method.
+    :func:`~.kazu.steps.step.document_iterating_step` or
+    :func:`~.kazu.steps.step.document_batch_step`\\, rather than implementing the error handling in
+    the :class:`Step` itself.
+
+    Normally, :func:`~.kazu.steps.step.document_iterating_step` would be used in preference to
+    :func:`~.kazu.steps.step.document_batch_step`\\, unless the method involves computation which
+    is more efficient when run in a batch, such as inference with a transformer-based Machine
+    Learning model, or using spacy's `pipe <https://spacy.io/api/language/#pipe>`_ method.
 
     Note that this will only work for a method of a class, rather than a standalone function,
     as it expects to have to pass through 'self' as a parameter.
 
     :param batch_doc_callable: A function that processes a batch of documents, that you want to use
         as the :literal:`__call__` method of a :class:`Step`. This must do its work by mutating the
         input documents: the return value is ignored.
```

### Comparing `kazu-0.1.0/kazu/steps/document_post_processing/abbreviation_finder.py` & `kazu-1.0.0/kazu/steps/document_post_processing/abbreviation_finder.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/steps/joint_ner_and_linking/explosion.py` & `kazu-1.0.0/kazu/steps/joint_ner_and_linking/explosion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 import logging
 from typing import Iterator, List, Tuple, Iterable, Dict, Set, cast
 
 import spacy
+from spacy.tokens import Span
+
 from kazu.data.data import (
     CharSpan,
     Document,
     Section,
     Entity,
     SynonymTermWithMetrics,
+    MentionConfidence,
 )
-from kazu.modelling.database.in_memory_db import SynonymDatabase
-from kazu.modelling.ontology_matching.ontology_matcher import OntologyMatcher
-from kazu.steps import Step, document_batch_step
-from kazu.utils.utils import PathLike
-from spacy.tokens import Span
+from kazu.database.in_memory_db import SynonymDatabase
+from kazu.ontology_matching import assemble_pipeline
+from kazu.ontology_matching.ontology_matcher import OntologyMatcher
+from kazu.ontology_preprocessing.base import OntologyParser
+from kazu.steps import document_batch_step
+from kazu.steps.step import ParserDependentStep
+from kazu.utils.utils import PathLike, as_path
 
 logger = logging.getLogger(__name__)
 
 
-class ExplosionStringMatchingStep(Step):
-    """
-    A wrapper for the explosion ontology-based entity matcher and linker.
-    """
+class ExplosionStringMatchingStep(ParserDependentStep):
+    """A wrapper for the explosion ontology-based entity matcher and linker."""
 
     def __init__(
         self,
+        parsers: Iterable[OntologyParser],
         path: PathLike,
         include_sentence_offsets: bool = True,
+        ignore_cache: bool = False,
     ):
         """
+
+
         :param path: path to spacy pipeline including Ontology Matcher.
         :param include_sentence_offsets: whether to add sentence offsets to the metadata.
+        :param ignore_cache: ignore cached version of spacy pipeline (if available) and rebuild
 
         """
+        super().__init__(parsers)
         self.include_sentence_offsets = include_sentence_offsets
-        self.path = path
+        self.path = as_path(path)
 
-        # TODO: config override for when how we map parser names to entity types has changed since the last pipeline build
-        # think about how this affects the OntologyMatcher's lookup of parser names in case they
-        # are not there in the new config.
-        self.spacy_pipeline = spacy.load(path)
+        if self.path.exists() and not ignore_cache:
+            logger.info("loading spacy pipeline from %s", str(path))
+            self.spacy_pipeline = spacy.load(path)
+        else:
+            logger.info(
+                "cached spacy pipeline not detected or ignore_cache=True. Creating it at %s. This may take some time",
+                str(self.path),
+            )
+            self.spacy_pipeline = assemble_pipeline.main(
+                output_dir=self.path, parsers=list(parsers)
+            )
         matcher = cast(OntologyMatcher, self.spacy_pipeline.get_pipe("ontology_matcher"))
         self.span_key = matcher.span_key
 
         self.synonym_db = SynonymDatabase()
 
     def extract_entity_data_from_spans(
         self, spans: Iterable[Span]
-    ) -> Iterator[Tuple[int, int, str, Dict[str, Set[Tuple[str, str]]]]]:
+    ) -> Iterator[Tuple[int, int, str, Dict[str, Set[Tuple[str, str, str]]]]]:
         for span in spans:
             yield span.start_char, span.end_char, span.text, span._.ontology_dict_
 
     @document_batch_step
     def __call__(self, docs: List[Document]) -> None:
         texts_and_sections = (
             (section.get_text(), section) for doc in docs for section in doc.sections
@@ -68,31 +84,35 @@
             spans = processed_text.spans[self.span_key]
             for (
                 start_char,
                 end_char,
                 text,
                 ontology_data,
             ) in self.extract_entity_data_from_spans(spans):
-                for entity_class, per_parser_term_norm_set in ontology_data.items():
 
+                for entity_class, per_parser_term_norm_set in ontology_data.items():
+                    confidences = set()
                     e = Entity.load_contiguous_entity(
                         start=start_char,
                         end=end_char,
                         match=text,
                         entity_class=entity_class,
                         namespace=self.namespace(),
                     )
-                    entities.append(e)
                     terms = []
-                    for parser_name, term_norm in per_parser_term_norm_set:
+                    for parser_name, term_norm, confidence in per_parser_term_norm_set:
+                        mention_confidence = MentionConfidence(int(confidence))
+                        confidences.add(mention_confidence)
                         term_with_metrics = SynonymTermWithMetrics.from_synonym_term(
                             self.synonym_db.get(parser_name, term_norm), exact_match=True
                         )
                         terms.append(term_with_metrics)
                     e.update_terms(terms)
+                    e.mention_confidence = max(confidences)
+                    entities.append(e)
 
             # add sentence offsets
             if self.include_sentence_offsets:
                 section.sentence_spans = (
                     CharSpan(sent.start_char, sent.end_char) for sent in processed_text.sents
                 )
```

### Comparing `kazu-0.1.0/kazu/steps/linking/dictionary.py` & `kazu-1.0.0/kazu/steps/linking/dictionary.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
-import traceback
-from typing import List, Tuple, Dict, Set, Optional
+from collections import defaultdict
+from typing import List, Set, Optional
 
-from kazu.data.data import Document, PROCESSING_EXCEPTION, SynonymTermWithMetrics
-from kazu.steps import Step
+from kazu.data.data import Document, SynonymTermWithMetrics
+from kazu.steps.step import Step, document_batch_step
 from kazu.utils.caching import EntityLinkingLookupCache
 from kazu.utils.grouping import sort_then_group
 from kazu.utils.link_index import DictionaryIndex
-from kazu.utils.utils import find_document_from_entity
 
 logger = logging.getLogger(__name__)
 
 
 class DictionaryEntityLinkingStep(Step):
-    """
-    Uses :class:`kazu.utils.link_index.DictionaryIndex` to match entities to ontologies.
+    """Uses :class:`kazu.utils.link_index.DictionaryIndex` to match entities to ontologies.
+
+    Note, this is not an instance of :class:`kazu.steps.step.ParserDependentStep`, as
+    this logic would duplicate the work of :class:`kazu.utils.link_index.DictionaryIndex`
     """
 
     def __init__(
         self,
         indices: List[DictionaryIndex],
         lookup_cache_size: int = 5000,
         top_n: int = 20,
@@ -28,73 +29,53 @@
 
         :param indices: indices to query
         :param lookup_cache_size: the size of the Least Recently Used lookup cache to maintain
         :param top_n: keep the top_n results for the query (passed to :class:`kazu.utils.link_index.DictionaryIndex`)
         :param skip_ner_namespaces: set of NER-step namespaces -- linking will be skipped for entities generated by
             these namespaces
         """
-        self.entity_class_to_indices: Dict[str, Set[DictionaryIndex]] = {}
+        self.entity_class_to_indices = defaultdict(set)
+        for index in indices:
+            self.entity_class_to_indices[index.entity_class].add(index)
         self.top_n = top_n
         self.skip_ner_namespaces = skip_ner_namespaces if skip_ner_namespaces is not None else set()
-        self.indices = indices
-        self.load_or_build_caches()
         self.lookup_cache = EntityLinkingLookupCache(lookup_cache_size)
 
-    def load_or_build_caches(self):
-        for index in self.indices:
-            index.load_or_build_cache()
-            indices_for_current_class = self.entity_class_to_indices.setdefault(
-                index.parser.entity_class, set()
-            )
-            indices_for_current_class.add(index)
-
-    def __call__(self, docs: List[Document]) -> Tuple[List[Document], List[Document]]:
+    @document_batch_step
+    def __call__(self, docs: List[Document]):
         """
         logic of entity linker:
 
         1. first obtain an entity list from all docs
         2. check the lookup LRUCache to see if an entity has been recently processed
         3. if the cache misses, run a string similarity search using the configured :class:`kazu.utils.link_index.DictionaryIndex` 's
 
         :param docs:
         :return:
         """
-        failed_docs: List[Document] = []
         entities = (
             ent
             for doc in docs
             for ent in doc.get_entities()
             if ent.namespace not in self.skip_ner_namespaces
         )
         ents_by_match_and_class = {
             k: list(v) for k, v in sort_then_group(entities, lambda x: (x.match, x.entity_class))
         }
         if len(ents_by_match_and_class) > 0:
             for ent_match_and_class, ents_this_match in ents_by_match_and_class.items():
-
                 cache_missed_entities = self.lookup_cache.check_lookup_cache(ents_this_match)
                 if len(cache_missed_entities) == 0:
                     continue
                 else:
-                    try:
-                        indices_to_search = self.entity_class_to_indices.get(ent_match_and_class[1])
-                        if indices_to_search:
-                            terms: List[SynonymTermWithMetrics] = []
-                            for index in indices_to_search:
-                                terms.extend(index.search(ent_match_and_class[0], self.top_n))
-
-                            for ent in ents_this_match:
-                                ent.update_terms(terms)
-
-                            self.lookup_cache.update_terms_lookup_cache(
-                                entity=next(iter(ents_this_match)), terms=terms
-                            )
+                    indices_to_search = self.entity_class_to_indices.get(ent_match_and_class[1])
+                    if indices_to_search:
+                        terms: List[SynonymTermWithMetrics] = []
+                        for index in indices_to_search:
+                            terms.extend(index.search(ent_match_and_class[0], self.top_n))
 
-                    except Exception:
-                        failed_docs_set: Set[Document] = set()
                         for ent in ents_this_match:
-                            doc = find_document_from_entity(docs, ent)
-                            doc.metadata[PROCESSING_EXCEPTION] = traceback.format_exc()
-                            failed_docs_set.add(doc)
-                        failed_docs.extend(failed_docs_set)
+                            ent.update_terms(terms)
 
-        return docs, failed_docs
+                        self.lookup_cache.update_terms_lookup_cache(
+                            entity=next(iter(ents_this_match)), terms=terms
+                        )
```

### Comparing `kazu-0.1.0/kazu/steps/linking/entity_class_disambiguation.py` & `kazu-1.0.0/kazu/steps/linking/entity_class_disambiguation.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/steps/linking/sapbert.py` & `kazu-1.0.0/kazu/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,208 @@
 import logging
-import sys
-from collections import defaultdict
-from typing import List, Iterable, Optional, Dict, Set
-
-import torch
-from kazu.data.data import Document, Entity, SynonymTermWithMetrics
-from kazu.modelling.linking.sapbert.train import PLSapbertModel
-from kazu.steps import Step, document_batch_step
-from kazu.utils.caching import EntityLinkingLookupCache
-from kazu.utils.link_index import EmbeddingIndex
-from pytorch_lightning import Trainer
+from pathlib import Path
+from typing import List, Dict, Tuple, Union, Iterable, Sequence, overload, Type, Any
+
+from transformers import BatchEncoding, PreTrainedTokenizerBase
+from transformers.file_utils import PaddingStrategy
+from transformers.tokenization_utils_base import TruncationStrategy
+
+from kazu.data.data import Document, Entity, Section
 
 logger = logging.getLogger(__name__)
 
 
-class SapBertForEntityLinkingStep(Step):
+def find_document_from_entity(docs: List[Document], entity: Entity) -> Document:
     """
-    This step wraps Sapbert: Self Alignment pretraining for biomedical entity representation.
-    Original paper https://aclanthology.org/2021.naacl-main.334.pdf
+    for a given entity and a list of docs, find the doc the entity belongs to
+
+    :param list_map:
+    :param entity:
+    :return:
     """
+    for doc in docs:
+        if entity in doc.get_entities():
+            return doc
+    raise RuntimeError(f"Error! Entity {entity}is not attached to a document")
 
-    def __init__(
-        self,
-        indices: List[EmbeddingIndex],
-        embedding_model: PLSapbertModel,
-        trainer: Trainer,
-        min_string_length_to_trigger: Optional[Dict[str, int]] = None,
-        ignore_high_conf: bool = True,
-        lookup_cache_size: int = 5000,
-        top_n: int = 20,
-        batch_size: int = 16,
-    ):
-        """
 
-        :param indices: list of EmbeddingIndex to use with this model
-        :param embedding_model: The SapBERT model to use to generate embeddings for entity mentions in input documents
-        :param trainer: PL trainer to call when generating embeddings
-        :param min_string_length_to_trigger: a per entity class mapping that signals sapbert will not run on matches
-            shorter than this. (sapbert is less good at symbolic matching than string processing techniques)
-        :param ignore_high_conf: If a perfect match has already been found, don't run sapbert
-        :param lookup_cache_size: the size of the Least Recently Used lookup cache to maintain
-        :param top_n: keep up to the top_n results for the query
-        :param batch_size: inference batch size
-        """
-        self.batch_size = batch_size
-        self.trainer = trainer
-        self.embedding_model = embedding_model
-        self.ignore_high_conf = ignore_high_conf
-        self.min_string_length_to_trigger = min_string_length_to_trigger
-        self.top_n = top_n
-        self.indices = indices
-        self.entity_class_to_indices: Dict[str, Set[EmbeddingIndex]] = {}
-        self.load_or_build_caches()
-
-        self.lookup_cache = EntityLinkingLookupCache(lookup_cache_size)
-
-    def load_or_build_caches(self):
-        for index in self.indices:
-            index.set_embedding_model(self.embedding_model, self.trainer)
-            index.load_or_build_cache()
-            indices_for_current_class = self.entity_class_to_indices.setdefault(
-                index.parser.entity_class, set()
-            )
-            indices_for_current_class.add(index)
+def documents_to_document_section_text_map(docs: List[Document]) -> Dict[Tuple[int, int], str]:
+    """
+    convert documents into a dict of <dochash + sectionhash>: text
 
-    @document_batch_step
-    def __call__(self, docs: List[Document]) -> None:
-        """
-        logic of entity linker:
+    :param docs:
+    :return:
+    """
+    return {
+        (
+            hash(doc),
+            hash(section),
+        ): section.get_text()
+        for doc in docs
+        for section in doc.sections
+    }
+
+
+def documents_to_id_section_map(docs: List[Document]) -> Dict[int, Section]:
+    """
+    return a map of documents, indexed by order of sections
+
+    :param docs:
+    :return:
+    """
+    result = {}
+    i = 0
+    for doc in docs:
+        for section in doc.sections:
+            result[i] = section
+            i += 1
+    return result
+
+
+def filter_entities_with_ontology_mappings(entities: List[Entity]) -> List[Entity]:
+    """
+    finds entities that have no kb mappings
+
+    :param entities:
+    :return:
+    """
+    return [x for x in entities if len(x.mappings) == 0]
+
+
+def documents_to_document_section_batch_encodings_map(
+    docs: List[Document],
+    tokenizer: PreTrainedTokenizerBase,
+    stride: int = 128,
+    max_length: int = 512,
+) -> Tuple[BatchEncoding, Dict[int, Section]]:
+    """
+    convert documents into a BatchEncoding. Also returns a list of <int + section> for the resulting encoding
 
-        1. first obtain an entity list from all docs
-        2. check the lookup LRUCache to see if it's been recently processed
-        3. generate embeddings for the entities based on the value of Entity.match
-        4. query this embedding against configured EmbeddingIndex 's to determine the best matches
-        5. update entity SynonymTermWithMetrics as appropriate
+    :param docs:
+    :return:
+    """
+    id_section_map = documents_to_id_section_map(docs)
+    strings = [section.get_text() for section in id_section_map.values()]
+
+    batch_encodings = tokenizer(
+        strings,
+        stride=stride,
+        max_length=max_length,
+        truncation=TruncationStrategy.LONGEST_FIRST,
+        return_overflowing_tokens=True,
+        padding=PaddingStrategy.MAX_LENGTH,
+    )
+    return batch_encodings, id_section_map
+
+
+def get_match_entity_class_hash(ent: Entity) -> int:
+    return hash(
+        (
+            ent.match,
+            ent.entity_class,
+        )
+    )
+
+
+PathLike = Union[str, Path]
+
+SinglePathLikeOrIterable = Union[PathLike, Iterable[PathLike]]
+
+
+def as_path(p: PathLike) -> Path:
+    return p if isinstance(p, Path) else Path(p)
+
+
+def get_cache_dir(path: PathLike, prefix: str = "", create_if_not_exist: bool = True) -> Path:
+    path = as_path(path)
+    new_path = path.with_name(f"cached_{prefix}_{path.name}")
+    if create_if_not_exist:
+        if new_path.exists():
+            logger.info(f"{new_path} already exists. Will not make it")
+        else:
+            new_path.mkdir()
+
+    return new_path
+
+
+def get_cache_path(path: PathLike, cache_id: str) -> Path:
+    path = as_path(path)
+    original_filename = path.name
+    cache_dir = get_cache_dir(path, create_if_not_exist=False)
+    new_path = cache_dir.joinpath(f"cached_{cache_id}_{original_filename}")
+    return new_path
+
+
+class EntityClassFilter:
+    """
+    A condition that returns True if a document has any entities that match the class of the required_entity_classes
+    """
+
+    def __init__(self, required_entity_classes: Iterable[str]):
+        """
 
-        :param docs:
-        :return:
+        :param required_entity_classes: list of str, specifying entity classes to assess
         """
-        entities_to_process = []
-        for doc in docs:
-            for ent in doc.get_entities():
-                if ent.entity_class not in self.entity_class_to_indices.keys():
-                    continue
-                if self.ignore_high_conf:
-                    # check every parser namespace has a high conf term
-                    # gives false by default, so if there are no terms for a parser
-                    # we run sapbert
-                    parser_has_high_conf_term: Dict[str, bool] = defaultdict(bool)
-                    for term in ent.syn_term_to_synonym_terms.values():
-                        if term.exact_match:
-                            parser_has_high_conf_term[term.parser_name] = True
-
-                    # TODO: in theory I think you could pass an embedding index when constructing
-                    # that never gets used because it isn't in the list of entities and ontologies
-                    # but I'm unclear here - unimportant enough to delay until later
-                    if not all(
-                        parser_has_high_conf_term[index.parser.name] for index in self.indices
-                    ):
-                        entities_to_process.append(ent)
-
-        self.process_entities(entities_to_process)
-
-    def process_entities(self, entities: Iterable[Entity]):
-        entities = self.lookup_cache.check_lookup_cache(entities)
-
-        if len(entities) > 0:
-            entity_string_to_ent_list = defaultdict(list)
-            # group entities by their match string, so we only need to process one string for all matches in a set
-            # of documents
-            for x in entities:
-                if self.min_string_length_to_trigger and self.min_string_length_to_trigger.get(
-                    x.entity_class, sys.maxsize
-                ) > len(x.match):
-                    continue
-                entity_string_to_ent_list[x.match].append(x)
-            if len(entity_string_to_ent_list) > 0:
-
-                results = self.embedding_model.get_embeddings_for_strings(
-                    list(entity_string_to_ent_list.keys()),
-                    trainer=self.trainer,
-                    batch_size=self.batch_size,
-                )
-                results = torch.unsqueeze(results, 1)
-                # look over the matched string and associated entities, updating the cache as we go
-                for entities_grouped, result in zip(entity_string_to_ent_list.values(), results):
-                    for entity in entities_grouped:
-                        cache_missed_entities = self.lookup_cache.check_lookup_cache([entity])
-                        if not len(cache_missed_entities) == 0:
-                            indices_to_search = self.entity_class_to_indices.get(
-                                entity.entity_class
-                            )
-                            if indices_to_search:
-                                terms: List[SynonymTermWithMetrics] = []
-                                for index in indices_to_search:
-                                    terms.extend(index.search(result, self.top_n))
-                                entity.update_terms(terms)
+        self.required_entities = set(required_entity_classes)
 
-                                self.lookup_cache.update_terms_lookup_cache(entity, terms)
+    def __call__(self, document: Document) -> bool:
+        return any(
+            (entity.entity_class in self.required_entities for entity in document.get_entities())
+        )
+
+
+@overload
+def _create_ngrams_iter(tokens: str, n: int) -> Iterable[str]:
+    pass
+
+
+@overload
+def _create_ngrams_iter(tokens: Sequence[str], n: int) -> Iterable[Sequence[str]]:
+    pass
+
+
+def _create_ngrams_iter(tokens, n=2):
+    """Yields ngrams of the input as a sequence of strings.
+
+    Tokens can be a single string where each token is a character, or an Iterable of words.
+    If tokens is a str"""
+    num_tokens = len(tokens)
+    for i in range(num_tokens):
+        ngram_end_index = i + n
+        if ngram_end_index > num_tokens:
+            # ngram would extend beyond end of parts
+            # it's ok for it to be the same number though as otherwise
+            # we don't get the final word of ngrams at the right of parts
+            break
+        yield tokens[i : i + n]
+
+
+def create_char_ngrams(s: str, n: int = 2) -> List[str]:
+    """Return list of char ngrams as a string."""
+    return list(_create_ngrams_iter(s, n))
+
+
+def create_word_ngrams(s: str, n: int = 2) -> List[str]:
+    """Return list of word ngrams as a single space-separated string."""
+    words = s.split(" ")
+    ngrams_iter = _create_ngrams_iter(words, n)
+    return [" ".join(ngram) for ngram in ngrams_iter]
+
+
+class Singleton(type):
+    _instances: Dict[Type, Any] = {}
+
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+    @staticmethod
+    def clear_all():
+        logger.warning(
+            "When clearing singletons, check that instances of classes with metaclass=Singleton are "
+            "not used as class fields, as this will cause unexpected behaviour. Also note that any existing "
+            "classes that use a Singleton will need to be re-instantiated to work correctly!. Much pain "
+            "can be avoided by observing this simple principle! Some people consider Singletons an "
+            "anti-pattern, and this is a reason why!!!"
+        )
+        Singleton._instances.clear()
```

### Comparing `kazu-0.1.0/kazu/steps/linking/post_processing/strategy_runner.py` & `kazu-1.0.0/kazu/steps/linking/post_processing/strategy_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import List, Tuple, Iterable, Dict, FrozenSet, Set, Optional
 
 from kazu.data.data import (
     Document,
     Entity,
     SynonymTermWithMetrics,
     Mapping,
+    MentionConfidence,
 )
 from kazu.steps.linking.post_processing.mapping_strategies.strategies import MappingStrategy
 from kazu.steps.linking.post_processing.xref_manager import CrossReferenceManager
 from kazu.utils.grouping import sort_then_group
 from kazu.utils.string_normalizer import StringNormalizer
 
 logger = logging.getLogger(__name__)
@@ -31,17 +32,17 @@
         e.match,
         e.match_norm,
         e.entity_class,
         frozenset(e.syn_term_to_synonym_terms),
     )
 
 
-class NamespaceStrategyExecution:
+class ConfidenceLevelStrategyExecution:
     """
-    The role of a NamespaceStrategyExecution is to track which entities have had mappings successfully resolved,
+    The role of this class is to track which entities have had mappings successfully resolved,
     and which require the application of further strategies.
 
     This is handled via tracking a dictionary of EntityKey to sets of parser names.
 
     See further details in the __call__ docstring.
     """
 
@@ -151,102 +152,67 @@
 
         Should be called when the underlying :class:`.Document` has changed.
         """
         self.unresolved_parsers.clear()
         self.entity_mapped.clear()
 
 
-NAMESPACE_ERROR_ENDING = "If entities with these namespace(s) appear, attempting to process them would cause an exception. It is likely that this class is mis-configured."
+CONFIDENCE_ERROR_ENDING = "If entities with this confidence(s) appear, attempting to process them would cause an exception. It is likely that this class is mis-configured."
 
 
 class StrategyRunner:
     """
     This is a complex class, designed to co-ordinate the running of various strategies over a document, with the end
     result producing mappings (grounding) for entities. Strategies that produce mappings may depend on the changing
     state of the Document, depending on whether other strategies are successful or not, hence why their precise
     co-ordination is crucial. Specifically we want the strategies that have higher precision to run before lower
     precision ones.
 
     Beyond the precision of the strategy itself, the variables to consider are:
 
-    1. the NER system (a.k.a namespace), in that different systems vary in terms of precision and recall for detecting
+    1. the confidence of the NER systems in the match, in that different systems vary in terms of precision and recall for detecting
        entity spans.
     2. what SynonymTerms are associated with the entity, and from which parser they originated from.
 
     The __call__ method of this class operates as follows:
 
-    1. group entities by order of NER namespace.
+    1. group entities by order of :class:`.MentionConfidence`\\.
     2. sub-group these entities again by :attr:`.Entity.match` and
        :attr:`.Entity.entity_class`\\ .
     3. divide these entities by whether they are symbolic or not.
     4. identify the maximum number of strategies that 'could' run.
-    5. get the appropriate :class:`NamespaceStrategyExecution` to run against this sub group.
+    5. get the appropriate :class:`ConfidenceLevelStrategyExecution` to run against this sub group.
     6. group the entities from 5. by EntityKey (i.e. a hashable representation of unique information required for
        mapping.
     7. conditionally execute the next strategy out of the maximum possible (from 4), and attach any resulting mappings
-       to the relevant entity group. Note, the :class:`NamespaceStrategyExecution` is responsible for deciding whether
+       to the relevant entity group. Note, the :class:`ConfidenceLevelStrategyExecution` is responsible for deciding whether
        a strategy is executed or not.
     """
 
     def __init__(
         self,
-        symbolic_strategies: Dict[str, NamespaceStrategyExecution],
-        non_symbolic_strategies: Dict[str, NamespaceStrategyExecution],
-        ner_namespace_processing_order: List[str],
+        symbolic_strategies: Dict[str, ConfidenceLevelStrategyExecution],
+        non_symbolic_strategies: Dict[str, ConfidenceLevelStrategyExecution],
         cross_ref_managers: Optional[List[CrossReferenceManager]] = None,
     ):
         """
 
 
-        :param symbolic_strategies: mapping of NER namespace to a :class:`NamespaceStrategyExecution` for symbolic
+        :param symbolic_strategies: mapping of mention confidence to a :class:`ConfidenceLevelStrategyExecution` for symbolic
             entities
-        :param non_symbolic_strategies: mapping of NER namespace to a :class:`NamespaceStrategyExecution` for
+        :param non_symbolic_strategies: mapping of mention confidence to a :class:`ConfidenceLevelStrategyExecution` for
             non-symbolic entities
-        :param ner_namespace_processing_order: Entities will be mapped in this namespace order. This is
-            useful if you have a high precision, low recall NER namespace, combined with a low precision high recall
-            namespace, as the mapping info derived from the high precision NER namespace can be used with a high
-            precision strategy for the low precision NER namespace
         :param cross_ref_managers: list of managers that will be applied to any created mappings, attempting to create
             xreferences
         """
-        self.symbolic_strategies = symbolic_strategies
-        self.non_symbolic_strategies = non_symbolic_strategies
+        self.symbolic_strategies = {MentionConfidence[k]: v for k, v in symbolic_strategies.items()}
+        self.non_symbolic_strategies = {
+            MentionConfidence[k]: v for k, v in non_symbolic_strategies.items()
+        }
         self.cross_ref_managers = cross_ref_managers
-        self.ner_namespace_processing_order = ner_namespace_processing_order
-
-        if len(self.ner_namespace_processing_order) == 0:
-            # no sort order given: sort alphabetically just to get some consistent (but arbitrary) sort key
-            self.get_namespace_sort_key = lambda ns: ns
-        else:
-            # Check that sets of namespaces are consistent
-            namespaces_with_a_namespace_strategy_execution = set(self.symbolic_strategies).union(
-                self.non_symbolic_strategies
-            )
-            processing_order_namespaces = set(self.ner_namespace_processing_order)
-            assert processing_order_namespaces.issubset(
-                namespaces_with_a_namespace_strategy_execution
-            ), (
-                "There are namespace(s) in the ner_namespace_processing_order that aren't associated"
-                " with any mapping strategies. " + NAMESPACE_ERROR_ENDING
-            )
-            assert namespaces_with_a_namespace_strategy_execution.issubset(
-                processing_order_namespaces
-            ), (
-                "There are namespace(s) associated with a strategy that aren't in the"
-                " ner_namespace_processing_order. " + NAMESPACE_ERROR_ENDING
-            )
-            # Note that the stricter:
-            # assert set(self.ner_namespace_processing_order) == set(self.symbolic_strategies) === set(self.non_symbolic_strategies)
-            # would rule out the case where we know that entities from a certain namespace will always be symbolic or non-symbolic, so
-            # the namespace only needs to be in either self.symbolic_strategies or self.non_symbolic_strategies, but not both.
-
-            self.ner_namespace_to_index = {
-                ns: ind for ind, ns in enumerate(self.ner_namespace_processing_order)
-            }
-            self.get_namespace_sort_key = lambda ns: self.ner_namespace_to_index[ns]
 
     @staticmethod
     def group_entities_by_symbolism(
         entities: Iterable[Entity],
     ) -> Tuple[List[Entity], List[Entity]]:
         """
         groups entities into symbolic and non-symbolic forms, so they can be processed separately.
@@ -272,75 +238,91 @@
 
     def __call__(self, doc: Document):
         """
 
         Run relevant strategies to decide what mappings to create.
 
         Generally speaking, noun phrases should be easier to normalise than symbolic mentions, as there is more
-        information to work with. Therefore, we group entities by configured namespace order, split by symbolism, then
+        information to work with. Therefore, we group entities by mention confidence, split by symbolism, then
         run :meth:`execute_hit_post_processing_strategies`\\ .
 
         :param doc:
         :return:
         """
+
         # do a separate sorted and groupby call (rather than our sort_then_group utility)
         # so we can do all the sorting we need in one go
+        # we inverse the sign of mention_confidence so that we process high confidence
+        # hits first
         sorted_entities = sorted(
             doc.get_entities(),
             key=lambda ent: (
-                self.get_namespace_sort_key(ent.namespace),
+                -ent.mention_confidence,
                 *entity_to_entity_key(ent),
             ),
         )
-        # add in ent.namespace, so we have it available in the group key.
-        # It won't affect the sorting since the first element of the tuple will be the same
-        # for all ents with the same namespace
-        entities_grouped_by_namespace_order = groupby(
-            sorted_entities,
-            key=lambda ent: (self.get_namespace_sort_key(ent.namespace), ent.namespace),
+        entities_grouped_by_confidence = groupby(
+            sorted_entities, key=lambda ent: ent.mention_confidence
         )
 
-        for (_namespace_sort_key, namespace), entities in entities_grouped_by_namespace_order:
-            logger.debug("mapping entities for namespace %s", namespace)
+        for mention_confidence, entities in entities_grouped_by_confidence:
+            logger.debug("mapping entities for confidence %s", mention_confidence)
             symbolic_entities, non_symbolic_entities = self.group_entities_by_symbolism(
                 entities=entities
             )
-            self.execute_hit_post_processing_strategies(
-                non_symbolic_entities, doc, self.non_symbolic_strategies[namespace]
-            )
-            self.execute_hit_post_processing_strategies(
-                symbolic_entities, doc, self.symbolic_strategies[namespace]
-            )
+
+            maybe_non_symbolic_strategies = self.non_symbolic_strategies.get(mention_confidence)
+            if maybe_non_symbolic_strategies is not None:
+                self.execute_hit_post_processing_strategies(
+                    non_symbolic_entities, doc, maybe_non_symbolic_strategies
+                )
+            else:
+                logger.warning(
+                    "No %s configured for %s ",
+                    ConfidenceLevelStrategyExecution.__name__,
+                    mention_confidence,
+                )
+            maybe_symbolic_strategies = self.symbolic_strategies.get(mention_confidence)
+            if maybe_symbolic_strategies is not None:
+                self.execute_hit_post_processing_strategies(
+                    symbolic_entities, doc, maybe_symbolic_strategies
+                )
+            else:
+                logger.warning(
+                    "No %s configured for %s ",
+                    ConfidenceLevelStrategyExecution.__name__,
+                    mention_confidence,
+                )
 
     def execute_hit_post_processing_strategies(
         self,
         ents_needing_mappings: List[Entity],
         document: Document,
-        namespace_strategy_execution: NamespaceStrategyExecution,
+        confidence_strategy_execution: ConfidenceLevelStrategyExecution,
     ):
         """
         This method executes parts 5 - 7 in the class Docstring.
 
         :param ents_needing_mappings: Expects entities to already be sorted based on :func:`entity_to_entity_key`\\ .
         :param document:
-        :param namespace_strategy_execution:
+        :param confidence_strategy_execution:
         :return:
         """
         try:
-            strategy_max_index = namespace_strategy_execution.longest_mapping_strategy_list_size
+            strategy_max_index = confidence_strategy_execution.longest_mapping_strategy_list_size
 
             groups = [
                 list(ents)
                 for _entity_key, ents in groupby(ents_needing_mappings, key=entity_to_entity_key)
             ]
 
             for i in range(0, strategy_max_index):
                 for entity_group in groups:
                     reference_entity = next(iter(entity_group))
-                    for mapping in namespace_strategy_execution(
+                    for mapping in confidence_strategy_execution(
                         entity=reference_entity,
                         strategy_index=i,
                         document=document,
                     ):
                         xref_mappings: Set[Mapping] = set()
                         if self.cross_ref_managers is not None:
                             for xref_manager in self.cross_ref_managers:
@@ -355,8 +337,8 @@
                             "mapping created: original string: %s, mapping: %s, cross-references: %s",
                             reference_entity.match,
                             mapping,
                             xref_mappings,
                         )
         finally:
             # in case exception is thrown - always reset state
-            namespace_strategy_execution.reset()
+            confidence_strategy_execution.reset()
```

### Comparing `kazu-0.1.0/kazu/steps/linking/post_processing/xref_manager.py` & `kazu-1.0.0/kazu/steps/linking/post_processing/xref_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 import json
 import logging
-import os
-import shutil
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from pathlib import Path
 from typing import Iterable, Set, Tuple, DefaultDict, Dict, List
 
 import requests
+from requests.adapters import HTTPAdapter, Retry
 
+from kazu.utils.caching import kazu_disk_cache
 from kazu.data.data import Mapping
 from kazu.steps.linking.post_processing.mapping_strategies.strategies import MappingFactory
-from kazu.utils.utils import get_cache_dir
 
 logger = logging.getLogger(__name__)
 
 
 SourceOntology = str
 SourceIdx = str
 
 TargetSourceAndIdx = Tuple[str, str]
 ToSourceAndIDXMap = Dict[SourceIdx, List[TargetSourceAndIdx]]
 XrefDatabase = Dict[SourceOntology, ToSourceAndIDXMap]
 
 
+def request_with_retry(url: str, headers: Dict, json_data: Dict):
+    s = requests.Session()
+
+    retries = Retry(
+        total=25,
+        backoff_factor=0.1,
+        status_forcelist=[500, 502, 503, 504],
+        allowed_methods=["POST"],
+    )
+
+    s.mount("https://", HTTPAdapter(max_retries=retries))
+
+    return s.post(url=url, headers=headers, json=json_data)
+
+
 class CrossReferenceManager(ABC):
 
     xref_db: XrefDatabase
 
     def __init__(self, source_to_parser_metadata_lookup: Dict[str, str], path: Path):
         """
         :param source_to_parser_metadata_lookup: when producing cross-referenced instances of Mapping, we need a
@@ -35,78 +49,25 @@
             This lookup dict tells the cross reference manager what underlying parser it should use for a given source,
             since different parsers may hold sub sets or supersets of ids of each other. For example, a MedDRA hit
             might map to specific MONDO id. Since MONDO ids are held in both OpenTargetsDiseaseOntologyParser and
             MondoOntologyParser, we need to specify which one we want to use to generate the mapping
         :param path: path to cross ref mapping resources required by this manager
         """
         self.source_to_parser_metadata_lookup = source_to_parser_metadata_lookup
-        self.load_or_build_cache(path)
+        self.xref_db = self.build_xref_cache(path)
 
     @abstractmethod
     def build_xref_cache(self, path: Path) -> XrefDatabase:
         """
         build a XrefDatabase suitable for caching
 
         :param path:
         :return:
         """
-        raise NotImplementedError()
-
-    def load_or_build_cache(self, path: Path, force_rebuild_cache: bool = False):
-        """
-        build the index, or if a cached version is available, load it instead
-
-        :param path:
-        :param force_rebuild_cache:
-        :return:
-        """
-        cache_dir = get_cache_dir(
-            path,
-            prefix=f"{self.__class__.__name__}",
-            create_if_not_exist=False,
-        )
-        if force_rebuild_cache:
-            logger.info("forcing a rebuild of the cache")
-            if cache_dir.exists():
-                shutil.rmtree(cache_dir)
-            self.xref_db = self.build_xref_cache(path)
-            self.save(cache_dir, self.xref_db)
-        elif cache_dir.exists():
-            logger.info(f"loading cached file from {cache_dir}")
-            self.load(cache_dir)
-        else:
-            logger.info("No cache file found. Building a new one")
-            self.xref_db = self.build_xref_cache(path)
-            self.save(cache_dir, self.xref_db)
-
-    def save(self, cache_path: Path, xref_db: XrefDatabase) -> Path:
-        """
-        save to disk. Makes a directory at the path location with all the index assets
-
-        :param cache_path: a dir to save the index.
-        :param xref_db: data to save
-        :return: a Path to where the data was saved
-        """
-        if cache_path.exists():
-            raise RuntimeError(f"{cache_path} already exists")
-
-        os.makedirs(cache_path, exist_ok=False)
-        with open(cache_path.joinpath("xref_db.json"), "w") as f:
-            json.dump(xref_db, f)
-        return cache_path
-
-    def load(self, cache_path: Path):
-        """
-        load from disk
-
-        :param cache_path: the path to the cached files. Normally created via .save
-        :return:
-        """
-        with open(cache_path.joinpath("xref_db.json"), "r") as f:
-            self.xref_db = json.load(f)
+        pass
 
     def create_xref_mappings(self, mapping: Mapping) -> Iterable[Mapping]:
         """
         attempt to create additional xref mappings from a source mapping
 
         :param mapping:
         :return:
@@ -124,14 +85,15 @@
                 xref_mapping = MappingFactory.create_mapping(
                     parser_name=metadata_parser_name,
                     xref_source_parser_name=mapping.parser_name,
                     source=target_source,
                     idx=target_idx,
                     string_match_strategy=self.__class__.__name__,
                     disambiguation_strategy=mapping.disambiguation_strategy,
+                    disambiguation_confidence=mapping.disambiguation_confidence,
                     string_match_confidence=mapping.string_match_confidence,
                     additional_metadata=mapping.metadata,
                 )
                 yield xref_mapping
             except KeyError:
                 # note, we've set this to debug, as xref mapping sources (e.g. OXO) generally aren't version aware
                 # i.e. this will probably fire a lot, and overload the logs if set anything higher than debug.
@@ -175,14 +137,15 @@
         """
 
         self.oxo_query = oxo_query
         self.uri_prefixes = uri_prefixes
         self.oxo_kazu_name_mapping = oxo_kazu_name_mapping
         super().__init__(source_to_parser_metadata_lookup, path)
 
+    @kazu_disk_cache.memoize(ignore={0})
     def build_xref_cache(self, path: Path) -> XrefDatabase:
         oxo_dump_path = path.joinpath("oxo_dump.json")
         logger.info(f"looking for oxo dump at {oxo_dump_path}")
         if oxo_dump_path.exists():
             with open(oxo_dump_path, "r") as f:
                 oxo_dump = json.load(f)
         else:
@@ -226,28 +189,30 @@
         for input_source, mapping_target in self.oxo_query.items():
             data = {
                 "ids": [],
                 "inputSource": input_source,
                 "mappingTarget": mapping_target,
                 "distance": "1",
             }
-            response = requests.post(f"{self.oxo_url}", headers=self.headers, json=data)
+            response = request_with_retry(
+                url=f"{self.oxo_url}", headers=self.headers, json_data=data
+            )
             response_data = response.json()
             link_info = response_data["_links"]
             last = link_info["last"]["href"]
             current = link_info["first"]["href"]
 
             while current != last:
-                response = requests.post(current, headers=self.headers, json=data)
+                response = request_with_retry(url=current, headers=self.headers, json_data=data)
                 response_data = response.json()
                 link_info = response_data["_links"]
                 next = link_info["next"]["href"]
                 current = next
                 results.append(response_data)
             else:
-                response = requests.post(last, headers=self.headers, json=data)
+                response = request_with_retry(url=last, headers=self.headers, json_data=data)
                 results.append(response.json())
 
         with open(path, "w") as f:
             json.dump(results, f)
 
         return results
```

### Comparing `kazu-0.1.0/kazu/steps/linking/post_processing/disambiguation/context_scoring.py` & `kazu-1.0.0/kazu/steps/linking/post_processing/disambiguation/context_scoring.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
-import pickle
-from pathlib import Path
 from typing import List, Tuple, Dict, Iterable
 
 import numpy as np
+from sklearn.feature_extraction.text import TfidfVectorizer
 
-from kazu.modelling.database.in_memory_db import SynonymDatabase
+from kazu.utils.caching import kazu_disk_cache
+from kazu.database.in_memory_db import SynonymDatabase
 from kazu.utils.utils import create_char_ngrams, create_word_ngrams, Singleton
-from sklearn.feature_extraction.text import TfidfVectorizer
 
 logger = logging.getLogger(__name__)
 
 
 def create_word_and_char_ngrams(
     s: str,
     words: Iterable[int] = (
@@ -44,50 +43,27 @@
     This class manages a set of TFIDF models (via
     :class:`sklearn.feature_extraction.text.TfidfVectorizer`\\ ).
 
     It's a singleton, so that the models can be accessed in multiple locations without the need to
     load them into memory multiple times.
     """
 
-    def __init__(self, path: Path):
-        """
-
-        :param path: to a directory of files containing serialised
-            :class:`sklearn.feature_extraction.text.TfidfVectorizer`\\ . The individual filenames
-            are used to map the models to the relevant parser
-        """
+    def __init__(self):
         self.synonym_db = SynonymDatabase()
-        self.parser_to_vectorizer: Dict[str, TfidfVectorizer] = {}
-        self.build_or_load_vectorizers(path)
-
-    def build_or_load_vectorizers(self, path: Path):
-        if path.exists():
-            self.load_vectorizers(path)
-        else:
-            self.build_vectorizers(path)
+        self.parser_to_vectorizer: Dict[str, TfidfVectorizer] = self.build_vectorizers()
 
-    def build_vectorizers(self, path: Path):
-        path.mkdir(parents=True)
+    @kazu_disk_cache.memoize(ignore={0})
+    def build_vectorizers(self) -> Dict[str, TfidfVectorizer]:
+        result: Dict[str, TfidfVectorizer] = {}
         for parser_name in self.synonym_db.loaded_parsers:
             synonyms = self.synonym_db.get_all(parser_name).keys()
             vectoriser = TfidfVectorizer(lowercase=False, analyzer=create_word_and_char_ngrams)
             vectoriser.fit(synonyms)
-            with path.joinpath(parser_name).open(mode="wb") as vectorizer_f:
-                pickle.dump(vectoriser, vectorizer_f)
-            self.parser_to_vectorizer[parser_name] = vectoriser
-
-    def load_vectorizers(self, path: Path):
-        self.parser_to_vectorizer.update(
-            {parser_path.name: self.load_vectorizer(parser_path) for parser_path in path.iterdir()}
-        )
-
-    @staticmethod
-    def load_vectorizer(path: Path) -> TfidfVectorizer:
-        with open(path, "rb") as f:
-            return pickle.load(f)
+            result[parser_name] = vectoriser
+        return result
 
     def __call__(
         self, strings: List[str], matrix: np.ndarray, parser: str
     ) -> Iterable[Tuple[str, float]]:
         """
         Transform a list of strings with a parser-specific vectorizer and score against a matrix.
```

### Comparing `kazu-0.1.0/kazu/steps/linking/post_processing/mapping_strategies/strategies.py` & `kazu-1.0.0/kazu/steps/linking/post_processing/mapping_strategies/strategies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import abc
 import itertools
-import urllib
 from abc import ABC
 from typing import List, Optional, Set, Iterable, Dict, FrozenSet, Tuple
 
 from kazu.data.data import (
     Document,
     Mapping,
     EquivalentIdSet,
     SynonymTermWithMetrics,
     StringMatchConfidence,
     DisambiguationConfidence,
 )
-from kazu.modelling.database.in_memory_db import MetadataDatabase, Metadata
-from kazu.modelling.language.string_similarity_scorers import StringSimilarityScorer
-from kazu.modelling.ontology_preprocessing.base import DEFAULT_LABEL
+from kazu.database.in_memory_db import MetadataDatabase, Metadata
+from kazu.language.string_similarity_scorers import StringSimilarityScorer
+from kazu.ontology_preprocessing.base import DEFAULT_LABEL
 from kazu.steps.linking.post_processing.disambiguation.strategies import DisambiguationStrategy
 
 
 class MappingFactory:
     """
     factory class to produce mappings
     """
@@ -28,51 +27,47 @@
         id_sets: Set[EquivalentIdSet],
         parser_name: str,
         string_match_strategy: str,
         string_match_confidence: StringMatchConfidence,
         disambiguation_strategy: Optional[str],
         disambiguation_confidence: Optional[DisambiguationConfidence] = None,
         additional_metadata: Optional[Dict] = None,
-        strip_url: bool = True,
     ) -> Iterable[Mapping]:
 
         for id_set in id_sets:
             yield from MappingFactory.create_mapping_from_id_set(
                 id_set=id_set,
                 parser_name=parser_name,
                 string_match_strategy=string_match_strategy,
                 string_match_confidence=string_match_confidence,
                 disambiguation_strategy=disambiguation_strategy,
                 disambiguation_confidence=disambiguation_confidence,
                 additional_metadata=additional_metadata,
-                strip_url=strip_url,
             )
 
     @staticmethod
     def create_mapping_from_id_set(
         id_set: EquivalentIdSet,
         parser_name: str,
         string_match_strategy: str,
         string_match_confidence: StringMatchConfidence,
         disambiguation_strategy: Optional[str],
         disambiguation_confidence: Optional[DisambiguationConfidence] = None,
         additional_metadata: Optional[Dict] = None,
-        strip_url: bool = True,
     ) -> Iterable[Mapping]:
         for idx, source in id_set.ids_and_source:
             yield MappingFactory.create_mapping(
                 parser_name=parser_name,
                 source=source,
                 idx=idx,
                 string_match_strategy=string_match_strategy,
                 string_match_confidence=string_match_confidence,
                 disambiguation_strategy=disambiguation_strategy,
                 disambiguation_confidence=disambiguation_confidence,
                 additional_metadata=additional_metadata if additional_metadata is not None else {},
-                strip_url=strip_url,
             )
 
     @staticmethod
     def _get_default_label_and_metadata_from_parser(
         parser_name: str, idx: str
     ) -> Tuple[str, Metadata]:
         metadata = MetadataDatabase().get_by_idx(name=parser_name, idx=idx)
@@ -86,49 +81,34 @@
         source: str,
         idx: str,
         string_match_strategy: str,
         string_match_confidence: StringMatchConfidence,
         disambiguation_strategy: Optional[str] = None,
         disambiguation_confidence: Optional[DisambiguationConfidence] = None,
         additional_metadata: Optional[Dict] = None,
-        strip_url: bool = True,
         xref_source_parser_name: Optional[str] = None,
     ) -> Mapping:
         default_label, metadata = MappingFactory._get_default_label_and_metadata_from_parser(
             parser_name, idx
         )
         if additional_metadata:
             metadata.update(additional_metadata)
-        if strip_url:
-            new_idx = MappingFactory._strip_url(idx)
-        else:
-            new_idx = idx
         return Mapping(
             default_label=default_label,
-            idx=new_idx,
+            idx=idx,
             source=source,
             string_match_strategy=string_match_strategy,
             string_match_confidence=string_match_confidence,
             disambiguation_strategy=disambiguation_strategy,
             disambiguation_confidence=disambiguation_confidence,
             parser_name=parser_name,
             metadata=metadata,
             xref_source_parser_name=xref_source_parser_name,
         )
 
-    @staticmethod
-    def _strip_url(idx):
-        url = urllib.parse.urlparse(idx)
-        if url.scheme == "":
-            # not a url
-            new_idx = idx
-        else:
-            new_idx = url.path.split("/")[-1]
-        return new_idx
-
 
 class MappingStrategy(ABC):
     """
     A MappingStrategy is responsible for actualising instances of :class:`.Mapping`\\ .
 
     This is performed in two steps:
 
@@ -143,24 +123,33 @@
 
     DISAMBIGUATION_NOT_REQUIRED = "disambiguation_not_required"
 
     def __init__(
         self,
         confidence: StringMatchConfidence,
         disambiguation_strategies: Optional[List[DisambiguationStrategy]] = None,
+        disambiguation_essential: bool = False,
     ):
         """
 
         :param confidence: the level of confidence that should be assigned to this strategy. This is simply a label
             for human users, and has no bearing on the actual algorithm.
         :param disambiguation_strategies: after :meth:`filter_terms` is called, these strategies are triggered if either
             multiple instances of :class:`.SynonymTermWithMetrics` remain, and/or any of them are ambiguous.
+        :param disambiguation_essential: disambiguation strategies MUST deliver a result, in order for this strategy to pass
         """
 
+        self.disambiguation_essential = disambiguation_essential
         self.confidence = confidence
+        if disambiguation_essential and (
+            disambiguation_strategies is None or len(disambiguation_strategies) == 0
+        ):
+            raise ValueError(
+                "disambiguation strategies must be provided, as disambiguation_essential=True"
+            )
         self.disambiguation_strategies = disambiguation_strategies
 
     def prepare(self, document: Document):
         """
         perform any setup that needs to run once per document.
 
         Care should be taken if trying to cache this step, as the Document state is liable to
@@ -192,15 +181,15 @@
         :param ent_match: the raw entity string.
         :param ent_match_norm: normalised version of the entity string.
         :param document: originating Document.
         :param terms: terms to filter.
         :param parser_name: parser name associated with these terms.
         :return: a set of filtered terms
         """
-        raise NotImplementedError()
+        pass
 
     def disambiguate_if_required(
         self, filtered_terms: Set[SynonymTermWithMetrics], document: Document, parser_name: str
     ) -> Tuple[Set[EquivalentIdSet], Optional[str], Optional[DisambiguationConfidence]]:
         """
         applies disambiguation strategies if configured, and either len(filtered_terms) > 1 or any
         of the filtered_terms are ambiguous. If ids are still ambiguous after all strategies have run,
@@ -210,28 +199,33 @@
         :param document: originating Document
         :param parser_name: parser name associated with these terms
         :return:
         """
 
         all_id_sets = set(id_set for term in filtered_terms for id_set in term.associated_id_sets)
 
-        if len(all_id_sets) == 1:
+        if not self.disambiguation_essential and len(all_id_sets) == 1:
             # there's a single id set that isn't ambiguous, no need to disambiguate
             return all_id_sets, self.DISAMBIGUATION_NOT_REQUIRED, None
-        elif self.disambiguation_strategies is None:
+        elif not self.disambiguation_essential and (
+            self.disambiguation_strategies is None or len(self.disambiguation_strategies) == 0
+        ):
             return all_id_sets, None, DisambiguationConfidence.AMBIGUOUS
         else:
+            assert self.disambiguation_strategies is not None
             for strategy in self.disambiguation_strategies:
                 filtered_id_sets = strategy(
                     id_sets=all_id_sets, document=document, parser_name=parser_name
                 )
                 if len(filtered_id_sets) == 1:
                     return filtered_id_sets, strategy.__class__.__name__, strategy.confidence
-
-            return all_id_sets, None, DisambiguationConfidence.AMBIGUOUS
+            if self.disambiguation_essential:
+                return set(), None, DisambiguationConfidence.AMBIGUOUS
+            else:
+                return all_id_sets, None, DisambiguationConfidence.AMBIGUOUS
 
     def __call__(
         self,
         ent_match: str,
         ent_match_norm: str,
         document: Document,
         terms: FrozenSet[SynonymTermWithMetrics],
@@ -335,25 +329,29 @@
     Works best on symbolic entities, e.g. "TESTIN gene" ->"TESTIN".
     """
 
     def __init__(
         self,
         confidence: StringMatchConfidence,
         disambiguation_strategies: Optional[List[DisambiguationStrategy]] = None,
+        disambiguation_essential: bool = False,
         min_term_norm_len_to_consider: int = 3,
     ):
         """
 
         :param confidence:
         :param disambiguation_strategies:
+        :param disambiguation_essential:
         :param min_term_norm_len_to_consider: only consider instances of
             :class:`.SynonymTermWithMetrics` where the length of :attr:`~.SynonymTerm.term_norm` is
             equal to or greater than this value.
         """
-        super().__init__(confidence, disambiguation_strategies)
+        super().__init__(
+            confidence, disambiguation_strategies, disambiguation_essential=disambiguation_essential
+        )
         self.min_term_norm_len_to_consider = min_term_norm_len_to_consider
 
     def filter_terms(
         self,
         ent_match: str,
         ent_match_norm: str,
         document: Document,
@@ -388,27 +386,31 @@
        differential (i.e. there are many close string matches).
     """
 
     def __init__(
         self,
         confidence: StringMatchConfidence,
         disambiguation_strategies: Optional[List[DisambiguationStrategy]] = None,
+        disambiguation_essential: bool = False,
         search_threshold=80.0,
         symbolic_only: bool = False,
         differential: float = 2.0,
     ):
         """
 
         :param confidence:
         :param disambiguation_strategies:
+        :param disambiguation_essential:
         :param search_threshold: only consider synonym terms above this search threshold
         :param symbolic_only: only consider terms that are symbolic
         :param differential: only consider terms with search scores equal or greater to the best match minus this value
         """
-        super().__init__(confidence, disambiguation_strategies)
+        super().__init__(
+            confidence, disambiguation_strategies, disambiguation_essential=disambiguation_essential
+        )
         self.differential = differential
         self.symbolic_only = symbolic_only
         self.search_threshold = search_threshold
 
     def filter_terms(
         self,
         ent_match: str,
@@ -450,35 +452,38 @@
     """
 
     def __init__(
         self,
         confidence: StringMatchConfidence,
         complex_string_scorer: StringSimilarityScorer,
         disambiguation_strategies: Optional[List[DisambiguationStrategy]] = None,
+        disambiguation_essential: bool = False,
         search_threshold: float = 80.0,
         embedding_threshold: float = 0.60,
         symbolic_only: bool = False,
         differential: float = 2.0,
     ):
         """
         :param confidence:
         :param complex_string_scorer: only consider synonym terms passing this string scorer call
         :param disambiguation_strategies:
+        :param disambiguation_essential:
         :param search_threshold: only consider synonym terms above this search threshold
         :param embedding_threshold: the Entity.match and one of the SynonymTermWithMetrics.terms must be
             above this threshold (according to the complex_string_scorer) for the term to be valid
         :param symbolic_only: only consider terms that are symbolic
         :param differential: only consider terms with search scores equal or greater to the best match minus this value
         """
         super().__init__(
             confidence=confidence,
             search_threshold=search_threshold,
             differential=differential,
             symbolic_only=symbolic_only,
             disambiguation_strategies=disambiguation_strategies,
+            disambiguation_essential=disambiguation_essential,
         )
         self.embedding_threshold = embedding_threshold
         self.complex_string_scorer = complex_string_scorer
 
     def filter_terms(
         self,
         ent_match: str,
@@ -505,23 +510,7 @@
                 selected_id_sets.add(term.associated_id_sets)
                 if any(
                     self.complex_string_scorer(ent_match, original_term) >= self.embedding_threshold
                     for original_term in term.terms
                 ):
                     selected_terms.add(term)
         return selected_terms
-
-
-class NoopMappingStrategy(MappingStrategy):
-    """
-    a No-op strategy in case you want to pass all terms straight through for disambiguation
-    """
-
-    def filter_terms(
-        self,
-        ent_match: str,
-        ent_match_norm: str,
-        document: Document,
-        terms: FrozenSet[SynonymTermWithMetrics],
-        parser_name: str,
-    ) -> Set[SynonymTermWithMetrics]:
-        return set(terms)
```

### Comparing `kazu-0.1.0/kazu/steps/ner/entity_post_processing.py` & `kazu-1.0.0/kazu/steps/ner/entity_post_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
 
         from kazu.steps.ner.entity_post_processing import SplitOnNumericalListPatternWithPrefix
         from kazu.data.data import Entity
 
     .. testcode::
 
         splitter = SplitOnNumericalListPatternWithPrefix()
-        ent = Entity.load_contiguous_entity(start=0, end=8, namespace="test", entity_class="gene", match="BRCA1/2/3")
+        ent = Entity.load_contiguous_entity(
+            start=0, end=8, namespace="test", entity_class="gene", match="BRCA1/2/3"
+        )
         print(splitter(ent, "BRCA1/2/3 are oncogenes"))
 
     .. testoutput::
 
         [BRCA1:gene:test:0:5, BRCA2:gene:test:0:7, BRCA3:gene:test:0:9]
```

### Comparing `kazu-0.1.0/kazu/steps/ner/hf_token_classification.py` & `kazu-1.0.0/kazu/steps/ner/hf_token_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     BatchEncoding,
     PreTrainedTokenizerBase,
 )
 from transformers.file_utils import PaddingStrategy
 
 from kazu.data.data import Document, Section
 from kazu.data.pytorch import HFDataset
-from kazu.modelling.hf_lightning_wrappers import PLAutoModelForTokenClassification
 from kazu.steps import Step, document_batch_step
+from kazu.steps.ner.hf_lightning_wrappers import PLAutoModelForTokenClassification
 from kazu.steps.ner.tokenized_word_processor import TokenizedWordProcessor, TokenizedWord
 from kazu.steps.ner.entity_post_processing import NonContiguousEntitySplitter
 from kazu.utils.utils import documents_to_document_section_batch_encodings_map
 
 logger = logging.getLogger(__name__)
```

### Comparing `kazu-0.1.0/kazu/steps/ner/seth.py` & `kazu-1.0.0/kazu/steps/ner/seth.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/steps/ner/spacy_ner.py` & `kazu-1.0.0/kazu/steps/ner/spacy_ner.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/steps/ner/tokenized_word_processor.py` & `kazu-1.0.0/kazu/steps/ner/tokenized_word_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import re
+from abc import ABC, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import List, Tuple, Dict, Optional, Set
 
 import torch
 from kazu.data.data import Entity, ENTITY_OUTSIDE_SYMBOL, ENTITY_START_SYMBOL, IS_SUBSPAN
 from torch import Tensor
@@ -33,15 +34,15 @@
     """
 
     clazz: str  # entity_class
     subspan: Optional[bool] = None  # is this a subspan? only relevant if using SmartSpanFinder
     tok_words: List[TokenizedWord] = field(default_factory=list)  # words associated with this span
 
 
-class SpanFinder:
+class SpanFinder(ABC):
     """
     Since Bert like models use wordpiece tokenisers to handle the OOV problem, we need to reconstitute this info
     back into document character indices to represent actual NEs.
 
     Since transformer NER is an inprecise art, we may want to use different logic in how this works, so we can
     subclass this class to determine how this should be done
 
@@ -60,36 +61,37 @@
         self.text = text
         self.active_spans: List[TokWordSpan] = []
         self.words: List[TokenizedWord] = []
         self.span_breaking_chars = {"(", ")", ";"}
         self.closed_spans: List[TokWordSpan] = []
         self.id2label = id2label
 
+    @abstractmethod
     def get_bio_and_class_labels(self, word: TokenizedWord) -> Set[Tuple[str, Optional[str]]]:
         """
         return a set of Tuple[<BIO label>,Optional[<class label>]] for a TokenizedWord. Optional[<class label>] is None
         if the BIO label is "O".
 
         :param word:
         :return:
         """
+        pass
 
-        raise NotImplementedError()
-
+    @abstractmethod
     def span_continue_condition(
         self, word: TokenizedWord, bio_and_class_labels: Set[Tuple[str, Optional[str]]]
     ):
         """
         based upon some logic, determine whether a span should continue or not
 
         :param word:
         :param bio_and_class_labels:
         :return:
         """
-        raise NotImplementedError()
+        pass
 
     def _update_active_spans(
         self, bio_and_class_labels: Set[Tuple[str, Optional[str]]], word: TokenizedWord
     ):
         """
         updates any active spans. If a B label is detected in an active span, make a copy and add to closed spans,
         as it's likely the start of another entity of the same class (but we still want to keep the original span open)
@@ -131,22 +133,23 @@
         close any active spans
         """
         for active_span in self.active_spans:
             if len(active_span.tok_words) > 0:
                 self.closed_spans.append(active_span)
         self.active_spans = []
 
+    @abstractmethod
     def process_next_word(self, word: TokenizedWord):
         """
         process the next word in the sequence, according to some logic
 
         :param word:
         :return:
         """
-        raise NotImplementedError()
+        pass
 
     def __call__(self, words: List[TokenizedWord]):
         for word in words:
             self.process_next_word(word)
         self.close_spans()
```

### Comparing `kazu-0.1.0/kazu/steps/other/merge_overlapping_ents.py` & `kazu-1.0.0/kazu/steps/other/merge_overlapping_ents.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     This step merges overlapping and nested entities. The final result should not allow any overlapped entities
     see algorithm description below
     """
 
     def __init__(
         self,
         ent_class_preferred_order: List[str],
-        ent_namespace_preferred_order: List[str],
         ignore_non_contiguous: bool = True,
     ):
         """
 
         The algorithm for selecting an entity span is as follows:
 
         1. group entities by location
@@ -34,44 +33,42 @@
            entities A, B and C are all considered to be part of the same location
 
         2. sort entities within each location, picking the best according to the following sort logic:
 
            1. prefer entities with mappings
            2. prefer longest spans
            3. prefer entities as configured by ent_class_preferred_order (see param description below)
-           4. If the proscribed entity class order is also equal, the preferred entity is selected on the basis of
+           4. prefer entities by level of confidence of entity mention
+           5. If all above are equal, the preferred entity is selected on the basis of
               the entity class name (reverse alphabetically ordered). Warning: This last sort criteria is arbitrary
 
 
         :param ent_class_preferred_order: order of namespaces to prefer. Any partially overlapped entities are
             eliminated according to this ordering (first = higher priority). If an entity class is not specified, it's
             assumed to have a priority of 0 (a.k.a lowest)
         :param ignore_non_contiguous: should non-contiguous entities be excluded from the merge process?
         """
         # store as dict for lookup speed
         self.ignore_non_contiguous = ignore_non_contiguous
         self.ent_class_preferred_order = {
             namespace: i for i, namespace in enumerate(reversed(ent_class_preferred_order))
         }
-        self.ent_namespace_preferred_order = {
-            namespace: i for i, namespace in enumerate(reversed(ent_namespace_preferred_order))
-        }
 
     def select_preferred_entity(self, ents: Set[Entity]) -> Tuple[Entity, List[Entity]]:
         """
         :param ents:
         :return: tuple of Entity<preferred> ,List[Entity]<other entities at this location>
         """
         preferred_ents = sorted(
             ents,
             key=lambda x: (
                 len(x.mappings) > 0,
                 (x.end - x.start),
                 self.ent_class_preferred_order.get(x.entity_class, 0),
-                self.ent_namespace_preferred_order.get(x.namespace, 0),
+                x.mention_confidence.value,
                 x.entity_class,
             ),
             reverse=True,
         )
         return preferred_ents[0], preferred_ents[1:]
 
     def filter_ents_across_class(self, ents: Dict[Tuple[int, int], Set[Entity]]) -> List[Entity]:
```

### Comparing `kazu-0.1.0/kazu/steps/other/stanza.py` & `kazu-1.0.0/kazu/steps/other/stanza.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/utils/abbreviation_detector.py` & `kazu-1.0.0/kazu/utils/abbreviation_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 from copy import deepcopy
 from typing import cast, Tuple, List, Optional, Set, Dict, DefaultDict, Iterable
 
 from spacy.language import Language
 from spacy.matcher import Matcher
 from spacy.tokens import Span, Doc
 
-from kazu.data.data import Document, Entity, Section
+from kazu.data.data import Document, Entity, Section, MentionConfidence
 
 logger = logging.getLogger(__name__)
 
 SectionAndLongToShortCandidates = Tuple[Section, Span, Span]
 SectionToSpacyDoc = Dict[Section, Doc]
 SectionToCharacterIndexedEntities = DefaultDict[Section, DefaultDict[Tuple[int, int], Set[Entity]]]
 
@@ -252,27 +252,31 @@
         """
         self.namespace = namespace
         self.exclude_abbrvs: Set[str] = set(exclude_abbrvs) if exclude_abbrvs is not None else set()
         self.nlp = nlp
         self.matcher = Matcher(nlp.vocab)
         self.matcher.add("parenthesis", [[{"ORTH": "("}, {"OP": "+"}, {"ORTH": ")"}]])
 
-    def __call__(self, document: Document):
+    def __call__(self, document: Document) -> None:
         (
             section_and_long_to_short_candidates,
             section_to_ents_by_char_index,
             section_to_spacy_doc,
         ) = self._find_candidates_and_index_sections(document)
 
         (
             global_matcher,
             long_form_string_to_source_ents,
         ) = self._build_matcher_and_identify_source_entities(
             section_and_long_to_short_candidates, section_to_ents_by_char_index
         )
+        if len(global_matcher) == 0:
+            # we haven't found any abbreviations to detect,
+            # so the next step can't have any effect, so skip it.
+            return
         self._find_abbreviations_and_override_entities(
             global_matcher,
             long_form_string_to_source_ents,
             section_to_ents_by_char_index,
             section_to_spacy_doc,
         )
 
@@ -362,23 +366,25 @@
         new_ent_data = deepcopy(source_ent.__dict__)
         new_ent_data.pop("start")
         new_ent_data.pop("end")
         new_ent_data.pop("spans")
         new_ent_data.pop("match_norm")
         new_ent_data.pop("match")
         new_ent_data.pop("namespace")
+        new_ent_data.pop("mention_confidence")
         new_ent = Entity.from_spans(
             text=section.get_text(),
             spans=[
                 (
                     abbrv_span.start_char,
                     abbrv_span.end_char,
                 )
             ],
             namespace=self.namespace,
+            mention_confidence=MentionConfidence.HIGHLY_LIKELY,
             join_str="",
             **new_ent_data,
         )
         return new_ent
 
     def _build_matcher_and_identify_source_entities(
         self,
```

### Comparing `kazu-0.1.0/kazu/utils/build_and_test_model_packs.py` & `kazu-1.0.0/kazu/utils/build_and_test_model_packs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 import argparse
 import json
 import logging
 import os
 import shutil
 import subprocess
 from dataclasses import dataclass, field
+from logging.config import fileConfig
 from pathlib import Path
 from typing import List, Optional
 
+import ray
 from hydra import initialize_config_dir, compose
 from hydra.utils import instantiate
 from omegaconf import DictConfig
 
-from kazu.modelling.annotation.acceptance_test import (
-    execute_full_pipeline_acceptance_test,
-    check_annotation_consistency,
-)
-from kazu.modelling.ontology_matching import assemble_pipeline
-from kazu.pipeline import load_steps_and_log_memory_usage
-from kazu.utils.constants import HYDRA_VERSION_BASE
-from kazu.utils.utils import Singleton
-
-logger = logging.getLogger(__name__)
-
 
 @dataclass
 class BuildConfiguration:
     """Dataclass that controls how a base model pack and config should be merged with a
     target model pack.
     """
 
@@ -57,262 +48,300 @@
 
 
 class ModelPackBuildError(Exception):
     pass
 
 
 class ModelPackBuilder:
-    @staticmethod
-    def load_build_configuration(model_pack_path: Path) -> BuildConfiguration:
+    def __init__(
+        self,
+        logging_config_path: Optional[Path],
+        target_model_pack_path: Path,
+        kazu_version: str,
+        build_dir: Path,
+        maybe_base_model_pack_path: Optional[Path],
+        maybe_base_configuration_path: Optional[Path],
+        skip_tests: bool,
+        zip_pack: bool,
+    ):
+        """A ModelPackBuilder is a helper class to assist in the building of a model pack.
+
+        .. danger::
+           WARNING! since this class will configure the kazu global cache, executing
+           multiple builds within the same python process could potentially lead to the
+           pollution of the cache. This is because the KAZU_MODEL_PACK env variable
+           is modified by this object, which should normally not happen. Rather
+           than instantiating this object directly, one should instead use
+           :func:`.build_all_model_packs`\\, which will control this process for you.
+
+
+        :param logging_config_path: passed to :func:`logging.config.fileConfig`
+        :param target_model_pack_path: path to model pack to process
+        :param kazu_version: version of kazu used to generate model pack
+        :param build_dir: build the pack in this directory
+        :param maybe_base_model_pack_path: if this pack requires the base model pack, specify path
+        :param maybe_base_configuration_path: if this pack requires the base configuration, specify path
+        :param skip_tests: don't run any tests
+        :param zip_pack: zip the pack at the end (requires the 'zip' CLI tool)
+        """
+        if logging_config_path is not None:
+            fileConfig(logging_config_path)
+        self.logger = logging.getLogger(__name__)
+        self.zip_pack = zip_pack
+        self.skip_tests = skip_tests
+        self.maybe_base_configuration_path = maybe_base_configuration_path
+        self.maybe_base_model_pack_path = maybe_base_model_pack_path
+        self.build_dir = build_dir
+        self.kazu_version = kazu_version
+        self.target_model_pack_path = target_model_pack_path
+        self.model_pack_build_path = self.build_dir.joinpath(self.target_model_pack_path.name)
+        os.environ["KAZU_MODEL_PACK"] = str(self.model_pack_build_path)
+        self.build_config = self.load_build_configuration()
+
+    def __repr__(self):
+        """For nice log messages."""
+        return f"ModelPackBuilder({self.target_model_pack_path.name})"
+
+    def build_model_pack(self) -> Path:
+        """Execute the build process.
+
+        :return: path of new pack
+        """
+
+        self.logger.info("building model pack at %s", self.model_pack_build_path)
+        self.model_pack_build_path.mkdir()
+        self.apply_merge_configurations()
+
+        self.clear_cached_resources_from_model_pack_dir()
+        # local import so the cache is correctly configured with KAZU_MODEL_PACK
+        from kazu.utils.constants import HYDRA_VERSION_BASE
+
+        with initialize_config_dir(
+            version_base=HYDRA_VERSION_BASE,
+            config_dir=str(self.model_pack_build_path.joinpath("conf")),
+        ):
+            cfg = compose(
+                config_name="config",
+                overrides=["hydra/job_logging=none", "hydra/hydra_logging=none"],
+            )
+            ModelPackBuilder.build_caches(cfg)
+            if not self.skip_tests:
+                # local import so the cache is correctly configured with KAZU_MODEL_PACK
+                from kazu.annotation.acceptance_test import (
+                    execute_full_pipeline_acceptance_test,
+                    check_annotation_consistency,
+                )
+
+                if self.build_config.run_consistency_checks:
+                    check_annotation_consistency(cfg)
+                if self.build_config.run_acceptance_tests:
+                    execute_full_pipeline_acceptance_test(cfg)
+            if self.zip_pack:
+                self.zip_model_pack()
+
+        return self.model_pack_build_path
+
+    def load_build_configuration(self) -> BuildConfiguration:
         """
         try to load a merge configuration from the model pack root. The merge configuration should be
         a json file called base_model_merge_config.json. None is returned if no model pack is found
 
         :param model_pack_path:
         :return:
         """
-        config_path = model_pack_path.joinpath("build_config.json")
+        config_path = self.target_model_pack_path.joinpath("build_config.json")
         if not config_path.exists():
             raise ModelPackBuildError(f"no merge config found at {str(config_path)}")
 
         with open(config_path, "r") as f:
             data = json.load(f)
         return BuildConfiguration(**data)
 
-    @staticmethod
-    def apply_merge_configurations(
-        build_config: BuildConfiguration,
-        maybe_base_model_pack_path: Optional[Path],
-        maybe_base_configuration_path: Optional[Path],
-        model_pack_build_path: Path,
-        uncached_model_pack_path: Path,
-    ):
+    def apply_merge_configurations(self):
 
         # copy the target pack to the target build dir
         shutil.copytree(
-            str(uncached_model_pack_path), str(model_pack_build_path), dirs_exist_ok=True
+            str(self.target_model_pack_path), str(self.model_pack_build_path), dirs_exist_ok=True
         )
         # copy base config if required
-        if build_config.requires_base_config:
-            if maybe_base_configuration_path is None:
+        if self.build_config.requires_base_config:
+            if self.maybe_base_configuration_path is None:
                 raise ModelPackBuildError(
-                    f"merge config asked for base configuration path but none was provided: {build_config}"
+                    f"merge config asked for base configuration path but none was provided: {self.build_config}"
                 )
-            model_pack_build_path.joinpath("conf").mkdir(exist_ok=True)
+            self.model_pack_build_path.joinpath("conf").mkdir(exist_ok=True)
             shutil.copytree(
-                str(maybe_base_configuration_path),
-                str(model_pack_build_path.joinpath("conf")),
+                str(self.maybe_base_configuration_path),
+                str(self.model_pack_build_path.joinpath("conf")),
                 dirs_exist_ok=True,
             )
-        if build_config.has_own_config:
+        if self.build_config.has_own_config:
             # and copy target config to override required elements (if required)
             shutil.copytree(
-                str(uncached_model_pack_path.joinpath("conf")),
-                str(model_pack_build_path.joinpath("conf")),
+                str(self.target_model_pack_path.joinpath("conf")),
+                str(self.model_pack_build_path.joinpath("conf")),
                 dirs_exist_ok=True,
             )
 
-        if maybe_base_model_pack_path is None and build_config.requires_base_model_pack:
+        if self.maybe_base_model_pack_path is None and self.build_config.requires_base_model_pack:
             raise ModelPackBuildError(
-                f"merge config asked for base model pack path but none was provided: {build_config}"
-            )
-        elif maybe_base_model_pack_path is not None and build_config.requires_base_model_pack:
-            ModelPackBuilder.copy_base_model_pack_resources_to_target(
-                build_config, maybe_base_model_pack_path, model_pack_build_path
+                f"merge config asked for base model pack path but none was provided: {self.build_config}"
             )
+        elif (
+            self.maybe_base_model_pack_path is not None
+            and self.build_config.requires_base_model_pack
+        ):
+            self.copy_base_model_pack_resources_to_target()
 
-    @staticmethod
-    def copy_base_model_pack_resources_to_target(
-        build_config: BuildConfiguration,
-        base_model_pack_path: Path,
-        model_pack_build_path: Path,
-    ):
-        for model in build_config.models:
-            model_source_path = base_model_pack_path.joinpath(model)
-            target_dir = model_pack_build_path.joinpath(model_source_path.name)
+    def copy_base_model_pack_resources_to_target(self):
+        assert isinstance(self.maybe_base_model_pack_path, Path)
+
+        for model in self.build_config.models:
+
+            model_source_path = self.maybe_base_model_pack_path.joinpath(model)
+            target_dir = self.model_pack_build_path.joinpath(model_source_path.name)
             shutil.copytree(str(model_source_path), str(target_dir), dirs_exist_ok=True)
-        for ontology_path_str in build_config.ontologies:
-            ontology_path = base_model_pack_path.joinpath(ontology_path_str)
-            target_path = model_pack_build_path.joinpath(ontology_path_str)
+        for ontology_path_str in self.build_config.ontologies:
+            ontology_path = self.maybe_base_model_pack_path.joinpath(ontology_path_str)
+            target_path = self.model_pack_build_path.joinpath(ontology_path_str)
             if ontology_path.is_dir():
                 shutil.copytree(str(ontology_path), str(target_path), dirs_exist_ok=True)
             else:
                 shutil.copy(ontology_path, target_path)
 
-    @staticmethod
-    def clear_cached_resources_from_model_pack_dir(model_pack_path: Path):
-        """
-        delete any cached data from the input path
+    def clear_cached_resources_from_model_pack_dir(self):
+        """Delete any cached data from the input path.
 
         :param model_pack_path:
         :return:
         """
-        for root, d_names, f_names in os.walk(model_pack_path):
-            for d_name in d_names:
-                if (
-                    d_name.startswith("cached")
-                    or d_name.startswith("tfidf")
-                    or d_name.startswith("spacy_pipeline")
-                ):
-                    deletion_path = os.path.join(root, d_name)
-                    logger.info(f"deleting cached resource: {deletion_path}")
-                    shutil.rmtree(deletion_path)
+        # local import so the cache is correctly configured with KAZU_MODEL_PACK
+        from kazu.utils.caching import kazu_disk_cache
 
-    @staticmethod
-    def zip_model_pack(model_pack_name: str, build_dir: Path):
+        kazu_disk_cache.clear()
+
+        maybe_spacy_pipeline = self.model_pack_build_path.joinpath("spacy_pipeline")
+        if maybe_spacy_pipeline.exists():
+            shutil.rmtree(maybe_spacy_pipeline)
+
+    def zip_model_pack(self):
         """
         call the zip subprocess to compress model pack (requires zip on CLI)
         also moves it to parent dir
 
         :param model_pack_name:
         :param build_dir:
         :return:
         """
-        logger.info(f"zipping model pack {model_pack_name}")
-        parent_directory = build_dir.parent
+        model_pack_name = f"{self.model_pack_build_path.name}-v{self.kazu_version}.zip"
+        self.logger.info(f"zipping model pack {model_pack_name}")
+        parent_directory = self.model_pack_build_path.parent
         model_pack_name_with_version = model_pack_name.removesuffix(".zip")
         subprocess.run(
             # make a symlink so the top-level directory in the resulting zip file
             # has the version of the model pack in it
-            ["ln", "-s", build_dir.name, model_pack_name_with_version],
+            ["ln", "-s", self.model_pack_build_path.name, model_pack_name_with_version],
             cwd=parent_directory,
         )
         subprocess.run(
             ["zip", "-r", model_pack_name, model_pack_name_with_version], cwd=parent_directory
         )
 
     @staticmethod
-    def build_all_model_packs(
-        maybe_base_model_pack_path: Optional[Path],
-        maybe_base_configuration_path: Optional[Path],
-        model_pack_paths: List[Path],
-        zip_pack: bool,
-        output_dir: Path,
-        skip_tests: bool,
-    ):
+    def build_caches(cfg: DictConfig) -> None:
         """
-        build multiple model packs
+        execute all processed required to build model pack caches
 
-        :param maybe_base_model_pack_path: Path to the base model pack, if required
-        :param maybe_base_configuration_path: Path to the base configuration, if required
-        :param model_pack_paths: list of paths to model pack resources
-        :param zip_pack: should the pack be zipped at the end?
-        :param output_dir: directory to build model packs in
-        :param skip_tests: don't run any tests
+        :param cfg:
         :return:
         """
-        if not output_dir.is_dir():
-            raise ModelPackBuildError(f"{str(output_dir)} is not a directory")
-        if len(os.listdir(output_dir)) > 0:
-            raise ModelPackBuildError(f"{str(output_dir)} is not empty")
-
-        kazu_version = (
-            subprocess.check_output("pip show kazu | grep Version", shell=True)
-            .decode("utf-8")
-            .split(" ")[1]
-            .strip()
-        )
-
-        for model_pack_path in model_pack_paths:
-            ModelPackBuilder.reset_singletons()
-            logger.info(f"building model pack at {model_pack_path}")
-            ModelPackBuilder.process_model_pack_path(
-                maybe_base_model_pack_path=maybe_base_model_pack_path,
-                maybe_base_configuration_path=maybe_base_configuration_path,
-                kazu_version=kazu_version,
-                zip_pack=zip_pack,
-                uncached_model_pack_path=model_pack_path,
-                build_dir=output_dir,
-                skip_tests=skip_tests,
-            )
-
-    @staticmethod
-    def reset_singletons():
-        """
-        this is required between different instantiations of the pipeline config, as singleton states
-        may conflict
+        parsers = instantiate(cfg.ontologies.parsers).values()
+        explosion_path = Path(os.environ["KAZU_MODEL_PACK"]).joinpath("spacy_pipeline")
+        # local import so the cache is correctly configured with KAZU_MODEL_PACK
+        from kazu.ontology_matching import assemble_pipeline
 
-        :return:
-        """
-        logger.info("clearing singletons")
-        Singleton.clear_all()
+        assemble_pipeline.main(
+            parsers=parsers,
+            output_dir=explosion_path,
+        )
+        from kazu.pipeline import load_steps_and_log_memory_usage
 
-    @staticmethod
-    def process_model_pack_path(
-        maybe_base_model_pack_path: Optional[Path],
-        maybe_base_configuration_path: Optional[Path],
-        kazu_version: str,
-        zip_pack: bool,
-        uncached_model_pack_path: Path,
-        build_dir: Path,
-        skip_tests: bool,
-    ) -> Path:
-        """
-        run all configured options on a given model pack path
+        load_steps_and_log_memory_usage(cfg)
 
-        :param maybe_base_model_pack_path: if this pack requires the base model pack, specify path
-        :param maybe_base_configuration_path: if this pack requires the base configuration, specify path
-        :param kazu_version: version of kazu used to generate model pack
-        :param zip_pack: should model pack be zipped?
-        :param uncached_model_pack_path: path to model pack to process
-        :param build_dir: directory pack should be built in
-        :param skip_tests: don't run any tests
-        :return:
-        """
 
-        model_pack_build_path = build_dir.joinpath(uncached_model_pack_path.name)
-        model_pack_build_path.mkdir()
+@ray.remote(num_cpus=1)
+class ModelPackBuilderActor(ModelPackBuilder):
+    pass
 
-        build_config = ModelPackBuilder.load_build_configuration(uncached_model_pack_path)
 
-        ModelPackBuilder.apply_merge_configurations(
-            build_config=build_config,
+def build_all_model_packs(
+    maybe_base_model_pack_path: Optional[Path],
+    maybe_base_configuration_path: Optional[Path],
+    model_pack_paths: List[Path],
+    zip_pack: bool,
+    output_dir: Path,
+    skip_tests: bool,
+    logging_config_path: Optional[Path],
+    max_parallel_build: Optional[int],
+):
+    """Build multiple model packs.
+
+    :param maybe_base_model_pack_path: Path to the base model pack, if required
+    :param maybe_base_configuration_path: Path to the base configuration, if required
+    :param model_pack_paths: list of paths to model pack resources
+    :param zip_pack: should the packs be zipped at the end?
+    :param output_dir: directory to build model packs in
+    :param skip_tests: don't run any tests
+    :param logging_config_path: passed to logging.config.fileConfig
+    :param max_parallel_build: build at most this many model packs simultaneously.
+        If None, use all available CPUs
+    :return:
+    """
+    if not output_dir.is_dir():
+        raise ModelPackBuildError(f"{str(output_dir)} is not a directory")
+    if len(list(output_dir.iterdir())) > 0:
+        raise ModelPackBuildError(f"{str(output_dir)} is not empty")
+
+    kazu_version = (
+        subprocess.check_output("pip show kazu | grep Version", shell=True)
+        .decode("utf-8")
+        .split(" ")[1]
+        .strip()
+    )
+    runtime_env = {"env_vars": {"PL_DISABLE_FORK": str(1), "TOKENIZERS_PARALLELISM": "false"}}
+    ray.init(num_cpus=max_parallel_build, runtime_env=runtime_env)
+    max_parallel_build = (
+        max_parallel_build if max_parallel_build is not None else ray.cluster_resources()["CPU"]
+    )
+    futures = []
+    for model_pack_path in model_pack_paths:
+        builder = ModelPackBuilderActor.remote(  # type: ignore[attr-defined]
+            logging_config_path=logging_config_path,
             maybe_base_model_pack_path=maybe_base_model_pack_path,
             maybe_base_configuration_path=maybe_base_configuration_path,
-            model_pack_build_path=model_pack_build_path,
-            uncached_model_pack_path=uncached_model_pack_path,
+            kazu_version=kazu_version,
+            zip_pack=zip_pack,
+            target_model_pack_path=model_pack_path,
+            build_dir=output_dir,
+            skip_tests=skip_tests,
         )
+        futures.append(builder.build_model_pack.remote())
+        while len(futures) >= max_parallel_build:
+            futures = wait_for_model_pack_completion(futures)
+
+    while len(futures) != 0:
+        futures = wait_for_model_pack_completion(futures)
 
-        ModelPackBuilder.clear_cached_resources_from_model_pack_dir(model_pack_build_path)
-        # set the env param so that hydra conf is correctly configured
-        os.environ["KAZU_MODEL_PACK"] = str(model_pack_build_path)
-        with initialize_config_dir(
-            version_base=HYDRA_VERSION_BASE, config_dir=str(model_pack_build_path.joinpath("conf"))
-        ):
-            cfg = compose(
-                config_name="config",
-                overrides=[],
-            )
-            ModelPackBuilder.build_caches(cfg)
-            if not skip_tests:
-                if build_config.run_consistency_checks:
-                    check_annotation_consistency(cfg)
-                if build_config.run_acceptance_tests:
-                    execute_full_pipeline_acceptance_test(cfg)
-            if zip_pack:
-                model_pack_name = f"{uncached_model_pack_path.name}-v{kazu_version}.zip"
-                ModelPackBuilder.zip_model_pack(model_pack_name, model_pack_build_path)
-        return model_pack_build_path
-
-    @staticmethod
-    def build_caches(cfg: DictConfig) -> None:
-        """
-        execute all processed required to build model pack caches
 
-        :param cfg:
-        :return:
-        """
-        parsers = instantiate(cfg.ontology_parser).values()
-        explosion_path = Path(os.environ["KAZU_MODEL_PACK"]).joinpath("spacy_pipeline")
-        assemble_pipeline.main(
-            parsers=parsers,
-            use_curations=True,
-            output_dir=explosion_path,
-        )
-        load_steps_and_log_memory_usage(cfg)
+def wait_for_model_pack_completion(futures) -> List:
+    # Returns the first ObjectRef that is ready.
+    finished, futures = ray.wait(futures, num_returns=1, timeout=180.0 * 60.0)
+    result = ray.get(finished[0])
+    print(f"model pack {result} build complete")
+    return futures
 
 
 if __name__ == "__main__":
     description = """Build and test model packs. This script takes a list of model
 pack directories, and creates model packs with a number of options. Depending on
 how it is called, one or more of the following may be required:
 
@@ -367,20 +396,26 @@
     )
     parser.add_argument(
         "--logging_config_path",
         type=Path,
         required=False,
         help="path to a logging config file, if required",
     )
+    parser.add_argument(
+        "--max_parallel_build",
+        type=int,
+        required=False,
+        help="build at most this many model packs simultaneously. If None, use all available CPUs",
+    )
 
     args = parser.parse_args()
-    if args.logging_config_path:
-        logging.config.fileConfig(args.logging_config_path)
 
-    ModelPackBuilder.build_all_model_packs(
+    build_all_model_packs(
         maybe_base_model_pack_path=args.base_model_pack_path,
         maybe_base_configuration_path=args.base_configuration_path,
         model_pack_paths=args.model_packs_to_build,
         zip_pack=args.zip_model_pack,
         output_dir=args.model_pack_output_path,
         skip_tests=args.skip_tests,
+        logging_config_path=args.logging_config_path,
+        max_parallel_build=args.max_parallel_build,
     )
```

### Comparing `kazu-0.1.0/kazu/utils/grouping.py` & `kazu-1.0.0/kazu/utils/grouping.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/utils/link_index.py` & `kazu-1.0.0/kazu/utils/string_normalizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,518 +1,600 @@
-import itertools
-import logging
-import os
-import pickle
-import shutil
-from abc import ABC, abstractmethod
-from pathlib import Path
-from typing import Tuple, Any, Dict, List, Iterable, Iterator, Optional, cast
-
-import numpy as np
-import torch
-from kazu.data.data import SimpleValue, SynonymTermWithMetrics
-from kazu.modelling.database.in_memory_db import MetadataDatabase, SynonymDatabase
-from kazu.modelling.language.string_similarity_scorers import BooleanStringSimilarityScorer
-from kazu.modelling.linking.sapbert.train import PLSapbertModel
-from kazu.modelling.ontology_preprocessing.base import (
-    SYN,
-    IDX,
-    MAPPING_TYPE,
-    DEFAULT_LABEL,
-    OntologyParser,
-)
-from kazu.utils.string_normalizer import StringNormalizer
-from kazu.utils.utils import create_char_ngrams, get_cache_dir
-from pytorch_lightning import Trainer
-from sklearn.feature_extraction.text import TfidfVectorizer
+import re
+from os import getenv
 
-logger = logging.getLogger(__name__)
+import regex
+from functools import lru_cache
+from typing import Optional, Dict, Protocol, Type, Tuple
 
+from kazu.language.language_phenomena import GREEK_SUBS, DASHES
 
-class Index(ABC):
+
+class EntityClassNormalizer(Protocol):
     """
-    base class for all indices.
+    protocol describing methods a normalizer should implement
     """
 
-    column_type_dict = {SYN: str, IDX: str, MAPPING_TYPE: list, DEFAULT_LABEL: str}
-
-    def __init__(
-        self,
-        parser: OntologyParser,
-    ):
+    @staticmethod
+    def is_symbol_like(original_string: str) -> bool:
         """
+        method to determine whether a string is a symbol (e.g. "AD") or a noun phrase (e.g. "Alzheimers Disease")
 
-        :param parser: The ontology parser to use with this index
+        :param original_string:
+        :return:
         """
-        self.parser = parser
-        self.metadata_db: MetadataDatabase = MetadataDatabase()
-        self.synonym_db: SynonymDatabase = SynonymDatabase()
-        self.namespace = self.__class__.__name__
+        pass
 
-    def save(self, directory: Path, overwrite: bool = False) -> Path:
+    @staticmethod
+    def normalize_symbol(original_string: str) -> str:
         """
-        save to disk. Makes a directory at the path location with all the index assets
+        method for normalising a symbol
 
-        :param directory: a dir to save the index.
-        :param overwrite: should the directory be deleted before attempting to save? (CAREFUL!)
-        :return: a Path to where the index was saved
+        :param original_string:
+        :return:
         """
-        if directory.exists() and overwrite:
-            shutil.rmtree(directory)
-        os.makedirs(directory, exist_ok=False)
-        with open(self.get_metadata_path(directory), "wb") as f:
-            pickle.dump(self.metadata_db.get_all(self.parser.name), f)
-        with open(self.get_synonym_data_path(directory), "wb") as f:
-            pickle.dump(list(self.synonym_db.get_all(self.parser.name).values()), f)
-        self._save(self.get_index_data_path(directory))
-        return directory
+        pass
 
-    def load(self, cache_path: Path):
+    @staticmethod
+    def normalize_noun_phrase(original_string: str) -> str:
         """
-        load from disk
+        method for normalising a noun phrase
 
-        :param cache_path: the path to the cached files. Normally created via .save
+        :param original_string:
         :return:
         """
-        with open(self.get_metadata_path(cache_path), "rb") as f:
-            self.metadata_db.add_parser(self.parser.name, pickle.load(f))
-        with open(self.get_synonym_data_path(cache_path), "rb") as f:
-            self.synonym_db.add(self.parser.name, pickle.load(f))
-        self._load(self.get_index_data_path(cache_path))
+        pass
+
+
+class DefaultStringNormalizer(EntityClassNormalizer):
+    """
+    normalize a biomedical string for search. Suitable for most use cases
+    """
+
+    allowed_additional_chars = {" ", "(", ")", "+", "-", "‐"}
+    greek_subs = GREEK_SUBS
+    greek_subs_upper = {x: f" {y.upper()} " for x, y in greek_subs.items()}
+    other_subs = {
+        "(": " (",
+        ")": ") ",
+        ",": " ",
+        "/": " ",
+        "VIII": " 8 ",
+        "VII": " 7 ",
+        "XII": " 12 ",
+        "III": " 3 ",
+        "VI": " 6 ",
+        "IV": " 4 ",
+        "IX": " 9 ",
+        "XI": " 11 ",
+        "II": " 2 ",
+    }
+    re_subs = {
+        re.compile(r"(?<!\()-(?!\))"): " ",  # minus not in brackets
+        re.compile(r"(?<!\()‐(?!\))"): " ",  # hyphen not in brackets
+        re.compile(r"\sI\s|\sI$"): " 1 ",
+        re.compile(r"\sV\s|\sV$"): " 5 ",
+        re.compile(r"\sX\s|\sX$"): " 10 ",
+    }
+    re_subs_2 = {
+        re.compile(r"\sA\s|\sA$|^A\s"): " ALPHA ",
+        re.compile(r"\sB\s|\sB$|^B\s"): " BETA ",
+    }
+
+    number_split_pattern = re.compile(r"(\d+)")
+
+    symbol_number_split = re.compile(r"(\d+)$")
+    trailing_lowercase_s_split = re.compile(r"(.*)(s)$")
 
     @staticmethod
-    def get_metadata_path(path: Path) -> Path:
-        return path.joinpath("ontology_metadata.pkl")
+    def is_symbol_like(original_string: str) -> bool:
+        """
+        checks for ratio of upper to lower case characters, and numeric to alpha characters.
+
+        :param original_string:
+        :return:
+        """
+        upper_count = 0
+        lower_count = 0
+        numeric_count = 0
+
+        tokens = original_string.split(" ")
+        token_count = len(tokens)
+
+        if token_count == 1 and len(original_string) <= 3:
+            return True
+
+        for i, char in enumerate(original_string):
+            if char.isalpha():
+                if char.isupper():
+                    upper_count += 1
+                    if i > 0 and token_count == 1:
+                        # if is single token, and any char apart from first is upper, assume symbol
+                        return True
+
+                else:
+                    lower_count += 1
+
+            elif char.isnumeric():
+                if token_count == 1:
+                    # if is single token and has a number in it, assume symbol
+                    return True
+                numeric_count += 1
+
+        if upper_count >= lower_count:
+            return True
+        elif numeric_count >= (upper_count + lower_count):
+            return True
+        else:
+            return False
 
     @staticmethod
-    def get_synonym_data_path(path: Path) -> Path:
-        return path.joinpath("ontology_synonym_data.pkl")
+    def normalize_symbol(original_string: str) -> str:
+        return " ".join(original_string.upper().split())
 
     @staticmethod
-    def get_index_data_path(path: Path) -> Path:
-        return path.joinpath("index.pkl")
+    def normalize_noun_phrase(original_string: str) -> str:
+        string = DefaultStringNormalizer.replace_substrings(original_string)
+        string = DefaultStringNormalizer.split_on_numbers(string)
+        string = DefaultStringNormalizer.replace_greek(string)
+        string = DefaultStringNormalizer.remove_non_alphanum(string)
+        string = DefaultStringNormalizer.depluralize(string)
+        string = DefaultStringNormalizer.sub_greek_char_abbreviations(string)
+        return " ".join(string.upper().split())
 
-    def _save(self, path: Path):
+    @staticmethod
+    def depluralize(string):
         """
-        concrete implementations should implement this to save any data specific to the implementation. This method is
-        called by self.save
+        apply some depluralisation rules
 
-        :param path:
+        :param string:
         :return:
         """
-        raise NotImplementedError()
+        if len(string) > 3:
+            string = GildaUtils.depluralize(string)[0]
+        return string
 
-    def _load(self, path: Path) -> None:
+    @staticmethod
+    def sub_greek_char_abbreviations(string):
         """
-        concrete implementations should implement this to load any data specific to the implementation. This method is
-        called by self.load
+        substitute single characters for alphanumeric representation - e.g. A -> ALPHA B--> BETA
 
-        :param path:
+        :param string:
         :return:
         """
-        raise NotImplementedError()
+        for re_sub, replace in DefaultStringNormalizer.re_subs_2.items():
+            string = re.sub(re_sub, replace, string)
+        return string
+
+    @staticmethod
+    def handle_lower_case_prefixes(string):
+        """
+        preserve case only if first char of contiguous subsequence is lower case, and is alphanum, and upper
+        case detected in rest of part. Currently unused as it causes problems with normalisation of e.g. erbB2, which
+        is a commonly used form of the symbol
+
+        :param debug:
+        :param string:
+        :return:
+        """
+        parts = string.split(" ")
+        new_parts = []
+        for part in parts:
+            if part != "":
+                if part.islower() and not len(part) == 1:
+                    new_parts.append(part.upper())
+                else:
+                    first_char_case = part[0].islower()
+                    if (first_char_case and part[0].isalnum()) or (
+                        first_char_case and len(part) == 1
+                    ):
+                        new_parts.append(part)
+                    else:
+                        new_parts.append(part.upper())
+        string = " ".join(new_parts)
+        return string
 
-    def _add(self, data: Any):
+    @staticmethod
+    def remove_non_alphanum(string):
         """
-        concrete implementations should implement this to add data to the index - e.g. synonym or embedding info. This
-        method is called by self.add
+        removes all non alphanumeric characters
 
-        :param data:
+        :param string:
         :return:
         """
-        raise NotImplementedError()
+        return "".join(
+            x
+            for x in string
+            if (x.isalnum() or x in DefaultStringNormalizer.allowed_additional_chars)
+        )
 
-    def add(self, data: Any, metadata: Dict[str, Dict[str, SimpleValue]]):
+    @staticmethod
+    def replace_greek(string):
         """
-        add data to the index
+        replaces greek characters with string representation
 
-        :param data:
+        :param string:
         :return:
         """
-        self.metadata_db.add_parser(self.parser.name, metadata)
-        self._add(data)
+        for substr, replace in DefaultStringNormalizer.greek_subs_upper.items():
+            if substr in string:
+                string = string.replace(substr, replace)
+        return string
 
-    def __len__(self) -> int:
-        """
-        should return the size of the index
+    @staticmethod
+    def split_on_numbers(string):
         """
-        return len(self.metadata_db.get_all(self.parser.name))
+        splits a string on numbers, for consistency
 
-    def load_or_build_cache(self, force_rebuild_cache: bool = False):
-        """
-        build the index, or if a cached version is available, load it instead
+        :param string:
+        :return:
         """
-        cache_dir = get_cache_dir(
-            self.parser.in_path,
-            prefix=f"{self.parser.name}_{self.__class__.__name__}",
-            create_if_not_exist=False,
+        return " ".join(
+            x.strip() for x in re.split(DefaultStringNormalizer.number_split_pattern, string)
         )
-        if force_rebuild_cache:
-            logger.info("forcing a rebuild of the ontology cache")
-            if cache_dir.exists():
-                shutil.rmtree(cache_dir)
-            self.build_ontology_cache(cache_dir)
-        elif cache_dir.exists():
-            logger.info(f"loading cached ontology file from {cache_dir}")
-            self.load(cache_dir)
-        else:
-            logger.info("No ontology cache file found. Building a new one")
-            self.build_ontology_cache(cache_dir)
 
-    def build_ontology_cache(self, cache_dir: Path):
-        cache_dir.mkdir()
-        self._build_ontology_cache(cache_dir)
-        self.load(cache_dir)
-
-    @abstractmethod
-    def _build_ontology_cache(self, cache_dir: Path):
+    @staticmethod
+    def replace_substrings(original_string):
         """
-        Implementations should implement this method to determine how an index gets built for a given parser
+        replaces a range of other strings that might be confusing to a classifier, such as roman numerals
 
-        :param cache_dir:
+        :param original_string:
         :return:
         """
-        pass
+        string = original_string
+        for substr, replace in DefaultStringNormalizer.other_subs.items():
+            if substr in string:
+                string = string.replace(substr, replace)
+        for re_sub, replace in DefaultStringNormalizer.re_subs.items():
+            string = re.sub(re_sub, replace, string)
+        return string
 
 
-class DictionaryIndex(Index):
-    """
-    The dictionary index looks for SynonymTerms via a char ngram search between the normalised version of the
-    query string and the term_norm of all SynonymTerms associated with the provided OntologyParser.
-    """
+class DiseaseStringNormalizer(EntityClassNormalizer):
+    known_disease_short_nouns = {"flu", "Flu", "HIV", "STI", "NSCLC"}
 
-    def __init__(
-        self,
-        parser: OntologyParser,
-        boolean_scorers: Optional[List[BooleanStringSimilarityScorer]] = None,
-    ):
-        """
-
-        :param parser:
-        :param boolean_scorers: precision can be increased by applying boolean checks on the returned result, for
-            instance, checking that all integers are represented, that any noun modifiers are present etc
-        """
-        super().__init__(parser=parser)
-        self.boolean_scorers = boolean_scorers
-        self.synonym_db: SynonymDatabase = SynonymDatabase()
-
-    def apply_boolean_scorers(self, reference_term: str, query_term: str) -> bool:
-
-        if self.boolean_scorers is not None:
-            return all(
-                scorer(reference_term=reference_term, query_term=query_term)
-                for scorer in self.boolean_scorers
-            )
+    @staticmethod
+    def is_symbol_like(original_string: str) -> bool:
+        if original_string in DiseaseStringNormalizer.known_disease_short_nouns:
+            return False
         else:
-            return True
-
-    def _search_index(
-        self, match: str, match_norm: str, top_n: int = 15
-    ) -> List[SynonymTermWithMetrics]:
-
-        exact_match_term = self.synonym_db.get_all(self.parser.name).get(match_norm)
-        if exact_match_term is not None:
-            term_with_metrics = SynonymTermWithMetrics.from_synonym_term(
-                exact_match_term, search_score=100.0, bool_score=True, exact_match=True
-            )
-            return [term_with_metrics]
+            return DefaultStringNormalizer.is_symbol_like(original_string)
 
-        else:
-            # benchmarking suggests converting to dense is faster than using the
-            # csr_matrix version. Strange...
-            query = self.vectorizer.transform([match_norm]).todense()
-            # minus to negate, so arg sort works in correct order
-            score_matrix = np.squeeze(-np.asarray(self.tf_idf_matrix.dot(query.T)))
-            neighbours = score_matrix.argsort()[:top_n]
-            # don't use torch for this - it's slow
-            # query = torch.FloatTensor(query)
-            # score_matrix = self.tf_idf_matrix_torch.matmul(query.T)
-            # score_matrix = torch.squeeze(score_matrix.T)
-            # neighbours = torch.argsort(score_matrix, descending=True)[:top_n]
-
-            distances = score_matrix[neighbours]
-            distances = 100 * -distances
-            result = []
-            synonym_list = list(self.synonym_db.get_all(self.parser.name).values())
-            for neighbour, score in zip(neighbours, distances):
-                # get by index
-                term = synonym_list[neighbour]
-                if self.apply_boolean_scorers(reference_term=match_norm, query_term=term.term_norm):
-                    term_with_metrics = SynonymTermWithMetrics.from_synonym_term(
-                        term, search_score=score, bool_score=True, exact_match=False
-                    )
-                    result.append(term_with_metrics)
-                else:
-                    logger.debug("filtered term %s as failed boolean checks", term)
-                # we don't sort the terms as we expect them to enter an unsorted set
-            return result
+    @staticmethod
+    def normalize_symbol(original_string: str) -> str:
+        """
+        revert to DefaultStringNormalizer.normalize_symbol
 
-    def search(self, query: str, top_n: int = 15) -> Iterable[SynonymTermWithMetrics]:
+        :param original_string:
+        :return:
         """
-        search the index
+        return DefaultStringNormalizer.normalize_symbol(original_string)
 
-        :param top_n: return a maximum of top_n SynonymTermWithMetrics
-        :param query: a string of text
+    @staticmethod
+    def normalize_noun_phrase(original_string: str) -> str:
+        """
+        revert to DefaultStringNormalizer.normalize_noun_phrase
+        :param original_string:
         :return:
         """
+        return DefaultStringNormalizer.normalize_noun_phrase(original_string)
 
-        match_norm = StringNormalizer.normalize(query, entity_class=self.parser.entity_class)
-        terms = self._search_index(query, match_norm, top_n=top_n)
-        yield from terms
 
-    def _load(self, path: Path) -> Any:
-        with open(path, "rb") as f:
-            (
-                self.vectorizer,
-                self.tf_idf_matrix,
-            ) = pickle.load(f)
+class AnatomyStringNormalizer(EntityClassNormalizer):
+    @staticmethod
+    def is_symbol_like(original_string: str) -> bool:
+        # anatomy tends not to have symbolic representations
+        return False
 
-    def _save(self, path: Path):
-        pickleable = (self.vectorizer, self.tf_idf_matrix)
-        with open(path, "wb") as f:
-            pickle.dump(pickleable, f)
+    @staticmethod
+    def normalize_symbol(original_string: str) -> str:
+        """
+        revert to DefaultStringNormalizer.normalize_noun_phrase (note, since
+        all anatomy is non-symbolic, this is theoretically superfluous, but we
+        include it anyway)
 
-    def _add(self, data: Any):
-        raise NotImplementedError(f"It's not possible to add data to a {self.__class__.__name__}")
+        :param original_string:
+        :return:
+        """
+        return DefaultStringNormalizer.normalize_noun_phrase(original_string)
 
-    def _build_ontology_cache(self, cache_dir: Path):
-        logger.info(f"creating index for {self.parser.in_path}")
+    @staticmethod
+    def normalize_noun_phrase(original_string: str) -> str:
+        """
+        revert to DefaultStringNormalizer.normalize_noun_phrase
+        :param original_string:
+        :return:
+        """
+        return DefaultStringNormalizer.normalize_noun_phrase(original_string)
 
-        self.parser.populate_databases()
-        self.vectorizer = TfidfVectorizer(min_df=1, analyzer=create_char_ngrams, lowercase=False)
-        self.tf_idf_matrix = self.vectorizer.fit_transform(
-            self.synonym_db.get_all(self.parser.name).keys()
-        )
-        index_path = self.save(cache_dir, overwrite=True)
-        logger.info(f"saved {self.parser.name} index to {index_path.absolute()}")
-        logger.info(f"final index size for {self.parser.name} is {len(self)}")
 
+class GeneStringNormalizer(EntityClassNormalizer):
+    gene_name_suffixes = {"in", "ase", "an", "gen", "gon"}
 
-class EmbeddingIndex(Index):
-    """
-    a wrapper around an embedding index strategy.
-    """
+    @staticmethod
+    def is_symbol_like(original_string: str) -> bool:
+        """
+        a symbol classifier that is designed to improve recall on natural text, especially gene symbols
+        looks at the ratio of upper case to lower case chars, and the ratio of integer to alpha chars. If the ratio of
+        upper case or integers is higher, assume it's a symbol. Also if the first char is lower case, and any
+        subsequent characters are upper case, it's probably a symbol (e.g. erbB2)
 
-    def __init__(self, parser: OntologyParser, ontology_partition_size: int = 1000):
-        super().__init__(parser=parser)
-        self.ontology_partition_size = ontology_partition_size
-        self.embedding_model: PLSapbertModel
-        self.trainer: Optional[Trainer]
+        :param original_string:
+        :return:
+        """
+        string = GildaUtils.replace_dashes(original_string, " ")
+        tokens = string.split(" ")
+        if len(tokens) == 1 and not any(
+            tokens[0].endswith(suffix) for suffix in GeneStringNormalizer.gene_name_suffixes
+        ):
+            # single tokens are likely gene symbols, or can be easily classified as gene symbols - can't trust
+            # capitalisation e.g. mTOR, erbBB2, egfr vs EGFR, Insulin
+            # in part because of convention to camel case animal homologous gene symbols
+            return True
+        else:
+            return all(len(x) < 4 or GeneStringNormalizer.gene_token_classifier(x) for x in tokens)
 
-    def set_embedding_model(
-        self, embedding_model: PLSapbertModel, trainer: Optional[Trainer] = None
-    ):
+    @staticmethod
+    def gene_token_classifier(original_string):
         """
-        set the embedding model to be used to generate target ontology embeddings when the cache is generated
-        (currently only PLSapbertModel supported). Also, optionally set a PL Trainer that should be used (a Trainer
-        configured with default params will be used otherwise)
+        slightly modified version of DefaultStringNormalizer.is_symbol_like, designed to work on single tokens. Checks
+        if the casing of the symbol changes from lower to upper (if so, is likely to be symbolic, e.g. erbB2)
 
-        :param embedding_model:
-        :param trainer:
+        :param original_string:
         :return:
         """
-        self.embedding_model = embedding_model
-        self.trainer = trainer
+        upper_count = 0
+        lower_count = 0
+        numeric_count = 0
+        first_char_is_lower = len(original_string) > 0 and original_string[0].islower()
+        for char in original_string:
+            if char.isalpha():
+                if char.isupper():
+                    upper_count += 1
+                    if first_char_is_lower:
+                        return True
+                else:
+                    lower_count += 1
+            elif char.isnumeric():
+                numeric_count += 1
+        if upper_count >= lower_count:
+            return True
+        elif numeric_count >= (upper_count + lower_count):
+            return True
+        else:
+            return False
 
-    def _add(self, embeddings: torch.Tensor):
+    @staticmethod
+    def remove_trailing_s_if_otherwise_capitalised(string: str):
         """
-        add embeddings to the index
+        frustratingly, some gene symbols are pluralised like ERBBs. we can't just remove trailing s as this breaks
+        genuine symbols like 'MDH-s' and 'GASP10ps'. So, we only strip the trailing 's' if the char before is upper
+        case
 
-        :param embeddings: a 2d tensor of embeddings
+        :param string:
         :return:
         """
-        if not hasattr(self, "index"):
-            self.index = self._create_index(embeddings)
+        if len(string) >= 3 and string[-2].isupper():
+            return string.removesuffix("s")
         else:
-            self._add_embeddings(embeddings)
+            return string
 
-    def _add_embeddings(self, embeddings: torch.Tensor):
+    @staticmethod
+    def normalize_symbol(original_string: str) -> str:
         """
-        concrete implementations should implement this method to add embeddings to the index
+        contrary to other entity classes, gene symbols require special handling because of their highly unusual
+        nature
 
-        :param embeddings:
+        :param original_string:
         :return:
         """
-        raise NotImplementedError()
+        string = GeneStringNormalizer.remove_trailing_s_if_otherwise_capitalised(original_string)
+        string = DefaultStringNormalizer.replace_substrings(string)
+        string = DefaultStringNormalizer.split_on_numbers(string)
+        string = DefaultStringNormalizer.replace_greek(string)
+        string = DefaultStringNormalizer.remove_non_alphanum(string)
+        string = DefaultStringNormalizer.sub_greek_char_abbreviations(string)
+        return " ".join(string.upper().split())
 
-    def _create_index(self, embeddings: torch.Tensor) -> Any:
+    @staticmethod
+    def normalize_noun_phrase(original_string: str) -> str:
         """
-        concrete implementations should implement this to create an index. This should also add the embeddings
-        after the index is created
+        revert to DefaultStringNormalizer.normalize_noun_phrase for non symbolic genes
 
-        :param embeddings:
+        :param original_string:
         :return:
         """
-        raise NotImplementedError()
+        return DefaultStringNormalizer.normalize_noun_phrase(original_string)
+
+
+class CompanyStringNormalizer(EntityClassNormalizer):
+    @staticmethod
+    def is_symbol_like(original_string: str) -> bool:
+        alpha_chars = filter(lambda x: x.isalpha(), original_string)
+        return all(x.isupper() for x in alpha_chars)
 
-    def _search_func(
-        self, query: torch.Tensor, score_cutoff: float = 99.0, top_n: int = 20, **kwargs
-    ) -> Tuple[np.ndarray, np.ndarray]:
+    @staticmethod
+    def normalize_symbol(original_string: str) -> str:
         """
-        should be implemented
+        just upper case.
 
-        :param query: a string of text
-        :param score_cutoff:
-        :param top_n: return up to this many results
+        :param original_string:
         :return:
         """
-        raise NotImplementedError()
+        return original_string.upper()
 
-    def search(
-        self,
-        query: torch.Tensor,
-        top_n: int = 1,
-    ) -> Iterable[SynonymTermWithMetrics]:
+    @staticmethod
+    def normalize_noun_phrase(original_string: str) -> str:
         """
-
-        :param query: a query tensor
-        :param top_n: return top_n instances of SynonymTermWithMetrics
+        revert to DefaultStringNormalizer.normalize_noun_phrase
+        :param original_string:
         :return:
         """
+        return DefaultStringNormalizer.normalize_noun_phrase(original_string)
 
-        distances, neighbours = self._search_func(query=query, top_n=top_n)
-        for score, neighbour in zip(distances, neighbours):
-            idx, metadata = self.metadata_db.get_by_index(self.parser.name, neighbour)
-            # the norm form of the default label should always be in the syn database
-            default_label = metadata[DEFAULT_LABEL]
-            assert isinstance(default_label, str)
-            string_norm = StringNormalizer.normalize(
-                default_label, entity_class=self.parser.entity_class
-            )
-            try:
 
-                term = self.synonym_db.get(self.parser.name, string_norm)
-                term_with_metrics = SynonymTermWithMetrics.from_synonym_term(
-                    term, embed_score=score
-                )
-                yield term_with_metrics
-            except KeyError:
-                logger.warning(
-                    f"{string_norm} is not in the synonym database! is the parser for {self.parser.name} correctly configured?"
-                )
+class StringNormalizer:
+    """
+    call custom entity class normalizers, or a default normalizer if none is available
+    """
 
-    def _build_ontology_cache(self, cache_dir: Path):
-        if not hasattr(self, "embedding_model"):
-            raise RuntimeError("you must call set_embedding_model before trying to build the cache")
+    normalizers: Dict[Optional[str], Type[EntityClassNormalizer]] = {
+        "gene": GeneStringNormalizer,
+        "anatomy": AnatomyStringNormalizer,
+        "disease": DiseaseStringNormalizer,
+        "company": CompanyStringNormalizer,
+    }
 
-        logger.info(f"creating index for {self.parser.in_path}")
+    @staticmethod
+    @lru_cache(maxsize=int(getenv("KAZU_STRING_NORMALIZER_CACHE_SIZE", 5000)))
+    def classify_symbolic(original_string: str, entity_class: Optional[str] = None) -> bool:
+        return StringNormalizer.normalizers.get(
+            entity_class, DefaultStringNormalizer
+        ).is_symbol_like(original_string)
 
-        # populate the databases
-        self.parser.populate_databases()
-        for (
-            partition_number,
-            metadata,
-            ontology_embeddings,
-        ) in self.predict_ontology_embeddings(self.parser.name):
-            logger.info(f"processing partition {partition_number} ")
-            self.add(data=ontology_embeddings, metadata=metadata)
-            logger.info(f"index size is now {len(self)}")
-        index_path = self.save(cache_dir, overwrite=True)
-        logger.info(f"saved {self.parser.name} index to {index_path.absolute()}")
-        logger.info(f"final index size for {self.parser.name} is {len(self)}")
+    @staticmethod
+    @lru_cache(maxsize=int(getenv("KAZU_STRING_NORMALIZER_CACHE_SIZE", 5000)))
+    def normalize(original_string: str, entity_class: Optional[str] = None) -> str:
+        normaliser_for_entity_class = StringNormalizer.normalizers.get(
+            entity_class, DefaultStringNormalizer
+        )
+        if normaliser_for_entity_class.is_symbol_like(original_string):
+            return normaliser_for_entity_class.normalize_symbol(original_string)
+        else:
+            return normaliser_for_entity_class.normalize_noun_phrase(original_string)
 
-    def enumerate_database_chunks(
-        self, name: str, chunk_size: int = 100000
-    ) -> Iterable[Tuple[int, Dict[str, Dict[str, SimpleValue]]]]:
-        """
-        generator to split up a dataframe into partitions
 
-        :param name: ontology name to query the metadata database with
-        :param chunk_size: size of partittions to create
-        :return:
-        """
+class GildaUtils:
+    """Functions derived from `gilda <https://github.com/indralab/gilda>`_ used by (some of) the :py:class:`~StringNormalizer`\\ s.
 
-        data = self.metadata_db.get_all(name)
-        for i in range(0, len(data), chunk_size):
-            yield i, dict(itertools.islice(data.items(), i, i + chunk_size))
+    Original Credit:
 
-    def predict_ontology_embeddings(
-        self, name: str
-    ) -> Iterator[Tuple[int, Dict[str, Dict[str, SimpleValue]], torch.Tensor]]:
-        """
-        since embeddings are memory hungry, we use a generator to partition an input dataframe into manageable chucks,
-        and add them to the index sequentially
+    | https://github.com/indralab/gilda
+    | https://github.com/indralab/gilda/blob/9e383213098144fe82103a3a5aa1bf4c14059e57/gilda/process.py
 
-        :param name: name of ontology
-        :return: partition number, metadata and embeddings
-        """
+    Paper:
 
-        for partition_number, metadata in self.enumerate_database_chunks(
-            name, self.ontology_partition_size
-        ):
-            len_df = len(metadata)
-            if len_df == 0:
-                return
-            logger.info(f"creating partitions for partition {partition_number}")
-            logger.info(f"read {len_df} rows from ontology")
-            # use cast to tell mypy this is already the right type
-            default_labels = cast(List[str], [x[DEFAULT_LABEL] for x in metadata.values()])
-            logger.info(f"predicting embeddings for default_labels. Examples: {default_labels[:3]}")
-            results = self.embedding_model.get_embeddings_for_strings(
-                texts=default_labels, trainer=self.trainer
-            )
-            yield partition_number, metadata, results
+    Benjamin M Gyori, Charles Tapley Hoyt, and Albert Steppi. 2022.
+    `Gilda: biomedical entity text normalization with machine-learned disambiguation as a service. <https://doi.org/10.1093/bioadv/vbac034>`_
+    Bioinformatics Advances. Vbac034.
 
+    .. raw:: html
 
-class TensorEmbeddingIndex(EmbeddingIndex):
-    """
-    a simple index of torch tensors.
-    """
+        <details>
+        <summary>Bibtex Citation Details</summary>
 
-    def __init__(
-        self,
-        parser: OntologyParser,
-    ):
-        super().__init__(parser=parser)
-        self.index: torch.Tensor
-
-    def _load(self, path: Path) -> Any:
-        with open(path, "rb") as f:
-            self.index = pickle.load(f)
-
-    def _save(self, path: Path):
-        pickleable = self.index
-        with open(path, "wb") as f:
-            pickle.dump(pickleable, f)
-
-    def _add_embeddings(self, embeddings: torch.Tensor):
-        self.index = torch.cat([self.index, embeddings])
-        return self.index
+    .. code:: bibtex
 
-    def _create_index(self, embeddings: torch.Tensor) -> Any:
-        return embeddings
+        @article{gyori2022gilda,
+            author = {Gyori, Benjamin M and Hoyt, Charles Tapley and Steppi, Albert},
+            title = "{{Gilda: biomedical entity text normalization with machine-learned disambiguation as a service}}",
+            journal = {Bioinformatics Advances},
+            year = {2022},
+            month = {05},
+            issn = {2635-0041},
+            doi = {10.1093/bioadv/vbac034},
+            url = {https://doi.org/10.1093/bioadv/vbac034},
+            note = {vbac034}
+        }
 
-    def __len__(self):
-        return len(self.index)
+    .. raw:: html
 
+        </details>
 
-class CDistTensorEmbeddingIndex(TensorEmbeddingIndex):
-    """
-    Calculate embedding based on cosine distance
-    """
 
-    def _search_func(
-        self, query: torch.Tensor, score_cutoff: float = 99.0, top_n: int = 20, **kwargs
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        score_matrix = torch.cdist(query, self.index)
-
-        score_matrix = torch.squeeze(score_matrix)
-        neighbours = torch.argsort(score_matrix, descending=False)[:top_n]
-        distances = score_matrix[neighbours]
-        return distances.cpu().numpy(), neighbours.cpu().numpy()
+    Licensed under BSD 2-Clause.
 
+    Copyright (c) 2019, Benjamin M. Gyori, Harvard Medical School All rights reserved.
+
+    .. raw:: html
+
+        <details>
+        <summary>Full License</summary>
+
+    BSD 2-Clause License
+
+    Copyright (c) 2019, Benjamin M. Gyori, Harvard Medical School
+    All rights reserved.
+
+    Redistribution and use in source and binary forms, with or without
+    modification, are permitted provided that the following conditions are met:
+
+    * Redistributions of source code must retain the above copyright notice, this
+      list of conditions and the following disclaimer.
+
+    * Redistributions in binary form must reproduce the above copyright notice,
+      this list of conditions and the following disclaimer in the documentation
+      and/or other materials provided with the distribution.
+
+    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+    AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+    SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+    OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+    .. raw:: html
+
+        </details>
 
-class MatMulTensorEmbeddingIndex(TensorEmbeddingIndex):
-    """
-    calculate embedding based on MatMul
     """
 
-    def _search_func(
-        self, query: torch.Tensor, score_cutoff: float = 99.0, top_n: int = 20, **kwargs
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        score_matrix = torch.matmul(query, self.index.T)
-
-        score_matrix = torch.squeeze(score_matrix)
-        neighbours = torch.argsort(score_matrix, descending=True)[:top_n]
-        distances = score_matrix[neighbours]
-        distances = 100 - (1 / distances)
-        return distances.cpu().numpy(), neighbours.cpu().numpy()
+    @staticmethod
+    def depluralize(word: str) -> Tuple[str, str]:
+        """
+        Return the depluralized version of the word, along with a status flag.
+
+        :param word: The word which is to be depluralized.
+        :return: The first element is the original word, if it is detected to be non-plural, or the
+            depluralized version of the word.
+
+            The second element is a status flag representing the detected pluralization status of
+            the word, with non_plural (e.g., BRAF), plural_oes (e.g., mosquitoes),
+            plural_ies (e.g., antibodies), plural_es (e.g., switches),
+            plural_cap_s (e.g., MAPKs), and plural_s (e.g., receptors).
+        """
+        # If the word doesn't end in s, we assume it's not plural
+        if not word.endswith("s"):
+            return word, "non_plural"
+        # Another case is words ending in -sis (e.g., apoptosis), these are almost
+        # exclusively non plural so we return here too
+        elif word.endswith("sis"):
+            return word, "non_plural"
+        # This is the case when the word ends with an o which is pluralized as oes
+        # e.g., mosquitoes
+        elif word.endswith("oes"):
+            return word[:-2], "plural_oes"
+        # This is the case when the word ends with a y which is pluralized as ies,
+        # e.g., antibodies
+        elif word.endswith("ies"):
+            return word[:-3] + "y", "plural_ies"
+        # These are the cases where words form plurals by adding -es so we
+        # return by stripping it off
+        elif word.endswith(("xes", "ses", "ches", "shes")):
+            return word[:-2], "plural_es"
+        # If the word is all caps and the last letter is an s, then it's a very
+        # strong signal that it is pluralized so we have a custom return value
+        # for that
+        elif regex.match(r"^\p{Lu}+$", word[:-1]):
+            return word[:-1], "plural_caps_s"
+        # Otherwise, we just go with the assumption that the last s is the
+        # plural marker
+        else:
+            return word[:-1], "plural_s"
+        # Note: there don't seem to be any compelling examples of -f or -fe -> ves
+        # so it is not implemented
+
+    @classmethod
+    def replace_dashes(cls, s: str, rep: str = "-") -> str:
+        """Replace all types of dashes in a given string with a given replacement.
+
+        :param s: The string in which all types of dashes should be replaced.
+        :param rep: The string with which dashes should be replaced. By default, the plain
+            ASCII dash (-) is used.
+        :return: The string in which dashes have been replaced.
+        """
+        for d in DASHES:
+            s = s.replace(d, rep)
+        return s
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kazu-0.1.0/kazu/utils/stanza_pipeline.py` & `kazu-1.0.0/kazu/utils/stanza_pipeline.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/utils/stopwatch.py` & `kazu-1.0.0/kazu/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/web/jwtauth.py` & `kazu-1.0.0/kazu/web/jwtauth.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/kazu/web/ls_web_utils.py` & `kazu-1.0.0/kazu/web/ls_web_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Tuple, Dict, List, Any
 
 from kazu.data.data import Document
-from kazu.modelling.annotation.label_studio import (
+from kazu.annotation.label_studio import (
     LabelStudioAnnotationView,
     KazuToLabelStudioConverter,
 )
 
 LSView = str
 LSTask = Dict[str, Any]
```

### Comparing `kazu-0.1.0/kazu/web/req_id_header.py` & `kazu-1.0.0/kazu/web/req_id_header.py`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/.gitignore` & `kazu-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/LICENSE` & `kazu-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kazu-0.1.0/README.md` & `kazu-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,52 +51,52 @@
 
 `export KAZU_MODEL_PACK=<path to the extracted archive>`
 
 Kazu is highly configurable (using [Hydra](https://hydra.cc/docs/intro/)), although it comes preconfigured with defaults appropriate for most literature processing use cases. 
 To make use of these, and process a simple document:
 
 ```python
-
 import hydra
 from hydra.utils import instantiate
 
 from kazu.data.data import Document
 from kazu.pipeline import Pipeline
 from kazu.utils.constants import HYDRA_VERSION_BASE
 from pathlib import Path
 import os
 
 # the hydra config is kept in the model pack
 cdir = Path(os.environ["KAZU_MODEL_PACK"]).joinpath("conf")
 
 
-@hydra.main(version_base=HYDRA_VERSION_BASE, config_path=str(cdir), config_name="config")
+@hydra.main(
+    version_base=HYDRA_VERSION_BASE, config_path=str(cdir), config_name="config"
+)
 def kazu_test(cfg):
     pipeline: Pipeline = instantiate(cfg.Pipeline)
     text = "EGFR mutations are often implicated in lung cancer"
     doc = Document.create_simple_document(text)
     pipeline([doc])
     print(f"{doc.get_entities()}")
 
 
 if __name__ == "__main__":
     kazu_test()
-
 ```
 
 # Documentation
 
 [Find our docs here](https://astrazeneca.github.io/KAZU/_build/html/index.html)
 
 ## License
 
 Licensed under [Apache 2.0](https://github.com/AstraZeneca/KAZU/blob/main/LICENSE).
 
 Kazu includes elements under compatible licenses (full licenses are in relevant files or as indicated):
-- Some elements are a modification of code licensed under MIT by Explosion.AI - see the README [here](https://github.com/AstraZeneca/KAZU/blob/main/kazu/modelling/ontology_matching/README.md).
+- Some elements are a modification of code licensed under MIT by Explosion.AI - see the README [here](https://github.com/AstraZeneca/KAZU/blob/main/kazu/ontology_matching/README.md).
 - The doc build process (conf.py's linkcode_resolve function) uses code modified from pandas, in turn modified from numpy. See [PANDAS_LICENSE.txt](https://github.com/AstraZeneca/KAZU/blob/main/docs/PANDAS_LICENSE.txt) and [NUMPY_LICENSE.txt](https://github.com/AstraZeneca/KAZU/blob/main/docs/NUMPY_LICENSE.txt)
 - Elements of the model distillation code are inspired by or modified from Huawei Noah's Ark Lab [TinyBERT](https://github.com/huawei-noah/Pretrained-Language-Model/blob/master/TinyBERT) and DMIS-Lab's [BioBERT](https://github.com/dmis-lab/biobert/tree/master).
   See the details in dataprocessor.py, models.py and tiny_transformer.py.
 - PLSapbertModel is inspired by the code from [sapbert](https://github.com/cambridgeltl/sapbert), licensed under MIT. See the file for details, and see the [SapBert](#sapbert) section below regarding use of the model.
 - GildaUtils in the string_normalizer.py file is modified from [Gilda](https://github.com/indralab/gilda). See the file for full details
   including the full BSD 2-Clause license.
 - The AbbreviationFinderStep uses KazuAbbreviationDetector, which is a modified version of
```

### Comparing `kazu-0.1.0/pyproject.toml` & `kazu-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -22,44 +22,51 @@
   "transformers>=4.0.0",
   "rdflib>=6.0.0",
   "requests>=2.20.0",
   "hydra-core>=1.3.0",
   "pytorch-lightning>=1.7.4,<2.0.0",
   "pandas>=1.0.0",
   "pyarrow>=8.0.0",
-  "pytorch-metric-learning>=0.9.99",
+  "pymongo>=4.3.3",
   "rapidfuzz>=1.0.0",
-  "seqeval>=1.0.0",
   "py4j>=0.10.9",
   "scikit-learn>=0.24.0",
   "stanza>=1.0.0",
   "regex>=2020.1.7",
   "psutil>=5.3.0",
-  "cachetools>=5.2.0"
+  "cachetools>=5.2.0",
+  "diskcache>=5.4.0"
 ]
 
 [project.urls]
 documentation = "https://astrazeneca.github.io/KAZU/_build/html/index.html"
 repository = "https://github.com/AstraZeneca/KAZU"
 
 [project.optional-dependencies]
 webserver = [
+  "fastapi<0.99.0",  # newer than this breaks our 'examples' in the Swagger page
+  "pydantic<2.0,",
   "ray[serve]>=1.10.0",
   "PyJWT>=2.0.0",
   ]
 typed = [
   "types-requests",
   "types-cachetools",
   "types-regex",
   "types-psutil",
-  "pandas-stubs",
+  "pandas-stubs>=2.0.0",
+]
+model_training = [
+  "pytorch-metric-learning>=0.9.99",
+  "seqeval>=1.0.0",
 ]
 dev = [
-  "kazu[webserver,typed]",
+  "kazu[webserver,typed,model_training]",
   "black~=22.0",
+  "blacken-docs",
   "flake8",
   "mypy",
   "bump2version",
   "pre-commit",
   "pytest",
   "pytest-mock",
   "pytest-cov",
@@ -67,14 +74,15 @@
   "sphinx",
   "myst_parser",
   "furo",
   # to allow profiling
   # of the steps.
   "tensorboard",
   "towncrier",
+  "ray>=1.10.0",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
@@ -124,14 +132,15 @@
     "transformers.*",
     "tokenizers.*",
     "stanza.*",
     "sklearn.*",
     "pytorch_metric_learning.*",
     "srsly.*",
     "py4j.*",
+    "diskcache.*",
 ]
 ignore_missing_imports = true
 
 [tool.towncrier]
 package = "kazu"
 directory = "docs/_changelog.d"
 package-dir = "kazu"
```

### Comparing `kazu-0.1.0/PKG-INFO` & `kazu-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kazu
-Version: 0.1.0
+Version: 1.0.0
 Summary: Biomedical Named Entity Recognition and Entity Linking for Enterprise use cases
 Project-URL: documentation, https://astrazeneca.github.io/KAZU/_build/html/index.html
 Project-URL: repository, https://github.com/AstraZeneca/KAZU
 Author: AstraZeneca AI and Korea University
 License-File: AUTHORS.md
 License-File: LICENSE
 Classifier: Intended Audience :: Healthcare Industry
@@ -12,54 +12,61 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: cachetools>=5.2.0
+Requires-Dist: diskcache>=5.4.0
 Requires-Dist: hydra-core>=1.3.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: psutil>=5.3.0
 Requires-Dist: py4j>=0.10.9
 Requires-Dist: pyarrow>=8.0.0
+Requires-Dist: pymongo>=4.3.3
 Requires-Dist: pytorch-lightning<2.0.0,>=1.7.4
-Requires-Dist: pytorch-metric-learning>=0.9.99
 Requires-Dist: rapidfuzz>=1.0.0
 Requires-Dist: rdflib>=6.0.0
 Requires-Dist: regex>=2020.1.7
 Requires-Dist: requests>=2.20.0
 Requires-Dist: scikit-learn>=0.24.0
-Requires-Dist: seqeval>=1.0.0
 Requires-Dist: spacy>=3.2.0
 Requires-Dist: stanza>=1.0.0
 Requires-Dist: torch>=1.12.0
 Requires-Dist: transformers>=4.0.0
 Provides-Extra: dev
+Requires-Dist: blacken-docs; extra == 'dev'
 Requires-Dist: black~=22.0; extra == 'dev'
 Requires-Dist: bump2version; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: furo; extra == 'dev'
-Requires-Dist: kazu[typed,webserver]; extra == 'dev'
+Requires-Dist: kazu[model-training,typed,webserver]; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: myst-parser; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
+Requires-Dist: ray>=1.10.0; extra == 'dev'
 Requires-Dist: sphinx; extra == 'dev'
 Requires-Dist: tensorboard; extra == 'dev'
 Requires-Dist: towncrier; extra == 'dev'
+Provides-Extra: model-training
+Requires-Dist: pytorch-metric-learning>=0.9.99; extra == 'model-training'
+Requires-Dist: seqeval>=1.0.0; extra == 'model-training'
 Provides-Extra: typed
-Requires-Dist: pandas-stubs; extra == 'typed'
+Requires-Dist: pandas-stubs>=2.0.0; extra == 'typed'
 Requires-Dist: types-cachetools; extra == 'typed'
 Requires-Dist: types-psutil; extra == 'typed'
 Requires-Dist: types-regex; extra == 'typed'
 Requires-Dist: types-requests; extra == 'typed'
 Provides-Extra: webserver
+Requires-Dist: fastapi<0.99.0; extra == 'webserver'
+Requires-Dist: pydantic<2.0; extra == 'webserver'
 Requires-Dist: pyjwt>=2.0.0; extra == 'webserver'
 Requires-Dist: ray[serve]>=1.10.0; extra == 'webserver'
 Description-Content-Type: text/markdown
 
 ![Maturity level-1](https://img.shields.io/badge/Maturity%20Level-ML--1-yellow)
 
 <p align="center">
@@ -113,52 +120,52 @@
 
 `export KAZU_MODEL_PACK=<path to the extracted archive>`
 
 Kazu is highly configurable (using [Hydra](https://hydra.cc/docs/intro/)), although it comes preconfigured with defaults appropriate for most literature processing use cases. 
 To make use of these, and process a simple document:
 
 ```python
-
 import hydra
 from hydra.utils import instantiate
 
 from kazu.data.data import Document
 from kazu.pipeline import Pipeline
 from kazu.utils.constants import HYDRA_VERSION_BASE
 from pathlib import Path
 import os
 
 # the hydra config is kept in the model pack
 cdir = Path(os.environ["KAZU_MODEL_PACK"]).joinpath("conf")
 
 
-@hydra.main(version_base=HYDRA_VERSION_BASE, config_path=str(cdir), config_name="config")
+@hydra.main(
+    version_base=HYDRA_VERSION_BASE, config_path=str(cdir), config_name="config"
+)
 def kazu_test(cfg):
     pipeline: Pipeline = instantiate(cfg.Pipeline)
     text = "EGFR mutations are often implicated in lung cancer"
     doc = Document.create_simple_document(text)
     pipeline([doc])
     print(f"{doc.get_entities()}")
 
 
 if __name__ == "__main__":
     kazu_test()
-
 ```
 
 # Documentation
 
 [Find our docs here](https://astrazeneca.github.io/KAZU/_build/html/index.html)
 
 ## License
 
 Licensed under [Apache 2.0](https://github.com/AstraZeneca/KAZU/blob/main/LICENSE).
 
 Kazu includes elements under compatible licenses (full licenses are in relevant files or as indicated):
-- Some elements are a modification of code licensed under MIT by Explosion.AI - see the README [here](https://github.com/AstraZeneca/KAZU/blob/main/kazu/modelling/ontology_matching/README.md).
+- Some elements are a modification of code licensed under MIT by Explosion.AI - see the README [here](https://github.com/AstraZeneca/KAZU/blob/main/kazu/ontology_matching/README.md).
 - The doc build process (conf.py's linkcode_resolve function) uses code modified from pandas, in turn modified from numpy. See [PANDAS_LICENSE.txt](https://github.com/AstraZeneca/KAZU/blob/main/docs/PANDAS_LICENSE.txt) and [NUMPY_LICENSE.txt](https://github.com/AstraZeneca/KAZU/blob/main/docs/NUMPY_LICENSE.txt)
 - Elements of the model distillation code are inspired by or modified from Huawei Noah's Ark Lab [TinyBERT](https://github.com/huawei-noah/Pretrained-Language-Model/blob/master/TinyBERT) and DMIS-Lab's [BioBERT](https://github.com/dmis-lab/biobert/tree/master).
   See the details in dataprocessor.py, models.py and tiny_transformer.py.
 - PLSapbertModel is inspired by the code from [sapbert](https://github.com/cambridgeltl/sapbert), licensed under MIT. See the file for details, and see the [SapBert](#sapbert) section below regarding use of the model.
 - GildaUtils in the string_normalizer.py file is modified from [Gilda](https://github.com/indralab/gilda). See the file for full details
   including the full BSD 2-Clause license.
 - The AbbreviationFinderStep uses KazuAbbreviationDetector, which is a modified version of
```

