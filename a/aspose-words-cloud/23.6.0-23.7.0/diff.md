# Comparing `tmp/aspose-words-cloud-23.6.0.tar.gz` & `tmp/aspose-words-cloud-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aspose-words-cloud-23.6.0.tar", last modified: Fri Jul 14 07:46:02 2023, max compression
+gzip compressed data, was "dist/aspose-words-cloud-23.7.0.tar", last modified: Mon Jul 24 08:59:22 2023, max compression
```

## Comparing `aspose-words-cloud-23.6.0.tar` & `aspose-words-cloud-23.7.0.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-14 07:45:24.000000 aspose-words-cloud-23.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12600 2023-07-14 07:45:24.000000 aspose-words-cloud-23.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/test/
--rw-r--r--   0 root         (0) root         (0)     3484 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/base_test_context.py
--rw-r--r--   0 root         (0) root         (0)     9634 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_batch.py
--rw-r--r--   0 root         (0) root         (0)     3318 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_url_encode.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_doc_with_password.py
--rw-r--r--   0 root         (0) root         (0)     4054 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_readme.py
--rw-r--r--   0 root         (0) root         (0)    13836 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2228 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/
--rw-r--r--   0 root         (0) root         (0)    11024 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_apply.py
--rw-r--r--   0 root         (0) root         (0)    45668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/jpeg_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_response.py
--rw-r--r--   0 root         (0) root         (0)     5562 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_insert.py
--rw-r--r--   0 root         (0) root         (0)     6354 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_response.py
--rw-r--r--   0 root         (0) root         (0)     8614 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/csv_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bmp_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    24397 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/word_ml_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6694 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_response.py
--rw-r--r--   0 root         (0) root         (0)     6444 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_levels.py
--rw-r--r--   0 root         (0) root         (0)     6538 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_response.py
--rw-r--r--   0 root         (0) root         (0)     6915 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_response.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/lists_response.py
--rw-r--r--   0 root         (0) root         (0)    14309 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_insert.py
--rw-r--r--   0 root         (0) root         (0)     6411 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_collection.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object_response.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/fields_response.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry_list.py
--rw-r--r--   0 root         (0) root         (0)    27747 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/dot_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     8827 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry.py
--rw-r--r--   0 root         (0) root         (0)    23377 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style.py
--rw-r--r--   0 root         (0) root         (0)     7026 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_link.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/dotx_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    50657 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tiff_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/save_response.py
--rw-r--r--   0 root         (0) root         (0)     6292 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_response.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_response.py
--rw-r--r--   0 root         (0) root         (0)    76376 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/epub_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_list_format_response.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/new_document_position.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xml_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)     8924 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_update.py
--rw-r--r--   0 root         (0) root         (0)    28013 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/ott_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7126 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell.py
--rw-r--r--   0 root         (0) root         (0)     6550 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_collection.py
--rw-r--r--   0 root         (0) root         (0)     6767 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert_dto.py
--rw-r--r--   0 root         (0) root         (0)     4838 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_dto.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks_response.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_outline_level_data.py
--rw-r--r--   0 root         (0) root         (0)    13381 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_update.py
--rw-r--r--   0 root         (0) root         (0)    34808 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_update.py
--rw-r--r--   0 root         (0) root         (0)     7124 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph.py
--rw-r--r--   0 root         (0) root         (0)     6565 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_response.py
--rw-r--r--   0 root         (0) root         (0)     7537 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_result.py
--rw-r--r--   0 root         (0) root         (0)    19100 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format.py
--rw-r--r--   0 root         (0) root         (0)     7099 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tags_response.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_response.py
--rw-r--r--   0 root         (0) root         (0)     6643 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_page_setup_response.py
--rw-r--r--   0 root         (0) root         (0)     6496 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink_response.py
--rw-r--r--   0 root         (0) root         (0)     8434 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field.py
--rw-r--r--   0 root         (0) root         (0)     9407 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer.py
--rw-r--r--   0 root         (0) root         (0)     6524 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stops_response.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_response.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_response.py
--rw-r--r--   0 root         (0) root         (0)    40523 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/page_setup.py
--rw-r--r--   0 root         (0) root         (0)    28040 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_data.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_response.py
--rw-r--r--   0 root         (0) root         (0)    30577 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/markdown_save_options_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/
--rw-r--r--   0 root         (0) root         (0)     1682 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_header_footer_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_border_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_footnote_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_bookmark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compress_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_list_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compare_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_run_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/protect_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_font_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_fields_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_with_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_row_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_row_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_comment_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_form_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_borders_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/remove_range_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_bookmark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_footnote_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     7176 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_comment_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1693 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_tiff_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/unprotect_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_form_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_border_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_range_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_properties_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/split_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_paragraph_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/copy_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_level_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_watermark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_cell_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_drawing_object_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/append_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/docm_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    32952 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/ps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6525 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comments_collection.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/dotm_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_response.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks.py
--rw-r--r--   0 root         (0) root         (0)     6249 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_link.py
--rw-r--r--   0 root         (0) root         (0)     6248 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xml_color.py
--rw-r--r--   0 root         (0) root         (0)     7024 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_update.py
--rw-r--r--   0 root         (0) root         (0)     6630 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_response.py
--rw-r--r--   0 root         (0) root         (0)    34159 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font_response.py
--rw-r--r--   0 root         (0) root         (0)     6496 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_response.py
--rw-r--r--   0 root         (0) root         (0)     6643 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_collection.py
--rw-r--r--   0 root         (0) root         (0)     7608 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert_dto.py
--rw-r--r--   0 root         (0) root         (0)     5761 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/range_document_dto.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_response.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_link.py
--rw-r--r--   0 root         (0) root         (0)     8999 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/file_link.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/node_link.py
--rw-r--r--   0 root         (0) root         (0)     7697 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data_response.py
--rw-r--r--   0 root         (0) root         (0)    34808 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_insert.py
--rw-r--r--   0 root         (0) root         (0)    16483 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compare_options.py
--rw-r--r--   0 root         (0) root         (0)     6817 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/load_web_document_data.py
--rw-r--r--   0 root         (0) root         (0)     8854 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_update.py
--rw-r--r--   0 root         (0) root         (0)     5256 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/report_build_options.py
--rw-r--r--   0 root         (0) root         (0)     6388 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/range_text_response.py
--rw-r--r--   0 root         (0) root         (0)     6773 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)    11839 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/report_engine_settings.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     6389 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_collection.py
--rw-r--r--   0 root         (0) root         (0)     7072 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_insert.py
--rw-r--r--   0 root         (0) root         (0)     5596 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_link.py
--rw-r--r--   0 root         (0) root         (0)     8058 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table.py
--rw-r--r--   0 root         (0) root         (0)     6730 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert.py
--rw-r--r--   0 root         (0) root         (0)     6721 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/modification_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     6810 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_collection.py
--rw-r--r--   0 root         (0) root         (0)    17850 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_checkbox.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)     5736 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/range_document.py
--rw-r--r--   0 root         (0) root         (0)     5739 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/story_child_nodes.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_collection.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link.py
--rw-r--r--   0 root         (0) root         (0)     6691 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_response.py
--rw-r--r--   0 root         (0) root         (0)     6366 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_link.py
--rw-r--r--   0 root         (0) root         (0)     8453 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/downsample_options_data.py
--rw-r--r--   0 root         (0) root         (0)    10167 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_digital_signature_details_data.py
--rw-r--r--   0 root         (0) root         (0)     6775 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_objects_response.py
--rw-r--r--   0 root         (0) root         (0)    10074 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format.py
--rw-r--r--   0 root         (0) root         (0)     7673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/save_result.py
--rw-r--r--   0 root         (0) root         (0)     8245 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_insert.py
--rw-r--r--   0 root         (0) root         (0)    36909 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/open_xps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6397 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/optimization_options.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range_dto.py
--rw-r--r--   0 root         (0) root         (0)    12026 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/styles_response.py
--rw-r--r--   0 root         (0) root         (0)     5795 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data.py
--rw-r--r--   0 root         (0) root         (0)    28658 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_macro_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     5915 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry.py
--rw-r--r--   0 root         (0) root         (0)    11051 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compress_response.py
--rw-r--r--   0 root         (0) root         (0)    28017 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/odt_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6117 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_update.py
--rw-r--r--   0 root         (0) root         (0)    16964 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_drop_down.py
--rw-r--r--   0 root         (0) root         (0)    12508 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_info.py
--rw-r--r--   0 root         (0) root         (0)     8786 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/classification_response.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_response.py
--rw-r--r--   0 root         (0) root         (0)     9566 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compare_data.py
--rw-r--r--   0 root         (0) root         (0)    28036 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/rtf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6468 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/watermark_text.py
--rw-r--r--   0 root         (0) root         (0)     8079 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_property.py
--rw-r--r--   0 root         (0) root         (0)     6220 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/info_additional_item.py
--rw-r--r--   0 root         (0) root         (0)     6350 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/borders_collection.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_collection.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/classification_result.py
--rw-r--r--   0 root         (0) root         (0)    75129 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/html_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    34704 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_fixed_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6770 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comments_response.py
--rw-r--r--   0 root         (0) root         (0)    38869 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/svg_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    28886 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/gif_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/borders_response.py
--rw-r--r--   0 root         (0) root         (0)     6773 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footers_response.py
--rw-r--r--   0 root         (0) root         (0)    36496 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    18821 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_level.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_insert.py
--rw-r--r--   0 root         (0) root         (0)    67826 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     5704 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_copy.py
--rw-r--r--   0 root         (0) root         (0)    17661 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object.py
--rw-r--r--   0 root         (0) root         (0)     6846 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/revisions_modification_response.py
--rw-r--r--   0 root         (0) root         (0)     7998 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/info_response.py
--rw-r--r--   0 root         (0) root         (0)     6618 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_update.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_insert.py
--rw-r--r--   0 root         (0) root         (0)    28275 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_response.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/png_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark.py
--rw-r--r--   0 root         (0) root         (0)    19338 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_text_input.py
--rw-r--r--   0 root         (0) root         (0)     6519 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_response.py
--rw-r--r--   0 root         (0) root         (0)     4792 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font_dto.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/user_information.py
--rw-r--r--   0 root         (0) root         (0)     7530 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_response.py
--rw-r--r--   0 root         (0) root         (0)     9717 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section.py
--rw-r--r--   0 root         (0) root         (0)    19476 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6372 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/runs_response.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert_dto.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_update.py
--rw-r--r--   0 root         (0) root         (0)     8412 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/time_zone_info_data.py
--rw-r--r--   0 root         (0) root         (0)     7456 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/protection_request.py
--rw-r--r--   0 root         (0) root         (0)    12430 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/metafile_rendering_options_data.py
--rw-r--r--   0 root         (0) root         (0)    10029 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_parameters.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/search_response.py
--rw-r--r--   0 root         (0) root         (0)     6607 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/search_results_collection.py
--rw-r--r--   0 root         (0) root         (0)     6668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_response.py
--rw-r--r--   0 root         (0) root         (0)    16738 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_level_update.py
--rw-r--r--   0 root         (0) root         (0)     6785 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_response.py
--rw-r--r--   0 root         (0) root         (0)     4808 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/file_reference.py
--rw-r--r--   0 root         (0) root         (0)     4837 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_dto.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_base.py
--rw-r--r--   0 root         (0) root         (0)     7559 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert.py
--rw-r--r--   0 root         (0) root         (0)    50559 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/html_fixed_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6751 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/runs.py
--rw-r--r--   0 root         (0) root         (0)     6382 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)    12966 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/outline_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_position.py
--rw-r--r--   0 root         (0) root         (0)    11766 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/border.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/
--rw-r--r--   0 root         (0) root         (0)     7318 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_request.py
--rw-r--r--   0 root         (0) root         (0)     7213 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5688 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_request.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_request.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py
--rw-r--r--   0 root         (0) root         (0)     6117 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_request.py
--rw-r--r--   0 root         (0) root         (0)     6286 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     5458 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5415 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     5591 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6908 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_request.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5332 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_request.py
--rw-r--r--   0 root         (0) root         (0)     7739 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_file_request.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6917 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_request.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_file_request.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7102 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7206 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_request.py
--rw-r--r--   0 root         (0) root         (0)     7118 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_request.py
--rw-r--r--   0 root         (0) root         (0)     8132 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7036 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7473 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6222 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7179 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6063 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_request.py
--rw-r--r--   0 root         (0) root         (0)     6355 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_request.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7627 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     5477 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_request.py
--rw-r--r--   0 root         (0) root         (0)     7849 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     6040 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_request.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/load_web_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5383 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py
--rw-r--r--   0 root         (0) root         (0)     7324 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_request.py
--rw-r--r--   0 root         (0) root         (0)     7750 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_request.py
--rw-r--r--   0 root         (0) root         (0)     7780 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_request.py
--rw-r--r--   0 root         (0) root         (0)     4231 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_request.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5654 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7448 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_request.py
--rw-r--r--   0 root         (0) root         (0)     6449 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6286 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7068 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_request.py
--rw-r--r--   0 root         (0) root         (0)     6175 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7816 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5961 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6076 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5467 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7658 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7814 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6220 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_with_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     4223 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_request.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_request.py
--rw-r--r--   0 root         (0) root         (0)     6856 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_request.py
--rw-r--r--   0 root         (0) root         (0)     7881 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7747 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_request.py
--rw-r--r--   0 root         (0) root         (0)     7996 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6462 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7021 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_request.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6364 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_request.py
--rw-r--r--   0 root         (0) root         (0)     7943 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7280 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/batch_request.py
--rw-r--r--   0 root         (0) root         (0)     7153 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7621 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7260 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_request.py
--rw-r--r--   0 root         (0) root         (0)     7124 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_request.py
--rw-r--r--   0 root         (0) root         (0)     8072 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5648 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5719 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_request.py
--rw-r--r--   0 root         (0) root         (0)     7954 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_request.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     8062 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_request.py
--rw-r--r--   0 root         (0) root         (0)     6345 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     7109 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6040 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_request.py
--rw-r--r--   0 root         (0) root         (0)    10973 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_request.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_info_request.py
--rw-r--r--   0 root         (0) root         (0)     7711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7667 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_request.py
--rw-r--r--   0 root         (0) root         (0)     5194 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7168 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_request.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_request.py
--rw-r--r--   0 root         (0) root         (0)     6429 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7091 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     6392 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6325 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_request.py
--rw-r--r--   0 root         (0) root         (0)     5851 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6185 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_request.py
--rw-r--r--   0 root         (0) root         (0)     4747 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     7910 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     6410 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py
--rw-r--r--   0 root         (0) root         (0)     7849 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     5738 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6910 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     5959 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7519 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_request.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/download_file_request.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7039 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7479 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7064 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_request.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_request.py
--rw-r--r--   0 root         (0) root         (0)     7860 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7029 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7915 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_request.py
--rw-r--r--   0 root         (0) root         (0)     6138 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7630 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7724 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py
--rw-r--r--   0 root         (0) root         (0)     7766 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5732 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_request.py
--rw-r--r--   0 root         (0) root         (0)     6984 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5641 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_request.py
--rw-r--r--   0 root         (0) root         (0)     6765 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_request.py
--rw-r--r--   0 root         (0) root         (0)     8009 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7152 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7251 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6208 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7417 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5783 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_request.py
--rw-r--r--   0 root         (0) root         (0)     5119 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7200 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)    33549 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6173 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     7082 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6135 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_request.py
--rw-r--r--   0 root         (0) root         (0)     5734 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_request.py
--rw-r--r--   0 root         (0) root         (0)     7165 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py
--rw-r--r--   0 root         (0) root         (0)     6081 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7568 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5849 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py
--rw-r--r--   0 root         (0) root         (0)    10926 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5498 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7559 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     7051 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6994 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_styles_from_template_request.py
--rw-r--r--   0 root         (0) root         (0)     6191 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7122 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reset_cache_request.py
--rw-r--r--   0 root         (0) root         (0)     6478 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_request.py
--rw-r--r--   0 root         (0) root         (0)     7779 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     5648 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6951 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py
--rw-r--r--   0 root         (0) root         (0)     5783 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_request.py
--rw-r--r--   0 root         (0) root         (0)     5162 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6839 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_request.py
--rw-r--r--   0 root         (0) root         (0)     5511 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     7592 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6264 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5989 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6910 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7149 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5174 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7901 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_request.py
--rw-r--r--   0 root         (0) root         (0)     7784 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     7840 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py
--rw-r--r--   0 root         (0) root         (0)     5316 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_request.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5150 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     5853 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5695 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7946 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8351 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_request.py
--rw-r--r--   0 root         (0) root         (0)     7903 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8154 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7596 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6637 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6443 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_request.py
--rw-r--r--   0 root         (0) root         (0)     7011 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7146 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_request.py
--rw-r--r--   0 root         (0) root         (0)     7483 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py
--rw-r--r--   0 root         (0) root         (0)     7112 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     3695 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_available_fonts_request.py
--rw-r--r--   0 root         (0) root         (0)     6917 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7241 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/base_request_object.py
--rw-r--r--   0 root         (0) root         (0)     5903 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7005 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_files_list_request.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5750 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_request.py
--rw-r--r--   0 root         (0) root         (0)     6961 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7136 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5552 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7707 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     5854 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/convert_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6118 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5779 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6135 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7001 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5095 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_request.py
--rw-r--r--   0 root         (0) root         (0)     6080 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     8051 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5957 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7269 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_request.py
--rw-r--r--   0 root         (0) root         (0)     7098 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_request.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6397 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5652 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6079 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7390 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     5537 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     7555 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_request.py
--rw-r--r--   0 root         (0) root         (0)     5617 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_request.py
--rw-r--r--   0 root         (0) root         (0)     8359 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7412 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6374 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_request.py
--rw-r--r--   0 root         (0) root         (0)     5933 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6255 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6159 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py
--rw-r--r--   0 root         (0) root         (0)     7161 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5165 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6969 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     7013 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6171 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py
--rw-r--r--   0 root         (0) root         (0)     6884 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_request.py
--rw-r--r--   0 root         (0) root         (0)     4877 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/upload_file_request.py
--rw-r--r--   0 root         (0) root         (0)     8075 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_request.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_public_key_request.py
--rw-r--r--   0 root         (0) root         (0)     6036 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6541 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5435 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7557 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_file_request.py
--rw-r--r--   0 root         (0) root         (0)     5420 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_request.py
--rw-r--r--   0 root         (0) root         (0)     7506 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_request.py
--rw-r--r--   0 root         (0) root         (0)     6791 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7308 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7284 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)    29269 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_format_update.py
--rw-r--r--   0 root         (0) root         (0)     5744 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_create_or_update.py
--rw-r--r--   0 root         (0) root         (0)    25901 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/emf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    43767 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_base.py
--rw-r--r--   0 root         (0) root         (0)     9470 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/shading.py
--rw-r--r--   0 root         (0) root         (0)     9094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_link.py
--rw-r--r--   0 root         (0) root         (0)    43991 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_update.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/public_key_response.py
--rw-r--r--   0 root         (0) root         (0)     7603 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_insert.py
--rw-r--r--   0 root         (0) root         (0)     6617 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_names_response.py
--rw-r--r--   0 root         (0) root         (0)     6774 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/docx_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     9741 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_update.py
--rw-r--r--   0 root         (0) root         (0)     7475 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/stat_data_response.py
--rw-r--r--   0 root         (0) root         (0)     6881 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_link.py
--rw-r--r--   0 root         (0) root         (0)     6626 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_fields_response.py
--rw-r--r--   0 root         (0) root         (0)    45246 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format.py
--rw-r--r--   0 root         (0) root         (0)     6437 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/lists.py
--rw-r--r--   0 root         (0) root         (0)     8308 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_format.py
--rw-r--r--   0 root         (0) root         (0)     6992 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_response.py
--rw-r--r--   0 root         (0) root         (0)     8924 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_insert.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_response.py
--rw-r--r--   0 root         (0) root         (0)     6527 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6939 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part.py
--rw-r--r--   0 root         (0) root         (0)    34298 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pcl_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_insert.py
--rw-r--r--   0 root         (0) root         (0)     6884 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/preferred_width.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)    33416 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/text_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    48113 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font.py
--rw-r--r--   0 root         (0) root         (0)     6382 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/border_response.py
--rw-r--r--   0 root         (0) root         (0)     6903 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     5788 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert.py
--rw-r--r--   0 root         (0) root         (0)     6869 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_list_item.py
--rw-r--r--   0 root         (0) root         (0)     8182 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font_info.py
--rw-r--r--   0 root         (0) root         (0)     6317 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_names.py
--rw-r--r--   0 root         (0) root         (0)     6694 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6280 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_link.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/link.py
--rw-r--r--   0 root         (0) root         (0)     7024 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_insert.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_response.py
--rw-r--r--   0 root         (0) root         (0)     8461 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     6712 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_stat_data.py
--rw-r--r--   0 root         (0) root         (0)     8043 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row.py
--rw-r--r--   0 root         (0) root         (0)    19951 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_options.py
--rw-r--r--   0 root         (0) root         (0)    27751 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/doc_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_permissions.py
--rw-r--r--   0 root         (0) root         (0)     6362 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_response.py
--rw-r--r--   0 root         (0) root         (0)     9736 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/page_number.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_response.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     6595 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     8974 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/available_fonts_response.py
--rw-r--r--   0 root         (0) root         (0)     4834 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_dto.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/search_result.py
--rw-r--r--   0 root         (0) root         (0)     8534 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/page_stat_data.py
--rw-r--r--   0 root         (0) root         (0)    25627 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     9840 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/json_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_link.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compress_options.py
--rw-r--r--   0 root         (0) root         (0)    76949 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/mhtml_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run.py
--rw-r--r--   0 root         (0) root         (0)     5648 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/words_response.py
--rw-r--r--   0 root         (0) root         (0)    11010 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/link_element.py
--rw-r--r--   0 root         (0) root         (0)     7902 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_encryption_details_data.py
--rw-r--r--   0 root         (0) root         (0)     9741 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_insert.py
--rw-r--r--   0 root         (0) root         (0)     6322 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_link.py
--rw-r--r--   0 root         (0) root         (0)     8156 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry_list.py
--rw-r--r--   0 root         (0) root         (0)    14358 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field.py
--rw-r--r--   0 root         (0) root         (0)     9637 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_stat_data.py
--rw-r--r--   0 root         (0) root         (0)    11506 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/rest.py
--rw-r--r--   0 root         (0) root         (0)    19684 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9423 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/apis/
--rw-r--r--   0 root         (0) root         (0)  1380535 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/apis/words_api.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    39456 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    13836 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12600 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/test/
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/base_test_context.py
+-rw-r--r--   0 root         (0) root         (0)     9634 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/test_batch.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/test_url_encode.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/test_doc_with_password.py
+-rw-r--r--   0 root         (0) root         (0)     4054 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/test/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)    13836 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/asposewordscloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/
+-rw-r--r--   0 root         (0) root         (0)    11024 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/style_apply.py
+-rw-r--r--   0 root         (0) root         (0)    45668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/jpeg_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6788 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_parts_response.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6354 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_response.py
+-rw-r--r--   0 root         (0) root         (0)     8614 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/csv_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bmp_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    24397 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/word_ml_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6694 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_response.py
+-rw-r--r--   0 root         (0) root         (0)     6444 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_levels.py
+-rw-r--r--   0 root         (0) root         (0)     6538 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmarks_response.py
+-rw-r--r--   0 root         (0) root         (0)     6915 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/lists_response.py
+-rw-r--r--   0 root         (0) root         (0)    14309 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_object_response.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/fields_response.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/image_entry_list.py
+-rw-r--r--   0 root         (0) root         (0)    27747 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/dot_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_entry.py
+-rw-r--r--   0 root         (0) root         (0)    23377 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/style.py
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_link.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/dotx_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    50657 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/tiff_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/save_response.py
+-rw-r--r--   0 root         (0) root         (0)     6292 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/run_response.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_response.py
+-rw-r--r--   0 root         (0) root         (0)    76376 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/epub_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_list_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/new_document_position.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/xml_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_update.py
+-rw-r--r--   0 root         (0) root         (0)    28013 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/ott_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell.py
+-rw-r--r--   0 root         (0) root         (0)     6550 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_objects_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6767 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_insert_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_format_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlinks_response.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmarks_outline_level_data.py
+-rw-r--r--   0 root         (0) root         (0)    13381 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_update.py
+-rw-r--r--   0 root         (0) root         (0)    34808 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_update.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph.py
+-rw-r--r--   0 root         (0) root         (0)     6565 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnotes_response.py
+-rw-r--r--   0 root         (0) root         (0)     7537 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/split_document_result.py
+-rw-r--r--   0 root         (0) root         (0)    19100 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_format.py
+-rw-r--r--   0 root         (0) root         (0)     7099 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tags_response.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/section_page_setup_response.py
+-rw-r--r--   0 root         (0) root         (0)     6496 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlink_response.py
+-rw-r--r--   0 root         (0) root         (0)     8434 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field.py
+-rw-r--r--   0 root         (0) root         (0)     9407 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer.py
+-rw-r--r--   0 root         (0) root         (0)     6524 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stops_response.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_response.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_response.py
+-rw-r--r--   0 root         (0) root         (0)    40523 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/page_setup.py
+-rw-r--r--   0 root         (0) root         (0)    28040 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark_data.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comment_response.py
+-rw-r--r--   0 root         (0) root         (0)    30577 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/markdown_save_options_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_header_footer_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_border_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_footnote_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_bookmark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/save_as_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/compress_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_list_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/compare_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_run_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/protect_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_table_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_run_font_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_fields_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/replace_with_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/replace_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_table_row_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_table_row_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_comment_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_form_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_borders_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/remove_range_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_bookmark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_footnote_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     7176 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_comment_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_run_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/save_as_tiff_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_list_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/unprotect_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_form_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_border_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/save_as_range_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_table_properties_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/split_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_paragraph_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/copy_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_list_level_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_watermark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_table_cell_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_drawing_object_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/append_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/docm_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    32952 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/ps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6525 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comments_collection.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/dotm_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark_response.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stop.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlinks.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_link.py
+-rw-r--r--   0 root         (0) root         (0)     6248 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/xml_color.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_update.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer_response.py
+-rw-r--r--   0 root         (0) root         (0)    34159 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/font_response.py
+-rw-r--r--   0 root         (0) root         (0)     6496 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_response.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7608 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_insert_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5761 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/range_document_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_response.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comment_link.py
+-rw-r--r--   0 root         (0) root         (0)     8999 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/file_link.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/node_link.py
+-rw-r--r--   0 root         (0) root         (0)     7697 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/protection_data_response.py
+-rw-r--r--   0 root         (0) root         (0)    34808 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_insert.py
+-rw-r--r--   0 root         (0) root         (0)    16483 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/compare_options.py
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/load_web_document_data.py
+-rw-r--r--   0 root         (0) root         (0)     8854 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/style_update.py
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/report_build_options.py
+-rw-r--r--   0 root         (0) root         (0)     6388 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/range_text_response.py
+-rw-r--r--   0 root         (0) root         (0)     6773 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)    11839 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/report_engine_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/words_api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     6389 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7072 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/style_insert.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_link.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table.py
+-rw-r--r--   0 root         (0) root         (0)     6730 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/modification_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     6810 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_parts_collection.py
+-rw-r--r--   0 root         (0) root         (0)    17850 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/section_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/range_document.py
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/story_child_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_link.py
+-rw-r--r--   0 root         (0) root         (0)     6691 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/split_document_response.py
+-rw-r--r--   0 root         (0) root         (0)     6366 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_link.py
+-rw-r--r--   0 root         (0) root         (0)     8453 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/downsample_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    10167 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_digital_signature_details_data.py
+-rw-r--r--   0 root         (0) root         (0)     6775 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)    10074 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_format.py
+-rw-r--r--   0 root         (0) root         (0)     7673 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/save_result.py
+-rw-r--r--   0 root         (0) root         (0)     8245 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stop_insert.py
+-rw-r--r--   0 root         (0) root         (0)    36909 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/open_xps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6397 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/optimization_options.py
+-rw-r--r--   0 root         (0) root         (0)     6788 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/replace_range_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12026 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_object.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/styles_response.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/protection_data.py
+-rw-r--r--   0 root         (0) root         (0)    28658 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_macro_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     5915 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/image_entry.py
+-rw-r--r--   0 root         (0) root         (0)    11051 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comment.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/compress_response.py
+-rw-r--r--   0 root         (0) root         (0)    28017 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/odt_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_update.py
+-rw-r--r--   0 root         (0) root         (0)    16964 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_drop_down.py
+-rw-r--r--   0 root         (0) root         (0)    12508 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_info.py
+-rw-r--r--   0 root         (0) root         (0)     8786 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/classification_response.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     9566 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/compare_data.py
+-rw-r--r--   0 root         (0) root         (0)    28036 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/rtf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/watermark_text.py
+-rw-r--r--   0 root         (0) root         (0)     8079 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_property.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/info_additional_item.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/borders_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6335 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/classification_result.py
+-rw-r--r--   0 root         (0) root         (0)    75129 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/html_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    34704 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/xaml_fixed_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6770 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comments_response.py
+-rw-r--r--   0 root         (0) root         (0)    38869 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/svg_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    28886 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_template_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/gif_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/borders_response.py
+-rw-r--r--   0 root         (0) root         (0)     6773 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/header_footers_response.py
+-rw-r--r--   0 root         (0) root         (0)    36496 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/xps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    18821 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_level.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/run_insert.py
+-rw-r--r--   0 root         (0) root         (0)    67826 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     5704 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/style_copy.py
+-rw-r--r--   0 root         (0) root         (0)    17661 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object.py
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/revisions_modification_response.py
+-rw-r--r--   0 root         (0) root         (0)     7998 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/info_response.py
+-rw-r--r--   0 root         (0) root         (0)     6618 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_update.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_insert.py
+-rw-r--r--   0 root         (0) root         (0)    28275 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/style_response.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/png_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark.py
+-rw-r--r--   0 root         (0) root         (0)    19338 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_text_input.py
+-rw-r--r--   0 root         (0) root         (0)     6519 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_response.py
+-rw-r--r--   0 root         (0) root         (0)     4792 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/font_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/user_information.py
+-rw-r--r--   0 root         (0) root         (0)     7530 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/replace_text_response.py
+-rw-r--r--   0 root         (0) root         (0)     9717 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/section.py
+-rw-r--r--   0 root         (0) root         (0)    19476 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6372 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/runs_response.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_insert_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/run_update.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/time_zone_info_data.py
+-rw-r--r--   0 root         (0) root         (0)     7456 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/protection_request.py
+-rw-r--r--   0 root         (0) root         (0)    12430 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/metafile_rendering_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/replace_text_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/search_response.py
+-rw-r--r--   0 root         (0) root         (0)     6607 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/search_results_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_response.py
+-rw-r--r--   0 root         (0) root         (0)    16738 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_level_update.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_property_response.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/file_reference.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_properties_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stop_base.py
+-rw-r--r--   0 root         (0) root         (0)     7559 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_insert.py
+-rw-r--r--   0 root         (0) root         (0)    50559 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/html_fixed_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/replace_range.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/runs.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)    12966 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/outline_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_position.py
+-rw-r--r--   0 root         (0) root         (0)    11766 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/border.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_page_numbers_request.py
+-rw-r--r--   0 root         (0) root         (0)     7213 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/append_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraphs_request.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     6286 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     5458 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/build_report_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     5591 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6908 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comments_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmarks_request.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comments_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5332 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comments_request.py
+-rw-r--r--   0 root         (0) root         (0)     7739 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_section_page_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/move_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6917 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/build_report_request.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/split_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7206 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_range_request.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_borders_request.py
+-rw-r--r--   0 root         (0) root         (0)     8132 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7036 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7473 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_with_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_statistics_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7179 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_from_document_element_request.py
+-rw-r--r--   0 root         (0) root         (0)     6355 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7627 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6977 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_watermark_request.py
+-rw-r--r--   0 root         (0) root         (0)     7849 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/load_web_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_borders_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5383 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py
+-rw-r--r--   0 root         (0) root         (0)     7324 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     7750 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     7780 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_tables_request.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/classify_request.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_runs_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_image_request.py
+-rw-r--r--   0 root         (0) root         (0)     6449 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/protect_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6286 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5431 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7068 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7816 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraphs_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7658 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7814 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_with_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_protection_request.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_lists_request.py
+-rw-r--r--   0 root         (0) root         (0)     6856 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_field_names_request.py
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7747 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     7996 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_row_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6462 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/unprotect_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7021 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_lists_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_macros_request.py
+-rw-r--r--   0 root         (0) root         (0)     7943 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/batch_request.py
+-rw-r--r--   0 root         (0) root         (0)     7153 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7260 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     8072 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_row_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7916 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     7954 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     8062 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_level_request.py
+-rw-r--r--   0 root         (0) root         (0)     6345 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     7109 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_field_request.py
+-rw-r--r--   0 root         (0) root         (0)    10973 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_tiff_request.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/optimize_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_info_request.py
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_office_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_page_request.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_request.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compress_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compress_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6325 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_font_request.py
+-rw-r--r--   0 root         (0) root         (0)     5851 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6185 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footers_request.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/move_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     7910 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6665 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py
+-rw-r--r--   0 root         (0) root         (0)     7849 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5711 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6910 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     5959 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7519 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/download_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_page_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7039 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     7860 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7029 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7915 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     6138 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7724 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6916 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compare_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py
+-rw-r--r--   0 root         (0) root         (0)     7766 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5732 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tags_request.py
+-rw-r--r--   0 root         (0) root         (0)     6984 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/remove_range_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnotes_request.py
+-rw-r--r--   0 root         (0) root         (0)     6765 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_borders_request.py
+-rw-r--r--   0 root         (0) root         (0)     8009 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7152 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/append_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6208 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7417 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/accept_all_revisions_request.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmarks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7200 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)    33549 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_macros_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6659 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/search_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmarks_request.py
+-rw-r--r--   0 root         (0) root         (0)     7165 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7568 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5849 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py
+-rw-r--r--   0 root         (0) root         (0)    10926 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_tiff_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5498 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7559 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_page_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     7051 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6994 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_styles_from_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/reset_cache_request.py
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_range_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     7779 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/reject_all_revisions_request.py
+-rw-r--r--   0 root         (0) root         (0)     5162 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6793 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6839 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/remove_range_request.py
+-rw-r--r--   0 root         (0) root         (0)     5511 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     7592 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_range_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6910 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_borders_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7149 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_protection_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7901 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_or_update_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     7840 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py
+-rw-r--r--   0 root         (0) root         (0)     5316 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_styles_request.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_sections_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     5853 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7946 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_level_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8351 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5718 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/search_request.py
+-rw-r--r--   0 root         (0) root         (0)     7903 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6977 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8154 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_cell_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7596 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6637 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_watermark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6443 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_statistics_request.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/optimize_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7146 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     7483 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py
+-rw-r--r--   0 root         (0) root         (0)     7112 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_available_fonts_request.py
+-rw-r--r--   0 root         (0) root         (0)     6917 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7241 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/base_request_object.py
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7005 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_files_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/split_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7136 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_field_names_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7707 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     5854 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/classify_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/convert_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6118 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_font_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compare_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5779 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6793 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_styles_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     8051 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_font_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5957 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_headers_footers_request.py
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6397 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/protect_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7390 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6916 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/execute_mail_merge_request.py
+-rw-r--r--   0 root         (0) root         (0)     5617 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/classify_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_runs_request.py
+-rw-r--r--   0 root         (0) root         (0)     8359 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7412 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comments_request.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6159 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py
+-rw-r--r--   0 root         (0) root         (0)     7161 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_range_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5165 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6969 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/unprotect_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6171 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/upload_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     8075 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_font_request.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_public_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6541 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5435 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_tables_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7557 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnotes_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_sections_request.py
+-rw-r--r--   0 root         (0) root         (0)     7506 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_with_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7308 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)    29269 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_format_update.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_property_create_or_update.py
+-rw-r--r--   0 root         (0) root         (0)    25901 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/emf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    43767 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format_base.py
+-rw-r--r--   0 root         (0) root         (0)     9470 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/shading.py
+-rw-r--r--   0 root         (0) root         (0)     9094 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/words_api_link.py
+-rw-r--r--   0 root         (0) root         (0)    43991 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format_update.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/public_key_response.py
+-rw-r--r--   0 root         (0) root         (0)     7603 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_names_response.py
+-rw-r--r--   0 root         (0) root         (0)     6774 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer_link.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/docx_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comment_update.py
+-rw-r--r--   0 root         (0) root         (0)     7475 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/stat_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/run_link.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_fields_response.py
+-rw-r--r--   0 root         (0) root         (0)    45246 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format.py
+-rw-r--r--   0 root         (0) root         (0)     6437 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/bookmarks.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/lists.py
+-rw-r--r--   0 root         (0) root         (0)     8308 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/list_format.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_response.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_response.py
+-rw-r--r--   0 root         (0) root         (0)     6527 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part.py
+-rw-r--r--   0 root         (0) root         (0)    34298 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/pcl_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/preferred_width.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)    33416 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/text_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    48113 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/font.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/border_response.py
+-rw-r--r--   0 root         (0) root         (0)     6903 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     5788 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6869 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_list_item.py
+-rw-r--r--   0 root         (0) root         (0)     8182 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/font_info.py
+-rw-r--r--   0 root         (0) root         (0)     6317 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_names.py
+-rw-r--r--   0 root         (0) root         (0)     6694 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/section_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_link.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     8461 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnotes_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)     8043 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row.py
+-rw-r--r--   0 root         (0) root         (0)    19951 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/field_options.py
+-rw-r--r--   0 root         (0) root         (0)    27751 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/doc_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlink.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     6362 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_response.py
+-rw-r--r--   0 root         (0) root         (0)     9736 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/page_number.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/section_response.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/available_fonts_response.py
+-rw-r--r--   0 root         (0) root         (0)     4834 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_format_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/search_result.py
+-rw-r--r--   0 root         (0) root         (0)     8534 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/page_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)    25627 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/xaml_flow_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/json_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/section_link.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/compress_options.py
+-rw-r--r--   0 root         (0) root         (0)    76949 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/mhtml_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/run.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/words_response.py
+-rw-r--r--   0 root         (0) root         (0)    11010 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/footnote.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/link_element.py
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_encryption_details_data.py
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/comment_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6322 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_link.py
+-rw-r--r--   0 root         (0) root         (0)     8156 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_entry_list.py
+-rw-r--r--   0 root         (0) root         (0)    14358 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/form_field.py
+-rw-r--r--   0 root         (0) root         (0)     9637 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/models/document_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)    11506 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/rest.py
+-rw-r--r--   0 root         (0) root         (0)    19684 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/asposewordscloud/apis/
+-rw-r--r--   0 root         (0) root         (0)  1380535 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/apis/words_api.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30710 2023-07-24 08:58:50.000000 aspose-words-cloud-23.7.0/asposewordscloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    39456 2023-07-24 08:59:21.000000 aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-24 08:59:21.000000 aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-24 08:59:21.000000 aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    13836 2023-07-24 08:59:21.000000 aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:59:21.000000 aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 08:59:22.000000 aspose-words-cloud-23.7.0/setup.cfg
```

### Comparing `aspose-words-cloud-23.6.0/LICENSE` & `aspose-words-cloud-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/README.md` & `aspose-words-cloud-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/base_test_context.py` & `aspose-words-cloud-23.7.0/test/base_test_context.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/test_batch.py` & `aspose-words-cloud-23.7.0/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/test_examples.py` & `aspose-words-cloud-23.7.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/__init__.py` & `aspose-words-cloud-23.7.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/test_url_encode.py` & `aspose-words-cloud-23.7.0/test/test_url_encode.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/test_doc_with_password.py` & `aspose-words-cloud-23.7.0/test/test_doc_with_password.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/test/test_readme.py` & `aspose-words-cloud-23.7.0/test/test_readme.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/PKG-INFO` & `aspose-words-cloud-23.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-words-cloud
-Version: 23.6.0
+Version: 23.7.0
 Summary: Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word file generation, manipulation, conversion & inspection features into your own python applications.
 Home-page: https://github.com/aspose-words-cloud/aspose-words-cloud-python
 Author: Yaroslaw Ekimov
 Author-email: yaroslaw.ekimov@aspose.com
 License: UNKNOWN
 Keywords: office,convert,word,pdf,docx,html,rtf,png,jpg,split,merge,edit,word to pdf,pdf to word,docx to pdf,pdf to docx,word to html,html to word,reporting,mailmerge,statistics,watermark,fields,generate,create,report,table,paragraph,images,text,generator,creator,maker
 Platform: UNKNOWN
