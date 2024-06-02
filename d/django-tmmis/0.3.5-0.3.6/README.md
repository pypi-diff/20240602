# Comparing `tmp/django-tmmis-0.3.5.tar.gz` & `tmp/django-tmmis-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tmmis-0.3.5.tar", last modified: Wed Nov  8 10:56:08 2023, max compression
+gzip compressed data, was "django-tmmis-0.3.6.tar", last modified: Wed Nov  8 12:21:17 2023, max compression
```

## Comparing `django-tmmis-0.3.5.tar` & `django-tmmis-0.3.6.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 10:56:08.597404 django-tmmis-0.3.5/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2079 2023-11-08 10:56:08.597404 django-tmmis-0.3.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 10:56:08.513405 django-tmmis-0.3.5/django_tmmis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2079 2023-11-08 10:56:08.000000 django-tmmis-0.3.5/django_tmmis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3594 2023-11-08 10:56:08.000000 django-tmmis-0.3.5/django_tmmis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 10:56:08.000000 django-tmmis-0.3.5/django_tmmis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-11-08 10:56:08.000000 django-tmmis-0.3.5/django_tmmis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-11-08 10:56:08.000000 django-tmmis-0.3.5/django_tmmis.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-11-08 10:56:08.601404 django-tmmis-0.3.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 10:56:08.529404 django-tmmis-0.3.5/tmmis/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 10:56:08.597404 django-tmmis-0.3.5/tmmis/models/
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/atf_file_attachment.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/atf_file_info.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/atf_file_type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_blank_template.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_call_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_call_doctor_status.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_citizen.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-11-08 10:55:19.000000 django-tmmis-0.3.5/tmmis/models/hlt_disp_result_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-11-08 10:55:19.000000 django-tmmis-0.3.5/tmmis/models/hlt_disp_result_type_value.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2023-11-08 10:55:19.000000 django-tmmis-0.3.5/tmmis/models/hlt_disp_result_value.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_doc_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_doctor_time_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_doctor_visit_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1525 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/hlt_lpu_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_med_record.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)     1933 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_mkb_tap.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_polis_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_reason_care.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_representative_mkab.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_smtap.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/hlt_tap.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_type_call_doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/hlt_uchastok.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/hlt_visit_history.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/kla_address.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/kla_house.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/kla_kladr.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/kla_street.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_complex_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_histological_block.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_lab_direction_type.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_lab_research_cause.py
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_lab_research_target.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory_kind.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_laboratory_type.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_option.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_option_enum_values.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_option_value.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_option_value_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3930 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_journal.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_param_value_type.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_param_values.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_result.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_sample.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_service.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_state.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_kind_doc_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_param.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_param_in_pack.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_param_to_research_type.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_to_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/lbr_research_type_to_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_department.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_age_group.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_dd_service.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_department_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_department_type.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_diagnos_type.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_disease_type.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_health_group.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_med_care_type.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_met_issl.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_profit_type.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_reason_type.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_soc_status.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_stat_cure_result.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_tip_oms.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_visit_place.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_kl_visit_result.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/oms_lpu.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_mkb.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_okato.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/oms_okved.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-02-06 03:36:56.000000 django-tmmis-0.3.5/tmmis/models/oms_organisation.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_prvd.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_prvs.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_service_medical.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_smo.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/oms_type_doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/x_doc_elem_def.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-11-03 14:06:58.000000 django-tmmis-0.3.5/tmmis/models/x_doc_type_def.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/models/x_user.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/router.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/tests.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-06 03:14:35.000000 django-tmmis-0.3.5/tmmis/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.323343 django-tmmis-0.3.6/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-11-08 12:21:17.323343 django-tmmis-0.3.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.283343 django-tmmis-0.3.6/django_tmmis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-11-08 12:21:17.000000 django-tmmis-0.3.6/django_tmmis.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-11-08 12:21:17.323343 django-tmmis-0.3.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.287343 django-tmmis-0.3.6/tmmis/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 12:21:17.319343 django-tmmis-0.3.6/tmmis/models/
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/atf_file_attachment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/atf_file_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/atf_file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_blank_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_call_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_call_doctor_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_citizen.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-11-08 12:20:29.000000 django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-11-08 12:20:29.000000 django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-11-08 12:20:29.000000 django-tmmis-0.3.6/tmmis/models/hlt_disp_result_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_doc_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_doctor_time_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_doctor_visit_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/hlt_lpu_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_med_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_mkb_tap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_polis_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_reason_care.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_representative_mkab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_smtap.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/hlt_tap.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_type_call_doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/hlt_uchastok.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/hlt_visit_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_address.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_house.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_kladr.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/kla_street.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_complex_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_histological_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_lab_direction_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_lab_research_cause.py
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_lab_research_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)     4525 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_laboratory_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option_enum_values.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_option_value_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3930 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_param_value_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_param_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind_doc_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_in_pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_to_research_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_department.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_age_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_dd_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_department_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_department_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_diagnos_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_disease_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_health_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_med_care_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_met_issl.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_profit_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_reason_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_soc_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_stat_cure_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_tip_oms.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_visit_place.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_kl_visit_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/oms_lpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_mkb.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_okato.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/oms_okved.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-02-06 03:36:56.000000 django-tmmis-0.3.6/tmmis/models/oms_organisation.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_prvd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_prvs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_service_medical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_smo.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/oms_type_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/x_doc_elem_def.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-11-03 14:06:58.000000 django-tmmis-0.3.6/tmmis/models/x_doc_type_def.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/models/x_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/router.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-02-06 03:14:35.000000 django-tmmis-0.3.6/tmmis/views.py
```

### Comparing `django-tmmis-0.3.5/PKG-INFO` & `django-tmmis-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tmmis
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Django app provided ORM to TrustMed medical information system
 Home-page: UNKNOWN
 Author: Chmelyuk Vladislav
 Author-email: neimp@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-tmmis-0.3.5/README.md` & `django-tmmis-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/django_tmmis.egg-info/PKG-INFO` & `django-tmmis-0.3.6/django_tmmis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tmmis
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Django app provided ORM to TrustMed medical information system
 Home-page: UNKNOWN
 Author: Chmelyuk Vladislav
 Author-email: neimp@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-tmmis-0.3.5/django_tmmis.egg-info/SOURCES.txt` & `django-tmmis-0.3.6/django_tmmis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/setup.cfg` & `django-tmmis-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/handlers.py` & `django-tmmis-0.3.6/tmmis/handlers.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/__init__.py` & `django-tmmis-0.3.6/tmmis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/atf_file_attachment.py` & `django-tmmis-0.3.6/tmmis/models/atf_file_attachment.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/atf_file_info.py` & `django-tmmis-0.3.6/tmmis/models/atf_file_info.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/atf_file_type.py` & `django-tmmis-0.3.6/tmmis/models/atf_file_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_blank_template.py` & `django-tmmis-0.3.6/tmmis/models/hlt_blank_template.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_call_doctor.py` & `django-tmmis-0.3.6/tmmis/models/hlt_call_doctor.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_citizen.py` & `django-tmmis-0.3.6/tmmis/models/hlt_citizen.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_disp_result_type.py` & `django-tmmis-0.3.6/tmmis/models/x_doc_elem_def.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from .base_model import *
 
 
-class HltDispResultType(BaseModel):
-    """
-    Тип результатов заключения
-    """
-
-    id = models.AutoField(db_column="disp_ResultTypeID", primary_key=True)
-    code = models.CharField(db_column="Code", max_length=100)
-    date_begin = models.DateTimeField(db_column="DateBegin")
-    date_end = models.DateTimeField(db_column="DateEnd")
+class XDocElemDef(BaseModel):
+    id = models.AutoField(db_column="DocElemDefID", primary_key=True)
+    type_def = models.ForeignKey("XDocTypeDef", db_column="DocTypeDefID", **FK_DEFAULT)
+    name = models.CharField(db_column="Name", max_length=50)
+    mnem_code = models.CharField(db_column="MnemCode", max_length=50)
+    caption = models.CharField(db_column="Caption", max_length=500)
+    description = models.CharField(db_column="Description", max_length=500)
+    elem_type = models.IntegerField(db_column="ElemType")
+    value_type = models.IntegerField(db_column="ValueType")
+    value_size = models.IntegerField(db_column="ValueSize")
+    value_scale = models.IntegerField(db_column="ValueScale")
+    field_name = models.CharField(db_column="FieldName", max_length=2500)
+    linked_doc_type_def_id = models.IntegerField(db_column="LinkedDocTypeDefID")
+    linked_doc_elem_def_id = models.IntegerField(db_column="LinkedDocElemDefID")
+    access_def = models.IntegerField(db_column="AccessDef", **NULL)
+    tag_name = models.CharField(db_column="TagName", max_length=50)
+    delete_mode = models.IntegerField(db_column="DeleteMode", **NULL)
+    show_mode = models.IntegerField(db_column="ShowMode", **NULL)
+    srv_doc_elem_def_id = models.IntegerField(db_column="SRVDocElemDefID")
+    guid = models.CharField(db_column="GUID", max_length=36)
+    pos = models.IntegerField(db_column="Pos")
+    outputformat = models.CharField(db_column="OutputFormat", max_length=50)
     flags = models.IntegerField(db_column="Flags")