```

### Comparing `aspose-words-cloud-23.6.0/setup.py` & `aspose-words-cloud-23.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     Aspose.Words for Cloud API Reference
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 23.6
+    OpenAPI spec version: 23.7
 
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "aspose-words-cloud"
-VERSION = "23.6.0"
+VERSION = "23.7.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/style_apply.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/style_apply.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/jpeg_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/jpeg_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_parts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/csv_data_load_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/csv_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bmp_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bmp_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/word_ml_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/word_ml_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_levels.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_levels.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_objects_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/lists_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/lists_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_object_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/fields_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/fields_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry_list.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/image_entry_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/dot_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/dot_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_entry.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/style.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/style.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/dotx_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/dotx_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/tiff_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/tiff_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/save_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/save_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/run_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/run_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/epub_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/epub_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_list_format_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_list_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/new_document_position.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/new_document_position.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/xml_data_load_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/xml_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/ott_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/ott_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_objects_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_insert_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_format_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlinks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_outline_level_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmarks_outline_level_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnotes_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_result.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tags_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tags_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/section_page_setup_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/section_page_setup_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlink_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stops_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stops_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/page_setup.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/page_setup.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comment_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/markdown_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/markdown_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_header_footer_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_header_footer_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_border_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_border_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_footnote_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_footnote_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_bookmark_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_bookmark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/save_as_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compress_document_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/compress_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_list_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_list_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compare_document_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/compare_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_field_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_run_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_run_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/protect_document_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/protect_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_table_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_style_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_font_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_run_font_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_fields_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_fields_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_with_text_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/replace_with_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_text_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/replace_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_row_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_table_row_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_row_format_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_table_row_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_comment_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_comment_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_field_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_form_field_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_form_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_borders_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_borders_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/remove_range_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/remove_range_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_bookmark_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_bookmark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_footnote_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_footnote_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/__init__.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_comment_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_comment_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_run_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_tiff_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/save_as_tiff_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_list_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_style_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/unprotect_document_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/unprotect_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_form_field_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_form_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_border_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_border_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_range_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/save_as_range_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_properties_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_table_properties_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/split_document_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/split_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_paragraph_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_paragraph_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/copy_style_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/copy_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_level_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_list_level_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_watermark_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/delete_watermark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_cell_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_table_cell_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_drawing_object_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/update_drawing_object_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/append_document_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/append_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/docm_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/docm_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/ps_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/ps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comments_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comments_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/dotm_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/dotm_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stop.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/xml_color.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/xml_color.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/font_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/font_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_insert_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/range_document_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/range_document_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comment_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/file_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/file_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/node_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/node_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/protection_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/compare_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/compare_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/load_web_document_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/load_web_document_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/style_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/style_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/report_build_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/report_build_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/range_text_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/range_text_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/report_engine_settings.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/report_engine_settings.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_error_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/words_api_error_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/style_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/style_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/modification_operation_result.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/modification_operation_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_parts_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_checkbox.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_checkbox.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/section_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/range_document.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/range_document.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/story_child_nodes.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/story_child_nodes.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/split_document_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/downsample_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/downsample_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_digital_signature_details_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_digital_signature_details_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_objects_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_objects_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/save_result.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/save_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stop_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/open_xps_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/open_xps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/optimization_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/optimization_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/replace_range_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/styles_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/styles_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/protection_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_macro_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_macro_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/image_entry.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comment.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comment.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/compress_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/compress_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/odt_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/odt_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_drop_down.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_drop_down.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_info.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_info.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/classification_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/classification_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/compare_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/compare_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/rtf_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/rtf_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/watermark_text.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/watermark_text.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_property.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/info_additional_item.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/info_additional_item.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/borders_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/borders_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/classification_result.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/classification_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/html_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/html_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_fixed_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/xaml_fixed_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comments_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comments_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/svg_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/svg_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_template_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/gif_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/gif_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/borders_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/borders_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footers_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/header_footers_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/xps_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/xps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_level.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_level.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/run_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/run_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/style_copy.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/style_copy.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/revisions_modification_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/revisions_modification_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/info_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/info_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/style_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/style_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/png_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/png_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_text_input.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_text_input.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_field_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/font_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/font_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/user_information.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/user_information.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/replace_text_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/section.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/section.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/__init__.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/runs_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/runs_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_insert_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/run_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/run_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/time_zone_info_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/time_zone_info_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/protection_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/protection_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/metafile_rendering_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/metafile_rendering_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_parameters.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/replace_text_parameters.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/search_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/search_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/search_results_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/search_results_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/drawing_object_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_level_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_level_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_property_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/file_reference.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/file_reference.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_properties_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_base.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/tab_stop_base.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/html_fixed_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/html_fixed_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/replace_range.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/runs.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/runs.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/files_upload_result.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/outline_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/outline_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_position.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_position.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/border.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/border.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_page_numbers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/append_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraphs_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_folder_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/build_report_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comments_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmarks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comments_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_section_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_file_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/move_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/build_report_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_file_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/split_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_range_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_borders_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_with_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_statistics_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_from_document_element_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_watermark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/load_web_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/load_web_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_borders_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_tables_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/classify_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_runs_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_image_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/protect_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraphs_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_with_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_with_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_protection_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_folder_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_lists_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_field_names_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_row_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/unprotect_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_lists_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_macros_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/batch_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/batch_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_row_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_level_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_tiff_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/optimize_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_info_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_info_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_office_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_page_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compress_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compress_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_font_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_folder_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/move_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/download_file_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/download_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_page_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compare_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tags_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/remove_range_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnotes_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_borders_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/append_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/accept_all_revisions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmarks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/__init__.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_macros_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/search_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmarks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_tiff_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_styles_from_template_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/copy_styles_from_template_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reset_cache_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/reset_cache_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_range_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/reject_all_revisions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/remove_range_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_range_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_borders_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_protection_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_or_update_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_styles_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_sections_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_list_level_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_folder_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/create_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/search_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_table_cell_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_watermark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_statistics_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/optimize_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_available_fonts_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_available_fonts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/base_request_object.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/base_request_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_files_list_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_files_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/split_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_field_names_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/classify_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/convert_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/convert_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_run_font_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/compare_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_cell_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_paragraph_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_styles_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_font_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_headers_footers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/protect_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_form_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/execute_mail_merge_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/classify_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_runs_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_comments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_office_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/save_as_range_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/unprotect_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/render_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/upload_file_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_run_font_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_public_key_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_public_key_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_tables_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_file_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_footnotes_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/get_sections_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/replace_with_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_online_request.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/requests/delete_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_format_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_format_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_create_or_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_property_create_or_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/emf_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/emf_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_base.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format_base.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/shading.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/shading.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/words_api_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/public_key_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/public_key_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/error.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmark_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_names_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_names_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/docx_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/docx_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_update.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comment_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/stat_data_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/stat_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/run_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/run_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_fields_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_fields_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/bookmarks.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/lists.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/lists.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/list_format.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/list_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/header_footer_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/pcl_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/pcl_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/preferred_width.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/preferred_width.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/error_details.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/text_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/text_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/font.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/font.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/border_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/border_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_cell_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_list_item.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/structured_document_tag_list_item.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/font_info.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/font_info.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_names.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_names.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/section_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnote_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/custom_xml_part_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/storage_file.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_stat_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnotes_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/field_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/field_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/doc_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/doc_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_permissions.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_permissions.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/page_number.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/page_number.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/files_list.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/section_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/section_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/api_error.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/available_fonts_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/available_fonts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_dto.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/table_row_format_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/search_result.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/search_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/page_stat_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/page_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/xaml_flow_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/json_data_load_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/json_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/section_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/section_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/compress_options.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/compress_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/mhtml_save_options_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/mhtml_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/run.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/run.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/words_response.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/words_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/footnote.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/link_element.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_encryption_details_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/pdf_encryption_details_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_insert.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/comment_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_link.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/office_math_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry_list.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_entry_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/form_field.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/models/document_stat_data.py` & `aspose-words-cloud-23.7.0/asposewordscloud/models/document_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/rest.py` & `aspose-words-cloud-23.7.0/asposewordscloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/__init__.py` & `aspose-words-cloud-23.7.0/asposewordscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/configuration.py` & `aspose-words-cloud-23.7.0/asposewordscloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.6\n"\
-               "SDK Package Version: 23.6".\
+               "Version of the API: 23.7\n"\
+               "SDK Package Version: 23.7".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/apis/words_api.py` & `aspose-words-cloud-23.7.0/asposewordscloud/apis/words_api.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/asposewordscloud/api_client.py` & `aspose-words-cloud-23.7.0/asposewordscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,20 @@
                  cookie=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-version': '23.6'}
+        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-version': '23.7'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 23.6'
+        self.user_agent = 'python sdk 23.7'
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/SOURCES.txt` & `aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/PKG-INFO` & `aspose-words-cloud-23.7.0/aspose_words_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-words-cloud
-Version: 23.6.0
+Version: 23.7.0
 Summary: Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word file generation, manipulation, conversion & inspection features into your own python applications.
 Home-page: https://github.com/aspose-words-cloud/aspose-words-cloud-python
 Author: Yaroslaw Ekimov
 Author-email: yaroslaw.ekimov@aspose.com
 License: UNKNOWN
 Keywords: office,convert,word,pdf,docx,html,rtf,png,jpg,split,merge,edit,word to pdf,pdf to word,docx to pdf,pdf to docx,word to html,html to word,reporting,mailmerge,statistics,watermark,fields,generate,create,report,table,paragraph,images,text,generator,creator,maker
 Platform: UNKNOWN
```