-    guid = models.CharField(db_column="Guid", max_length=36, unique=True)
-    name = models.TextField(db_column="Name")
-    rf_disp_type_guid = models.CharField(db_column="rf_DispTypeGuid", max_length=36)
-    is_main = models.BooleanField(db_column="IsMain")
-    is_show_ctrl = models.SmallIntegerField(db_column="IsShowCtrl")
-    age_from = models.IntegerField(db_column="AgeFrom")
-    age_to = models.IntegerField(db_column="AgeTo")
-    sex_id = models.IntegerField(db_column="rf_kl_SexID")
-    rf_result_type_display_id = models.IntegerField(db_column="rf_ResultTypeDisplayID")
-    rf_disp_question_type_id = models.IntegerField(db_column="rf_disp_QuestionTypeID")
-    rf_mkbid = models.IntegerField(db_column="rf_MKBID")
-    rf_question_guid = models.CharField(db_column="rf_QuestionGuid", max_length=36)
+    category_name = models.CharField(db_column="CategoryName", max_length=50)
+    sql_data_type = models.CharField(db_column="SqlDataType", max_length=50)
 
     class Meta:
         managed = False
-        db_table = "hlt_disp_ResultType"
+        db_table = "x_DocElemDef"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_disp_result_type_value.py` & `django-tmmis-0.3.6/tmmis/models/oms_okved.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 from .base_model import *
 
 
-class HltDispResultTypeValue(BaseModel):
+class OmsOkved(BaseModel):
     """
-    Значения типов результата
+    Код экономического вида деятельности по ОКВЭД
     """
 
-    id = models.AutoField(db_column="disp_ResultTypeValueID", primary_key=True)
-    code = models.CharField(db_column="Code", max_length=100)
-    date_begin = models.DateTimeField(db_column="DateBegin")
-    date_end = models.DateTimeField(db_column="DateEnd")
-    flags = models.IntegerField(db_column="Flags")
-    guid = models.CharField(db_column="Guid", max_length=36, unique=True)
-    name = models.TextField(db_column="Name")
-    rf_disp_type_guid = models.CharField(db_column="rf_DispTypeGuid", max_length=36)
-    result_type = models.ForeignKey(
-        "HltDispResultType",
-        models.DO_NOTHING,
-        to_field="guid",
-        db_column="rf_ResultTypeGuid",
-        max_length=36,
-    )
-    rf_variant_guid = models.CharField(db_column="rf_VariantGuid", max_length=36)
-    point = models.DecimalField(db_column="Point", max_digits=18, decimal_places=2)
+    id = models.AutoField(db_column="OKVEDID", primary_key=True)
+    uuid = models.CharField(db_column="UGUID", max_length=36, unique=True, default=uuid4)
+    name = models.CharField(db_column="NAME", max_length=100)
+    code = models.CharField(db_column="OKVED_CODE", max_length=10)
+    date_in = models.DateTimeField(db_column="DATEIN")
+    date_out = models.DateTimeField(db_column="DATEOUT")
+    date_edit = models.DateTimeField(db_column="DATEEDIT")
 
     class Meta:
         managed = False
-        db_table = "hlt_disp_ResultTypeValue"
+        db_table = "oms_OKVED"
```

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_disp_result_value.py` & `django-tmmis-0.3.6/tmmis/models/hlt_disp_result_type_value.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from .base_model import *
 
 
-class HltDispResultValue(BaseModel):
+class HltDispResultTypeValue(BaseModel):
     """
-    Результат прохождения обследования
+    Значения типов результата
     """
 
-    id = models.AutoField(db_column="disp_ResultValueID", primary_key=True)
+    id = models.AutoField(db_column="disp_ResultTypeValueID", primary_key=True)
     code = models.CharField(db_column="Code", max_length=100)
-    flags = models.IntegerField(db_column="Flags")
-    guid = models.CharField(db_column="Guid", max_length=36)
     name = models.TextField(db_column="Name")
-    rf_card_guid = models.CharField(db_column="rf_CardGuid", max_length=36)
+    guid = models.CharField(db_column="Guid", max_length=36, unique=True, default=uuid4)
+    date_begin = models.DateTimeField(db_column="DateBegin", default=timezone.now)
+    date_end = models.DateTimeField(db_column="DateEnd", default=timezone.datetime(2222, 1, 1))
+    flags = models.IntegerField(db_column="Flags", default=0)
+    rf_disp_type_guid = models.CharField(
+        db_column="rf_DispTypeGuid",
+        max_length=36,
+        default="00000000-0000-0000-0000-000000000000",
+    )
     result_type = models.ForeignKey(
         "HltDispResultType",
         models.DO_NOTHING,
         to_field="guid",
         db_column="rf_ResultTypeGuid",
         max_length=36,
     )
-    result_type_value = models.ForeignKey(
-        "HltDispResultTypeValue",
-        models.DO_NOTHING,
-        to_field="guid",
-        db_column="rf_ResultTypeValueGuid",
+    rf_variant_guid = models.CharField(
+        db_column="rf_VariantGuid",
         max_length=36,
+        default="00000000-0000-0000-0000-000000000000",
     )
-    value1 = models.TextField(db_column="Value1")
-    value2 = models.DecimalField(db_column="Value2", max_digits=9, decimal_places=4)
-    document_id = models.IntegerField(db_column="DocumentId")
-    doc_type_guid = models.CharField(db_column="DocTypeGuid", max_length=36)
-    tap = models.ForeignKey("HltTap", models.DO_NOTHING, db_column="rf_TAPID", related_name="+")
-    is_auto = models.BooleanField(db_column="IsAuto")
-    rf_exam_guid = models.CharField(db_column="rf_ExamGuid", max_length=36)
+    point = models.DecimalField(db_column="Point", max_digits=18, decimal_places=2, default="0.0")
 
     class Meta:
         managed = False
-        db_table = "hlt_disp_ResultValue"
+        db_table = "hlt_disp_ResultTypeValue"
```

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_doc_prvd.py` & `django-tmmis-0.3.6/tmmis/models/hlt_doc_prvd.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_doctor_time_table.py` & `django-tmmis-0.3.6/tmmis/models/hlt_doctor_time_table.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_doctor_visit_table.py` & `django-tmmis-0.3.6/tmmis/models/hlt_doctor_visit_table.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_lpu_doctor.py` & `django-tmmis-0.3.6/tmmis/models/hlt_lpu_doctor.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_med_record.py` & `django-tmmis-0.3.6/tmmis/models/hlt_med_record.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_mkab.py` & `django-tmmis-0.3.6/tmmis/models/hlt_mkab.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_mkb_tap.py` & `django-tmmis-0.3.6/tmmis/models/hlt_mkb_tap.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_polis_mkab.py` & `django-tmmis-0.3.6/tmmis/models/hlt_polis_mkab.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_reason_care.py` & `django-tmmis-0.3.6/tmmis/models/hlt_reason_care.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_representative_mkab.py` & `django-tmmis-0.3.6/tmmis/models/hlt_representative_mkab.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_smtap.py` & `django-tmmis-0.3.6/tmmis/models/hlt_smtap.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_tap.py` & `django-tmmis-0.3.6/tmmis/models/hlt_tap.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_type_call_doctor.py` & `django-tmmis-0.3.6/tmmis/models/hlt_type_call_doctor.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_uchastok.py` & `django-tmmis-0.3.6/tmmis/models/hlt_uchastok.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/hlt_visit_history.py` & `django-tmmis-0.3.6/tmmis/models/hlt_visit_history.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/kla_address.py` & `django-tmmis-0.3.6/tmmis/models/kla_address.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/kla_house.py` & `django-tmmis-0.3.6/tmmis/models/kla_house.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/kla_kladr.py` & `django-tmmis-0.3.6/tmmis/models/kla_kladr.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/kla_street.py` & `django-tmmis-0.3.6/tmmis/models/kla_street.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_complex_research_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_complex_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_histological_block.py` & `django-tmmis-0.3.6/tmmis/models/lbr_histological_block.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_lab_direction_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_lab_direction_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_lab_research_cause.py` & `django-tmmis-0.3.6/tmmis/models/lbr_lab_research_cause.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_lab_research_target.py` & `django-tmmis-0.3.6/tmmis/models/lbr_lab_research_target.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory_kind.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_kind.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research_in_pack.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_in_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research_pack.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory_research_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_laboratory_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_laboratory_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_option.py` & `django-tmmis-0.3.6/tmmis/models/lbr_option.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_option_enum_values.py` & `django-tmmis-0.3.6/tmmis/models/lbr_option_enum_values.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_option_value.py` & `django-tmmis-0.3.6/tmmis/models/lbr_option_value.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_option_value_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_option_value_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_journal.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_journal.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_param_values.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_param_values.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_result.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_result.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_sample.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_sample.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_service.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_service.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_in_pack.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_in_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_kind.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_kind_doc_prvd.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_kind_doc_prvd.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_param.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_param.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_param_in_pack.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_in_pack.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_param_to_research_type.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_param_to_research_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_to_lpu.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_lpu.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/lbr_research_type_to_profile.py` & `django-tmmis-0.3.6/tmmis/models/lbr_research_type_to_profile.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_department.py` & `django-tmmis-0.3.6/tmmis/models/oms_department.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_age_group.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_age_group.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_diagnos_type.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_diagnos_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_met_issl.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_met_issl.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_profit_type.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_profit_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_reason_type.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_reason_type.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_soc_status.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_soc_status.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_stat_cure_result.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_stat_cure_result.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_tip_oms.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_tip_oms.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_kl_visit_result.py` & `django-tmmis-0.3.6/tmmis/models/oms_kl_visit_result.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_lpu.py` & `django-tmmis-0.3.6/tmmis/models/oms_lpu.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_mkb.py` & `django-tmmis-0.3.6/tmmis/models/oms_mkb.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_okato.py` & `django-tmmis-0.3.6/tmmis/models/oms_okato.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_okved.py` & `django-tmmis-0.3.6/tmmis/models/oms_prvd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .base_model import *
 
 
-class OmsOkved(BaseModel):
+class OmsPrvd(BaseModel):
     """
-    Код экономического вида деятельности по ОКВЭД
+    В: Должности
     """
 
-    id = models.AutoField(db_column="OKVEDID", primary_key=True)
-    uuid = models.CharField(db_column="UGUID", max_length=36, unique=True, default=uuid4)
+    id = models.AutoField(db_column="PRVDID", primary_key=True)
     name = models.CharField(db_column="NAME", max_length=100)
-    code = models.CharField(db_column="OKVED_CODE", max_length=10)
-    date_in = models.DateTimeField(db_column="DATEIN")
-    date_out = models.DateTimeField(db_column="DATEOUT")
-    date_edit = models.DateTimeField(db_column="DATEEDIT")
+    c_prvd = models.CharField(db_column="C_PRVD", max_length=50)
+    msg_text = models.CharField(db_column="MSG_TEXT", max_length=100)
+    date_b = models.DateTimeField(db_column="Date_B")
+    date_e = models.DateTimeField(db_column="Date_E")
+    profit_type = models.ForeignKey("OmsKlProfitType", models.DO_NOTHING, db_column="rf_kl_ProfitTypeID")
 
     class Meta:
         managed = False
-        db_table = "oms_OKVED"
+        db_table = "oms_PRVD"
```

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_organisation.py` & `django-tmmis-0.3.6/tmmis/models/oms_organisation.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_prvs.py` & `django-tmmis-0.3.6/tmmis/models/oms_prvs.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_service_medical.py` & `django-tmmis-0.3.6/tmmis/models/oms_service_medical.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_smo.py` & `django-tmmis-0.3.6/tmmis/models/oms_smo.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/oms_type_doc.py` & `django-tmmis-0.3.6/tmmis/models/oms_type_doc.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/x_doc_type_def.py` & `django-tmmis-0.3.6/tmmis/models/x_doc_type_def.py`

 * *Files identical despite different names*

### Comparing `django-tmmis-0.3.5/tmmis/models/x_user.py` & `django-tmmis-0.3.6/tmmis/models/x_user.py`

 * *Files identical despite different names*

