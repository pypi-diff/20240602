# Comparing `tmp/streamlit_nightly-1.35.1.dev20240530.tar.gz` & `tmp/streamlit_nightly-1.35.1.dev20240531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.35.1.dev20240530.tar", last modified: Fri May 31 06:54:55 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.35.1.dev20240531.tar", last modified: Sat Jun  1 06:54:40 2024, max compression
```

## Comparing `streamlit_nightly-1.35.1.dev20240530.tar` & `streamlit_nightly-1.35.1.dev20240531.tar`

### file list

```diff
@@ -1,572 +1,579 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.185959 streamlit_nightly-1.35.1.dev20240530/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-31 06:54:55.185959 streamlit_nightly-1.35.1.dev20240530/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.065959 streamlit_nightly-1.35.1.dev20240530/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 06:54:55.185959 streamlit_nightly-1.35.1.dev20240530/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.073959 streamlit_nightly-1.35.1.dev20240530/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.073959 streamlit_nightly-1.35.1.dev20240530/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.073959 streamlit_nightly-1.35.1.dev20240530/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.073959 streamlit_nightly-1.35.1.dev20240530/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.073959 streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.077959 streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43657 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.077959 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.081959 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    27609 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.085959 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30696 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)    69887 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.089959 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    36465 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17699 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11717 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26704 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22376 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30085 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.089959 streamlit_nightly-1.35.1.dev20240530/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.089959 streamlit_nightly-1.35.1.dev20240530/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.089959 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.089959 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.117959 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12304 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-31 06:51:04.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.121959 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36663 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.121959 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/legacy_cache_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.125959 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.125959 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.125959 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.125959 streamlit_nightly-1.35.1.dev20240530/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-31 06:51:33.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.065959 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.129959 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/8148.49dfd2ce.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.161959 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1168.14f7c6ff.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3513.7dedbda2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4113.99983645.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/474.7eb0c6cd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5345.73d26e5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5379.f08eddd1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5441.1b94928f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6013.4ba2d616.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6950.70fe55c2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7175.583ff733.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    51165 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8148.293984e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8691.4211c305.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9336.3e046ad7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4405464 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/main.9978e612.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/main.9978e612.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.177959 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-31 06:54:52.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.177959 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.177959 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.177959 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.177959 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.177959 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.181959 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.181959 streamlit_nightly-1.35.1.dev20240530/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.181959 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.185959 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-31 06:54:53.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23268 2024-05-31 06:54:53.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:54:53.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 06:54:53.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:50:59.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-31 06:54:53.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 06:54:53.000000 streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:54:55.185959 streamlit_nightly-1.35.1.dev20240530/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-31 06:49:31.000000 streamlit_nightly-1.35.1.dev20240530/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.742800 streamlit_nightly-1.35.1.dev20240531/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-06-01 06:54:40.742800 streamlit_nightly-1.35.1.dev20240531/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.626799 streamlit_nightly-1.35.1.dev20240531/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:54:40.742800 streamlit_nightly-1.35.1.dev20240531/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.630799 streamlit_nightly-1.35.1.dev20240531/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.634799 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.634799 streamlit_nightly-1.35.1.dev20240531/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.634799 streamlit_nightly-1.35.1.dev20240531/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.634799 streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.634799 streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43657 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.634799 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.642799 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27609 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.642799 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30696 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29682 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19231 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69887 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.646799 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33018 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36467 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18081 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26706 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22380 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.646799 streamlit_nightly-1.35.1.dev20240531/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.646799 streamlit_nightly-1.35.1.dev20240531/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.646799 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.650799 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/material_icon_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.650799 streamlit_nightly-1.35.1.dev20240531/streamlit/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/navigation/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.674799 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Navigation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Navigation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-06-01 06:50:48.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.678799 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37234 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.678799 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/legacy_cache_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.682799 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/pages_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.682799 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29067 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.682799 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.682799 streamlit_nightly-1.35.1.dev20240531/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-06-01 06:51:18.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.622799 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.686799 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/8148.49dfd2ce.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.718800 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1168.14f7c6ff.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3513.7dedbda2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/474.7eb0c6cd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5345.73d26e5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5379.f08eddd1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5441.1b94928f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7175.583ff733.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51165 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8148.293984e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21241 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8571.cfc22b99.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8691.4211c305.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9336.3e046ad7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398776 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9945.47d54f35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9945.47d54f35.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4420585 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/main.707da454.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/main.707da454.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.734800 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-06-01 06:54:37.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.734800 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.738800 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36775 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.738800 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.738800 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.738800 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.738800 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.738800 streamlit_nightly-1.35.1.dev20240531/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.742800 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.742800 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-06-01 06:54:39.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23467 2024-06-01 06:54:39.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:54:39.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 06:54:39.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:50:43.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-01 06:54:39.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 06:54:39.000000 streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:40.742800 streamlit_nightly-1.35.1.dev20240531/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-06-01 06:49:16.000000 streamlit_nightly-1.35.1.dev20240531/tests/testutil.py
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/PKG-INFO` & `streamlit_nightly-1.35.1.dev20240531/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.35.1.dev20240530
+Version: 1.35.1.dev20240531
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/bin/streamlit.cmd` & `streamlit_nightly-1.35.1.dev20240531/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/setup.py` & `streamlit_nightly-1.35.1.dev20240531/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.35.1.dev20240530"  # PEP-440
+VERSION = "1.35.1.dev20240531"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
 
 # Modules that the user should have access to. These are imported with the "as" syntax and the same name; note that renaming the import with "as" does not make it an explicit export.
 # In this case, you should import it with an underscore to make clear that it is internal and then assign it to a variable with the new intended name.
 # You can check the export behavior by running 'mypy --strict example_app.py', which disables implicit_reexport, where you use the respective command in the example_app.py Streamlit app.
 
 from streamlit.echo import echo as echo
 from streamlit.commands.logo import logo as logo
+from streamlit.commands.navigation import navigation as navigation
+from streamlit.navigation.page import Page as Page
 from streamlit.elements.spinner import spinner as spinner
 
 from streamlit.commands.page_config import set_page_config as set_page_config
 from streamlit.commands.execution_control import (
     stop as stop,
     rerun as rerun,
     experimental_rerun as _experimental_rerun,
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/__main__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/case_converters.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/cli_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/code_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/color_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/column_config.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/commands/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/commands/execution_control.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/commands/execution_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 from __future__ import annotations
 
 import os
 from typing import Final, NoReturn
 
 import streamlit as st
-from streamlit import source_util
 from streamlit.deprecation_util import make_deprecated_name_warning
 from streamlit.errors import NoSessionContext, StreamlitAPIException
 from streamlit.file_util import get_main_script_directory, normalize_path_join
 from streamlit.logger import get_logger
+from streamlit.navigation.page import StreamlitPage
 from streamlit.runtime.metrics_util import gather_metrics
 from streamlit.runtime.scriptrunner import RerunData, get_script_run_ctx
 
 _LOGGER: Final = get_logger(__name__)
 
 
 @gather_metrics("stop")
@@ -92,27 +92,29 @@
     # by the rerun. We do not send a frontend warning because it wouldn't
     # be seen.
     _LOGGER.warning(msg)
     rerun()
 
 
 @gather_metrics("switch_page")
-def switch_page(page: str) -> NoReturn:  # type: ignore[misc]
+def switch_page(page: str | StreamlitPage) -> NoReturn:  # type: ignore[misc]
     """Programmatically switch the current page in a multipage app.
 
     When ``st.switch_page`` is called, the current page execution stops and
     the specified page runs as if the user clicked on it in the sidebar
     navigation. The specified page must be recognized by Streamlit's multipage
     architecture (your main Python file or a Python file in a ``pages/``
     folder). Arbitrary Python scripts cannot be passed to ``st.switch_page``.
 
     Parameters
     ----------
-    page: str
-        The file path (relative to the main script) of the page to switch to.
+    page: str or st.Page
+        The file path (relative to the main script) or an st.Page indicating
+        the page to switch to.
+
 
     Example
     -------
     Consider the following example given this file structure:
 
     >>> your-repository/
     >>> ├── pages/
@@ -137,26 +139,34 @@
 
     ctx = get_script_run_ctx()
 
     if not ctx or not ctx.script_requests:
         # This should never be the case
         raise NoSessionContext()
 
-    main_script_directory = get_main_script_directory(ctx.main_script_path)
-    requested_page = os.path.realpath(normalize_path_join(main_script_directory, page))
-    all_app_pages = source_util.get_pages(ctx.main_script_path).values()
-
-    matched_pages = [p for p in all_app_pages if p["script_path"] == requested_page]
-
-    if len(matched_pages) == 0:
-        raise StreamlitAPIException(
-            f"Could not find page: `{page}`. Must be the file path relative to the main script, from the directory: `{os.path.basename(main_script_directory)}`. Only the main app file and files in the `pages/` directory are supported."
+    page_script_hash = ""
+    if isinstance(page, StreamlitPage):
+        page_script_hash = page._script_hash
+    else:
+        main_script_directory = get_main_script_directory(ctx.main_script_path)
+        requested_page = os.path.realpath(
+            normalize_path_join(main_script_directory, page)
         )
+        all_app_pages = ctx.pages_manager.get_pages().values()
+
+        matched_pages = [p for p in all_app_pages if p["script_path"] == requested_page]
+
+        if len(matched_pages) == 0:
+            raise StreamlitAPIException(
+                f"Could not find page: `{page}`. Must be the file path relative to the main script, from the directory: `{os.path.basename(main_script_directory)}`. Only the main app file and files in the `pages/` directory are supported."
+            )
+
+        page_script_hash = matched_pages[0]["page_script_hash"]
 
     ctx.script_requests.request_rerun(
         RerunData(
             query_string=ctx.query_string,
-            page_script_hash=matched_pages[0]["page_script_hash"],
+            page_script_hash=page_script_hash,
         )
     )
     # Force a yield point so the runner can do the rerun
     st.empty()
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/commands/logo.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/commands/logo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/commands/page_config.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/components.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/components/v1/custom_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,25 +176,25 @@
                     user_key=key,
                     name=self.name,
                     form_id=current_form_id(dg),
                     url=self.url,
                     key=key,
                     json_args=serialized_json_args,
                     special_args=special_args,
-                    page=ctx.page_script_hash if ctx else None,
+                    page=ctx.active_script_hash if ctx else None,
                 )
             else:
                 computed_id = compute_widget_id(
                     "component_instance",
                     user_key=key,
                     name=self.name,
                     form_id=current_form_id(dg),
                     url=self.url,
                     key=key,
-                    page=ctx.page_script_hash if ctx else None,
+                    page=ctx.active_script_hash if ctx else None,
                 )
             element.component_instance.id = computed_id
 
             def deserialize_component(ui_value, widget_id=""):
                 # ui_value is an object from json, an ArrowTable proto, or a bytearray
                 return ui_value
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/config.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/config_option.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/config_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/connections/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/connections/base_connection.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/connections/util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/constants.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/cursor.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/delta_generator.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/deprecation_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/development.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/echo.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/alert.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/arrow.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/balloons.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/code.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/doc_string.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/empty.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/exception.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/form.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/heading.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/html.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/iframe.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/image.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/json.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/layouts.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/policies.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/policies.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/lib/utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/lib/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/map.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/markdown.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/media.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,15 +572,15 @@
             url=proto.url,
             mimetype=mimetype,
             start_time=start_time,
             end_time=end_time,
             loop=loop,
             autoplay=autoplay,
             muted=muted,
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         proto.id = id
 
 
 def _parse_start_time_end_time(
     start_time: MediaTime, end_time: MediaTime | None
@@ -748,10 +748,10 @@
             url=proto.url,
             mimetype=mimetype,
             start_time=start_time,
             sample_rate=sample_rate,
             end_time=end_time,
             loop=loop,
             autoplay=autoplay,
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
         proto.id = id
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/metric.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/plotly_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
             plotly_spec=plotly_chart_proto.spec,
             plotly_config=plotly_chart_proto.config,
             selection_mode=selection_mode,
             is_selection_activated=is_selection_activated,
             theme=theme,
             form_id=plotly_chart_proto.form_id,
             use_container_width=use_container_width,
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         if is_selection_activated:
             # Selections are activated, treat plotly chart as a widget:
             plotly_chart_proto.selection_mode.extend(
                 parse_selection_mode(selection_mode)
             )
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/progress.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/pyplot.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/snow.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/spinner.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/text.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/toast.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/vega_charts.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/vega_charts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 import os
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import TYPE_CHECKING, BinaryIO, Final, Literal, TextIO, Union, cast
 
 from typing_extensions import TypeAlias
 
-from streamlit import runtime, source_util
+from streamlit import runtime
 from streamlit.elements.form import current_form_id, is_in_form
 from streamlit.elements.lib.policies import (
     check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.file_util import get_main_script_directory, normalize_path_join
+from streamlit.navigation.page import StreamlitPage
 from streamlit.proto.Button_pb2 import Button as ButtonProto
 from streamlit.proto.DownloadButton_pb2 import DownloadButton as DownloadButtonProto
 from streamlit.proto.LinkButton_pb2 import LinkButton as LinkButtonProto
 from streamlit.proto.PageLink_pb2 import PageLink as PageLinkProto
 from streamlit.runtime.metrics_util import gather_metrics
 from streamlit.runtime.scriptrunner import ScriptRunContext, get_script_run_ctx
 from streamlit.runtime.state import (
@@ -42,14 +43,15 @@
     WidgetCallback,
     WidgetKwargs,
     register_widget,
 )
 from streamlit.runtime.state.common import compute_widget_id, save_for_app_testing
 from streamlit.string_util import validate_icon_or_emoji
 from streamlit.type_util import Key, to_key
+from streamlit.url_util import is_url
 
 if TYPE_CHECKING:
     from streamlit.delta_generator import DeltaGenerator
 
 FORM_DOCS_INFO: Final = """
 
 For more information, refer to the
@@ -439,15 +441,15 @@
             type=type,
             use_container_width=use_container_width,
         )
 
     @gather_metrics("page_link")
     def page_link(
         self,
-        page: str,
+        page: str | StreamlitPage,
         *,
         label: str | None = None,
         icon: str | None = None,
         help: str | None = None,
         disabled: bool = False,
         use_container_width: bool | None = None,
     ) -> DeltaGenerator:
@@ -459,18 +461,18 @@
 
         If an external page is specified, clicking ``st.page_link`` opens a new
         tab to the specified page. The current script run will continue if not
         complete.
 
         Parameters
         ----------
-        page : str
-            The file path (relative to the main script) of the page to switch to.
-            Alternatively, this can be the URL to an external page (must start
-            with "http://" or "https://").
+        page : str or st.Page
+            The file path (relative to the main script) or an st.Page indicating
+            the page to switch to. Alternatively, this can be the URL to an
+            external page (must start with "http://" or "https://").
         label : str
             The label for the page link. Labels are required for external pages.
             Labels can optionally contain Markdown and supports the following
             elements: Bold, Italics, Strikethroughs, Inline Code, and Emojis.
 
             This also supports:
 
@@ -589,15 +591,15 @@
             label=label,
             file_name=file_name,
             mime=mime,
             key=key,
             help=help,
             type=type,
             use_container_width=use_container_width,
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         if is_in_form(self.dg):
             raise StreamlitAPIException(
                 f"`st.download_button()` can't be used in an `st.form()`.{FORM_DOCS_INFO}"
             )
 
@@ -652,15 +654,15 @@
         if help is not None:
             link_button_proto.help = dedent(help)
 
         return self.dg._enqueue("link_button", link_button_proto)
 
     def _page_link(
         self,
-        page: str,
+        page: str | StreamlitPage,
         *,  # keyword-only arguments:
         label: str | None = None,
         icon: str | None = None,
         help: str | None = None,
         disabled: bool = False,
         use_container_width: bool | None = None,
     ) -> DeltaGenerator:
@@ -675,46 +677,53 @@
 
         if help is not None:
             page_link_proto.help = dedent(help)
 
         if use_container_width is not None:
             page_link_proto.use_container_width = use_container_width
 
-        # Handle external links:
-        if page.startswith("http://") or page.startswith("https://"):
-            if label is None or label == "":
-                raise StreamlitAPIException(
-                    f"The label param is required for external links used with st.page_link - please provide a label."
-                )
-            else:
-                page_link_proto.page = page
-                page_link_proto.external = True
-                return self.dg._enqueue("page_link", page_link_proto)
-
-        ctx = get_script_run_ctx()
-        ctx_main_script = ""
-        if ctx:
-            ctx_main_script = ctx.main_script_path
-
-        main_script_directory = get_main_script_directory(ctx_main_script)
-        requested_page = os.path.realpath(
-            normalize_path_join(main_script_directory, page)
-        )
-        all_app_pages = source_util.get_pages(ctx_main_script).values()
+        if isinstance(page, StreamlitPage):
+            page_link_proto.page_script_hash = page._script_hash
+            page_link_proto.page = page.url_path
+            if label is None:
+                page_link_proto.label = page.title
+        else:
+            # Handle external links:
+            if is_url(page):
+                if label is None or label == "":
+                    raise StreamlitAPIException(
+                        "The label param is required for external links used with st.page_link - please provide a label."
+                    )
+                else:
+                    page_link_proto.page = page
+                    page_link_proto.external = True
+                    return self.dg._enqueue("page_link", page_link_proto)
+
+            ctx = get_script_run_ctx()
+            ctx_main_script = ""
+            all_app_pages = {}
+            if ctx:
+                ctx_main_script = ctx.main_script_path
+                all_app_pages = ctx.pages_manager.get_pages()
+
+            main_script_directory = get_main_script_directory(ctx_main_script)
+            requested_page = os.path.realpath(
+                normalize_path_join(main_script_directory, page)
+            )
 
-        # Handle retrieving the page_script_hash & page
-        for page_data in all_app_pages:
-            full_path = page_data["script_path"]
-            page_name = page_data["page_name"]
-            if requested_page == full_path:
-                if label is None:
-                    page_link_proto.label = page_name.replace("_", " ")
-                page_link_proto.page_script_hash = page_data["page_script_hash"]
-                page_link_proto.page = page_name
-                break
+            # Handle retrieving the page_script_hash & page
+            for page_data in all_app_pages.values():
+                full_path = page_data["script_path"]
+                page_name = page_data["page_name"]
+                if requested_page == full_path:
+                    if label is None:
+                        page_link_proto.label = page_name.replace("_", " ")
+                    page_link_proto.page_script_hash = page_data["page_script_hash"]
+                    page_link_proto.page = page_name
+                    break
 
         if page_link_proto.page_script_hash == "":
             raise StreamlitAPIException(
                 f"Could not find page: `{page}`. Must be the file path relative to the main script, from the directory: `{os.path.basename(main_script_directory)}`. Only the main app file and files in the `pages/` directory are supported."
             )
 
         return self.dg._enqueue("page_link", page_link_proto)
@@ -746,15 +755,15 @@
             user_key=key,
             label=label,
             key=key,
             help=help,
             is_form_submitter=is_form_submitter,
             type=type,
             use_container_width=use_container_width,
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         # It doesn't make sense to create a button inside a form (except
         # for the "Form Submitter" button that's automatically created in
         # every form). We throw an error to warn the user about this.
         # We omit this check for scripts running outside streamlit, because
         # they will have no script_run_ctx.
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/camera_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         id = compute_widget_id(
             "camera_input",
             user_key=key,
             label=label,
             key=key,
             help=help,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         camera_input_proto = CameraInputProto()
         camera_input_proto.id = id
         camera_input_proto.label = label
         camera_input_proto.form_id = current_form_id(self.dg)
         camera_input_proto.disabled = disabled
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         ctx = get_script_run_ctx()
         id = compute_widget_id(
             "chat_input",
             user_key=key,
             key=key,
             placeholder=placeholder,
             max_chars=max_chars,
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         # It doesn't make sense to create a chat input inside a form.
         # We throw an error to warn the user about this.
         # We omit this check for scripts running outside streamlit, because
         # they will have no script_run_ctx.
         if runtime.exists():
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/checkbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             "toggle" if type == CheckboxProto.StyleType.TOGGLE else "checkbox",
             user_key=key,
             label=label,
             value=bool(value),
             key=key,
             help=help,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         checkbox_proto = CheckboxProto()
         checkbox_proto.id = id
         checkbox_proto.label = label
         checkbox_proto.default = bool(value)
         checkbox_proto.type = type
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/color_picker.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             "color_picker",
             user_key=key,
             label=label,
             value=str(value),
             key=key,
             help=help,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         # set value default
         if value is None:
             value = "#000000"
 
         # make sure the value is a string
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/data_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -879,15 +879,15 @@
             height=height,
             use_container_width=use_container_width,
             column_order=column_order,
             column_config_mapping=str(column_config_mapping),
             num_rows=num_rows,
             key=key,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         proto = ArrowProto()
         proto.id = id
 
         proto.use_container_width = use_container_width
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/file_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
             user_key=key,
             label=label,
             type=type,
             accept_multiple_files=accept_multiple_files,
             key=key,
             help=help,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         if type:
             if isinstance(type, str):
                 type = [type]
 
             # May need a regex or a library to validate file types are valid
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/multiselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
             options=[str(format_func(option)) for option in opt],
             default=indices,
             key=key,
             help=help,
             max_selections=max_selections,
             placeholder=placeholder,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         default_value: list[int] = [] if indices is None else indices
 
         multiselect_proto = MultiSelectProto()
         multiselect_proto.id = id
         multiselect_proto.label = label
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/number_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
             value=value,
             step=step,
             format=format,
             key=key,
             help=help,
             placeholder=None if placeholder is None else str(placeholder),
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         # Ensure that all arguments are of the same type.
         number_input_args = [min_value, max_value, value, step]
 
         int_args = all(
             isinstance(a, (numbers.Integral, type(None), str))
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/radio.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             options=[str(format_func(option)) for option in opt],
             index=index,
             key=key,
             help=help,
             horizontal=horizontal,
             captions=captions,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         if not isinstance(index, int) and index is not None:
             raise StreamlitAPIException(
                 "Radio Value has invalid type: %s" % type(index).__name__
             )
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/select_slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
             user_key=key,
             label=label,
             options=[str(format_func(option)) for option in opt],
             value=slider_value,
             key=key,
             help=help,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         slider_proto = SliderProto()
         slider_proto.id = id
         slider_proto.type = SliderProto.Type.SELECT_SLIDER
         slider_proto.label = label
         slider_proto.format = "%s"
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/selectbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
             label=label,
             options=[str(format_func(option)) for option in opt],
             index=index,
             key=key,
             help=help,
             placeholder=placeholder,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         if not isinstance(index, int) and index is not None:
             raise StreamlitAPIException(
                 "Selectbox Value has invalid type: %s" % type(index).__name__
             )
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
             max_value=max_value,
             value=value,
             step=step,
             format=format,
             key=key,
             help=help,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         SUPPORTED_TYPES = {
             Integral: SliderProto.INT,
             Real: SliderProto.FLOAT,
             datetime: SliderProto.DATETIME,
             date: SliderProto.DATE,
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/text_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
             max_chars=max_chars,
             key=key,
             type=type,
             help=help,
             autocomplete=autocomplete,
             placeholder=str(placeholder),
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         session_state = get_session_state().filtered_state
         if key is not None and key in session_state and session_state[key] is None:
             value = None
 
         text_input_proto = TextInputProto()
@@ -542,15 +542,15 @@
             value=value,
             height=height,
             max_chars=max_chars,
             key=key,
             help=help,
             placeholder=str(placeholder),
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
 
         session_state = get_session_state().filtered_state
         if key is not None and key in session_state and session_state[key] is None:
             value = None
 
         text_area_proto = TextAreaProto()
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/widgets/time_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,15 @@
             user_key=key,
             label=label,
             value=parsed_time if isinstance(value, (datetime, time)) else value,
             key=key,
             help=help,
             step=step,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
         del value
 
         session_state = get_session_state().filtered_state
         if key is not None and key in session_state and session_state[key] is None:
             parsed_time = None
 
@@ -727,15 +727,15 @@
             value=parsed,
             min_value=parsed_min_date,
             max_value=parsed_max_date,
             key=key,
             help=help,
             format=format,
             form_id=current_form_id(self.dg),
-            page=ctx.page_script_hash if ctx else None,
+            page=ctx.active_script_hash if ctx else None,
         )
         if not bool(ALLOWED_DATE_FORMATS.match(format)):
             raise StreamlitAPIException(
                 f"The provided format (`{format}`) is not valid. DateInput format "
                 "should be one of `YYYY/MM/DD`, `DD/MM/YYYY`, or `MM/DD/YYYY` "
                 "and can also use a period (.) or hyphen (-) as separators."
             )
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/elements/write.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/emojis.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/env_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/error_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/errors.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/external/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/file_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/folder_black_list.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/git_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/Hello.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/hello/utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/js_number.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/logger.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/material_icon_names.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/net_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/platform.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Toast_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: streamlit/proto/AppPage.proto
+# source: streamlit/proto/Toast.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dstreamlit/proto/AppPage.proto\"D\n\x07\x41ppPage\x12\x18\n\x10page_script_hash\x18\x01 \x01(\t\x12\x11\n\tpage_name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\tB,\n\x1c\x63om.snowflake.apps.streamlitB\x0c\x41ppPageProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Toast.proto\"#\n\x05Toast\x12\x0c\n\x04\x62ody\x18\x01 \x01(\t\x12\x0c\n\x04icon\x18\x02 \x01(\tB*\n\x1c\x63om.snowflake.apps.streamlitB\nToastProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.AppPage_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.Toast_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\014AppPageProto'
-  _APPPAGE._serialized_start=33
-  _APPPAGE._serialized_end=101
+  DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\nToastProto'
+  _TOAST._serialized_start=31
+  _TOAST._serialized_end=66
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BokehChart_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -24,34 +24,29 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class AppPage(google.protobuf.message.Message):
-    """A page in the app. Includes both the name of the page as well as the full
-    path to the corresponding script file.
-
-    NOTE: This proto type is used by some external services so needs to remain
-    relatively stable. While it isn't entirely set in stone, changing it
-    may require a good amount of effort so should be avoided if possible.
-    """
-
+class BokehChart(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PAGE_SCRIPT_HASH_FIELD_NUMBER: builtins.int
-    PAGE_NAME_FIELD_NUMBER: builtins.int
-    ICON_FIELD_NUMBER: builtins.int
-    page_script_hash: builtins.str
-    page_name: builtins.str
-    icon: builtins.str
+    FIGURE_FIELD_NUMBER: builtins.int
+    USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
+    ELEMENT_ID_FIELD_NUMBER: builtins.int
+    figure: builtins.str
+    """A JSON-formatted string from the Bokeh chart figure."""
+    use_container_width: builtins.bool
+    """If True, will overwrite the chart width spec to fit to container."""
+    element_id: builtins.str
+    """A unique ID of this element."""
     def __init__(
         self,
         *,
-        page_script_hash: builtins.str = ...,
-        page_name: builtins.str = ...,
-        icon: builtins.str = ...,
+        figure: builtins.str = ...,
+        use_container_width: builtins.bool = ...,
+        element_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["icon", b"icon", "page_name", b"page_name", "page_script_hash", b"page_script_hash"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["element_id", b"element_id", "figure", b"figure", "use_container_width", b"use_container_width"]) -> None: ...
 
-global___AppPage = AppPage
+global___BokehChart = BokehChart
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Spinner_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -24,29 +24,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class BokehChart(google.protobuf.message.Message):
+class Spinner(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    FIGURE_FIELD_NUMBER: builtins.int
-    USE_CONTAINER_WIDTH_FIELD_NUMBER: builtins.int
-    ELEMENT_ID_FIELD_NUMBER: builtins.int
-    figure: builtins.str
-    """A JSON-formatted string from the Bokeh chart figure."""
-    use_container_width: builtins.bool
-    """If True, will overwrite the chart width spec to fit to container."""
-    element_id: builtins.str
-    """A unique ID of this element."""
+    TEXT_FIELD_NUMBER: builtins.int
+    CACHE_FIELD_NUMBER: builtins.int
+    text: builtins.str
+    """A message to display while executing that block."""
+    cache: builtins.bool
+    """Whether spinner used in caching functions."""
     def __init__(
         self,
         *,
-        figure: builtins.str = ...,
-        use_container_width: builtins.bool = ...,
-        element_id: builtins.str = ...,
+        text: builtins.str = ...,
+        cache: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["element_id", b"element_id", "figure", b"figure", "use_container_width", b"use_container_width"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cache", b"cache", "text", b"text"]) -> None: ...
 
-global___BokehChart = BokehChart
+global___Spinner = Spinner
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ForwardMsg_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 
 
 from streamlit.proto import AutoRerun_pb2 as streamlit_dot_proto_dot_AutoRerun__pb2
 from streamlit.proto import Common_pb2 as streamlit_dot_proto_dot_Common__pb2
 from streamlit.proto import Delta_pb2 as streamlit_dot_proto_dot_Delta__pb2
 from streamlit.proto import GitInfo_pb2 as streamlit_dot_proto_dot_GitInfo__pb2
 from streamlit.proto import Logo_pb2 as streamlit_dot_proto_dot_Logo__pb2
+from streamlit.proto import Navigation_pb2 as streamlit_dot_proto_dot_Navigation__pb2
 from streamlit.proto import NewSession_pb2 as streamlit_dot_proto_dot_NewSession__pb2
 from streamlit.proto import PageConfig_pb2 as streamlit_dot_proto_dot_PageConfig__pb2
 from streamlit.proto import PageInfo_pb2 as streamlit_dot_proto_dot_PageInfo__pb2
 from streamlit.proto import PageProfile_pb2 as streamlit_dot_proto_dot_PageProfile__pb2
 from streamlit.proto import PageNotFound_pb2 as streamlit_dot_proto_dot_PageNotFound__pb2
 from streamlit.proto import PagesChanged_pb2 as streamlit_dot_proto_dot_PagesChanged__pb2
 from streamlit.proto import ParentMessage_pb2 as streamlit_dot_proto_dot_ParentMessage__pb2
 from streamlit.proto import SessionEvent_pb2 as streamlit_dot_proto_dot_SessionEvent__pb2
 from streamlit.proto import SessionStatus_pb2 as streamlit_dot_proto_dot_SessionStatus__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n streamlit/proto/ForwardMsg.proto\x1a\x1fstreamlit/proto/AutoRerun.proto\x1a\x1cstreamlit/proto/Common.proto\x1a\x1bstreamlit/proto/Delta.proto\x1a\x1dstreamlit/proto/GitInfo.proto\x1a\x1astreamlit/proto/Logo.proto\x1a streamlit/proto/NewSession.proto\x1a streamlit/proto/PageConfig.proto\x1a\x1estreamlit/proto/PageInfo.proto\x1a!streamlit/proto/PageProfile.proto\x1a\"streamlit/proto/PageNotFound.proto\x1a\"streamlit/proto/PagesChanged.proto\x1a#streamlit/proto/ParentMessage.proto\x1a\"streamlit/proto/SessionEvent.proto\x1a#streamlit/proto/SessionStatus.proto\"\xfc\x06\n\nForwardMsg\x12\x0c\n\x04hash\x18\x01 \x01(\t\x12%\n\x08metadata\x18\x02 \x01(\x0b\x32\x13.ForwardMsgMetadata\x12\"\n\x0bnew_session\x18\x04 \x01(\x0b\x32\x0b.NewSessionH\x00\x12\x17\n\x05\x64\x65lta\x18\x05 \x01(\x0b\x32\x06.DeltaH\x00\x12&\n\x11page_info_changed\x18\x0c \x01(\x0b\x32\t.PageInfoH\x00\x12*\n\x13page_config_changed\x18\r \x01(\x0b\x32\x0b.PageConfigH\x00\x12;\n\x0fscript_finished\x18\x06 \x01(\x0e\x32 .ForwardMsg.ScriptFinishedStatusH\x00\x12$\n\x10git_info_changed\x18\x0e \x01(\x0b\x32\x08.GitInfoH\x00\x12$\n\x0cpage_profile\x18\x12 \x01(\x0b\x32\x0c.PageProfileH\x00\x12\x30\n\x16session_status_changed\x18\t \x01(\x0b\x32\x0e.SessionStatusH\x00\x12&\n\rsession_event\x18\n \x01(\x0b\x32\r.SessionEventH\x00\x12\'\n\x0epage_not_found\x18\x0f \x01(\x0b\x32\r.PageNotFoundH\x00\x12&\n\rpages_changed\x18\x10 \x01(\x0b\x32\r.PagesChangedH\x00\x12/\n\x12\x66ile_urls_response\x18\x13 \x01(\x0b\x32\x11.FileURLsResponseH\x00\x12 \n\nauto_rerun\x18\x15 \x01(\x0b\x32\n.AutoRerunH\x00\x12\x15\n\x04logo\x18\x16 \x01(\x0b\x32\x05.LogoH\x00\x12(\n\x0eparent_message\x18\x14 \x01(\x0b\x32\x0e.ParentMessageH\x00\x12\x12\n\x08ref_hash\x18\x0b \x01(\tH\x00\x12\x1d\n\x15\x64\x65\x62ug_last_backmsg_id\x18\x11 \x01(\t\"\x98\x01\n\x14ScriptFinishedStatus\x12\x19\n\x15\x46INISHED_SUCCESSFULLY\x10\x00\x12\x1f\n\x1b\x46INISHED_WITH_COMPILE_ERROR\x10\x01\x12\x1c\n\x18\x46INISHED_EARLY_FOR_RERUN\x10\x02\x12&\n\"FINISHED_FRAGMENT_RUN_SUCCESSFULLY\x10\x03\x42\x06\n\x04typeJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"r\n\x12\x46orwardMsgMetadata\x12\x11\n\tcacheable\x18\x01 \x01(\x08\x12\x12\n\ndelta_path\x18\x02 \x03(\r\x12\x35\n\x16\x65lement_dimension_spec\x18\x03 \x01(\x0b\x32\x15.ElementDimensionSpec\"5\n\x14\x45lementDimensionSpec\x12\r\n\x05width\x18\x01 \x01(\r\x12\x0e\n\x06height\x18\x02 \x01(\rB/\n\x1c\x63om.snowflake.apps.streamlitB\x0f\x46orwardMsgProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n streamlit/proto/ForwardMsg.proto\x1a\x1fstreamlit/proto/AutoRerun.proto\x1a\x1cstreamlit/proto/Common.proto\x1a\x1bstreamlit/proto/Delta.proto\x1a\x1dstreamlit/proto/GitInfo.proto\x1a\x1astreamlit/proto/Logo.proto\x1a streamlit/proto/Navigation.proto\x1a streamlit/proto/NewSession.proto\x1a streamlit/proto/PageConfig.proto\x1a\x1estreamlit/proto/PageInfo.proto\x1a!streamlit/proto/PageProfile.proto\x1a\"streamlit/proto/PageNotFound.proto\x1a\"streamlit/proto/PagesChanged.proto\x1a#streamlit/proto/ParentMessage.proto\x1a\"streamlit/proto/SessionEvent.proto\x1a#streamlit/proto/SessionStatus.proto\"\x9f\x07\n\nForwardMsg\x12\x0c\n\x04hash\x18\x01 \x01(\t\x12%\n\x08metadata\x18\x02 \x01(\x0b\x32\x13.ForwardMsgMetadata\x12\"\n\x0bnew_session\x18\x04 \x01(\x0b\x32\x0b.NewSessionH\x00\x12\x17\n\x05\x64\x65lta\x18\x05 \x01(\x0b\x32\x06.DeltaH\x00\x12&\n\x11page_info_changed\x18\x0c \x01(\x0b\x32\t.PageInfoH\x00\x12*\n\x13page_config_changed\x18\r \x01(\x0b\x32\x0b.PageConfigH\x00\x12;\n\x0fscript_finished\x18\x06 \x01(\x0e\x32 .ForwardMsg.ScriptFinishedStatusH\x00\x12$\n\x10git_info_changed\x18\x0e \x01(\x0b\x32\x08.GitInfoH\x00\x12$\n\x0cpage_profile\x18\x12 \x01(\x0b\x32\x0c.PageProfileH\x00\x12\x30\n\x16session_status_changed\x18\t \x01(\x0b\x32\x0e.SessionStatusH\x00\x12&\n\rsession_event\x18\n \x01(\x0b\x32\r.SessionEventH\x00\x12!\n\nnavigation\x18\x17 \x01(\x0b\x32\x0b.NavigationH\x00\x12\'\n\x0epage_not_found\x18\x0f \x01(\x0b\x32\r.PageNotFoundH\x00\x12&\n\rpages_changed\x18\x10 \x01(\x0b\x32\r.PagesChangedH\x00\x12/\n\x12\x66ile_urls_response\x18\x13 \x01(\x0b\x32\x11.FileURLsResponseH\x00\x12 \n\nauto_rerun\x18\x15 \x01(\x0b\x32\n.AutoRerunH\x00\x12\x15\n\x04logo\x18\x16 \x01(\x0b\x32\x05.LogoH\x00\x12(\n\x0eparent_message\x18\x14 \x01(\x0b\x32\x0e.ParentMessageH\x00\x12\x12\n\x08ref_hash\x18\x0b \x01(\tH\x00\x12\x1d\n\x15\x64\x65\x62ug_last_backmsg_id\x18\x11 \x01(\t\"\x98\x01\n\x14ScriptFinishedStatus\x12\x19\n\x15\x46INISHED_SUCCESSFULLY\x10\x00\x12\x1f\n\x1b\x46INISHED_WITH_COMPILE_ERROR\x10\x01\x12\x1c\n\x18\x46INISHED_EARLY_FOR_RERUN\x10\x02\x12&\n\"FINISHED_FRAGMENT_RUN_SUCCESSFULLY\x10\x03\x42\x06\n\x04typeJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"\x8e\x01\n\x12\x46orwardMsgMetadata\x12\x11\n\tcacheable\x18\x01 \x01(\x08\x12\x12\n\ndelta_path\x18\x02 \x03(\r\x12\x35\n\x16\x65lement_dimension_spec\x18\x03 \x01(\x0b\x32\x15.ElementDimensionSpec\x12\x1a\n\x12\x61\x63tive_script_hash\x18\x04 \x01(\t\"5\n\x14\x45lementDimensionSpec\x12\r\n\x05width\x18\x01 \x01(\r\x12\x0e\n\x06height\x18\x02 \x01(\rB/\n\x1c\x63om.snowflake.apps.streamlitB\x0f\x46orwardMsgProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.ForwardMsg_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\017ForwardMsgProto'
-  _FORWARDMSG._serialized_start=505
-  _FORWARDMSG._serialized_end=1397
-  _FORWARDMSG_SCRIPTFINISHEDSTATUS._serialized_start=1225
-  _FORWARDMSG_SCRIPTFINISHEDSTATUS._serialized_end=1377
-  _FORWARDMSGMETADATA._serialized_start=1399
-  _FORWARDMSGMETADATA._serialized_end=1513
-  _ELEMENTDIMENSIONSPEC._serialized_start=1515
-  _ELEMENTDIMENSIONSPEC._serialized_end=1568
+  _FORWARDMSG._serialized_start=539
+  _FORWARDMSG._serialized_end=1466
+  _FORWARDMSG_SCRIPTFINISHEDSTATUS._serialized_start=1294
+  _FORWARDMSG_SCRIPTFINISHEDSTATUS._serialized_end=1446
+  _FORWARDMSGMETADATA._serialized_start=1469
+  _FORWARDMSGMETADATA._serialized_end=1611
+  _ELEMENTDIMENSIONSPEC._serialized_start=1613
+  _ELEMENTDIMENSIONSPEC._serialized_end=1666
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import streamlit.proto.AutoRerun_pb2
 import streamlit.proto.Common_pb2
 import streamlit.proto.Delta_pb2
 import streamlit.proto.GitInfo_pb2
 import streamlit.proto.Logo_pb2
+import streamlit.proto.Navigation_pb2
 import streamlit.proto.NewSession_pb2
 import streamlit.proto.PageConfig_pb2
 import streamlit.proto.PageInfo_pb2
 import streamlit.proto.PageNotFound_pb2
 import streamlit.proto.PageProfile_pb2
 import streamlit.proto.PagesChanged_pb2
 import streamlit.proto.ParentMessage_pb2
@@ -85,14 +86,15 @@
     PAGE_INFO_CHANGED_FIELD_NUMBER: builtins.int
     PAGE_CONFIG_CHANGED_FIELD_NUMBER: builtins.int
     SCRIPT_FINISHED_FIELD_NUMBER: builtins.int
     GIT_INFO_CHANGED_FIELD_NUMBER: builtins.int
     PAGE_PROFILE_FIELD_NUMBER: builtins.int
     SESSION_STATUS_CHANGED_FIELD_NUMBER: builtins.int
     SESSION_EVENT_FIELD_NUMBER: builtins.int
+    NAVIGATION_FIELD_NUMBER: builtins.int
     PAGE_NOT_FOUND_FIELD_NUMBER: builtins.int
     PAGES_CHANGED_FIELD_NUMBER: builtins.int
     FILE_URLS_RESPONSE_FIELD_NUMBER: builtins.int
     AUTO_RERUN_FIELD_NUMBER: builtins.int
     LOGO_FIELD_NUMBER: builtins.int
     PARENT_MESSAGE_FIELD_NUMBER: builtins.int
     REF_HASH_FIELD_NUMBER: builtins.int
@@ -120,17 +122,19 @@
     def page_profile(self) -> streamlit.proto.PageProfile_pb2.PageProfile: ...
     @property
     def session_status_changed(self) -> streamlit.proto.SessionStatus_pb2.SessionStatus:
         """Status change and event messages."""
     @property
     def session_event(self) -> streamlit.proto.SessionEvent_pb2.SessionEvent: ...
     @property
-    def page_not_found(self) -> streamlit.proto.PageNotFound_pb2.PageNotFound:
+    def navigation(self) -> streamlit.proto.Navigation_pb2.Navigation:
         """Other messages."""
     @property
+    def page_not_found(self) -> streamlit.proto.PageNotFound_pb2.PageNotFound: ...
+    @property
     def pages_changed(self) -> streamlit.proto.PagesChanged_pb2.PagesChanged: ...
     @property
     def file_urls_response(self) -> streamlit.proto.Common_pb2.FileURLsResponse: ...
     @property
     def auto_rerun(self) -> streamlit.proto.AutoRerun_pb2.AutoRerun: ...
     @property
     def logo(self) -> streamlit.proto.Logo_pb2.Logo:
@@ -159,26 +163,27 @@
         page_info_changed: streamlit.proto.PageInfo_pb2.PageInfo | None = ...,
         page_config_changed: streamlit.proto.PageConfig_pb2.PageConfig | None = ...,
         script_finished: global___ForwardMsg.ScriptFinishedStatus.ValueType = ...,
         git_info_changed: streamlit.proto.GitInfo_pb2.GitInfo | None = ...,
         page_profile: streamlit.proto.PageProfile_pb2.PageProfile | None = ...,
         session_status_changed: streamlit.proto.SessionStatus_pb2.SessionStatus | None = ...,
         session_event: streamlit.proto.SessionEvent_pb2.SessionEvent | None = ...,
+        navigation: streamlit.proto.Navigation_pb2.Navigation | None = ...,
         page_not_found: streamlit.proto.PageNotFound_pb2.PageNotFound | None = ...,
         pages_changed: streamlit.proto.PagesChanged_pb2.PagesChanged | None = ...,
         file_urls_response: streamlit.proto.Common_pb2.FileURLsResponse | None = ...,
         auto_rerun: streamlit.proto.AutoRerun_pb2.AutoRerun | None = ...,
         logo: streamlit.proto.Logo_pb2.Logo | None = ...,
         parent_message: streamlit.proto.ParentMessage_pb2.ParentMessage | None = ...,
         ref_hash: builtins.str = ...,
         debug_last_backmsg_id: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["auto_rerun", b"auto_rerun", "delta", b"delta", "file_urls_response", b"file_urls_response", "git_info_changed", b"git_info_changed", "logo", b"logo", "metadata", b"metadata", "new_session", b"new_session", "page_config_changed", b"page_config_changed", "page_info_changed", b"page_info_changed", "page_not_found", b"page_not_found", "page_profile", b"page_profile", "pages_changed", b"pages_changed", "parent_message", b"parent_message", "ref_hash", b"ref_hash", "script_finished", b"script_finished", "session_event", b"session_event", "session_status_changed", b"session_status_changed", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["auto_rerun", b"auto_rerun", "debug_last_backmsg_id", b"debug_last_backmsg_id", "delta", b"delta", "file_urls_response", b"file_urls_response", "git_info_changed", b"git_info_changed", "hash", b"hash", "logo", b"logo", "metadata", b"metadata", "new_session", b"new_session", "page_config_changed", b"page_config_changed", "page_info_changed", b"page_info_changed", "page_not_found", b"page_not_found", "page_profile", b"page_profile", "pages_changed", b"pages_changed", "parent_message", b"parent_message", "ref_hash", b"ref_hash", "script_finished", b"script_finished", "session_event", b"session_event", "session_status_changed", b"session_status_changed", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["new_session", "delta", "page_info_changed", "page_config_changed", "script_finished", "git_info_changed", "page_profile", "session_status_changed", "session_event", "page_not_found", "pages_changed", "file_urls_response", "auto_rerun", "logo", "parent_message", "ref_hash"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["auto_rerun", b"auto_rerun", "delta", b"delta", "file_urls_response", b"file_urls_response", "git_info_changed", b"git_info_changed", "logo", b"logo", "metadata", b"metadata", "navigation", b"navigation", "new_session", b"new_session", "page_config_changed", b"page_config_changed", "page_info_changed", b"page_info_changed", "page_not_found", b"page_not_found", "page_profile", b"page_profile", "pages_changed", b"pages_changed", "parent_message", b"parent_message", "ref_hash", b"ref_hash", "script_finished", b"script_finished", "session_event", b"session_event", "session_status_changed", b"session_status_changed", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["auto_rerun", b"auto_rerun", "debug_last_backmsg_id", b"debug_last_backmsg_id", "delta", b"delta", "file_urls_response", b"file_urls_response", "git_info_changed", b"git_info_changed", "hash", b"hash", "logo", b"logo", "metadata", b"metadata", "navigation", b"navigation", "new_session", b"new_session", "page_config_changed", b"page_config_changed", "page_info_changed", b"page_info_changed", "page_not_found", b"page_not_found", "page_profile", b"page_profile", "pages_changed", b"pages_changed", "parent_message", b"parent_message", "ref_hash", b"ref_hash", "script_finished", b"script_finished", "session_event", b"session_event", "session_status_changed", b"session_status_changed", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["new_session", "delta", "page_info_changed", "page_config_changed", "script_finished", "git_info_changed", "page_profile", "session_status_changed", "session_event", "navigation", "page_not_found", "pages_changed", "file_urls_response", "auto_rerun", "logo", "parent_message", "ref_hash"] | None: ...
 
 global___ForwardMsg = ForwardMsg
 
 class ForwardMsgMetadata(google.protobuf.message.Message):
     """ForwardMsgMetadata contains all data that does _not_ get hashed (or cached)
     in our ForwardMsgCache. (That is, when we cache a ForwardMsg, we clear its
     metadata field first.) This allows us to, e.g., have a large unchanging
@@ -187,35 +192,42 @@
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CACHEABLE_FIELD_NUMBER: builtins.int
     DELTA_PATH_FIELD_NUMBER: builtins.int
     ELEMENT_DIMENSION_SPEC_FIELD_NUMBER: builtins.int
+    ACTIVE_SCRIPT_HASH_FIELD_NUMBER: builtins.int
     cacheable: builtins.bool
     """If this is set, the server will have cached this message,
     and a client that receives it should do the same.
     """
     @property
     def delta_path(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The path that identifies a delta's location in the report tree.
         Only set for Delta messages.
         """
     @property
     def element_dimension_spec(self) -> global___ElementDimensionSpec:
         """DEPRECATED: This is not used anymore."""
+    active_script_hash: builtins.str
+    """active_script_hash the forward message is associated from.
+    For multipage apps v1, this will always be the page file running
+    For multipage apps v2, this can be the main script or the page script
+    """
     def __init__(
         self,
         *,
         cacheable: builtins.bool = ...,
         delta_path: collections.abc.Iterable[builtins.int] | None = ...,
         element_dimension_spec: global___ElementDimensionSpec | None = ...,
+        active_script_hash: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["element_dimension_spec", b"element_dimension_spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cacheable", b"cacheable", "delta_path", b"delta_path", "element_dimension_spec", b"element_dimension_spec"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["active_script_hash", b"active_script_hash", "cacheable", b"cacheable", "delta_path", b"delta_path", "element_dimension_spec", b"element_dimension_spec"]) -> None: ...
 
 global___ForwardMsgMetadata = ForwardMsgMetadata
 
 class ElementDimensionSpec(google.protobuf.message.Message):
     """DEPRECATED: This is not used anymore.
     Specifies the dimensions for the element
     """
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NewSession_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 _sym_db = _symbol_database.Default()
 
 
 from streamlit.proto import AppPage_pb2 as streamlit_dot_proto_dot_AppPage__pb2
 from streamlit.proto import SessionStatus_pb2 as streamlit_dot_proto_dot_SessionStatus__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n streamlit/proto/NewSession.proto\x1a\x1dstreamlit/proto/AppPage.proto\x1a#streamlit/proto/SessionStatus.proto\"\x8b\x02\n\nNewSession\x12\x1f\n\ninitialize\x18\x01 \x01(\x0b\x32\x0b.Initialize\x12\x15\n\rscript_run_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x18\n\x10main_script_path\x18\x04 \x01(\t\x12\x17\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x07.Config\x12(\n\x0c\x63ustom_theme\x18\x07 \x01(\x0b\x32\x12.CustomThemeConfig\x12\x1b\n\tapp_pages\x18\x08 \x03(\x0b\x32\x08.AppPage\x12\x18\n\x10page_script_hash\x18\t \x01(\t\x12\x1d\n\x15\x66ragment_ids_this_run\x18\n \x03(\tJ\x04\x08\x05\x10\x06\"\xba\x01\n\nInitialize\x12\x1c\n\tuser_info\x18\x01 \x01(\x0b\x32\t.UserInfo\x12*\n\x10\x65nvironment_info\x18\x03 \x01(\x0b\x32\x10.EnvironmentInfo\x12&\n\x0esession_status\x18\x04 \x01(\x0b\x32\x0e.SessionStatus\x12\x14\n\x0c\x63ommand_line\x18\x05 \x01(\t\x12\x12\n\nsession_id\x18\x06 \x01(\t\x12\x10\n\x08is_hello\x18\x07 \x01(\x08\"\x97\x02\n\x06\x43onfig\x12\x1a\n\x12gather_usage_stats\x18\x02 \x01(\x08\x12\x1e\n\x16max_cached_message_age\x18\x03 \x01(\x05\x12\x14\n\x0cmapbox_token\x18\x04 \x01(\t\x12\x19\n\x11\x61llow_run_on_save\x18\x05 \x01(\x08\x12\x14\n\x0chide_top_bar\x18\x06 \x01(\x08\x12\x18\n\x10hide_sidebar_nav\x18\x07 \x01(\x08\x12)\n\x0ctoolbar_mode\x18\x08 \x01(\x0e\x32\x13.Config.ToolbarMode\"?\n\x0bToolbarMode\x12\x08\n\x04\x41UTO\x10\x00\x12\r\n\tDEVELOPER\x10\x01\x12\n\n\x06VIEWER\x10\x02\x12\x0b\n\x07MINIMAL\x10\x03J\x04\x08\x01\x10\x02\"\x8c\x04\n\x11\x43ustomThemeConfig\x12\x15\n\rprimary_color\x18\x01 \x01(\t\x12\"\n\x1asecondary_background_color\x18\x02 \x01(\t\x12\x18\n\x10\x62\x61\x63kground_color\x18\x03 \x01(\t\x12\x12\n\ntext_color\x18\x04 \x01(\t\x12+\n\x04\x66ont\x18\x05 \x01(\x0e\x32\x1d.CustomThemeConfig.FontFamily\x12*\n\x04\x62\x61se\x18\x06 \x01(\x0e\x32\x1c.CustomThemeConfig.BaseTheme\x12\x1f\n\x17widget_background_color\x18\x07 \x01(\t\x12\x1b\n\x13widget_border_color\x18\x08 \x01(\t\x12\x15\n\x05radii\x18\t \x01(\x0b\x32\x06.Radii\x12\x11\n\tbody_font\x18\r \x01(\t\x12\x11\n\tcode_font\x18\x0e \x01(\t\x12\x1d\n\nfont_faces\x18\x0f \x03(\x0b\x32\t.FontFace\x12\x1e\n\nfont_sizes\x18\x10 \x01(\x0b\x32\n.FontSizes\x12!\n\x19skeleton_background_color\x18\x11 \x01(\t\" \n\tBaseTheme\x12\t\n\x05LIGHT\x10\x00\x12\x08\n\x04\x44\x41RK\x10\x01\"6\n\nFontFamily\x12\x0e\n\nSANS_SERIF\x10\x00\x12\t\n\x05SERIF\x10\x01\x12\r\n\tMONOSPACE\x10\x02\"F\n\x08\x46ontFace\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61mily\x18\x02 \x01(\t\x12\x0e\n\x06weight\x18\x03 \x01(\x05\x12\r\n\x05style\x18\x04 \x01(\t\"<\n\x05Radii\x12\x1a\n\x12\x62\x61se_widget_radius\x18\x01 \x01(\x05\x12\x17\n\x0f\x63heckbox_radius\x18\x02 \x01(\x05\"T\n\tFontSizes\x12\x16\n\x0etiny_font_size\x18\x01 \x01(\x05\x12\x17\n\x0fsmall_font_size\x18\x02 \x01(\x05\x12\x16\n\x0e\x62\x61se_font_size\x18\x03 \x01(\x05\"E\n\x08UserInfo\x12\x17\n\x0finstallation_id\x18\x01 \x01(\t\x12\x1a\n\x12installation_id_v3\x18\x05 \x01(\tJ\x04\x08\x02\x10\x03\"D\n\x0f\x45nvironmentInfo\x12\x19\n\x11streamlit_version\x18\x01 \x01(\t\x12\x16\n\x0epython_version\x18\x02 \x01(\tB/\n\x1c\x63om.snowflake.apps.streamlitB\x0fNewSessionProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n streamlit/proto/NewSession.proto\x1a\x1dstreamlit/proto/AppPage.proto\x1a#streamlit/proto/SessionStatus.proto\"\xa5\x02\n\nNewSession\x12\x1f\n\ninitialize\x18\x01 \x01(\x0b\x32\x0b.Initialize\x12\x15\n\rscript_run_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x18\n\x10main_script_path\x18\x04 \x01(\t\x12\x17\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x07.Config\x12(\n\x0c\x63ustom_theme\x18\x07 \x01(\x0b\x32\x12.CustomThemeConfig\x12\x1b\n\tapp_pages\x18\x08 \x03(\x0b\x32\x08.AppPage\x12\x18\n\x10page_script_hash\x18\t \x01(\t\x12\x1d\n\x15\x66ragment_ids_this_run\x18\n \x03(\t\x12\x18\n\x10main_script_hash\x18\x0b \x01(\tJ\x04\x08\x05\x10\x06\"\xba\x01\n\nInitialize\x12\x1c\n\tuser_info\x18\x01 \x01(\x0b\x32\t.UserInfo\x12*\n\x10\x65nvironment_info\x18\x03 \x01(\x0b\x32\x10.EnvironmentInfo\x12&\n\x0esession_status\x18\x04 \x01(\x0b\x32\x0e.SessionStatus\x12\x14\n\x0c\x63ommand_line\x18\x05 \x01(\t\x12\x12\n\nsession_id\x18\x06 \x01(\t\x12\x10\n\x08is_hello\x18\x07 \x01(\x08\"\x97\x02\n\x06\x43onfig\x12\x1a\n\x12gather_usage_stats\x18\x02 \x01(\x08\x12\x1e\n\x16max_cached_message_age\x18\x03 \x01(\x05\x12\x14\n\x0cmapbox_token\x18\x04 \x01(\t\x12\x19\n\x11\x61llow_run_on_save\x18\x05 \x01(\x08\x12\x14\n\x0chide_top_bar\x18\x06 \x01(\x08\x12\x18\n\x10hide_sidebar_nav\x18\x07 \x01(\x08\x12)\n\x0ctoolbar_mode\x18\x08 \x01(\x0e\x32\x13.Config.ToolbarMode\"?\n\x0bToolbarMode\x12\x08\n\x04\x41UTO\x10\x00\x12\r\n\tDEVELOPER\x10\x01\x12\n\n\x06VIEWER\x10\x02\x12\x0b\n\x07MINIMAL\x10\x03J\x04\x08\x01\x10\x02\"\x8c\x04\n\x11\x43ustomThemeConfig\x12\x15\n\rprimary_color\x18\x01 \x01(\t\x12\"\n\x1asecondary_background_color\x18\x02 \x01(\t\x12\x18\n\x10\x62\x61\x63kground_color\x18\x03 \x01(\t\x12\x12\n\ntext_color\x18\x04 \x01(\t\x12+\n\x04\x66ont\x18\x05 \x01(\x0e\x32\x1d.CustomThemeConfig.FontFamily\x12*\n\x04\x62\x61se\x18\x06 \x01(\x0e\x32\x1c.CustomThemeConfig.BaseTheme\x12\x1f\n\x17widget_background_color\x18\x07 \x01(\t\x12\x1b\n\x13widget_border_color\x18\x08 \x01(\t\x12\x15\n\x05radii\x18\t \x01(\x0b\x32\x06.Radii\x12\x11\n\tbody_font\x18\r \x01(\t\x12\x11\n\tcode_font\x18\x0e \x01(\t\x12\x1d\n\nfont_faces\x18\x0f \x03(\x0b\x32\t.FontFace\x12\x1e\n\nfont_sizes\x18\x10 \x01(\x0b\x32\n.FontSizes\x12!\n\x19skeleton_background_color\x18\x11 \x01(\t\" \n\tBaseTheme\x12\t\n\x05LIGHT\x10\x00\x12\x08\n\x04\x44\x41RK\x10\x01\"6\n\nFontFamily\x12\x0e\n\nSANS_SERIF\x10\x00\x12\t\n\x05SERIF\x10\x01\x12\r\n\tMONOSPACE\x10\x02\"F\n\x08\x46ontFace\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61mily\x18\x02 \x01(\t\x12\x0e\n\x06weight\x18\x03 \x01(\x05\x12\r\n\x05style\x18\x04 \x01(\t\"<\n\x05Radii\x12\x1a\n\x12\x62\x61se_widget_radius\x18\x01 \x01(\x05\x12\x17\n\x0f\x63heckbox_radius\x18\x02 \x01(\x05\"T\n\tFontSizes\x12\x16\n\x0etiny_font_size\x18\x01 \x01(\x05\x12\x17\n\x0fsmall_font_size\x18\x02 \x01(\x05\x12\x16\n\x0e\x62\x61se_font_size\x18\x03 \x01(\x05\"E\n\x08UserInfo\x12\x17\n\x0finstallation_id\x18\x01 \x01(\t\x12\x1a\n\x12installation_id_v3\x18\x05 \x01(\tJ\x04\x08\x02\x10\x03\"D\n\x0f\x45nvironmentInfo\x12\x19\n\x11streamlit_version\x18\x01 \x01(\t\x12\x16\n\x0epython_version\x18\x02 \x01(\tB/\n\x1c\x63om.snowflake.apps.streamlitB\x0fNewSessionProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.NewSession_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\017NewSessionProto'
   _NEWSESSION._serialized_start=105
-  _NEWSESSION._serialized_end=372
-  _INITIALIZE._serialized_start=375
-  _INITIALIZE._serialized_end=561
-  _CONFIG._serialized_start=564
-  _CONFIG._serialized_end=843
-  _CONFIG_TOOLBARMODE._serialized_start=774
-  _CONFIG_TOOLBARMODE._serialized_end=837
-  _CUSTOMTHEMECONFIG._serialized_start=846
-  _CUSTOMTHEMECONFIG._serialized_end=1370
-  _CUSTOMTHEMECONFIG_BASETHEME._serialized_start=1282
-  _CUSTOMTHEMECONFIG_BASETHEME._serialized_end=1314
-  _CUSTOMTHEMECONFIG_FONTFAMILY._serialized_start=1316
-  _CUSTOMTHEMECONFIG_FONTFAMILY._serialized_end=1370
-  _FONTFACE._serialized_start=1372
-  _FONTFACE._serialized_end=1442
-  _RADII._serialized_start=1444
-  _RADII._serialized_end=1504
-  _FONTSIZES._serialized_start=1506
-  _FONTSIZES._serialized_end=1590
-  _USERINFO._serialized_start=1592
-  _USERINFO._serialized_end=1661
-  _ENVIRONMENTINFO._serialized_start=1663
-  _ENVIRONMENTINFO._serialized_end=1731
+  _NEWSESSION._serialized_end=398
+  _INITIALIZE._serialized_start=401
+  _INITIALIZE._serialized_end=587
+  _CONFIG._serialized_start=590
+  _CONFIG._serialized_end=869
+  _CONFIG_TOOLBARMODE._serialized_start=800
+  _CONFIG_TOOLBARMODE._serialized_end=863
+  _CUSTOMTHEMECONFIG._serialized_start=872
+  _CUSTOMTHEMECONFIG._serialized_end=1396
+  _CUSTOMTHEMECONFIG_BASETHEME._serialized_start=1308
+  _CUSTOMTHEMECONFIG_BASETHEME._serialized_end=1340
+  _CUSTOMTHEMECONFIG_FONTFAMILY._serialized_start=1342
+  _CUSTOMTHEMECONFIG_FONTFAMILY._serialized_end=1396
+  _FONTFACE._serialized_start=1398
+  _FONTFACE._serialized_end=1468
+  _RADII._serialized_start=1470
+  _RADII._serialized_end=1530
+  _FONTSIZES._serialized_start=1532
+  _FONTSIZES._serialized_end=1616
+  _USERINFO._serialized_start=1618
+  _USERINFO._serialized_end=1687
+  _ENVIRONMENTINFO._serialized_start=1689
+  _ENVIRONMENTINFO._serialized_end=1757
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NewSession_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     NAME_FIELD_NUMBER: builtins.int
     MAIN_SCRIPT_PATH_FIELD_NUMBER: builtins.int
     CONFIG_FIELD_NUMBER: builtins.int
     CUSTOM_THEME_FIELD_NUMBER: builtins.int
     APP_PAGES_FIELD_NUMBER: builtins.int
     PAGE_SCRIPT_HASH_FIELD_NUMBER: builtins.int
     FRAGMENT_IDS_THIS_RUN_FIELD_NUMBER: builtins.int
+    MAIN_SCRIPT_HASH_FIELD_NUMBER: builtins.int
     @property
     def initialize(self) -> global___Initialize:
         """Initialization data. This data does *not* change from rerun to rerun,
         but we send it every time so that we don't have to track whether the
         client has already received it. The client is responsible for
         performing initialization logic only once.
         """
@@ -84,29 +85,32 @@
     page_script_hash: builtins.str
     """A hash of the script corresponding to the page currently being viewed."""
     @property
     def fragment_ids_this_run(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """The fragment IDs being run in this session if it corresponds to a fragment
         script run.
         """
+    main_script_hash: builtins.str
+    """Hash of the main script running (ie streamlit run main_script.py)"""
     def __init__(
         self,
         *,
         initialize: global___Initialize | None = ...,
         script_run_id: builtins.str = ...,
         name: builtins.str = ...,
         main_script_path: builtins.str = ...,
         config: global___Config | None = ...,
         custom_theme: global___CustomThemeConfig | None = ...,
         app_pages: collections.abc.Iterable[streamlit.proto.AppPage_pb2.AppPage] | None = ...,
         page_script_hash: builtins.str = ...,
         fragment_ids_this_run: collections.abc.Iterable[builtins.str] | None = ...,
+        main_script_hash: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config", "custom_theme", b"custom_theme", "initialize", b"initialize"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_pages", b"app_pages", "config", b"config", "custom_theme", b"custom_theme", "fragment_ids_this_run", b"fragment_ids_this_run", "initialize", b"initialize", "main_script_path", b"main_script_path", "name", b"name", "page_script_hash", b"page_script_hash", "script_run_id", b"script_run_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_pages", b"app_pages", "config", b"config", "custom_theme", b"custom_theme", "fragment_ids_this_run", b"fragment_ids_this_run", "initialize", b"initialize", "main_script_hash", b"main_script_hash", "main_script_path", b"main_script_path", "name", b"name", "page_script_hash", b"page_script_hash", "script_run_id", b"script_run_id"]) -> None: ...
 
 global___NewSession = NewSession
 
 class Initialize(google.protobuf.message.Message):
     """Contains the session status that existed at the time the user connected.
     The contents of this message don't change over the lifetime of the app by
     definition.
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Text_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class Spinner(google.protobuf.message.Message):
+class Text(google.protobuf.message.Message):
+    """Preformatted text"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TEXT_FIELD_NUMBER: builtins.int
-    CACHE_FIELD_NUMBER: builtins.int
-    text: builtins.str
-    """A message to display while executing that block."""
-    cache: builtins.bool
-    """Whether spinner used in caching functions."""
+    BODY_FIELD_NUMBER: builtins.int
+    HELP_FIELD_NUMBER: builtins.int
+    body: builtins.str
+    """Content to display."""
+    help: builtins.str
     def __init__(
         self,
         *,
-        text: builtins.str = ...,
-        cache: builtins.bool = ...,
+        body: builtins.str = ...,
+        help: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cache", b"cache", "text", b"text"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "help", b"help"]) -> None: ...
 
-global___Spinner = Spinner
+global___Text = Text
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Toast_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -24,26 +24,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class Text(google.protobuf.message.Message):
-    """Preformatted text"""
-
+class Toast(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BODY_FIELD_NUMBER: builtins.int
-    HELP_FIELD_NUMBER: builtins.int
+    ICON_FIELD_NUMBER: builtins.int
     body: builtins.str
-    """Content to display."""
-    help: builtins.str
+    """Display message"""
+    icon: builtins.str
+    """Emoji"""
     def __init__(
         self,
         *,
         body: builtins.str = ...,
-        help: builtins.str = ...,
+        icon: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "help", b"help"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "icon", b"icon"]) -> None: ...
 
-global___Text = Text
+global___Toast = Toast
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/AppPage_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: streamlit/proto/Toast.proto
+# source: streamlit/proto/AppPage.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Toast.proto\"#\n\x05Toast\x12\x0c\n\x04\x62ody\x18\x01 \x01(\t\x12\x0c\n\x04icon\x18\x02 \x01(\tB*\n\x1c\x63om.snowflake.apps.streamlitB\nToastProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dstreamlit/proto/AppPage.proto\"\x86\x01\n\x07\x41ppPage\x12\x18\n\x10page_script_hash\x18\x01 \x01(\t\x12\x11\n\tpage_name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x12\n\nis_default\x18\x04 \x01(\x08\x12\x16\n\x0esection_header\x18\x05 \x01(\t\x12\x14\n\x0curl_pathname\x18\x06 \x01(\tB,\n\x1c\x63om.snowflake.apps.streamlitB\x0c\x41ppPageProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.Toast_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.AppPage_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\nToastProto'
-  _TOAST._serialized_start=31
-  _TOAST._serialized_end=66
+  DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\014AppPageProto'
+  _APPPAGE._serialized_start=34
+  _APPPAGE._serialized_end=168
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240531/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/app_session.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/app_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import asyncio
 import sys
 import uuid
 from enum import Enum
 from typing import TYPE_CHECKING, Callable, Final
 
 import streamlit.elements.exception as exception_utils
-from streamlit import config, runtime, source_util
+from streamlit import config, runtime
 from streamlit.case_converters import to_snake_case
 from streamlit.logger import get_logger
 from streamlit.proto.BackMsg_pb2 import BackMsg
 from streamlit.proto.ClientState_pb2 import ClientState
 from streamlit.proto.Common_pb2 import FileURLs, FileURLsRequest
 from streamlit.proto.ForwardMsg_pb2 import ForwardMsg
 from streamlit.proto.GitInfo_pb2 import GitInfo
@@ -36,19 +36,21 @@
     UserInfo,
 )
 from streamlit.proto.PagesChanged_pb2 import PagesChanged
 from streamlit.runtime import caching
 from streamlit.runtime.forward_msg_queue import ForwardMsgQueue
 from streamlit.runtime.fragment import FragmentStorage, MemoryFragmentStorage
 from streamlit.runtime.metrics_util import Installation
+from streamlit.runtime.pages_manager import PagesManager
 from streamlit.runtime.script_data import ScriptData
 from streamlit.runtime.scriptrunner import RerunData, ScriptRunner, ScriptRunnerEvent
 from streamlit.runtime.scriptrunner.script_cache import ScriptCache
 from streamlit.runtime.secrets import secrets_singleton
 from streamlit.runtime.uploaded_file_manager import UploadedFileManager
+from streamlit.source_util import PageHash, PageInfo
 from streamlit.version import STREAMLIT_VERSION_STRING
 from streamlit.watcher import LocalSourcesWatcher
 
 if TYPE_CHECKING:
     from streamlit.runtime.state import SessionState
 
 _LOGGER: Final = get_logger(__name__)
@@ -123,14 +125,17 @@
         # Each AppSession has a unique string ID.
         self.id = session_id_override or str(uuid.uuid4())
 
         self._event_loop = asyncio.get_running_loop()
         self._script_data = script_data
         self._uploaded_file_mgr = uploaded_file_manager
         self._script_cache = script_cache
+        self._pages_manager = PagesManager(
+            script_data.main_script_path, self._script_cache
+        )
 
         # The browser queue contains messages that haven't yet been
         # delivered to the browser. Periodically, the server flushes
         # this queue and delivers its contents to the browser.
         self._browser_queue = ForwardMsgQueue()
         self._message_enqueued_callback = message_enqueued_callback
 
@@ -178,25 +183,23 @@
           * the project-level secrets.toml files
 
         This method is called automatically on AppSession construction, but it may be
         called again in the case when a session is disconnected and is being reconnect
         to.
         """
         if self._local_sources_watcher is None:
-            self._local_sources_watcher = LocalSourcesWatcher(
-                self._script_data.main_script_path
-            )
+            self._local_sources_watcher = LocalSourcesWatcher(self._pages_manager)
 
         self._local_sources_watcher.register_file_change_callback(
             self._on_source_file_changed
         )
         self._stop_config_listener = config.on_config_parsed(
             self._on_source_file_changed, force_connect=True
         )
-        self._stop_pages_listener = source_util.register_pages_changed_callback(
+        self._stop_pages_listener = self._pages_manager.register_pages_changed_callback(
             self._on_pages_changed
         )
         secrets_singleton.file_change_listener.connect(self._on_secrets_file_changed)
 
     def disconnect_file_watchers(self) -> None:
         """Disconnect the file watcher handlers registered by register_file_watchers."""
         if self._local_sources_watcher is not None:
@@ -404,25 +407,25 @@
             main_script_path=self._script_data.main_script_path,
             session_state=self._session_state,
             uploaded_file_mgr=self._uploaded_file_mgr,
             script_cache=self._script_cache,
             initial_rerun_data=initial_rerun_data,
             user_info=self._user_info,
             fragment_storage=self._fragment_storage,
+            pages_manager=self._pages_manager,
         )
         self._scriptrunner.on_event.connect(self._on_scriptrunner_event)
         self._scriptrunner.start()
 
     @property
     def session_state(self) -> SessionState:
         return self._session_state
 
     def _should_rerun_on_file_change(self, filepath: str) -> bool:
-        main_script_path = self._script_data.main_script_path
-        pages = source_util.get_pages(main_script_path)
+        pages = self._pages_manager.get_pages()
 
         changed_page_script_hash = next(
             filter(lambda k: pages[k]["script_path"] == filepath, pages),
             None,
         )
 
         if changed_page_script_hash is not None:
@@ -451,15 +454,15 @@
         # to `connect` / `disconnect` directly is that every function that is passed to `connect` / `disconnect`
         # must have at least one argument for `sender` (in this case we don't really care about it, thus `_`),
         # and introducing an unnecessary argument to `_on_source_file_changed` just for this purpose sounded finicky.
         self._on_source_file_changed()
 
     def _on_pages_changed(self, _) -> None:
         msg = ForwardMsg()
-        _populate_app_pages(msg.pages_changed, self._script_data.main_script_path)
+        self._populate_app_pages(msg.pages_changed, self._pages_manager.get_pages())
         self._enqueue_forward_msg(msg)
 
         if self._local_sources_watcher is not None:
             self._local_sources_watcher.update_watched_pages()
 
     def _clear_queue(self) -> None:
         self._browser_queue.clear(retain_lifecycle_msgs=True)
@@ -469,14 +472,15 @@
         sender: ScriptRunner | None,
         event: ScriptRunnerEvent,
         forward_msg: ForwardMsg | None = None,
         exception: BaseException | None = None,
         client_state: ClientState | None = None,
         page_script_hash: str | None = None,
         fragment_ids_this_run: set[str] | None = None,
+        pages: dict[PageHash, PageInfo] | None = None,
     ) -> None:
         """Called when our ScriptRunner emits an event.
 
         This is generally called from the sender ScriptRunner's script thread.
         We forward the event on to _handle_scriptrunner_event_on_event_loop,
         which will be called on the main thread.
         """
@@ -485,26 +489,28 @@
                 sender,
                 event,
                 forward_msg,
                 exception,
                 client_state,
                 page_script_hash,
                 fragment_ids_this_run,
+                pages,
             )
         )
 
     def _handle_scriptrunner_event_on_event_loop(
         self,
         sender: ScriptRunner | None,
         event: ScriptRunnerEvent,
         forward_msg: ForwardMsg | None = None,
         exception: BaseException | None = None,
         client_state: ClientState | None = None,
         page_script_hash: str | None = None,
         fragment_ids_this_run: set[str] | None = None,
+        pages: dict[PageHash, PageInfo] | None = None,
     ) -> None:
         """Handle a ScriptRunner event.
 
         This function must only be called on our eventloop thread.
 
         Parameters
         ----------
@@ -568,15 +574,15 @@
             # fragment, so dropping the messages may result in the app missing
             # information.
             if not fragment_ids_this_run:
                 self._clear_queue()
 
             self._enqueue_forward_msg(
                 self._create_new_session_message(
-                    page_script_hash, fragment_ids_this_run
+                    page_script_hash, fragment_ids_this_run, pages
                 )
             )
 
         elif (
             event == ScriptRunnerEvent.SCRIPT_STOPPED_WITH_SUCCESS
             or event == ScriptRunnerEvent.SCRIPT_STOPPED_WITH_COMPILE_ERROR
             or event == ScriptRunnerEvent.FRAGMENT_STOPPED_WITH_SUCCESS
@@ -599,14 +605,15 @@
                 or event == ScriptRunnerEvent.FRAGMENT_STOPPED_WITH_SUCCESS
             ):
                 # The script completed successfully: update our
                 # LocalSourcesWatcher to account for any source code changes
                 # that change which modules should be watched.
                 if self._local_sources_watcher:
                     self._local_sources_watcher.update_watched_modules()
+                    self._local_sources_watcher.update_watched_pages()
             else:
                 # The script didn't complete successfully: send the exception
                 # to the frontend.
                 assert (
                     exception is not None
                 ), "exception must be set for the SCRIPT_STOPPED_WITH_COMPILE_ERROR event"
                 msg = ForwardMsg()
@@ -662,28 +669,34 @@
     def _create_file_change_message(self) -> ForwardMsg:
         """Create and return a 'script_changed_on_disk' ForwardMsg."""
         msg = ForwardMsg()
         msg.session_event.script_changed_on_disk = True
         return msg
 
     def _create_new_session_message(
-        self, page_script_hash: str, fragment_ids_this_run: set[str] | None = None
+        self,
+        page_script_hash: str,
+        fragment_ids_this_run: set[str] | None = None,
+        pages: dict[PageHash, PageInfo] | None = None,
     ) -> ForwardMsg:
         """Create and return a new_session ForwardMsg."""
         msg = ForwardMsg()
 
         msg.new_session.script_run_id = _generate_scriptrun_id()
         msg.new_session.name = self._script_data.name
-        msg.new_session.main_script_path = self._script_data.main_script_path
+        msg.new_session.main_script_path = self._pages_manager.main_script_path
+        msg.new_session.main_script_hash = self._pages_manager.main_script_hash
         msg.new_session.page_script_hash = page_script_hash
 
         if fragment_ids_this_run:
             msg.new_session.fragment_ids_this_run.extend(fragment_ids_this_run)
 
-        _populate_app_pages(msg.new_session, self._script_data.main_script_path)
+        self._populate_app_pages(
+            msg.new_session, pages or self._pages_manager.get_pages()
+        )
         _populate_config_msg(msg.new_session.config)
         _populate_theme_msg(msg.new_session.custom_theme)
 
         # Immutable session data. We send this every time a new session is
         # started, to avoid having to track whether the client has already
         # received it. It does not change from run to run; it's up to the
         # to perform one-time initialization only once.
@@ -825,14 +838,24 @@
                     upload_url=upload_url_info.upload_url,
                     delete_url=upload_url_info.delete_url,
                 )
             )
 
         self._enqueue_forward_msg(msg)
 
+    def _populate_app_pages(
+        self, msg: NewSession | PagesChanged, pages: dict[PageHash, PageInfo]
+    ) -> None:
+        for page_script_hash, page_info in pages.items():
+            page_proto = msg.app_pages.add()
+
+            page_proto.page_script_hash = page_script_hash
+            page_proto.page_name = page_info["page_name"]
+            page_proto.icon = page_info["icon"]
+
 
 # Config.ToolbarMode.ValueType does not exist at runtime (only in the pyi stubs), so
 # we need to use quotes.
 # This field will be available at runtime as of protobuf 3.20.1, but
 # we are using an older version.
 # For details, see: https://github.com/protocolbuffers/protobuf/issues/8175
 def _get_toolbar_mode() -> Config.ToolbarMode.ValueType:
@@ -909,16 +932,7 @@
         else:
             msg.font = font_map[font]
 
 
 def _populate_user_info_msg(msg: UserInfo) -> None:
     msg.installation_id = Installation.instance().installation_id
     msg.installation_id_v3 = Installation.instance().installation_id_v3
-
-
-def _populate_app_pages(msg: NewSession | PagesChanged, main_script_path: str) -> None:
-    for page_script_hash, page_info in source_util.get_pages(main_script_path).items():
-        page_proto = msg.app_pages.add()
-
-        page_proto.page_script_hash = page_script_hash
-        page_proto.page_name = page_info["page_name"]
-        page_proto.icon = page_info["icon"]
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/legacy_cache_api.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/legacy_cache_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/credentials.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/fragment.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/fragment.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
         h.update(
             f"{non_optional_func.__module__}.{non_optional_func.__qualname__}{active_dg._get_delta_path_str()}".encode(
                 "utf-8"
             )
         )
         fragment_id = h.hexdigest()
 
+        # We intentionally want to capture the active script hash here to ensure
+        # that the fragment is associated with the correct script running.
+        initialized_active_script_hash = ctx.active_script_hash
+
         def wrapped_fragment():
             import streamlit as st
 
             # NOTE: We need to call get_script_run_ctx here again and can't just use the
             # value of ctx from above captured by the closure because subsequent
             # fragment runs will generally run in a new script run, thus we'll have a
             # new ctx.
@@ -153,16 +157,28 @@
                 # Otherwise, we must be in a full script run. We need to temporarily set
                 # ctx.current_fragment_id so that elements corresponding to this
                 # fragment get tagged with the appropriate ID. ctx.current_fragment_id
                 # gets reset after the fragment function finishes running.
                 ctx.current_fragment_id = fragment_id
 
             try:
-                with st.container():
-                    result = non_optional_func(*args, **kwargs)
+                # Make sure we set the active script hash to the same value
+                # for the fragment run as when defined upon initialization
+                # This ensures that elements (especially widgets) are tied
+                # to a consistent active script hash
+                active_hash_context = (
+                    ctx.pages_manager.run_with_active_hash(
+                        initialized_active_script_hash
+                    )
+                    if initialized_active_script_hash != ctx.active_script_hash
+                    else contextlib.nullcontext()
+                )
+                with active_hash_context:
+                    with st.container():
+                        result = non_optional_func(*args, **kwargs)
             finally:
                 ctx.current_fragment_id = None
 
             return result
 
         ctx.fragment_storage.set(fragment_id, wrapped_fragment)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/runtime.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/script_data.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from streamlit.proto.PageProfile_pb2 import Command
 from streamlit.runtime.scriptrunner.script_requests import ScriptRequests
 from streamlit.runtime.state import SafeSessionState
 from streamlit.runtime.uploaded_file_manager import UploadedFileManager
 
 if TYPE_CHECKING:
     from streamlit.runtime.fragment import FragmentStorage
+    from streamlit.runtime.pages_manager import PagesManager
 
 _LOGGER: Final = get_logger(__name__)
 
 UserInfo: TypeAlias = Dict[str, Union[str, None]]
 
 
 @dataclass
@@ -56,17 +57,17 @@
 
     session_id: str
     _enqueue: Callable[[ForwardMsg], None]
     query_string: str
     session_state: SafeSessionState
     uploaded_file_mgr: UploadedFileManager
     main_script_path: str
-    page_script_hash: str
     user_info: UserInfo
     fragment_storage: "FragmentStorage"
+    pages_manager: "PagesManager"
 
     gather_usage_stats: bool = False
     command_tracking_deactivated: bool = False
     tracked_commands: list[Command] = field(default_factory=list)
     tracked_commands_counter: Counter[str] = field(default_factory=collections.Counter)
     _set_page_config_allowed: bool = True
     _has_script_started: bool = False
@@ -83,26 +84,34 @@
     # the usage of widgets.
     disallow_cached_widget_usage: bool = False
 
     # TODO(willhuang1997): Remove this variable when experimental query params are removed
     _experimental_query_params_used = False
     _production_query_params_used = False
 
+    @property
+    def page_script_hash(self):
+        return self.pages_manager.get_current_page_script_hash()
+
+    @property
+    def active_script_hash(self):
+        return self.pages_manager.get_active_script_hash()
+
     def reset(
         self,
         query_string: str = "",
         page_script_hash: str = "",
         fragment_ids_this_run: set[str] | None = None,
     ) -> None:
         self.cursors = {}
         self.widget_ids_this_run = set()
         self.widget_user_keys_this_run = set()
         self.form_ids_this_run = set()
         self.query_string = query_string
-        self.page_script_hash = page_script_hash
+        self.pages_manager.set_current_page_script_hash(page_script_hash)
         # Permit set_page_config when the ScriptRunContext is reused on a rerun
         self._set_page_config_allowed = True
         self._has_script_started = False
         self.command_tracking_deactivated: bool = False
         self.tracked_commands = []
         self.tracked_commands_counter = collections.Counter()
         self.current_fragment_id = None
@@ -138,14 +147,16 @@
         # - set_page_config was called on this message
         # - The script has already started and a different st call occurs (a delta)
         if msg.HasField("page_config_changed") or (
             msg.HasField("delta") and self._has_script_started
         ):
             self._set_page_config_allowed = False
 
+        msg.metadata.active_script_hash = self.active_script_hash
+
         # Pass the message up to our associated ScriptRunner.
         self._enqueue(msg)
 
     def ensure_single_query_api_used(self):
         if self._experimental_query_params_used and self._production_query_params_used:
             raise StreamlitAPIException(
                 "Using `st.query_params` together with either `st.experimental_get_query_params` "
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 )
 from streamlit.runtime.state.session_state import SCRIPT_RUN_PAGE_SCRIPT_HASH_KEY
 from streamlit.runtime.uploaded_file_manager import UploadedFileManager
 from streamlit.vendor.ipython.modified_sys_path import modified_sys_path
 
 if TYPE_CHECKING:
     from streamlit.runtime.fragment import FragmentStorage
+    from streamlit.runtime.pages_manager import PagesManager
 
 _LOGGER: Final = get_logger(__name__)
 
 
 class ScriptRunnerEvent(Enum):
     ## "Control" events. These are emitted when the ScriptRunner's state changes.
 
@@ -111,14 +112,15 @@
         main_script_path: str,
         session_state: SessionState,
         uploaded_file_mgr: UploadedFileManager,
         script_cache: ScriptCache,
         initial_rerun_data: RerunData,
         user_info: dict[str, str | None],
         fragment_storage: "FragmentStorage",
+        pages_manager: "PagesManager",
     ):
         """Initialize the ScriptRunner.
 
         (The ScriptRunner won't start executing until start() is called.)
 
         Parameters
         ----------
@@ -160,14 +162,15 @@
             session_state, yield_callback=self._maybe_handle_execution_control_request
         )
         self._uploaded_file_mgr = uploaded_file_mgr
         self._script_cache = script_cache
         self._user_info = user_info
         self._fragment_storage = fragment_storage
 
+        self._pages_manager = pages_manager
         self._requests = ScriptRequests()
         self._requests.request_rerun(initial_rerun_data)
 
         self.on_event = Signal(
             doc="""Emitted when a ScriptRunnerEvent occurs.
 
             This signal is generally emitted on the ScriptRunner's script
@@ -287,18 +290,18 @@
             session_id=self._session_id,
             _enqueue=self._enqueue_forward_msg,
             script_requests=self._requests,
             query_string="",
             session_state=self._session_state,
             uploaded_file_mgr=self._uploaded_file_mgr,
             main_script_path=self._main_script_path,
-            page_script_hash="",
             user_info=self._user_info,
             gather_usage_stats=bool(config.get_option("browser.gatherUsageStats")),
             fragment_storage=self._fragment_storage,
+            pages_manager=self._pages_manager,
         )
         add_script_run_ctx(threading.current_thread(), ctx)
 
         request = self._requests.on_scriptrunner_ready()
         while request.type == ScriptRequestType.RERUN:
             # When the script thread starts, we'll have a pending rerun
             # request that we'll handle immediately. When the script finishes,
@@ -422,47 +425,26 @@
             _LOGGER.debug("Running script %s", rerun_data)
             start_time: float = timer()
             prep_time: float = 0  # This will be overwritten once preparations are done.
 
             # Reset DeltaGenerators, widgets, media files.
             runtime.get_instance().media_file_mgr.clear_session_refs()
 
-            main_script_path = self._main_script_path
-            pages = source_util.get_pages(main_script_path)
-            # Safe because pages will at least contain the app's main page.
-            main_page_info = list(pages.values())[0]
-            current_page_info = None
+            self._pages_manager.set_script_intent(
+                rerun_data.page_script_hash, rerun_data.page_name
+            )
+            active_script = self._pages_manager.get_initial_active_script(
+                rerun_data.page_script_hash, rerun_data.page_name
+            )
+            main_page_info = self._pages_manager.get_main_page()
             uncaught_exception = None
 
-            if rerun_data.page_script_hash:
-                current_page_info = pages.get(rerun_data.page_script_hash, None)
-            elif not rerun_data.page_script_hash and rerun_data.page_name:
-                # If a user navigates directly to a non-main page of an app, we get
-                # the first script run request before the list of pages has been
-                # sent to the frontend. In this case, we choose the first script
-                # with a name matching the requested page name.
-                current_page_info = next(
-                    filter(
-                        # There seems to be this weird bug with mypy where it
-                        # thinks that p can be None (which is impossible given the
-                        # types of pages), so we add `p and` at the beginning of
-                        # the predicate to circumvent this.
-                        lambda p: p and (p["page_name"] == rerun_data.page_name),
-                        pages.values(),
-                    ),
-                    None,
-                )
-            else:
-                # If no information about what page to run is given, default to
-                # running the main page.
-                current_page_info = main_page_info
-
             page_script_hash = (
-                current_page_info["page_script_hash"]
-                if current_page_info is not None
+                active_script["page_script_hash"]
+                if active_script is not None
                 else main_page_info["page_script_hash"]
             )
 
             fragment_ids_this_run = set(rerun_data.fragment_id_queue)
 
             # Clear widget state on page change. This normally happens implicitly
             # in the script run cleanup steps, but doing it explicitly ensures
@@ -484,24 +466,26 @@
             )
 
             self.on_event.send(
                 self,
                 event=ScriptRunnerEvent.SCRIPT_STARTED,
                 page_script_hash=page_script_hash,
                 fragment_ids_this_run=fragment_ids_this_run,
+                pages=self._pages_manager.get_pages(),
             )
 
             # Compile the script. Any errors thrown here will be surfaced
             # to the user via a modal dialog in the frontend, and won't result
             # in their previous script elements disappearing.
             try:
-                if current_page_info:
-                    script_path = current_page_info["script_path"]
+                if active_script is not None:
+                    script_path = active_script["script_path"]
                 else:
-                    script_path = main_script_path
+                    # page must not be found
+                    script_path = main_page_info["script_path"]
 
                     # At this point, we know that either
                     #   * the script corresponding to the hash requested no longer
                     #     exists, or
                     #   * we were not able to find a script with the requested page
                     #     name.
                     # In both of these cases, we want to send a page_not_found
@@ -642,17 +626,19 @@
 
                         # Create and send page profile information
                         ctx.enqueue(
                             create_page_profile_message(
                                 ctx.tracked_commands,
                                 exec_time=to_microseconds(timer() - start_time),
                                 prep_time=to_microseconds(prep_time),
-                                uncaught_exception=type(uncaught_exception).__name__
-                                if uncaught_exception
-                                else None,
+                                uncaught_exception=(
+                                    type(uncaught_exception).__name__
+                                    if uncaught_exception
+                                    else None
+                                ),
                             )
                         )
                     except Exception as ex:
                         # Always capture all exceptions since we want to make sure that
                         # the telemetry never causes any issues.
                         _LOGGER.debug("Failed to create page profile", exc_info=ex)
                 self._on_script_finished(ctx, finished_event, premature_stop)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/secrets.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/common.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/stats.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/source_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/source_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,38 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import re
 import threading
 from pathlib import Path
-from typing import Any, Callable, Final, cast
+from typing import Any, Callable, Final, TypedDict, cast
 
 from blinker import Signal
+from typing_extensions import NotRequired, TypeAlias
 
 from streamlit.logger import get_logger
 from streamlit.string_util import extract_leading_emoji
 from streamlit.util import calc_md5
 
 _LOGGER: Final = get_logger(__name__)
 
+PageHash: TypeAlias = str
+PageName: TypeAlias = str
+ScriptPath: TypeAlias = str
+Icon: TypeAlias = str
+
+
+class PageInfo(TypedDict):
+    script_path: ScriptPath
+    page_script_hash: PageHash
+    icon: NotRequired[Icon]
+    page_name: NotRequired[PageName]
+    url_pathname: NotRequired[str]
+
 
 def open_python_file(filename: str):
     """Open a read-only Python file taking proper care of its encoding.
 
     In Python 3, we would like all files to be opened with utf-8 encoding.
     However, some author like to specify PEP263 headers in their source files
     with their own encodings. In that case, we should respect the author's
@@ -87,52 +101,52 @@
         r"[_ ]+", "_", extraction.group(2)
     ).strip() or extraction.group(1)
 
     return extract_leading_emoji(icon_and_name)
 
 
 _pages_cache_lock = threading.RLock()
-_cached_pages: dict[str, dict[str, str]] | None = None
+_cached_pages: dict[PageHash, PageInfo] | None = None
 _on_pages_changed = Signal(doc="Emitted when the pages directory is changed")
 
 
 def invalidate_pages_cache() -> None:
     global _cached_pages
 
     _LOGGER.debug("Pages directory changed")
     with _pages_cache_lock:
         _cached_pages = None
 
     _on_pages_changed.send()
 
 
-def get_pages(main_script_path_str: str) -> dict[str, dict[str, str]]:
+def get_pages(main_script_path_str: ScriptPath) -> dict[PageHash, PageInfo]:
     global _cached_pages
 
     # Avoid taking the lock if the pages cache hasn't been invalidated.
-    pages = _cached_pages
-    if pages is not None:
-        return pages
+    precached_pages = _cached_pages
+    if precached_pages is not None:
+        return precached_pages
 
     with _pages_cache_lock:
         # The cache may have been repopulated while we were waiting to grab
         # the lock.
         if _cached_pages is not None:
             return _cached_pages
 
         main_script_path = Path(main_script_path_str)
         main_page_icon, main_page_name = page_icon_and_name(main_script_path)
-        main_page_script_hash = calc_md5(main_script_path_str)
+        main_script_hash = calc_md5(main_script_path_str)
 
-        # NOTE: We include the page_script_hash in the dict even though it is
+        # NOTE: We include the script_hash in the dict even though it is
         #       already used as the key because that occasionally makes things
         #       easier for us when we need to iterate over pages.
-        pages = {
-            main_page_script_hash: {
-                "page_script_hash": main_page_script_hash,
+        pages: dict[PageHash, PageInfo] = {
+            main_script_hash: {
+                "page_script_hash": main_script_hash,
                 "page_name": main_page_name,
                 "icon": main_page_icon,
                 "script_path": str(main_script_path.resolve()),
             }
         }
 
         pages_dir = main_script_path.parent / "pages"
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/asset-manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8258333333333333%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.707da454.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.707da454.js', 'static/js/9945.47d54f35.chunk.js': "*

 * *            "'./static/js/9945.47d54f35.chunk.js', 'static/js/8571.cfc22b99.chunk.js': "*

 * *            "'./static/js/8571.cfc22b99.chunk.js', delete: ['static/js/6950.70fe55c2.chunk.js', "*

 * *            "'static/js/5117.04bfe5d3.chunk.js']}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "entrypoints": [
         "static/css/main.3aaaea00.css",
-        "static/js/main.9978e612.js"
+        "static/js/main.707da454.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.3aaaea00.css",
-        "main.js": "./static/js/main.9978e612.js",
+        "main.js": "./static/js/main.707da454.js",
         "static/css/3466.8b8f33d6.chunk.css": "./static/css/3466.8b8f33d6.chunk.css",
         "static/css/5441.e3b876c5.chunk.css": "./static/css/5441.e3b876c5.chunk.css",
         "static/css/8148.49dfd2ce.chunk.css": "./static/css/8148.49dfd2ce.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.14f7c6ff.chunk.js": "./static/js/1168.14f7c6ff.chunk.js",
         "static/js/1307.0f0cca93.chunk.js": "./static/js/1307.0f0cca93.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
@@ -32,44 +32,44 @@
         "static/js/4177.69f9f18d.chunk.js": "./static/js/4177.69f9f18d.chunk.js",
         "static/js/4319.bf1c86bf.chunk.js": "./static/js/4319.bf1c86bf.chunk.js",
         "static/js/4477.1bd49702.chunk.js": "./static/js/4477.1bd49702.chunk.js",
         "static/js/4500.b6f348d1.chunk.js": "./static/js/4500.b6f348d1.chunk.js",
         "static/js/4666.c4b22a63.chunk.js": "./static/js/4666.c4b22a63.chunk.js",
         "static/js/474.7eb0c6cd.chunk.js": "./static/js/474.7eb0c6cd.chunk.js",
         "static/js/5106.44f0ff51.chunk.js": "./static/js/5106.44f0ff51.chunk.js",
-        "static/js/5117.04bfe5d3.chunk.js": "./static/js/5117.04bfe5d3.chunk.js",
         "static/js/5249.f2f4070d.chunk.js": "./static/js/5249.f2f4070d.chunk.js",
         "static/js/5345.73d26e5d.chunk.js": "./static/js/5345.73d26e5d.chunk.js",
         "static/js/5379.f08eddd1.chunk.js": "./static/js/5379.f08eddd1.chunk.js",
         "static/js/5441.1b94928f.chunk.js": "./static/js/5441.1b94928f.chunk.js",
         "static/js/5791.9a42fb4b.chunk.js": "./static/js/5791.9a42fb4b.chunk.js",
         "static/js/6013.4ba2d616.chunk.js": "./static/js/6013.4ba2d616.chunk.js",
         "static/js/6405.ac5a6f23.chunk.js": "./static/js/6405.ac5a6f23.chunk.js",
         "static/js/6718.802da17e.chunk.js": "./static/js/6718.802da17e.chunk.js",
         "static/js/6853.93dd1c4c.chunk.js": "./static/js/6853.93dd1c4c.chunk.js",
-        "static/js/6950.70fe55c2.chunk.js": "./static/js/6950.70fe55c2.chunk.js",
         "static/js/7142.83028745.chunk.js": "./static/js/7142.83028745.chunk.js",
         "static/js/7175.583ff733.chunk.js": "./static/js/7175.583ff733.chunk.js",
         "static/js/7323.b74cc85b.chunk.js": "./static/js/7323.b74cc85b.chunk.js",
         "static/js/7483.64f23be7.chunk.js": "./static/js/7483.64f23be7.chunk.js",
         "static/js/7602.e8abc06b.chunk.js": "./static/js/7602.e8abc06b.chunk.js",
         "static/js/7805.acc6316a.chunk.js": "./static/js/7805.acc6316a.chunk.js",
         "static/js/8005.43974a35.chunk.js": "./static/js/8005.43974a35.chunk.js",
         "static/js/8148.293984e0.chunk.js": "./static/js/8148.293984e0.chunk.js",
         "static/js/8427.bd0a7cf3.chunk.js": "./static/js/8427.bd0a7cf3.chunk.js",
         "static/js/8477.de889fe5.chunk.js": "./static/js/8477.de889fe5.chunk.js",
         "static/js/8492.0d93bd08.chunk.js": "./static/js/8492.0d93bd08.chunk.js",
         "static/js/8536.f8de3d9a.chunk.js": "./static/js/8536.f8de3d9a.chunk.js",
         "static/js/8570.6de19120.chunk.js": "./static/js/8570.6de19120.chunk.js",
+        "static/js/8571.cfc22b99.chunk.js": "./static/js/8571.cfc22b99.chunk.js",
         "static/js/8691.4211c305.chunk.js": "./static/js/8691.4211c305.chunk.js",
         "static/js/9330.2b4c99e0.chunk.js": "./static/js/9330.2b4c99e0.chunk.js",
         "static/js/9336.3e046ad7.chunk.js": "./static/js/9336.3e046ad7.chunk.js",
         "static/js/937.a1248039.chunk.js": "./static/js/937.a1248039.chunk.js",
         "static/js/9656.8c935274.chunk.js": "./static/js/9656.8c935274.chunk.js",
         "static/js/9865.fd93213d.chunk.js": "./static/js/9865.fd93213d.chunk.js",
+        "static/js/9945.47d54f35.chunk.js": "./static/js/9945.47d54f35.chunk.js",
         "static/media/KaTeX_AMS-Regular.ttf": "./static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf",
         "static/media/KaTeX_AMS-Regular.woff": "./static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff",
         "static/media/KaTeX_AMS-Regular.woff2": "./static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2",
         "static/media/KaTeX_Caligraphic-Bold.ttf": "./static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf",
         "static/media/KaTeX_Caligraphic-Bold.woff": "./static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff",
         "static/media/KaTeX_Caligraphic-Bold.woff2": "./static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2",
         "static/media/KaTeX_Caligraphic-Regular.ttf": "./static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf",
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/favicon.png` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/index.html` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.9978e612.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.707da454.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/8148.49dfd2ce.chunk.css` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/8148.49dfd2ce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1168.14f7c6ff.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1168.14f7c6ff.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/3513.7dedbda2.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/3513.7dedbda2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4113.99983645.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/474.7eb0c6cd.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/474.7eb0c6cd.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8571.cfc22b99.chunk.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,10 @@
 "use strict";
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
-    [5117], {
-        30351: (e, t, n) => {
-            n.d(t, {
-                s: () => a
-            });
-            var r = n(25773),
-                i = n(66845),
-                o = n(69),
-                a = i.forwardRef((function(e, t) {
-                    return i.createElement(o.D, (0, r.Z)({
-                        iconAttrs: {
-                            fill: "currentColor",
-                            xmlns: "http://www.w3.org/2000/svg"
-                        },
-                        iconVerticalAlign: "middle",
-                        iconViewBox: "0 0 24 24"
-                    }, e, {
-                        ref: t
-                    }), i.createElement("path", {
-                        fill: "none",
-                        d: "M0 0h24v24H0V0z"
-                    }), i.createElement("path", {
-                        d: "M15.41 7.41L14 6l-6 6 6 6 1.41-1.41L10.83 12l4.58-4.59z"
-                    }))
-                }));
-            a.displayName = "ChevronLeft"
-        },
+    [8571], {
         31197: (e, t, n) => {
             n.d(t, {
                 U: () => a
             });
             var r = n(25773),
                 i = n(66845),
                 o = n(69),
@@ -321,33 +295,33 @@
                     var r = e[n];
                     t.push(r)
                 }
                 return t
             }
 
             function g(e) {
-                if ("function" !== typeof e.webkitGetAsEntry) return h(e);
+                if ("function" !== typeof e.webkitGetAsEntry) return b(e);
                 var t = e.webkitGetAsEntry();
-                return t && t.isDirectory ? w(t) : h(e)
+                return t && t.isDirectory ? w(t) : b(e)
             }
 
             function y(e) {
                 return e.reduce((function(e, t) {
                     return (0, a.fl)(e, Array.isArray(t) ? y(t) : [t])
                 }), [])
             }
 
-            function h(e) {
+            function b(e) {
                 var t = e.getAsFile();
                 if (!t) return Promise.reject(e + " is not a File");
                 var n = l(t);
                 return Promise.resolve(n)
             }
 
-            function b(e) {
+            function h(e) {
                 return (0, a.mG)(this, void 0, void 0, (function() {
                     return (0, a.Jh)(this, (function(t) {
                         return [2, e.isDirectory ? w(e) : D(e)]
                     }))
                 }))
             }
 
@@ -370,15 +344,15 @@
                                         case 2:
                                             return o = a.sent(), e(o), [3, 4];
                                         case 3:
                                             return c = a.sent(), n(c), [3, 4];
                                         case 4:
                                             return [3, 6];
                                         case 5:
-                                            l = Promise.all(t.map(b)), r.push(l), i(), a.label = 6;
+                                            l = Promise.all(t.map(h)), r.push(l), i(), a.label = 6;
                                         case 6:
                                             return [2]
                                     }
                                 }))
                             }))
                         }), (function(e) {
                             n(e)
@@ -431,15 +405,15 @@
                     value: n,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = n, e
             }
 
-            function E(e, t) {
+            function F(e, t) {
                 return function(e) {
                     if (Array.isArray(e)) return e
                 }(e) || function(e, t) {
                     var n = null == e ? null : "undefined" !== typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null == n) return;
                     var r, i, o = [],
                         a = !0,
@@ -454,64 +428,64 @@
                         } finally {
                             if (c) throw i
                         }
                     }
                     return o
                 }(e, t) || function(e, t) {
                     if (!e) return;
-                    if ("string" === typeof e) return F(e, t);
+                    if ("string" === typeof e) return E(e, t);
                     var n = Object.prototype.toString.call(e).slice(8, -1);
                     "Object" === n && e.constructor && (n = e.constructor.name);
                     if ("Map" === n || "Set" === n) return Array.from(e);
-                    if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return F(e, t)
+                    if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return E(e, t)
                 }(e, t) || function() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }
 
-            function F(e, t) {
+            function E(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
                 return r
             }
-            var C = "file-invalid-type",
-                k = "file-too-large",
+            var k = "file-invalid-type",
+                C = "file-too-large",
                 z = "file-too-small",
                 P = "too-many-files",
                 S = function(e) {
                     e = Array.isArray(e) && 1 === e.length ? e[0] : e;
                     var t = Array.isArray(e) ? "one of ".concat(e.join(", ")) : e;
                     return {
-                        code: C,
+                        code: k,
                         message: "File type must be ".concat(t)
                     }
                 },
                 R = function(e) {
                     return {
-                        code: k,
+                        code: C,
                         message: "File is larger than ".concat(e, " ").concat(1 === e ? "byte" : "bytes")
                     }
                 },
                 M = function(e) {
                     return {
                         code: z,
                         message: "File is smaller than ".concat(e, " ").concat(1 === e ? "byte" : "bytes")
                     }
                 },
-                L = {
+                T = {
                     code: P,
                     message: "Too many files"
                 };
 
-            function T(e, t) {
+            function I(e, t) {
                 var n = "application/x-moz-file" === e.type || (0, x.Z)(e, t);
                 return [n, n ? null : S(t)]
             }
 
-            function I(e, t, n) {
+            function L(e, t, n) {
                 if (V(e.size))
                     if (V(t) && V(n)) {
                         if (e.size > n) return [!1, R(n)];
                         if (e.size < t) return [!1, M(t)]
                     } else {
                         if (V(t) && e.size < t) return [!1, M(t)];
                         if (V(n) && e.size > n) return [!1, R(n)]
@@ -522,21 +496,21 @@
                 return void 0 !== e && null !== e
             }
 
             function B(e) {
                 return "function" === typeof e.isPropagationStopped ? e.isPropagationStopped() : "undefined" !== typeof e.cancelBubble && e.cancelBubble
             }
 
-            function H(e) {
+            function K(e) {
                 return e.dataTransfer ? Array.prototype.some.call(e.dataTransfer.types, (function(e) {
                     return "Files" === e || "application/x-moz-file" === e
                 })) : !!e.target && !!e.target.files
             }
 
-            function K(e) {
+            function H(e) {
                 e.preventDefault()
             }
 
             function G() {
                 for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                 return function(e) {
                     for (var n = arguments.length, r = new Array(n > 1 ? n - 1 : 0), i = 1; i < n; i++) r[i - 1] = arguments[i];
@@ -552,17 +526,17 @@
                     accept: Array.isArray(e) ? e.filter((function(e) {
                         return "audio/*" === e || "video/*" === e || "image/*" === e || "text/*" === e || /\w+\/[-+.\w]+/g.test(e)
                     })).reduce((function(e, t) {
                         return A(A({}, e), {}, j({}, t, []))
                     }), {}) : {}
                 }]
             }
-            var N = ["children"],
-                _ = ["open"],
-                J = ["refKey", "role", "onKeyDown", "onFocus", "onBlur", "onClick", "onDragEnter", "onDragOver", "onDragLeave", "onDrop"],
+            var _ = ["children"],
+                J = ["open"],
+                N = ["refKey", "role", "onKeyDown", "onFocus", "onBlur", "onClick", "onDragEnter", "onDragOver", "onDragLeave", "onDrop"],
                 U = ["refKey", "onChange", "onClick"];
 
             function $(e) {
                 return function(e) {
                     if (Array.isArray(e)) return Y(e)
                 }(e) || function(e) {
                     if ("undefined" !== typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
@@ -674,95 +648,95 @@
                             f = t.onDragLeave,
                             p = t.onDragOver,
                             d = t.onDrop,
                             m = t.onDropAccepted,
                             v = t.onDropRejected,
                             g = t.onFileDialogCancel,
                             y = t.onFileDialogOpen,
-                            h = t.useFsAccessApi,
-                            b = t.preventDropOnDocument,
+                            b = t.useFsAccessApi,
+                            h = t.preventDropOnDocument,
                             w = t.noClick,
                             D = t.noKeyboard,
                             x = t.noDrag,
                             O = t.noDragEventsBubbling,
                             A = t.validator,
                             j = (0, r.useMemo)((function() {
                                 return "function" === typeof y ? y : ce
                             }), [y]),
-                            F = (0, r.useMemo)((function() {
+                            E = (0, r.useMemo)((function() {
                                 return "function" === typeof g ? g : ce
                             }), [g]),
-                            C = (0, r.useRef)(null),
                             k = (0, r.useRef)(null),
+                            C = (0, r.useRef)(null),
                             z = q((0, r.useReducer)(ae, oe), 2),
                             P = z[0],
                             S = z[1],
                             R = P.isFocused,
                             M = P.isFileDialogActive,
                             V = P.draggedFiles,
-                            N = (0, r.useRef)("undefined" !== typeof window && window.isSecureContext && h && "showOpenFilePicker" in window),
-                            _ = function() {
-                                !N.current && M && setTimeout((function() {
-                                    k.current && (k.current.files.length || (S({
+                            _ = (0, r.useRef)("undefined" !== typeof window && window.isSecureContext && b && "showOpenFilePicker" in window),
+                            J = function() {
+                                !_.current && M && setTimeout((function() {
+                                    C.current && (C.current.files.length || (S({
                                         type: "closeDialog"
-                                    }), F()))
+                                    }), E()))
                                 }), 300)
                             };
                         (0, r.useEffect)((function() {
-                            return window.addEventListener("focus", _, !1),
+                            return window.addEventListener("focus", J, !1),
                                 function() {
-                                    window.removeEventListener("focus", _, !1)
+                                    window.removeEventListener("focus", J, !1)
                                 }
-                        }), [k, M, F, N]);
+                        }), [C, M, E, _]);
                         var W = (0, r.useRef)([]),
                             Y = function(e) {
-                                C.current && C.current.contains(e.target) || (e.preventDefault(), W.current = [])
+                                k.current && k.current.contains(e.target) || (e.preventDefault(), W.current = [])
                             };
                         (0, r.useEffect)((function() {
-                            return b && (document.addEventListener("dragover", K, !1), document.addEventListener("drop", Y, !1)),
+                            return h && (document.addEventListener("dragover", H, !1), document.addEventListener("drop", Y, !1)),
                                 function() {
-                                    b && (document.removeEventListener("dragover", K), document.removeEventListener("drop", Y))
+                                    h && (document.removeEventListener("dragover", H), document.removeEventListener("drop", Y))
                                 }
-                        }), [C, b]);
+                        }), [k, h]);
                         var Q = (0, r.useCallback)((function(e) {
-                                e.preventDefault(), e.persist(), he(e), W.current = [].concat($(W.current), [e.target]), H(e) && Promise.resolve(o(e)).then((function(t) {
+                                e.preventDefault(), e.persist(), be(e), W.current = [].concat($(W.current), [e.target]), K(e) && Promise.resolve(o(e)).then((function(t) {
                                     B(e) && !O || (S({
                                         draggedFiles: t,
                                         isDragActive: !0,
                                         type: "setDraggedFiles"
                                     }), s && s(e))
                                 }))
                             }), [o, s, O]),
                             ne = (0, r.useCallback)((function(e) {
-                                e.preventDefault(), e.persist(), he(e);
-                                var t = H(e);
+                                e.preventDefault(), e.persist(), be(e);
+                                var t = K(e);
                                 if (t && e.dataTransfer) try {
                                     e.dataTransfer.dropEffect = "copy"
                                 } catch (n) {}
                                 return t && p && p(e), !1
                             }), [p, O]),
                             ie = (0, r.useCallback)((function(e) {
-                                e.preventDefault(), e.persist(), he(e);
+                                e.preventDefault(), e.persist(), be(e);
                                 var t = W.current.filter((function(e) {
-                                        return C.current && C.current.contains(e)
+                                        return k.current && k.current.contains(e)
                                     })),
                                     n = t.indexOf(e.target); - 1 !== n && t.splice(n, 1), W.current = t, t.length > 0 || (S({
                                     isDragActive: !1,
                                     type: "setDraggedFiles",
                                     draggedFiles: []
-                                }), H(e) && f && f(e))
-                            }), [C, f, O]),
+                                }), K(e) && f && f(e))
+                            }), [k, f, O]),
                             le = (0, r.useCallback)((function(e, t) {
                                 var r = [],
                                     i = [];
                                 e.forEach((function(e) {
-                                    var t = q(T(e, n), 2),
+                                    var t = q(I(e, n), 2),
                                         o = t[0],
                                         l = t[1],
-                                        u = q(I(e, c, a), 2),
+                                        u = q(L(e, c, a), 2),
                                         s = u[0],
                                         f = u[1],
                                         p = A ? A(e) : null;
                                     if (o && s && !p) r.push(e);
                                     else {
                                         var d = [l, f];
                                         p && (d = d.concat(p)), i.push({
@@ -771,31 +745,31 @@
                                                 return e
                                             }))
                                         })
                                     }
                                 })), (!l && r.length > 1 || l && u >= 1 && r.length > u) && (r.forEach((function(e) {
                                     i.push({
                                         file: e,
-                                        errors: [L]
+                                        errors: [T]
                                     })
                                 })), r.splice(0)), S({
                                     acceptedFiles: r,
                                     fileRejections: i,
                                     type: "setFiles"
                                 }), d && d(r, i, t), i.length > 0 && v && v(i, t), r.length > 0 && m && m(r, t)
                             }), [S, l, n, c, a, u, d, m, v, A]),
                             ue = (0, r.useCallback)((function(e) {
-                                e.preventDefault(), e.persist(), he(e), W.current = [], H(e) && Promise.resolve(o(e)).then((function(t) {
+                                e.preventDefault(), e.persist(), be(e), W.current = [], K(e) && Promise.resolve(o(e)).then((function(t) {
                                     B(e) && !O || le(t, e)
                                 })), S({
                                     type: "reset"
                                 })
                             }), [o, le, O]),
                             se = (0, r.useCallback)((function() {
-                                if (N.current) {
+                                if (_.current) {
                                     S({
                                         type: "openDialog"
                                     }), j();
                                     var e = {
                                         multiple: l,
                                         types: Z(n)
                                     };
@@ -803,27 +777,27 @@
                                         return o(e)
                                     })).then((function(e) {
                                         le(e, null), S({
                                             type: "closeDialog"
                                         })
                                     })).catch((function(e) {
                                         var t;
-                                        (t = e) instanceof DOMException && ("AbortError" === t.name || t.code === t.ABORT_ERR) ? (F(e), S({
+                                        (t = e) instanceof DOMException && ("AbortError" === t.name || t.code === t.ABORT_ERR) ? (E(e), S({
                                             type: "closeDialog"
                                         })) : function(e) {
                                             return e instanceof DOMException && ("SecurityError" === e.name || e.code === e.SECURITY_ERR)
-                                        }(e) && (N.current = !1, k.current && (k.current.value = null, k.current.click()))
+                                        }(e) && (_.current = !1, C.current && (C.current.value = null, C.current.click()))
                                     }))
-                                } else k.current && (S({
+                                } else C.current && (S({
                                     type: "openDialog"
-                                }), j(), k.current.value = null, k.current.click())
-                            }), [S, j, F, h, le, n, l]),
+                                }), j(), C.current.value = null, C.current.click())
+                            }), [S, j, E, b, le, n, l]),
                             fe = (0, r.useCallback)((function(e) {
-                                C.current && C.current.isEqualNode(e.target) && (" " !== e.key && "Enter" !== e.key && 32 !== e.keyCode && 13 !== e.keyCode || (e.preventDefault(), se()))
-                            }), [C, se]),
+                                k.current && k.current.isEqualNode(e.target) && (" " !== e.key && "Enter" !== e.key && 32 !== e.keyCode && 13 !== e.keyCode || (e.preventDefault(), se()))
+                            }), [k, se]),
                             pe = (0, r.useCallback)((function() {
                                 S({
                                     type: "focus"
                                 })
                             }), []),
                             de = (0, r.useCallback)((function() {
                                 S({
@@ -845,47 +819,47 @@
                             },
                             ge = function(e) {
                                 return D ? null : ve(e)
                             },
                             ye = function(e) {
                                 return x ? null : ve(e)
                             },
-                            he = function(e) {
+                            be = function(e) {
                                 O && e.stopPropagation()
                             },
-                            be = (0, r.useMemo)((function() {
+                            he = (0, r.useMemo)((function() {
                                 return function() {
                                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                                         t = e.refKey,
                                         n = void 0 === t ? "ref" : t,
                                         r = e.role,
                                         o = e.onKeyDown,
                                         a = e.onFocus,
                                         c = e.onBlur,
                                         l = e.onClick,
                                         u = e.onDragEnter,
                                         s = e.onDragOver,
                                         f = e.onDragLeave,
                                         p = e.onDrop,
-                                        d = te(e, J);
+                                        d = te(e, N);
                                     return X(X(ee({
                                         onKeyDown: ge(G(o, fe)),
                                         onFocus: ge(G(a, pe)),
                                         onBlur: ge(G(c, de)),
                                         onClick: ve(G(l, me)),
                                         onDragEnter: ye(G(u, Q)),
                                         onDragOver: ye(G(s, ne)),
                                         onDragLeave: ye(G(f, ie)),
                                         onDrop: ye(G(p, ue)),
                                         role: "string" === typeof r && "" !== r ? r : "button"
-                                    }, n, C), i || D ? {} : {
+                                    }, n, k), i || D ? {} : {
                                         tabIndex: 0
                                     }), d)
                                 }
-                            }), [C, fe, pe, de, me, Q, ne, ie, ue, D, x, i]),
+                            }), [k, fe, pe, de, me, Q, ne, ie, ue, D, x, i]),
                             we = (0, r.useCallback)((function(e) {
                                 e.stopPropagation()
                             }), []),
                             De = (0, r.useMemo)((function() {
                                 return function() {
                                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                                         t = e.refKey,
@@ -899,28 +873,28 @@
                                         type: "file",
                                         style: {
                                             display: "none"
                                         },
                                         onChange: ve(G(i, ue)),
                                         onClick: ve(G(o, we)),
                                         tabIndex: -1
-                                    }, r, k)), a)
+                                    }, r, C)), a)
                                 }
-                            }), [k, n, l, ue, i]),
+                            }), [C, n, l, ue, i]),
                             xe = V.length,
                             Oe = xe > 0 && function(e) {
                                 var t = e.files,
                                     n = e.accept,
                                     r = e.minSize,
                                     i = e.maxSize,
                                     o = e.multiple,
                                     a = e.maxFiles;
                                 return !(!o && t.length > 1 || o && a >= 1 && t.length > a) && t.every((function(e) {
-                                    var t = E(T(e, n), 1)[0],
-                                        o = E(I(e, r, i), 1)[0];
+                                    var t = F(I(e, n), 1)[0],
+                                        o = F(L(e, r, i), 1)[0];
                                     return t && o
                                 }))
                             }({
                                 files: V,
                                 accept: n,
                                 minSize: c,
                                 maxSize: a,
@@ -928,23 +902,23 @@
                                 maxFiles: u
                             }),
                             Ae = xe > 0 && !Oe;
                         return X(X({}, P), {}, {
                             isDragAccept: Oe,
                             isDragReject: Ae,
                             isFocused: R && !i,
-                            getRootProps: be,
+                            getRootProps: he,
                             getInputProps: De,
-                            rootRef: C,
-                            inputRef: k,
+                            rootRef: k,
+                            inputRef: C,
                             open: ve(se)
                         })
-                    }(te(e, N)),
+                    }(te(e, _)),
                     o = i.open,
-                    a = te(i, _);
+                    a = te(i, J);
                 return (0, r.useImperativeHandle)(t, (function() {
                     return {
                         open: o
                     }
                 }), [o]), r.createElement(r.Fragment, null, n(X(X({}, a), {}, {
                     open: o
                 })))
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5345.73d26e5d.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5345.73d26e5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5379.f08eddd1.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5379.f08eddd1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5441.1b94928f.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5441.1b94928f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6013.4ba2d616.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/6950.70fe55c2.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9945.47d54f35.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
-/*! For license information please see 6950.70fe55c2.chunk.js.LICENSE.txt */
+/*! For license information please see 9945.47d54f35.chunk.js.LICENSE.txt */
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
-    [6950], {
+    [9945], {
         97943: (e, t, n) => {
             "use strict";
             n.d(t, {
                 m: () => l
             });
             var o = n(25773),
                 i = n(66845),
@@ -24,14 +24,41 @@
                         d: "M0 0h24v24H0V0z"
                     }), i.createElement("path", {
                         d: "M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"
                     }))
                 }));
             l.displayName = "Add"
         },
+        20545: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                x: () => l
+            });
+            var o = n(25773),
+                i = n(66845),
+                r = n(69),
+                l = i.forwardRef((function(e, t) {
+                    return i.createElement(r.D, (0, o.Z)({
+                        iconAttrs: {
+                            fill: "currentColor",
+                            xmlns: "http://www.w3.org/2000/svg"
+                        },
+                        iconVerticalAlign: "middle",
+                        iconViewBox: "0 0 24 24"
+                    }, e, {
+                        ref: t
+                    }), i.createElement("path", {
+                        fill: "none",
+                        d: "M0 0h24v24H0V0z"
+                    }), i.createElement("path", {
+                        d: "M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12 19 6.41z"
+                    }))
+                }));
+            l.displayName = "Close"
+        },
         57463: (e, t, n) => {
             "use strict";
             n.d(t, {
                 H: () => l
             });
             var o = n(25773),
                 i = n(66845),
@@ -290,31 +317,14 @@
                     return s.displayName = n.name, s.__linaria = {
                         className: n.class || t,
                         extends: e
                     }, s
                 }
             }
         },
-        29916: e => {
-            e.exports = function(e, t, n, o) {
-                for (var i = -1, r = null == e ? 0 : e.length; ++i < r;) {
-                    var l = e[i];
-                    t(o, l, n(l), e)
-                }
-                return o
-            }
-        },
-        70199: (e, t, n) => {
-            var o = n(64811);
-            e.exports = function(e, t, n, i) {
-                return o(e, (function(e, o, r) {
-                    t(i, e, n(e), r)
-                })), i
-            }
-        },
         18471: e => {
             e.exports = function(e, t, n) {
                 return e === e && (void 0 !== n && (e = e <= n ? e : n), void 0 !== t && (e = e >= t ? e : t)), e
             }
         },
         48003: e => {
             var t = Object.prototype.hasOwnProperty;
@@ -350,27 +360,14 @@
                             if (p[w] === m) continue e;
                         t && p.push(m), f.push(g)
                     } else u(p, m, n) || (p !== f && p.push(m), f.push(g))
                 }
                 return f
             }
         },
-        98718: (e, t, n) => {
-            var o = n(29916),
-                i = n(70199),
-                r = n(48603),
-                l = n(12697);
-            e.exports = function(e, t) {
-                return function(n, a) {
-                    var s = l(n) ? o : i,
-                        c = t ? t() : {};
-                    return s(n, e, r(a, 2), c)
-                }
-            }
-        },
         58938: (e, t, n) => {
             var o = n(64626),
                 i = n(55304),
                 r = n(21278),
                 l = o && 1 / r(new o([, -0]))[1] == 1 / 0 ? function(e) {
                     return new o(e)
                 } : i;
@@ -434,23 +431,14 @@
                 return t = r(t) || 0, o(n) && (v = !!n.leading, u = (g = "maxWait" in n) ? l(r(n.maxWait) || 0, t) : u, m = "trailing" in n ? !!n.trailing : m), k.cancel = function() {
                     void 0 !== h && clearTimeout(h), p = 0, s = f = c = h = void 0
                 }, k.flush = function() {
                     return void 0 === h ? d : x(i())
                 }, k
             }
         },
-        76236: (e, t, n) => {
-            var o = n(45742),
-                i = n(98718),
-                r = Object.prototype.hasOwnProperty,
-                l = i((function(e, t, n) {
-                    r.call(e, n) ? e[n].push(t) : o(e, n, [t])
-                }));
-            e.exports = l
-        },
         82781: (e, t, n) => {
             var o = n(48003),
                 i = n(98869);
             e.exports = function(e, t) {
                 return null != e && i(e, t, o)
             }
         },
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7175.583ff733.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7175.583ff733.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8148.293984e0.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8148.293984e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/8691.4211c305.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/8691.4211c305.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9336.3e046ad7.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9336.3e046ad7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/main.9978e612.js` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/main.707da454.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.9978e612.js.LICENSE.txt */
+/*! For license information please see main.707da454.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -36073,44 +36073,45 @@
                         return Object.fromEntries((e.fields || []).map(((e, t) => [e.name.startsWith("__index_level_") ? e.name : String(t), e])))
                     }
                 }
             },
             16295: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    AG: () => T,
+                    AG: () => k,
                     BN: () => A,
-                    De: () => E,
+                    De: () => _,
                     Eh: () => c,
                     Fp: () => b,
-                    KR: () => P,
-                    MA: () => _,
-                    Od: () => C,
+                    KR: () => D,
+                    MA: () => x,
+                    Od: () => W,
                     PW: () => m,
-                    Pz: () => R,
+                    Pz: () => T,
                     UG: () => S,
                     W_: () => z,
                     XZ: () => d,
-                    Y2: () => x,
+                    Y2: () => R,
                     Zh: () => h,
                     _b: () => u,
                     bZ: () => l,
                     eI: () => y,
                     ef: () => v,
                     gO: () => p,
-                    hP: () => k,
+                    hP: () => C,
                     hz: () => g,
-                    iE: () => I,
-                    iR: () => W,
+                    iE: () => P,
+                    iR: () => N,
                     jM: () => M,
                     jb: () => q,
                     kM: () => w,
-                    nk: () => L,
-                    oi: () => N,
+                    nk: () => I,
+                    oi: () => L,
                     qj: () => f,
+                    uh: () => E,
                     xO: () => O
                 });
                 var r = n(36328);
                 const o = r.Reader,
                     i = r.Writer,
                     a = r.util,
                     s = r.roots.default || (r.roots.default = {}),
@@ -36207,18 +36208,18 @@
                         }(), e
                     })(),
                     c = (s.AppPage = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.pageScriptHash = "", e.prototype.pageName = "", e.prototype.icon = "", e.create = function(t) {
+                        return e.prototype.pageScriptHash = "", e.prototype.pageName = "", e.prototype.icon = "", e.prototype.isDefault = !1, e.prototype.sectionHeader = "", e.prototype.urlPathname = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
-                            return t || (t = i.create()), null != e.pageScriptHash && Object.hasOwnProperty.call(e, "pageScriptHash") && t.uint32(10).string(e.pageScriptHash), null != e.pageName && Object.hasOwnProperty.call(e, "pageName") && t.uint32(18).string(e.pageName), null != e.icon && Object.hasOwnProperty.call(e, "icon") && t.uint32(26).string(e.icon), t
+                            return t || (t = i.create()), null != e.pageScriptHash && Object.hasOwnProperty.call(e, "pageScriptHash") && t.uint32(10).string(e.pageScriptHash), null != e.pageName && Object.hasOwnProperty.call(e, "pageName") && t.uint32(18).string(e.pageName), null != e.icon && Object.hasOwnProperty.call(e, "icon") && t.uint32(26).string(e.icon), null != e.isDefault && Object.hasOwnProperty.call(e, "isDefault") && t.uint32(32).bool(e.isDefault), null != e.sectionHeader && Object.hasOwnProperty.call(e, "sectionHeader") && t.uint32(42).string(e.sectionHeader), null != e.urlPathname && Object.hasOwnProperty.call(e, "urlPathname") && t.uint32(50).string(e.urlPathname), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.AppPage;
                             for (; e.pos < n;) {
@@ -36229,31 +36230,40 @@
                                         break;
                                     case 2:
                                         r.pageName = e.string();
                                         break;
                                     case 3:
                                         r.icon = e.string();
                                         break;
+                                    case 4:
+                                        r.isDefault = e.bool();
+                                        break;
+                                    case 5:
+                                        r.sectionHeader = e.string();
+                                        break;
+                                    case 6:
+                                        r.urlPathname = e.string();
+                                        break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
                         }, e.verify = function(e) {
-                            return "object" !== typeof e || null === e ? "object expected" : null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && !a.isString(e.pageScriptHash) ? "pageScriptHash: string expected" : null != e.pageName && e.hasOwnProperty("pageName") && !a.isString(e.pageName) ? "pageName: string expected" : null != e.icon && e.hasOwnProperty("icon") && !a.isString(e.icon) ? "icon: string expected" : null
+                            return "object" !== typeof e || null === e ? "object expected" : null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && !a.isString(e.pageScriptHash) ? "pageScriptHash: string expected" : null != e.pageName && e.hasOwnProperty("pageName") && !a.isString(e.pageName) ? "pageName: string expected" : null != e.icon && e.hasOwnProperty("icon") && !a.isString(e.icon) ? "icon: string expected" : null != e.isDefault && e.hasOwnProperty("isDefault") && "boolean" !== typeof e.isDefault ? "isDefault: boolean expected" : null != e.sectionHeader && e.hasOwnProperty("sectionHeader") && !a.isString(e.sectionHeader) ? "sectionHeader: string expected" : null != e.urlPathname && e.hasOwnProperty("urlPathname") && !a.isString(e.urlPathname) ? "urlPathname: string expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.AppPage) return e;
                             let t = new s.AppPage;
-                            return null != e.pageScriptHash && (t.pageScriptHash = String(e.pageScriptHash)), null != e.pageName && (t.pageName = String(e.pageName)), null != e.icon && (t.icon = String(e.icon)), t
+                            return null != e.pageScriptHash && (t.pageScriptHash = String(e.pageScriptHash)), null != e.pageName && (t.pageName = String(e.pageName)), null != e.icon && (t.icon = String(e.icon)), null != e.isDefault && (t.isDefault = Boolean(e.isDefault)), null != e.sectionHeader && (t.sectionHeader = String(e.sectionHeader)), null != e.urlPathname && (t.urlPathname = String(e.urlPathname)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            return t.defaults && (n.pageScriptHash = "", n.pageName = "", n.icon = ""), null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && (n.pageScriptHash = e.pageScriptHash), null != e.pageName && e.hasOwnProperty("pageName") && (n.pageName = e.pageName), null != e.icon && e.hasOwnProperty("icon") && (n.icon = e.icon), n
+                            return t.defaults && (n.pageScriptHash = "", n.pageName = "", n.icon = "", n.isDefault = !1, n.sectionHeader = "", n.urlPathname = ""), null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && (n.pageScriptHash = e.pageScriptHash), null != e.pageName && e.hasOwnProperty("pageName") && (n.pageName = e.pageName), null != e.icon && e.hasOwnProperty("icon") && (n.icon = e.icon), null != e.isDefault && e.hasOwnProperty("isDefault") && (n.isDefault = e.isDefault), null != e.sectionHeader && e.hasOwnProperty("sectionHeader") && (n.sectionHeader = e.sectionHeader), null != e.urlPathname && e.hasOwnProperty("urlPathname") && (n.urlPathname = e.urlPathname), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/AppPage"
                         }, e
                     })(), s.Arrow = (() => {
                         function e(e) {
@@ -41922,21 +41932,21 @@
                         }, e
                     })(), s.ForwardMsg = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         let t;
-                        return e.prototype.hash = "", e.prototype.metadata = null, e.prototype.newSession = null, e.prototype.delta = null, e.prototype.pageInfoChanged = null, e.prototype.pageConfigChanged = null, e.prototype.scriptFinished = null, e.prototype.gitInfoChanged = null, e.prototype.pageProfile = null, e.prototype.sessionStatusChanged = null, e.prototype.sessionEvent = null, e.prototype.pageNotFound = null, e.prototype.pagesChanged = null, e.prototype.fileUrlsResponse = null, e.prototype.autoRerun = null, e.prototype.logo = null, e.prototype.parentMessage = null, e.prototype.refHash = null, e.prototype.debugLastBackmsgId = "", Object.defineProperty(e.prototype, "type", {
-                            get: a.oneOfGetter(t = ["newSession", "delta", "pageInfoChanged", "pageConfigChanged", "scriptFinished", "gitInfoChanged", "pageProfile", "sessionStatusChanged", "sessionEvent", "pageNotFound", "pagesChanged", "fileUrlsResponse", "autoRerun", "logo", "parentMessage", "refHash"]),
+                        return e.prototype.hash = "", e.prototype.metadata = null, e.prototype.newSession = null, e.prototype.delta = null, e.prototype.pageInfoChanged = null, e.prototype.pageConfigChanged = null, e.prototype.scriptFinished = null, e.prototype.gitInfoChanged = null, e.prototype.pageProfile = null, e.prototype.sessionStatusChanged = null, e.prototype.sessionEvent = null, e.prototype.navigation = null, e.prototype.pageNotFound = null, e.prototype.pagesChanged = null, e.prototype.fileUrlsResponse = null, e.prototype.autoRerun = null, e.prototype.logo = null, e.prototype.parentMessage = null, e.prototype.refHash = null, e.prototype.debugLastBackmsgId = "", Object.defineProperty(e.prototype, "type", {
+                            get: a.oneOfGetter(t = ["newSession", "delta", "pageInfoChanged", "pageConfigChanged", "scriptFinished", "gitInfoChanged", "pageProfile", "sessionStatusChanged", "sessionEvent", "navigation", "pageNotFound", "pagesChanged", "fileUrlsResponse", "autoRerun", "logo", "parentMessage", "refHash"]),
                             set: a.oneOfSetter(t)
                         }), e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
-                            return t || (t = i.create()), null != e.hash && Object.hasOwnProperty.call(e, "hash") && t.uint32(10).string(e.hash), null != e.metadata && Object.hasOwnProperty.call(e, "metadata") && s.ForwardMsgMetadata.encode(e.metadata, t.uint32(18).fork()).ldelim(), null != e.newSession && Object.hasOwnProperty.call(e, "newSession") && s.NewSession.encode(e.newSession, t.uint32(34).fork()).ldelim(), null != e.delta && Object.hasOwnProperty.call(e, "delta") && s.Delta.encode(e.delta, t.uint32(42).fork()).ldelim(), null != e.scriptFinished && Object.hasOwnProperty.call(e, "scriptFinished") && t.uint32(48).int32(e.scriptFinished), null != e.sessionStatusChanged && Object.hasOwnProperty.call(e, "sessionStatusChanged") && s.SessionStatus.encode(e.sessionStatusChanged, t.uint32(74).fork()).ldelim(), null != e.sessionEvent && Object.hasOwnProperty.call(e, "sessionEvent") && s.SessionEvent.encode(e.sessionEvent, t.uint32(82).fork()).ldelim(), null != e.refHash && Object.hasOwnProperty.call(e, "refHash") && t.uint32(90).string(e.refHash), null != e.pageInfoChanged && Object.hasOwnProperty.call(e, "pageInfoChanged") && s.PageInfo.encode(e.pageInfoChanged, t.uint32(98).fork()).ldelim(), null != e.pageConfigChanged && Object.hasOwnProperty.call(e, "pageConfigChanged") && s.PageConfig.encode(e.pageConfigChanged, t.uint32(106).fork()).ldelim(), null != e.gitInfoChanged && Object.hasOwnProperty.call(e, "gitInfoChanged") && s.GitInfo.encode(e.gitInfoChanged, t.uint32(114).fork()).ldelim(), null != e.pageNotFound && Object.hasOwnProperty.call(e, "pageNotFound") && s.PageNotFound.encode(e.pageNotFound, t.uint32(122).fork()).ldelim(), null != e.pagesChanged && Object.hasOwnProperty.call(e, "pagesChanged") && s.PagesChanged.encode(e.pagesChanged, t.uint32(130).fork()).ldelim(), null != e.debugLastBackmsgId && Object.hasOwnProperty.call(e, "debugLastBackmsgId") && t.uint32(138).string(e.debugLastBackmsgId), null != e.pageProfile && Object.hasOwnProperty.call(e, "pageProfile") && s.PageProfile.encode(e.pageProfile, t.uint32(146).fork()).ldelim(), null != e.fileUrlsResponse && Object.hasOwnProperty.call(e, "fileUrlsResponse") && s.FileURLsResponse.encode(e.fileUrlsResponse, t.uint32(154).fork()).ldelim(), null != e.parentMessage && Object.hasOwnProperty.call(e, "parentMessage") && s.ParentMessage.encode(e.parentMessage, t.uint32(162).fork()).ldelim(), null != e.autoRerun && Object.hasOwnProperty.call(e, "autoRerun") && s.AutoRerun.encode(e.autoRerun, t.uint32(170).fork()).ldelim(), null != e.logo && Object.hasOwnProperty.call(e, "logo") && s.Logo.encode(e.logo, t.uint32(178).fork()).ldelim(), t
+                            return t || (t = i.create()), null != e.hash && Object.hasOwnProperty.call(e, "hash") && t.uint32(10).string(e.hash), null != e.metadata && Object.hasOwnProperty.call(e, "metadata") && s.ForwardMsgMetadata.encode(e.metadata, t.uint32(18).fork()).ldelim(), null != e.newSession && Object.hasOwnProperty.call(e, "newSession") && s.NewSession.encode(e.newSession, t.uint32(34).fork()).ldelim(), null != e.delta && Object.hasOwnProperty.call(e, "delta") && s.Delta.encode(e.delta, t.uint32(42).fork()).ldelim(), null != e.scriptFinished && Object.hasOwnProperty.call(e, "scriptFinished") && t.uint32(48).int32(e.scriptFinished), null != e.sessionStatusChanged && Object.hasOwnProperty.call(e, "sessionStatusChanged") && s.SessionStatus.encode(e.sessionStatusChanged, t.uint32(74).fork()).ldelim(), null != e.sessionEvent && Object.hasOwnProperty.call(e, "sessionEvent") && s.SessionEvent.encode(e.sessionEvent, t.uint32(82).fork()).ldelim(), null != e.refHash && Object.hasOwnProperty.call(e, "refHash") && t.uint32(90).string(e.refHash), null != e.pageInfoChanged && Object.hasOwnProperty.call(e, "pageInfoChanged") && s.PageInfo.encode(e.pageInfoChanged, t.uint32(98).fork()).ldelim(), null != e.pageConfigChanged && Object.hasOwnProperty.call(e, "pageConfigChanged") && s.PageConfig.encode(e.pageConfigChanged, t.uint32(106).fork()).ldelim(), null != e.gitInfoChanged && Object.hasOwnProperty.call(e, "gitInfoChanged") && s.GitInfo.encode(e.gitInfoChanged, t.uint32(114).fork()).ldelim(), null != e.pageNotFound && Object.hasOwnProperty.call(e, "pageNotFound") && s.PageNotFound.encode(e.pageNotFound, t.uint32(122).fork()).ldelim(), null != e.pagesChanged && Object.hasOwnProperty.call(e, "pagesChanged") && s.PagesChanged.encode(e.pagesChanged, t.uint32(130).fork()).ldelim(), null != e.debugLastBackmsgId && Object.hasOwnProperty.call(e, "debugLastBackmsgId") && t.uint32(138).string(e.debugLastBackmsgId), null != e.pageProfile && Object.hasOwnProperty.call(e, "pageProfile") && s.PageProfile.encode(e.pageProfile, t.uint32(146).fork()).ldelim(), null != e.fileUrlsResponse && Object.hasOwnProperty.call(e, "fileUrlsResponse") && s.FileURLsResponse.encode(e.fileUrlsResponse, t.uint32(154).fork()).ldelim(), null != e.parentMessage && Object.hasOwnProperty.call(e, "parentMessage") && s.ParentMessage.encode(e.parentMessage, t.uint32(162).fork()).ldelim(), null != e.autoRerun && Object.hasOwnProperty.call(e, "autoRerun") && s.AutoRerun.encode(e.autoRerun, t.uint32(170).fork()).ldelim(), null != e.logo && Object.hasOwnProperty.call(e, "logo") && s.Logo.encode(e.logo, t.uint32(178).fork()).ldelim(), null != e.navigation && Object.hasOwnProperty.call(e, "navigation") && s.Navigation.encode(e.navigation, t.uint32(186).fork()).ldelim(), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.ForwardMsg;
                             for (; e.pos < n;) {
@@ -41971,14 +41981,17 @@
                                         break;
                                     case 9:
                                         r.sessionStatusChanged = s.SessionStatus.decode(e, e.uint32());
                                         break;
                                     case 10:
                                         r.sessionEvent = s.SessionEvent.decode(e, e.uint32());
                                         break;
+                                    case 23:
+                                        r.navigation = s.Navigation.decode(e, e.uint32());
+                                        break;
                                     case 15:
                                         r.pageNotFound = s.PageNotFound.decode(e, e.uint32());
                                         break;
                                     case 16:
                                         r.pagesChanged = s.PagesChanged.decode(e, e.uint32());
                                         break;
                                     case 19:
@@ -42084,14 +42097,22 @@
                                 if (1 === t.type) return "type: multiple values";
                                 t.type = 1;
                                 {
                                     let t = s.SessionEvent.verify(e.sessionEvent);
                                     if (t) return "sessionEvent." + t
                                 }
                             }
+                            if (null != e.navigation && e.hasOwnProperty("navigation")) {
+                                if (1 === t.type) return "type: multiple values";
+                                t.type = 1;
+                                {
+                                    let t = s.Navigation.verify(e.navigation);
+                                    if (t) return "navigation." + t
+                                }
+                            }
                             if (null != e.pageNotFound && e.hasOwnProperty("pageNotFound")) {
                                 if (1 === t.type) return "type: multiple values";
                                 t.type = 1;
                                 {
                                     let t = s.PageNotFound.verify(e.pageNotFound);
                                     if (t) return "pageNotFound." + t
                                 }
@@ -42199,14 +42220,18 @@
                                 if ("object" !== typeof e.sessionStatusChanged) throw TypeError(".ForwardMsg.sessionStatusChanged: object expected");
                                 t.sessionStatusChanged = s.SessionStatus.fromObject(e.sessionStatusChanged)
                             }
                             if (null != e.sessionEvent) {
                                 if ("object" !== typeof e.sessionEvent) throw TypeError(".ForwardMsg.sessionEvent: object expected");
                                 t.sessionEvent = s.SessionEvent.fromObject(e.sessionEvent)
                             }
+                            if (null != e.navigation) {
+                                if ("object" !== typeof e.navigation) throw TypeError(".ForwardMsg.navigation: object expected");
+                                t.navigation = s.Navigation.fromObject(e.navigation)
+                            }
                             if (null != e.pageNotFound) {
                                 if ("object" !== typeof e.pageNotFound) throw TypeError(".ForwardMsg.pageNotFound: object expected");
                                 t.pageNotFound = s.PageNotFound.fromObject(e.pageNotFound)
                             }
                             if (null != e.pagesChanged) {
                                 if ("object" !== typeof e.pagesChanged) throw TypeError(".ForwardMsg.pagesChanged: object expected");
                                 t.pagesChanged = s.PagesChanged.fromObject(e.pagesChanged)
@@ -42227,15 +42252,15 @@
                                 if ("object" !== typeof e.parentMessage) throw TypeError(".ForwardMsg.parentMessage: object expected");
                                 t.parentMessage = s.ParentMessage.fromObject(e.parentMessage)
                             }
                             return null != e.refHash && (t.refHash = String(e.refHash)), null != e.debugLastBackmsgId && (t.debugLastBackmsgId = String(e.debugLastBackmsgId)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            return t.defaults && (n.hash = "", n.metadata = null, n.debugLastBackmsgId = ""), null != e.hash && e.hasOwnProperty("hash") && (n.hash = e.hash), null != e.metadata && e.hasOwnProperty("metadata") && (n.metadata = s.ForwardMsgMetadata.toObject(e.metadata, t)), null != e.newSession && e.hasOwnProperty("newSession") && (n.newSession = s.NewSession.toObject(e.newSession, t), t.oneofs && (n.type = "newSession")), null != e.delta && e.hasOwnProperty("delta") && (n.delta = s.Delta.toObject(e.delta, t), t.oneofs && (n.type = "delta")), null != e.scriptFinished && e.hasOwnProperty("scriptFinished") && (n.scriptFinished = t.enums === String ? void 0 === s.ForwardMsg.ScriptFinishedStatus[e.scriptFinished] ? e.scriptFinished : s.ForwardMsg.ScriptFinishedStatus[e.scriptFinished] : e.scriptFinished, t.oneofs && (n.type = "scriptFinished")), null != e.sessionStatusChanged && e.hasOwnProperty("sessionStatusChanged") && (n.sessionStatusChanged = s.SessionStatus.toObject(e.sessionStatusChanged, t), t.oneofs && (n.type = "sessionStatusChanged")), null != e.sessionEvent && e.hasOwnProperty("sessionEvent") && (n.sessionEvent = s.SessionEvent.toObject(e.sessionEvent, t), t.oneofs && (n.type = "sessionEvent")), null != e.refHash && e.hasOwnProperty("refHash") && (n.refHash = e.refHash, t.oneofs && (n.type = "refHash")), null != e.pageInfoChanged && e.hasOwnProperty("pageInfoChanged") && (n.pageInfoChanged = s.PageInfo.toObject(e.pageInfoChanged, t), t.oneofs && (n.type = "pageInfoChanged")), null != e.pageConfigChanged && e.hasOwnProperty("pageConfigChanged") && (n.pageConfigChanged = s.PageConfig.toObject(e.pageConfigChanged, t), t.oneofs && (n.type = "pageConfigChanged")), null != e.gitInfoChanged && e.hasOwnProperty("gitInfoChanged") && (n.gitInfoChanged = s.GitInfo.toObject(e.gitInfoChanged, t), t.oneofs && (n.type = "gitInfoChanged")), null != e.pageNotFound && e.hasOwnProperty("pageNotFound") && (n.pageNotFound = s.PageNotFound.toObject(e.pageNotFound, t), t.oneofs && (n.type = "pageNotFound")), null != e.pagesChanged && e.hasOwnProperty("pagesChanged") && (n.pagesChanged = s.PagesChanged.toObject(e.pagesChanged, t), t.oneofs && (n.type = "pagesChanged")), null != e.debugLastBackmsgId && e.hasOwnProperty("debugLastBackmsgId") && (n.debugLastBackmsgId = e.debugLastBackmsgId), null != e.pageProfile && e.hasOwnProperty("pageProfile") && (n.pageProfile = s.PageProfile.toObject(e.pageProfile, t), t.oneofs && (n.type = "pageProfile")), null != e.fileUrlsResponse && e.hasOwnProperty("fileUrlsResponse") && (n.fileUrlsResponse = s.FileURLsResponse.toObject(e.fileUrlsResponse, t), t.oneofs && (n.type = "fileUrlsResponse")), null != e.parentMessage && e.hasOwnProperty("parentMessage") && (n.parentMessage = s.ParentMessage.toObject(e.parentMessage, t), t.oneofs && (n.type = "parentMessage")), null != e.autoRerun && e.hasOwnProperty("autoRerun") && (n.autoRerun = s.AutoRerun.toObject(e.autoRerun, t), t.oneofs && (n.type = "autoRerun")), null != e.logo && e.hasOwnProperty("logo") && (n.logo = s.Logo.toObject(e.logo, t), t.oneofs && (n.type = "logo")), n
+                            return t.defaults && (n.hash = "", n.metadata = null, n.debugLastBackmsgId = ""), null != e.hash && e.hasOwnProperty("hash") && (n.hash = e.hash), null != e.metadata && e.hasOwnProperty("metadata") && (n.metadata = s.ForwardMsgMetadata.toObject(e.metadata, t)), null != e.newSession && e.hasOwnProperty("newSession") && (n.newSession = s.NewSession.toObject(e.newSession, t), t.oneofs && (n.type = "newSession")), null != e.delta && e.hasOwnProperty("delta") && (n.delta = s.Delta.toObject(e.delta, t), t.oneofs && (n.type = "delta")), null != e.scriptFinished && e.hasOwnProperty("scriptFinished") && (n.scriptFinished = t.enums === String ? void 0 === s.ForwardMsg.ScriptFinishedStatus[e.scriptFinished] ? e.scriptFinished : s.ForwardMsg.ScriptFinishedStatus[e.scriptFinished] : e.scriptFinished, t.oneofs && (n.type = "scriptFinished")), null != e.sessionStatusChanged && e.hasOwnProperty("sessionStatusChanged") && (n.sessionStatusChanged = s.SessionStatus.toObject(e.sessionStatusChanged, t), t.oneofs && (n.type = "sessionStatusChanged")), null != e.sessionEvent && e.hasOwnProperty("sessionEvent") && (n.sessionEvent = s.SessionEvent.toObject(e.sessionEvent, t), t.oneofs && (n.type = "sessionEvent")), null != e.refHash && e.hasOwnProperty("refHash") && (n.refHash = e.refHash, t.oneofs && (n.type = "refHash")), null != e.pageInfoChanged && e.hasOwnProperty("pageInfoChanged") && (n.pageInfoChanged = s.PageInfo.toObject(e.pageInfoChanged, t), t.oneofs && (n.type = "pageInfoChanged")), null != e.pageConfigChanged && e.hasOwnProperty("pageConfigChanged") && (n.pageConfigChanged = s.PageConfig.toObject(e.pageConfigChanged, t), t.oneofs && (n.type = "pageConfigChanged")), null != e.gitInfoChanged && e.hasOwnProperty("gitInfoChanged") && (n.gitInfoChanged = s.GitInfo.toObject(e.gitInfoChanged, t), t.oneofs && (n.type = "gitInfoChanged")), null != e.pageNotFound && e.hasOwnProperty("pageNotFound") && (n.pageNotFound = s.PageNotFound.toObject(e.pageNotFound, t), t.oneofs && (n.type = "pageNotFound")), null != e.pagesChanged && e.hasOwnProperty("pagesChanged") && (n.pagesChanged = s.PagesChanged.toObject(e.pagesChanged, t), t.oneofs && (n.type = "pagesChanged")), null != e.debugLastBackmsgId && e.hasOwnProperty("debugLastBackmsgId") && (n.debugLastBackmsgId = e.debugLastBackmsgId), null != e.pageProfile && e.hasOwnProperty("pageProfile") && (n.pageProfile = s.PageProfile.toObject(e.pageProfile, t), t.oneofs && (n.type = "pageProfile")), null != e.fileUrlsResponse && e.hasOwnProperty("fileUrlsResponse") && (n.fileUrlsResponse = s.FileURLsResponse.toObject(e.fileUrlsResponse, t), t.oneofs && (n.type = "fileUrlsResponse")), null != e.parentMessage && e.hasOwnProperty("parentMessage") && (n.parentMessage = s.ParentMessage.toObject(e.parentMessage, t), t.oneofs && (n.type = "parentMessage")), null != e.autoRerun && e.hasOwnProperty("autoRerun") && (n.autoRerun = s.AutoRerun.toObject(e.autoRerun, t), t.oneofs && (n.type = "autoRerun")), null != e.logo && e.hasOwnProperty("logo") && (n.logo = s.Logo.toObject(e.logo, t), t.oneofs && (n.type = "logo")), null != e.navigation && e.hasOwnProperty("navigation") && (n.navigation = s.Navigation.toObject(e.navigation, t), t.oneofs && (n.type = "navigation")), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/ForwardMsg"
                         }, e.ScriptFinishedStatus = function() {
                             const e = {},
                                 t = Object.create(e);
@@ -42243,23 +42268,23 @@
                         }(), e
                     })()),
                     A = s.ForwardMsgMetadata = (() => {
                         function e(e) {
                             if (this.deltaPath = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.cacheable = !1, e.prototype.deltaPath = a.emptyArray, e.prototype.elementDimensionSpec = null, e.create = function(t) {
+                        return e.prototype.cacheable = !1, e.prototype.deltaPath = a.emptyArray, e.prototype.elementDimensionSpec = null, e.prototype.activeScriptHash = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
                             if (t || (t = i.create()), null != e.cacheable && Object.hasOwnProperty.call(e, "cacheable") && t.uint32(8).bool(e.cacheable), null != e.deltaPath && e.deltaPath.length) {
                                 t.uint32(18).fork();
                                 for (let n = 0; n < e.deltaPath.length; ++n) t.uint32(e.deltaPath[n]);
                                 t.ldelim()
                             }
-                            return null != e.elementDimensionSpec && Object.hasOwnProperty.call(e, "elementDimensionSpec") && s.ElementDimensionSpec.encode(e.elementDimensionSpec, t.uint32(26).fork()).ldelim(), t
+                            return null != e.elementDimensionSpec && Object.hasOwnProperty.call(e, "elementDimensionSpec") && s.ElementDimensionSpec.encode(e.elementDimensionSpec, t.uint32(26).fork()).ldelim(), null != e.activeScriptHash && Object.hasOwnProperty.call(e, "activeScriptHash") && t.uint32(34).string(e.activeScriptHash), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.ForwardMsgMetadata;
                             for (; e.pos < n;) {
@@ -42273,14 +42298,17 @@
                                             let t = e.uint32() + e.pos;
                                             for (; e.pos < t;) r.deltaPath.push(e.uint32())
                                         } else r.deltaPath.push(e.uint32());
                                         break;
                                     case 3:
                                         r.elementDimensionSpec = s.ElementDimensionSpec.decode(e, e.uint32());
                                         break;
+                                    case 4:
+                                        r.activeScriptHash = e.string();
+                                        break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
@@ -42292,36 +42320,36 @@
                                 for (let t = 0; t < e.deltaPath.length; ++t)
                                     if (!a.isInteger(e.deltaPath[t])) return "deltaPath: integer[] expected"
                             }
                             if (null != e.elementDimensionSpec && e.hasOwnProperty("elementDimensionSpec")) {
                                 let t = s.ElementDimensionSpec.verify(e.elementDimensionSpec);
                                 if (t) return "elementDimensionSpec." + t
                             }
-                            return null
+                            return null != e.activeScriptHash && e.hasOwnProperty("activeScriptHash") && !a.isString(e.activeScriptHash) ? "activeScriptHash: string expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.ForwardMsgMetadata) return e;
                             let t = new s.ForwardMsgMetadata;
                             if (null != e.cacheable && (t.cacheable = Boolean(e.cacheable)), e.deltaPath) {
                                 if (!Array.isArray(e.deltaPath)) throw TypeError(".ForwardMsgMetadata.deltaPath: array expected");
                                 t.deltaPath = [];
                                 for (let n = 0; n < e.deltaPath.length; ++n) t.deltaPath[n] = e.deltaPath[n] >>> 0
                             }
                             if (null != e.elementDimensionSpec) {
                                 if ("object" !== typeof e.elementDimensionSpec) throw TypeError(".ForwardMsgMetadata.elementDimensionSpec: object expected");
                                 t.elementDimensionSpec = s.ElementDimensionSpec.fromObject(e.elementDimensionSpec)
                             }
-                            return t
+                            return null != e.activeScriptHash && (t.activeScriptHash = String(e.activeScriptHash)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            if ((t.arrays || t.defaults) && (n.deltaPath = []), t.defaults && (n.cacheable = !1, n.elementDimensionSpec = null), null != e.cacheable && e.hasOwnProperty("cacheable") && (n.cacheable = e.cacheable), e.deltaPath && e.deltaPath.length) {
+                            if ((t.arrays || t.defaults) && (n.deltaPath = []), t.defaults && (n.cacheable = !1, n.elementDimensionSpec = null, n.activeScriptHash = ""), null != e.cacheable && e.hasOwnProperty("cacheable") && (n.cacheable = e.cacheable), e.deltaPath && e.deltaPath.length) {
                                 n.deltaPath = [];
                                 for (let t = 0; t < e.deltaPath.length; ++t) n.deltaPath[t] = e.deltaPath[t]
                             }
-                            return null != e.elementDimensionSpec && e.hasOwnProperty("elementDimensionSpec") && (n.elementDimensionSpec = s.ElementDimensionSpec.toObject(e.elementDimensionSpec, t)), n
+                            return null != e.elementDimensionSpec && e.hasOwnProperty("elementDimensionSpec") && (n.elementDimensionSpec = s.ElementDimensionSpec.toObject(e.elementDimensionSpec, t)), null != e.activeScriptHash && e.hasOwnProperty("activeScriptHash") && (n.activeScriptHash = e.activeScriptHash), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/ForwardMsgMetadata"
                         }, e
                     })(),
                     v = (s.ElementDimensionSpec = (() => {
@@ -43499,27 +43527,143 @@
                             let n = {};
                             return t.defaults && (n.name = "", n.data = null, n.hasName = !1), null != e.name && e.hasOwnProperty("name") && (n.name = e.name), null != e.data && e.hasOwnProperty("data") && (n.data = s.DataFrame.toObject(e.data, t)), null != e.hasName && e.hasOwnProperty("hasName") && (n.hasName = e.hasName), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/NamedDataSet"
                         }, e
-                    })(), s.NewSession = (() => {
+                    })(), s.Navigation = (() => {
+                        function e(e) {
+                            if (this.sections = [], this.appPages = [], e)
+                                for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
+                        }
+                        return e.prototype.sections = a.emptyArray, e.prototype.appPages = a.emptyArray, e.prototype.position = 0, e.prototype.pageScriptHash = "", e.create = function(t) {
+                            return new e(t)
+                        }, e.encode = function(e, t) {
+                            if (t || (t = i.create()), null != e.sections && e.sections.length)
+                                for (let n = 0; n < e.sections.length; ++n) t.uint32(10).string(e.sections[n]);
+                            if (null != e.appPages && e.appPages.length)
+                                for (let n = 0; n < e.appPages.length; ++n) s.AppPage.encode(e.appPages[n], t.uint32(18).fork()).ldelim();
+                            return null != e.position && Object.hasOwnProperty.call(e, "position") && t.uint32(24).int32(e.position), null != e.pageScriptHash && Object.hasOwnProperty.call(e, "pageScriptHash") && t.uint32(34).string(e.pageScriptHash), t
+                        }, e.encodeDelimited = function(e, t) {
+                            return this.encode(e, t).ldelim()
+                        }, e.decode = function(e, t) {
+                            e instanceof o || (e = o.create(e));
+                            let n = void 0 === t ? e.len : e.pos + t,
+                                r = new s.Navigation;
+                            for (; e.pos < n;) {
+                                let t = e.uint32();
+                                switch (t >>> 3) {
+                                    case 1:
+                                        r.sections && r.sections.length || (r.sections = []), r.sections.push(e.string());
+                                        break;
+                                    case 2:
+                                        r.appPages && r.appPages.length || (r.appPages = []), r.appPages.push(s.AppPage.decode(e, e.uint32()));
+                                        break;
+                                    case 3:
+                                        r.position = e.int32();
+                                        break;
+                                    case 4:
+                                        r.pageScriptHash = e.string();
+                                        break;
+                                    default:
+                                        e.skipType(7 & t)
+                                }
+                            }
+                            return r
+                        }, e.decodeDelimited = function(e) {
+                            return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
+                        }, e.verify = function(e) {
+                            if ("object" !== typeof e || null === e) return "object expected";
+                            if (null != e.sections && e.hasOwnProperty("sections")) {
+                                if (!Array.isArray(e.sections)) return "sections: array expected";
+                                for (let t = 0; t < e.sections.length; ++t)
+                                    if (!a.isString(e.sections[t])) return "sections: string[] expected"
+                            }
+                            if (null != e.appPages && e.hasOwnProperty("appPages")) {
+                                if (!Array.isArray(e.appPages)) return "appPages: array expected";
+                                for (let t = 0; t < e.appPages.length; ++t) {
+                                    let n = s.AppPage.verify(e.appPages[t]);
+                                    if (n) return "appPages." + n
+                                }
+                            }
+                            if (null != e.position && e.hasOwnProperty("position")) switch (e.position) {
+                                default:
+                                    return "position: enum value expected";
+                                case 0:
+                                case 1:
+                            }
+                            return null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && !a.isString(e.pageScriptHash) ? "pageScriptHash: string expected" : null
+                        }, e.fromObject = function(e) {
+                            if (e instanceof s.Navigation) return e;
+                            let t = new s.Navigation;
+                            if (e.sections) {
+                                if (!Array.isArray(e.sections)) throw TypeError(".Navigation.sections: array expected");
+                                t.sections = [];
+                                for (let n = 0; n < e.sections.length; ++n) t.sections[n] = String(e.sections[n])
+                            }
+                            if (e.appPages) {
+                                if (!Array.isArray(e.appPages)) throw TypeError(".Navigation.appPages: array expected");
+                                t.appPages = [];
+                                for (let n = 0; n < e.appPages.length; ++n) {
+                                    if ("object" !== typeof e.appPages[n]) throw TypeError(".Navigation.appPages: object expected");
+                                    t.appPages[n] = s.AppPage.fromObject(e.appPages[n])
+                                }
+                            }
+                            switch (e.position) {
+                                default:
+                                    if ("number" === typeof e.position) {
+                                        t.position = e.position;
+                                        break
+                                    }
+                                    break;
+                                case "HIDDEN":
+                                case 0:
+                                    t.position = 0;
+                                    break;
+                                case "SIDEBAR":
+                                case 1:
+                                    t.position = 1
+                            }
+                            return null != e.pageScriptHash && (t.pageScriptHash = String(e.pageScriptHash)), t
+                        }, e.toObject = function(e, t) {
+                            t || (t = {});
+                            let n = {};
+                            if ((t.arrays || t.defaults) && (n.sections = [], n.appPages = []), t.defaults && (n.position = t.enums === String ? "HIDDEN" : 0, n.pageScriptHash = ""), e.sections && e.sections.length) {
+                                n.sections = [];
+                                for (let t = 0; t < e.sections.length; ++t) n.sections[t] = e.sections[t]
+                            }
+                            if (e.appPages && e.appPages.length) {
+                                n.appPages = [];
+                                for (let r = 0; r < e.appPages.length; ++r) n.appPages[r] = s.AppPage.toObject(e.appPages[r], t)
+                            }
+                            return null != e.position && e.hasOwnProperty("position") && (n.position = t.enums === String ? void 0 === s.Navigation.Position[e.position] ? e.position : s.Navigation.Position[e.position] : e.position), null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && (n.pageScriptHash = e.pageScriptHash), n
+                        }, e.prototype.toJSON = function() {
+                            return this.constructor.toObject(this, r.util.toJSONOptions)
+                        }, e.getTypeUrl = function(e) {
+                            return void 0 === e && (e = "type.googleapis.com"), e + "/Navigation"
+                        }, e.Position = function() {
+                            const e = {},
+                                t = Object.create(e);
+                            return t[e[0] = "HIDDEN"] = 0, t[e[1] = "SIDEBAR"] = 1, t
+                        }(), e
+                    })()),
+                    _ = (s.NewSession = (() => {
                         function e(e) {
                             if (this.appPages = [], this.fragmentIdsThisRun = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.initialize = null, e.prototype.scriptRunId = "", e.prototype.name = "", e.prototype.mainScriptPath = "", e.prototype.config = null, e.prototype.customTheme = null, e.prototype.appPages = a.emptyArray, e.prototype.pageScriptHash = "", e.prototype.fragmentIdsThisRun = a.emptyArray, e.create = function(t) {
+                        return e.prototype.initialize = null, e.prototype.scriptRunId = "", e.prototype.name = "", e.prototype.mainScriptPath = "", e.prototype.config = null, e.prototype.customTheme = null, e.prototype.appPages = a.emptyArray, e.prototype.pageScriptHash = "", e.prototype.fragmentIdsThisRun = a.emptyArray, e.prototype.mainScriptHash = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
                             if (t || (t = i.create()), null != e.initialize && Object.hasOwnProperty.call(e, "initialize") && s.Initialize.encode(e.initialize, t.uint32(10).fork()).ldelim(), null != e.scriptRunId && Object.hasOwnProperty.call(e, "scriptRunId") && t.uint32(18).string(e.scriptRunId), null != e.name && Object.hasOwnProperty.call(e, "name") && t.uint32(26).string(e.name), null != e.mainScriptPath && Object.hasOwnProperty.call(e, "mainScriptPath") && t.uint32(34).string(e.mainScriptPath), null != e.config && Object.hasOwnProperty.call(e, "config") && s.Config.encode(e.config, t.uint32(50).fork()).ldelim(), null != e.customTheme && Object.hasOwnProperty.call(e, "customTheme") && s.CustomThemeConfig.encode(e.customTheme, t.uint32(58).fork()).ldelim(), null != e.appPages && e.appPages.length)
                                 for (let n = 0; n < e.appPages.length; ++n) s.AppPage.encode(e.appPages[n], t.uint32(66).fork()).ldelim();
                             if (null != e.pageScriptHash && Object.hasOwnProperty.call(e, "pageScriptHash") && t.uint32(74).string(e.pageScriptHash), null != e.fragmentIdsThisRun && e.fragmentIdsThisRun.length)
                                 for (let n = 0; n < e.fragmentIdsThisRun.length; ++n) t.uint32(82).string(e.fragmentIdsThisRun[n]);
-                            return t
+                            return null != e.mainScriptHash && Object.hasOwnProperty.call(e, "mainScriptHash") && t.uint32(90).string(e.mainScriptHash), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.NewSession;
                             for (; e.pos < n;) {
@@ -43548,14 +43692,17 @@
                                         break;
                                     case 9:
                                         r.pageScriptHash = e.string();
                                         break;
                                     case 10:
                                         r.fragmentIdsThisRun && r.fragmentIdsThisRun.length || (r.fragmentIdsThisRun = []), r.fragmentIdsThisRun.push(e.string());
                                         break;
+                                    case 11:
+                                        r.mainScriptHash = e.string();
+                                        break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
@@ -43585,15 +43732,15 @@
                             }
                             if (null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && !a.isString(e.pageScriptHash)) return "pageScriptHash: string expected";
                             if (null != e.fragmentIdsThisRun && e.hasOwnProperty("fragmentIdsThisRun")) {
                                 if (!Array.isArray(e.fragmentIdsThisRun)) return "fragmentIdsThisRun: array expected";
                                 for (let t = 0; t < e.fragmentIdsThisRun.length; ++t)
                                     if (!a.isString(e.fragmentIdsThisRun[t])) return "fragmentIdsThisRun: string[] expected"
                             }
-                            return null
+                            return null != e.mainScriptHash && e.hasOwnProperty("mainScriptHash") && !a.isString(e.mainScriptHash) ? "mainScriptHash: string expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.NewSession) return e;
                             let t = new s.NewSession;
                             if (null != e.initialize) {
                                 if ("object" !== typeof e.initialize) throw TypeError(".NewSession.initialize: object expected");
                                 t.initialize = s.Initialize.fromObject(e.initialize)
                             }
@@ -43614,27 +43761,27 @@
                                 }
                             }
                             if (null != e.pageScriptHash && (t.pageScriptHash = String(e.pageScriptHash)), e.fragmentIdsThisRun) {
                                 if (!Array.isArray(e.fragmentIdsThisRun)) throw TypeError(".NewSession.fragmentIdsThisRun: array expected");
                                 t.fragmentIdsThisRun = [];
                                 for (let n = 0; n < e.fragmentIdsThisRun.length; ++n) t.fragmentIdsThisRun[n] = String(e.fragmentIdsThisRun[n])
                             }
-                            return t
+                            return null != e.mainScriptHash && (t.mainScriptHash = String(e.mainScriptHash)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            if ((t.arrays || t.defaults) && (n.appPages = [], n.fragmentIdsThisRun = []), t.defaults && (n.initialize = null, n.scriptRunId = "", n.name = "", n.mainScriptPath = "", n.config = null, n.customTheme = null, n.pageScriptHash = ""), null != e.initialize && e.hasOwnProperty("initialize") && (n.initialize = s.Initialize.toObject(e.initialize, t)), null != e.scriptRunId && e.hasOwnProperty("scriptRunId") && (n.scriptRunId = e.scriptRunId), null != e.name && e.hasOwnProperty("name") && (n.name = e.name), null != e.mainScriptPath && e.hasOwnProperty("mainScriptPath") && (n.mainScriptPath = e.mainScriptPath), null != e.config && e.hasOwnProperty("config") && (n.config = s.Config.toObject(e.config, t)), null != e.customTheme && e.hasOwnProperty("customTheme") && (n.customTheme = s.CustomThemeConfig.toObject(e.customTheme, t)), e.appPages && e.appPages.length) {
+                            if ((t.arrays || t.defaults) && (n.appPages = [], n.fragmentIdsThisRun = []), t.defaults && (n.initialize = null, n.scriptRunId = "", n.name = "", n.mainScriptPath = "", n.config = null, n.customTheme = null, n.pageScriptHash = "", n.mainScriptHash = ""), null != e.initialize && e.hasOwnProperty("initialize") && (n.initialize = s.Initialize.toObject(e.initialize, t)), null != e.scriptRunId && e.hasOwnProperty("scriptRunId") && (n.scriptRunId = e.scriptRunId), null != e.name && e.hasOwnProperty("name") && (n.name = e.name), null != e.mainScriptPath && e.hasOwnProperty("mainScriptPath") && (n.mainScriptPath = e.mainScriptPath), null != e.config && e.hasOwnProperty("config") && (n.config = s.Config.toObject(e.config, t)), null != e.customTheme && e.hasOwnProperty("customTheme") && (n.customTheme = s.CustomThemeConfig.toObject(e.customTheme, t)), e.appPages && e.appPages.length) {
                                 n.appPages = [];
                                 for (let r = 0; r < e.appPages.length; ++r) n.appPages[r] = s.AppPage.toObject(e.appPages[r], t)
                             }
                             if (null != e.pageScriptHash && e.hasOwnProperty("pageScriptHash") && (n.pageScriptHash = e.pageScriptHash), e.fragmentIdsThisRun && e.fragmentIdsThisRun.length) {
                                 n.fragmentIdsThisRun = [];
                                 for (let t = 0; t < e.fragmentIdsThisRun.length; ++t) n.fragmentIdsThisRun[t] = e.fragmentIdsThisRun[t]
                             }
-                            return n
+                            return null != e.mainScriptHash && e.hasOwnProperty("mainScriptHash") && (n.mainScriptHash = e.mainScriptHash), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/NewSession"
                         }, e
                     })(), s.Initialize = (() => {
                         function e(e) {
@@ -43819,15 +43966,15 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/Config"
                         }, e.ToolbarMode = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "AUTO"] = 0, t[e[1] = "DEVELOPER"] = 1, t[e[2] = "VIEWER"] = 2, t[e[3] = "MINIMAL"] = 3, t
                         }(), e
                     })()),
-                    _ = s.CustomThemeConfig = (() => {
+                    x = s.CustomThemeConfig = (() => {
                         function e(e) {
                             if (this.fontFaces = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.primaryColor = "", e.prototype.secondaryBackgroundColor = "", e.prototype.backgroundColor = "", e.prototype.textColor = "", e.prototype.font = 0, e.prototype.base = 0, e.prototype.widgetBackgroundColor = "", e.prototype.widgetBorderColor = "", e.prototype.radii = null, e.prototype.bodyFont = "", e.prototype.codeFont = "", e.prototype.fontFaces = a.emptyArray, e.prototype.fontSizes = null, e.prototype.skeletonBackgroundColor = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -44003,15 +44150,15 @@
                             return t[e[0] = "LIGHT"] = 0, t[e[1] = "DARK"] = 1, t
                         }(), e.FontFamily = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "SANS_SERIF"] = 0, t[e[1] = "SERIF"] = 1, t[e[2] = "MONOSPACE"] = 2, t
                         }(), e
                     })(),
-                    x = (s.FontFace = (() => {
+                    R = (s.FontFace = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.url = "", e.prototype.family = "", e.prototype.weight = 0, e.prototype.style = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -44390,15 +44537,15 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/NumberInput"
                         }, e.DataType = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "INT"] = 0, t[e[1] = "FLOAT"] = 1, t
                         }(), e
                     })()),
-                    R = s.PageConfig = (() => {
+                    T = s.PageConfig = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.title = "", e.prototype.favicon = "", e.prototype.layout = 0, e.prototype.initialSidebarState = 0, e.prototype.menuItems = null, e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -44567,15 +44714,15 @@
                             return t[e[0] = "CENTERED"] = 0, t[e[1] = "WIDE"] = 1, t
                         }(), e.SidebarState = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "AUTO"] = 0, t[e[1] = "EXPANDED"] = 1, t[e[2] = "COLLAPSED"] = 2, t
                         }(), e
                     })(),
-                    T = (s.PageInfo = (() => {
+                    k = (s.PageInfo = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.queryString = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -44852,15 +44999,15 @@
                             return null != e.os && e.hasOwnProperty("os") && (n.os = e.os), null != e.timezone && e.hasOwnProperty("timezone") && (n.timezone = e.timezone), null != e.headless && e.hasOwnProperty("headless") && (n.headless = e.headless), null != e.isFragmentRun && e.hasOwnProperty("isFragmentRun") && (n.isFragmentRun = e.isFragmentRun), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/PageProfile"
                         }, e
                     })()),
-                    k = (s.Argument = (() => {
+                    C = (s.Argument = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.k = "", e.prototype.t = "", e.prototype.m = "", e.prototype.p = 0, e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -45220,15 +45367,15 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/PlotlyChart"
                         }, e.SelectionMode = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "POINTS"] = 0, t[e[1] = "BOX"] = 1, t[e[2] = "LASSO"] = 2, t
                         }(), e
                     })()),
-                    C = (s.Figure = (() => {
+                    W = (s.Figure = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.spec = "", e.prototype.config = "", e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -45760,15 +45907,15 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/Skeleton"
                         }, e.SkeletonStyle = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "ELEMENT"] = 0, t[e[1] = "APP"] = 1, t
                         }(), e
                     })()),
-                    W = s.Slider = (() => {
+                    N = s.Slider = (() => {
                         function e(e) {
                             if (this.default = [], this.value = [], this.options = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.id = "", e.prototype.formId = "", e.prototype.label = "", e.prototype.format = "", e.prototype.dataType = 0, e.prototype.default = a.emptyArray, e.prototype.min = 0, e.prototype.max = 0, e.prototype.step = 0, e.prototype.value = a.emptyArray, e.prototype.setValue = !1, e.prototype.options = a.emptyArray, e.prototype.help = "", e.prototype.disabled = !1, e.prototype.labelVisibility = null, e.prototype.type = 0, e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -45998,15 +46145,15 @@
                             return t[e[0] = "INT"] = 0, t[e[1] = "FLOAT"] = 1, t[e[2] = "DATETIME"] = 2, t[e[3] = "DATE"] = 3, t[e[4] = "TIME"] = 4, t
                         }(), e.Type = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "UNSPECIFIED"] = 0, t[e[1] = "SLIDER"] = 1, t[e[2] = "SELECT_SLIDER"] = 2, t
                         }(), e
                     })(),
-                    N = (s.Snow = (() => {
+                    L = (s.Snow = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.show = !1, e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -46365,15 +46512,15 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/TextInput"
                         }, e.Type = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "DEFAULT"] = 0, t[e[1] = "PASSWORD"] = 1, t
                         }(), e
                     })()),
-                    L = (s.TimeInput = (() => {
+                    I = (s.TimeInput = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         let t;
                         return e.prototype.id = "", e.prototype.label = "", e.prototype.default = null, e.prototype.help = "", e.prototype.formId = "", e.prototype.value = null, e.prototype.setValue = !1, e.prototype.disabled = !1, e.prototype.labelVisibility = null, e.prototype.step = a.Long ? a.Long.fromBits(0, 0, !1) : 0, Object.defineProperty(e.prototype, "_default", {
                             get: a.oneOfGetter(t = ["default"]),
@@ -46762,15 +46909,15 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/Video"
                         }, e.Type = function() {
                             const e = {},
                                 t = Object.create(e);
                             return t[e[0] = "UNUSED"] = 0, t[e[1] = "NATIVE"] = 1, t[e[2] = "YOUTUBE_IFRAME"] = 2, t
                         }(), e
                     })()),
-                    I = s.WidgetStates = (() => {
+                    P = s.WidgetStates = (() => {
                         function e(e) {
                             if (this.widgets = [], e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         return e.prototype.widgets = a.emptyArray, e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
@@ -46823,15 +46970,15 @@
                             return n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/WidgetStates"
                         }, e
                     })(),
-                    P = s.WidgetState = (() => {
+                    D = s.WidgetState = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         let t;
                         return e.prototype.id = "", e.prototype.triggerValue = null, e.prototype.boolValue = null, e.prototype.doubleValue = null, e.prototype.intValue = null, e.prototype.stringValue = null, e.prototype.doubleArrayValue = null, e.prototype.intArrayValue = null, e.prototype.stringArrayValue = null, e.prototype.jsonValue = null, e.prototype.arrowValue = null, e.prototype.bytesValue = null, e.prototype.fileUploaderStateValue = null, e.prototype.stringTriggerValue = null, Object.defineProperty(e.prototype, "value", {
                             get: a.oneOfGetter(t = ["triggerValue", "boolValue", "doubleValue", "intValue", "stringValue", "doubleArrayValue", "intArrayValue", "stringArrayValue", "jsonValue", "arrowValue", "bytesValue", "fileUploaderStateValue", "stringTriggerValue"]),
@@ -49503,24 +49650,28 @@
                         return (0, r.useEffect)((() => {
                             t.current = e
                         }), [e]), t.current
                     },
                     i = (e, t) => {
                         const {
                             current: n
-                        } = e, [o, i] = (0, r.useState)(!1);
-                        return (0, r.useEffect)((() => {
+                        } = e, [o, i] = (0, r.useState)(!1), a = (0, r.useCallback)((() => {
                             if (n) {
                                 const {
                                     scrollHeight: e,
                                     clientHeight: t
                                 } = n;
                                 i(e > t)
                             }
-                        }), [i, t, n, null === n || void 0 === n ? void 0 : n.clientHeight]), o
+                        }), [n]);
+                        return (0, r.useEffect)((() => {
+                            a()
+                        }), [t, null === n || void 0 === n ? void 0 : n.clientHeight]), (0, r.useEffect)((() => (window.addEventListener("resize", a), () => {
+                            window.removeEventListener("resize", a)
+                        })), [a]), o
                     }
             },
             90994: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     T: () => r,
                     p: () => o
@@ -49906,18 +50057,18 @@
                     })),
                     d = (0, a.Z)(p, {
                         target: "ex0cdmw0"
                     })("display:inline-block;vertical-align:", (function(e) {
                         return e.iconVerticalAlign
                     }), ";overflow:hidden;")
             },
-            14609: (e, t, n) => {
+            30351: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    _: () => a
+                    s: () => a
                 });
                 var r = n(25773),
                     o = n(66845),
                     i = n(69),
                     a = o.forwardRef((function(e, t) {
                         return o.createElement(i.D, (0, r.Z)({
                             iconAttrs: {
@@ -49928,23 +50079,23 @@
                             iconViewBox: "0 0 24 24"
                         }, e, {
                             ref: t
                         }), o.createElement("path", {
                             fill: "none",
                             d: "M0 0h24v24H0V0z"
                         }), o.createElement("path", {
-                            d: "M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6-6-6z"
+                            d: "M15.41 7.41L14 6l-6 6 6 6 1.41-1.41L10.83 12l4.58-4.59z"
                         }))
                     }));
-                a.displayName = "ChevronRight"
+                a.displayName = "ChevronLeft"
             },
-            20545: (e, t, n) => {
+            14609: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    x: () => a
+                    _: () => a
                 });
                 var r = n(25773),
                     o = n(66845),
                     i = n(69),
                     a = o.forwardRef((function(e, t) {
                         return o.createElement(i.D, (0, r.Z)({
                             iconAttrs: {
@@ -49955,18 +50106,18 @@
                             iconViewBox: "0 0 24 24"
                         }, e, {
                             ref: t
                         }), o.createElement("path", {
                             fill: "none",
                             d: "M0 0h24v24H0V0z"
                         }), o.createElement("path", {
-                            d: "M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12 19 6.41z"
+                            d: "M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6-6-6z"
                         }))
                     }));
-                a.displayName = "Close"
+                a.displayName = "ChevronRight"
             },
             17715: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Z: () => oe
                 });
                 var r = function() {
@@ -65783,14 +65934,23 @@
                             return e.call(t, n[0], n[1]);
                         case 3:
                             return e.call(t, n[0], n[1], n[2])
                     }
                     return e.apply(t, n)
                 }
             },
+            29916: e => {
+                e.exports = function(e, t, n, r) {
+                    for (var o = -1, i = null == e ? 0 : e.length; ++o < i;) {
+                        var a = e[o];
+                        t(r, a, n(a), e)
+                    }
+                    return r
+                }
+            },
             67036: e => {
                 e.exports = function(e, t) {
                     for (var n = -1, r = null == e ? 0 : e.length; ++n < r && !1 !== t(e[n], n, e););
                     return e
                 }
             },
             36549: e => {
@@ -65893,14 +66053,22 @@
                 var r = n(42319);
                 e.exports = function(e, t) {
                     for (var n = e.length; n--;)
                         if (r(e[n][0], t)) return n;
                     return -1
                 }
             },
+            70199: (e, t, n) => {
+                var r = n(64811);
+                e.exports = function(e, t, n, o) {
+                    return r(e, (function(e, r, i) {
+                        t(o, e, n(e), i)
+                    })), o
+                }
+            },
             49142: (e, t, n) => {
                 var r = n(52959),
                     o = n(46876);
                 e.exports = function(e, t) {
                     return e && r(t, o(t), e)
                 }
             },
@@ -66688,14 +66856,27 @@
                     return r(e, o(e), t)
                 }
             },
             96137: (e, t, n) => {
                 var r = n(19661)["__core-js_shared__"];
                 e.exports = r
             },
+            98718: (e, t, n) => {
+                var r = n(29916),
+                    o = n(70199),
+                    i = n(48603),
+                    a = n(12697);
+                e.exports = function(e, t) {
+                    return function(n, s) {
+                        var l = a(n) ? r : o,
+                            c = t ? t() : {};
+                        return l(n, e, i(s, 2), c)
+                    }
+                }
+            },
             80693: (e, t, n) => {
                 var r = n(26724),
                     o = n(18621);
                 e.exports = function(e) {
                     return r((function(t, n) {
                         var r = -1,
                             i = n.length,
@@ -67821,14 +68002,23 @@
             36031: (e, t, n) => {
                 var r = n(30120);
                 e.exports = function(e, t, n) {
                     var o = null == e ? void 0 : r(e, t);
                     return void 0 === o ? n : o
                 }
             },
+            76236: (e, t, n) => {
+                var r = n(45742),
+                    o = n(98718),
+                    i = Object.prototype.hasOwnProperty,
+                    a = o((function(e, t, n) {
+                        i.call(e, n) ? e[n].push(t) : r(e, n, [t])
+                    }));
+                e.exports = a
+            },
             57100: (e, t, n) => {
                 var r = n(38170),
                     o = n(98869);
                 e.exports = function(e, t) {
                     return null != e && o(e, t, r)
                 }
             },
@@ -116092,43 +116282,43 @@
         4132: "49bf3f2c",
         4177: "69f9f18d",
         4319: "bf1c86bf",
         4477: "1bd49702",
         4500: "b6f348d1",
         4666: "c4b22a63",
         5106: "44f0ff51",
-        5117: "04bfe5d3",
         5249: "f2f4070d",
         5345: "73d26e5d",
         5379: "f08eddd1",
         5441: "1b94928f",
         5791: "9a42fb4b",
         6013: "4ba2d616",
         6405: "ac5a6f23",
         6718: "802da17e",
         6853: "93dd1c4c",
-        6950: "70fe55c2",
         7142: "83028745",
         7175: "583ff733",
         7323: "b74cc85b",
         7483: "64f23be7",
         7602: "e8abc06b",
         7805: "acc6316a",
         8005: "43974a35",
         8148: "293984e0",
         8427: "bd0a7cf3",
         8477: "de889fe5",
         8492: "0d93bd08",
         8536: "f8de3d9a",
         8570: "6de19120",
+        8571: "cfc22b99",
         8691: "4211c305",
         9330: "2b4c99e0",
         9336: "3e046ad7",
         9656: "8c935274",
-        9865: "fd93213d"
+        9865: "fd93213d",
+        9945: "47d54f35"
     } [e] + ".chunk.js", __webpack_require__.miniCssF = e => "static/css/" + e + "." + {
         3466: "8b8f33d6",
         5441: "e3b876c5",
         8148: "49dfd2ce"
     } [e] + ".chunk.css", __webpack_require__.g = function() {
         if ("object" === typeof globalThis) return globalThis;
         try {
@@ -117028,16 +117218,16 @@
         });
         var Ue = __webpack_require__(66694),
             Ve = __webpack_require__(91191),
             He = __webpack_require__(63765),
             Xe = __webpack_require__(50641);
         const Ge = "NO_SCRIPT_RUN_ID";
         class $e {
-            constructor(e, t, n, r) {
-                this.element = void 0, this.metadata = void 0, this.scriptRunId = void 0, this.fragmentId = void 0, this.lazyQuiverElement = void 0, this.lazyVegaLiteChartElement = void 0, this.element = e, this.metadata = t, this.scriptRunId = n, this.fragmentId = r
+            constructor(e, t, n, r, o) {
+                this.element = void 0, this.metadata = void 0, this.scriptRunId = void 0, this.fragmentId = void 0, this.lazyQuiverElement = void 0, this.lazyVegaLiteChartElement = void 0, this.activeScriptHash = void 0, this.element = e, this.metadata = t, this.scriptRunId = n, this.activeScriptHash = r, this.fragmentId = o
             }
             get quiverElement() {
                 if (void 0 !== this.lazyQuiverElement) return this.lazyQuiverElement;
                 if ("arrowTable" !== this.element.type && "arrowDataFrame" !== this.element.type) throw new Error("elementType '".concat(this.element.type, "' is not a valid Quiver element!"));
                 const e = new Ve.fu(this.element[this.element.type]);
                 return this.lazyQuiverElement = e, e
             }
@@ -117063,23 +117253,26 @@
                 };
                 return this.lazyVegaLiteChartElement = r, r
             }
             getIn() {}
             setIn() {
                 throw new Error("'setIn' cannot be called on an ElementNode")
             }
+            filterMainScriptElements(e) {
+                if (this.activeScriptHash === e) return this
+            }
             clearStaleNodes(e, t, n) {
                 return !t || !t.length || this.fragmentId && t.includes(this.fragmentId) && this.fragmentId == n ? this.scriptRunId === e ? this : void 0 : this
             }
             getElements(e) {
                 return null == e && (e = new Set), e.add(this.element), e
             }
             arrowAddRows(e, t) {
                 const n = this.element.type,
-                    r = new $e(this.element, this.metadata, t, this.fragmentId);
+                    r = new $e(this.element, this.metadata, t, this.activeScriptHash, this.fragmentId);
                 switch (n) {
                     case "arrowTable":
                     case "arrowDataFrame":
                         r.lazyQuiverElement = $e.quiverAddRowsHelper(this.quiverElement, e);
                         break;
                     case "arrowVegaLiteChart":
                         r.lazyVegaLiteChartElement = $e.vegaLiteChartAddRowsHelper(this.vegaLiteChartElement, e);
@@ -117103,80 +117296,87 @@
                         return e.find((e => e.hasName && e.name === t))
                     }(e.datasets, n);
                     t ? t.data = t.data.addRows(r) : e.data = e.data ? e.data.addRows(r) : r
                 }))
             }
         }
         class Ke {
-            constructor(e, t, n, r) {
-                this.children = void 0, this.deltaBlock = void 0, this.scriptRunId = void 0, this.fragmentId = void 0, this.children = null !== e && void 0 !== e ? e : [], this.deltaBlock = null !== t && void 0 !== t ? t : new je.gO({}), this.scriptRunId = null !== n && void 0 !== n ? n : Ge, this.fragmentId = r
+            constructor(e, t, n, r, o) {
+                this.children = void 0, this.deltaBlock = void 0, this.scriptRunId = void 0, this.fragmentId = void 0, this.activeScriptHash = void 0, this.activeScriptHash = e, this.children = null !== t && void 0 !== t ? t : [], this.deltaBlock = null !== n && void 0 !== n ? n : new je.gO({}), this.scriptRunId = null !== r && void 0 !== r ? r : Ge, this.fragmentId = o
             }
             get isEmpty() {
                 return 0 === this.children.length
             }
             getIn(e) {
                 if (0 === e.length) return;
                 const t = e[0];
                 return t < 0 || t >= this.children.length ? void 0 : 1 === e.length ? this.children[t] : this.children[t].getIn(e.slice(1))
             }
             setIn(e, t, n) {
                 if (0 === e.length) throw new Error("empty path!");
                 const r = e[0];
                 if (r < 0 || r > this.children.length) throw new Error("Bad 'setIn' index ".concat(r, " (should be between [0, ").concat(this.children.length, "])"));
                 const o = this.children.slice();
-                return 1 === e.length ? o[r] = t : o[r] = o[r].setIn(e.slice(1), t, n), new Ke(o, this.deltaBlock, n, this.fragmentId)
+                return 1 === e.length ? o[r] = t : o[r] = o[r].setIn(e.slice(1), t, n), new Ke(this.activeScriptHash, o, this.deltaBlock, n, this.fragmentId)
+            }
+            filterMainScriptElements(e) {
+                if (this.activeScriptHash !== e) return;
+                const t = this.children.map((t => t.filterMainScriptElements(e))).filter(Xe.Av);
+                return new Ke(this.activeScriptHash, t, this.deltaBlock, this.scriptRunId, this.fragmentId)
             }
             clearStaleNodes(e, t, n) {
                 if (t && t.length) {
                     if (this.fragmentId) {
                         if (!t.includes(this.fragmentId)) return this;
                         n = this.fragmentId
                     }
                 } else if (this.scriptRunId !== e) return;
                 const r = this.children.map((r => r.clearStaleNodes(e, t, n))).filter(Xe.Av);
-                return new Ke(r, this.deltaBlock, e, this.fragmentId)
+                return new Ke(this.activeScriptHash, r, this.deltaBlock, e, this.fragmentId)
             }
             getElements(e) {
                 null == e && (e = new Set);
                 for (const t of this.children) t.getElements(e);
                 return e
             }
         }
         class Ye {
             static empty() {
-                let e = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0],
-                    t = arguments.length > 1 ? arguments[1] : void 0;
-                const n = [];
-                let r;
+                let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "",
+                    t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1],
+                    n = arguments.length > 2 ? arguments[2] : void 0;
+                const r = [];
+                let o;
                 switch ((0, Xe.WK)()) {
                     case Xe.io.NONE:
                         break;
                     case Xe.io.V1:
-                        e && (r = (0, Xe.fg)("Please wait..."));
+                        t && (o = (0, Xe.fg)("Please wait..."));
                         break;
                     default:
-                        r = (0, Xe.MO)()
+                        o = (0, Xe.MO)()
                 }
-                r && n.push(new $e(r, je.BN.create({}), Ge));
-                const o = new Ke(n, new je.gO({
+                o && r.push(new $e(o, je.BN.create({}), Ge, e));
+                const i = new Ke(e, r, new je.gO({
                         allowEmpty: !0
                     }), Ge),
-                    i = t || new Ke([], new je.gO({
+                    a = n || new Ke(e, [], new je.gO({
                         allowEmpty: !0
                     }), Ge),
-                    a = new Ke([], new je.gO({
+                    s = new Ke(e, [], new je.gO({
                         allowEmpty: !0
                     }), Ge),
-                    s = new Ke([], new je.gO({
+                    l = new Ke(e, [], new je.gO({
                         allowEmpty: !0
                     }), Ge);
-                return new Ye(new Ke([o, i, a, s]))
+                return new Ye(e, new Ke(e, [i, a, s, l]), null)
             }
-            constructor(e) {
-                if (this.root = void 0, this.root = e, 4 !== this.root.children.length || null == this.main || null == this.sidebar || null == this.event || null == this.bottom) throw new Error("Invalid root node children! ".concat(e))
+            constructor(e, t) {
+                let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
+                if (this.root = void 0, this.mainScriptHash = void 0, this.appLogo = void 0, this.mainScriptHash = e, this.root = t, this.appLogo = n, 4 !== this.root.children.length || null == this.main || null == this.sidebar || null == this.event || null == this.bottom) throw new Error("Invalid root node children! ".concat(t))
             }
             get main() {
                 const [e] = this.root.children;
                 return e
             }
             get sidebar() {
                 const [, e] = this.root.children;
@@ -117186,64 +117386,90 @@
                 const [, , e] = this.root.children;
                 return e
             }
             get bottom() {
                 const [, , , e] = this.root.children;
                 return e
             }
+            get logo() {
+                var e, t;
+                return null !== (e = null === (t = this.appLogo) || void 0 === t ? void 0 : t.logo) && void 0 !== e ? e : null
+            }
+            appRootWithLogo(e, t) {
+                const {
+                    activeScriptHash: n
+                } = t;
+                return new Ye(this.mainScriptHash, this.root, {
+                    logo: e,
+                    activeScriptHash: n
+                })
+            }
             applyDelta(e, t, n) {
                 const {
-                    deltaPath: r
+                    deltaPath: r,
+                    activeScriptHash: o
                 } = n;
                 switch (t.type) {
                     case "newElement": {
-                        const o = t.newElement;
-                        return this.addElement(r, e, o, n, t.fragmentId)
+                        const i = t.newElement;
+                        return this.addElement(r, e, i, n, o, t.fragmentId)
                     }
                     case "addBlock":
-                        return this.addBlock(r, t.addBlock, e, t.fragmentId);
+                        return this.addBlock(r, t.addBlock, e, o, t.fragmentId);
                     case "arrowAddRows":
                         try {
                             return this.arrowAddRows(r, t.arrowAddRows, e)
-                        } catch (o) {
-                            const t = (0, Xe.sZ)((0, He.b)(o).message);
-                            return this.addElement(r, e, t, n)
+                        } catch (i) {
+                            const t = (0, Xe.sZ)((0, He.b)(i).message);
+                            return this.addElement(r, e, t, n, o)
                         }
                     default:
                         throw new Error("Unrecognized deltaType: '".concat(t.type, "'"))
                 }
             }
+            filterMainScriptElements(e) {
+                var t;
+                const n = this.main.scriptRunId,
+                    r = this.main.filterMainScriptElements(e) || new Ke(e),
+                    o = this.sidebar.filterMainScriptElements(e) || new Ke(e),
+                    i = this.event.filterMainScriptElements(e) || new Ke(e),
+                    a = this.bottom.filterMainScriptElements(e) || new Ke(e),
+                    s = (null === (t = this.appLogo) || void 0 === t ? void 0 : t.activeScriptHash) === e ? this.appLogo : null;
+                return new Ye(e, new Ke(e, [r, o, i, a], new je.gO({
+                    allowEmpty: !0
+                }), n), s)
+            }
             clearStaleNodes(e, t) {
-                const n = this.main.clearStaleNodes(e, t) || new Ke,
-                    r = this.sidebar.clearStaleNodes(e, t) || new Ke,
-                    o = this.event.clearStaleNodes(e, t) || new Ke,
-                    i = this.bottom.clearStaleNodes(e, t) || new Ke;
-                return new Ye(new Ke([n, r, o, i], new je.gO({
+                const n = this.main.clearStaleNodes(e, t) || new Ke(this.mainScriptHash),
+                    r = this.sidebar.clearStaleNodes(e, t) || new Ke(this.mainScriptHash),
+                    o = this.event.clearStaleNodes(e, t) || new Ke(this.mainScriptHash),
+                    i = this.bottom.clearStaleNodes(e, t) || new Ke(this.mainScriptHash);
+                return new Ye(this.mainScriptHash, new Ke(this.mainScriptHash, [n, r, o, i], new je.gO({
                     allowEmpty: !0
-                }), e))
+                }), e), this.appLogo)
             }
             getElements() {
                 const e = new Set;
                 return this.main.getElements(e), this.sidebar.getElements(e), this.event.getElements(e), this.bottom.getElements(e), e
             }
-            addElement(e, t, n, r, o) {
-                const i = new $e(n, r, t, o);
-                return new Ye(this.root.setIn(e, i, t))
-            }
-            addBlock(e, t, n, r) {
-                const o = this.root.getIn(e),
-                    i = o instanceof Ke ? o.children : [],
-                    a = new Ke(i, t, n, r);
-                return new Ye(this.root.setIn(e, a, n))
+            addElement(e, t, n, r, o, i) {
+                const a = new $e(n, r, t, o, i);
+                return new Ye(this.mainScriptHash, this.root.setIn(e, a, t), this.appLogo)
+            }
+            addBlock(e, t, n, r, o) {
+                const i = this.root.getIn(e),
+                    a = i instanceof Ke ? i.children : [],
+                    s = new Ke(r, a, t, n, o);
+                return new Ye(this.mainScriptHash, this.root.setIn(e, s, n), this.appLogo)
             }
             arrowAddRows(e, t, n) {
                 const r = this.root.getIn(e);
                 if (null == r) throw new Error("Can't arrowAddRows: invalid deltaPath: ".concat(e));
                 const o = r.arrowAddRows(t, n);
-                return new Ye(this.root.setIn(e, o, n))
+                return new Ye(this.mainScriptHash, this.root.setIn(e, o, n), this.appLogo)
             }
         }
         var Ze = __webpack_require__(36989),
             Je = __webpack_require__(59033);
         let Qe;
         ! function(e) {
             e.NOT_RUNNING = "notRunning", e.RUNNING = "running", e.RERUN_REQUESTED = "rerunRequested", e.STOP_REQUESTED = "stopRequested", e.COMPILATION_ERROR = "compilationError"
@@ -121139,15 +121365,15 @@
                         overflow: "auto"
                     }
                 }
             }), ""),
             Ii = n.lazy((() => __webpack_require__.e(9330).then(__webpack_require__.bind(__webpack_require__, 69330)))),
             Pi = n.lazy((() => __webpack_require__.e(2736).then(__webpack_require__.bind(__webpack_require__, 62736)))),
             Di = n.lazy((() => __webpack_require__.e(3301).then(__webpack_require__.bind(__webpack_require__, 69436)))),
-            Bi = n.lazy((() => Promise.all([__webpack_require__.e(6950), __webpack_require__.e(8148)]).then(__webpack_require__.bind(__webpack_require__, 75064)))),
+            Bi = n.lazy((() => Promise.all([__webpack_require__.e(9945), __webpack_require__.e(8148)]).then(__webpack_require__.bind(__webpack_require__, 75064)))),
             ji = n.lazy((() => Promise.all([__webpack_require__.e(2178), __webpack_require__.e(7483), __webpack_require__.e(5441)]).then(__webpack_require__.bind(__webpack_require__, 5441)))),
             Fi = n.lazy((() => __webpack_require__.e(8427).then(__webpack_require__.bind(__webpack_require__, 18427)))),
             Ui = Pr(n.lazy((() => __webpack_require__.e(7323).then(__webpack_require__.bind(__webpack_require__, 47323)))), 100),
             Vi = n.lazy((() => Promise.all([__webpack_require__.e(2178), __webpack_require__.e(3466), __webpack_require__.e(8536)]).then(__webpack_require__.bind(__webpack_require__, 72394)))),
             Hi = n.lazy((() => Promise.all([__webpack_require__.e(5249), __webpack_require__.e(7805)]).then(__webpack_require__.bind(__webpack_require__, 32508)))),
             Xi = n.lazy((() => __webpack_require__.e(4500).then(__webpack_require__.bind(__webpack_require__, 54500)))),
             Gi = n.lazy((() => __webpack_require__.e(1307).then(__webpack_require__.bind(__webpack_require__, 51307)))),
@@ -121165,15 +121391,15 @@
             ia = n.lazy((() => Promise.all([__webpack_require__.e(937), __webpack_require__.e(2634)]).then(__webpack_require__.bind(__webpack_require__, 72634)))),
             aa = n.lazy((() => __webpack_require__.e(1074).then(__webpack_require__.bind(__webpack_require__, 91074)))),
             sa = n.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(8477)]).then(__webpack_require__.bind(__webpack_require__, 58477)))),
             la = n.lazy((() => __webpack_require__.e(6853).then(__webpack_require__.bind(__webpack_require__, 76853)))),
             ca = n.lazy((() => __webpack_require__.e(4477).then(__webpack_require__.bind(__webpack_require__, 74477)))),
             ua = n.lazy((() => __webpack_require__.e(4319).then(__webpack_require__.bind(__webpack_require__, 47618)))),
             pa = n.lazy((() => Promise.all([__webpack_require__.e(2187), __webpack_require__.e(5106)]).then(__webpack_require__.bind(__webpack_require__, 5106)))),
-            da = n.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(5117), __webpack_require__.e(4666)]).then(__webpack_require__.bind(__webpack_require__, 14666)))),
+            da = n.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(8571), __webpack_require__.e(4666)]).then(__webpack_require__.bind(__webpack_require__, 14666)))),
             ba = n.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(5379)]).then(__webpack_require__.bind(__webpack_require__, 35379)))),
             fa = n.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(8691)]).then(__webpack_require__.bind(__webpack_require__, 58691)))),
             ha = n.lazy((() => Promise.all([__webpack_require__.e(7142), __webpack_require__.e(6718)]).then(__webpack_require__.bind(__webpack_require__, 36718)))),
             ma = n.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(1479), __webpack_require__.e(7175)]).then(__webpack_require__.bind(__webpack_require__, 67175)))),
             Ma = n.lazy((() => Promise.resolve().then(__webpack_require__.bind(__webpack_require__, 88112))));
 
         function Oa(e, t) {
@@ -121762,21 +121988,21 @@
                 theme: n || _a.t,
                 children: (0, ze.jsx)(_e.a, {
                     theme: t,
                     children: r
                 })
             })
         };
-        var Ra, Ta = __webpack_require__(14609),
-            ka = __webpack_require__(20545),
-            Ca = __webpack_require__(17330),
-            Wa = __webpack_require__(35365),
-            Na = __webpack_require__(50669);
-        const La = (0, et.Z)("section", {
-                target: "eczjsme16"
+        var Ra = __webpack_require__(14609),
+            Ta = __webpack_require__(30351),
+            ka = __webpack_require__(17330),
+            Ca = __webpack_require__(35365),
+            Wa = __webpack_require__(16167);
+        const Na = (0, et.Z)("section", {
+                target: "eczjsme18"
             })((e => {
                 let {
                     theme: t,
                     isCollapsed: n,
                     adjustTop: r,
                     sidebarWidth: o
                 } = e;
@@ -121801,187 +122027,138 @@
                         display: n ? "none" : "initial",
                         height: "auto !important",
                         maxHeight: "99%",
                         boxShadow: "none"
                     }
                 }
             }), ""),
-            Ia = (0, et.Z)("div", {
-                target: "eczjsme15"
+            La = (0, et.Z)("div", {
+                target: "eczjsme17"
             })((() => ({
                 position: "relative"
             })), ""),
-            Pa = (0, et.Z)("ul", {
-                target: "eczjsme14"
+            Ia = (0, et.Z)("ul", {
+                target: "eczjsme16"
             })((e => {
                 let {
                     isExpanded: t,
-                    isOverflowing: n,
-                    hasSidebarElements: r,
-                    theme: o
+                    hasSidebarElements: n
                 } = e;
                 return {
-                    maxHeight: r ? t ? "75vh" : "33vh" : "100vh",
+                    maxHeight: t ? "none" : "30vh",
                     listStyle: "none",
-                    overflow: ["auto", "overlay"],
+                    overflow: t && n ? ["auto", "overlay"] : "hidden",
                     margin: 0,
-                    paddingTop: o.spacing.lg,
-                    paddingBottom: o.spacing.lg,
-                    "@media print": {
-                        paddingTop: o.spacing.threeXL
-                    },
-                    "&::before": n ? {
-                        content: '" "',
-                        backgroundImage: "linear-gradient(0deg, transparent, ".concat(o.colors.bgColor, ")"),
-                        width: "100%",
-                        height: "2rem",
-                        position: "absolute",
-                        top: 0,
-                        left: 0,
-                        right: 0,
-                        pointerEvents: "none"
-                    } : null,
-                    "&::after": n ? {
-                        content: '" "',
-                        backgroundImage: "linear-gradient(0deg, ".concat(o.colors.bgColor, ", transparent)"),
-                        height: "2rem",
-                        position: "absolute",
-                        bottom: 0,
-                        left: 0,
-                        right: 0,
-                        pointerEvents: "none"
-                    } : null
-                }
-            }), ""),
-            Da = (0, ge.F4)(Ra || (Ra = (0, Na.Z)(["\n  from, to {\n    transform: translateY(0);\n  }\n\n  50% {\n    transform: translateY(-0.25rem);\n  }\n"]))),
-            Ba = (0, et.Z)("div", {
-                target: "eczjsme13"
-            })((e => {
-                let {
-                    isExpanded: t,
-                    isOverflowing: n,
-                    theme: r
-                } = e;
-                return {
-                    cursor: t || n ? "pointer" : "default",
-                    position: "absolute",
-                    height: r.spacing.lg,
-                    left: 0,
-                    right: 0,
-                    bottom: 0,
-                    display: "flex",
-                    alignItems: "center",
-                    justifyContent: "center",
-                    color: r.colors.fadedText60,
-                    borderBottom: "1px solid ".concat(r.colors.fadedText10),
-                    transition: "color 500ms",
-                    ...(t || n) && {
-                        "&:hover": {
-                            color: r.colors.bodyText,
-                            background: "linear-gradient(0deg, ".concat(r.colors.darkenedBgMix15, ", transparent)"),
-                            "& > *": {
-                                animation: "".concat(Da, " 0.5s ease infinite")
-                            }
-                        }
-                    }
+                    paddingBottom: "0.125rem"
                 }
             }), ""),
-            ja = (0, et.Z)("div", {
-                target: "eczjsme12"
+            Pa = (0, et.Z)("div", {
+                target: "eczjsme15"
             })((() => ({
                 display: "flex",
                 flexDirection: "column"
             })), ""),
-            Fa = (0, et.Z)("a", {
-                target: "eczjsme11"
+            Da = (0, et.Z)("a", {
+                target: "eczjsme14"
             })((e => {
                 let {
                     isActive: t,
                     theme: n
                 } = e;
-                const r = {
-                    textDecoration: "none",
-                    fontWeight: t ? 600 : 400
-                };
+                const r = (0, Ae.Iy)(n),
+                    o = r ? n.colors.gray90 : n.colors.gray10,
+                    i = r ? n.colors.gray60 : n.colors.gray70,
+                    a = r ? n.colors.darkenedBgMix15 : (0, xe.DZ)(n.colors.gray100, .6),
+                    s = {
+                        textDecoration: "none",
+                        fontWeight: t ? 600 : 400
+                    };
                 return {
-                    ...r,
+                    ...s,
                     display: "flex",
                     flexDirection: "row",
                     alignItems: "center",
                     gap: n.spacing.sm,
                     borderRadius: n.spacing.twoXS,
                     paddingLeft: n.spacing.sm,
                     paddingRight: n.spacing.sm,
-                    marginLeft: n.spacing.lg,
-                    marginRight: n.spacing.lg,
+                    marginLeft: n.spacing.twoXL,
+                    marginRight: n.spacing.twoXL,
                     marginTop: n.spacing.threeXS,
                     marginBottom: n.spacing.threeXS,
                     lineHeight: n.lineHeights.menuItem,
-                    backgroundColor: t ? n.colors.darkenedBgMix15 : "transparent",
+                    color: r ? n.colors.gray80 : n.colors.gray40,
+                    backgroundColor: t ? a : "transparent",
+                    [Wa.m]: {
+                        color: t ? o : i,
+                        fontWeight: t ? 600 : 400
+                    },
                     "&:hover": {
-                        backgroundColor: t ? n.colors.darkenedBgMix25 : n.colors.darkenedBgMix15
+                        backgroundColor: a
                     },
                     "&:active,&:visited,&:hover": {
-                        ...r
+                        ...s
                     },
                     "&:focus": {
                         outline: "none"
                     },
                     "&:focus-visible": {
                         backgroundColor: n.colors.darkenedBgMix15
                     },
                     "@media print": {
                         paddingLeft: n.spacing.none
                     }
                 }
             }), ""),
-            Ua = (0, et.Z)("span", {
-                target: "eczjsme10"
+            Ba = (0, et.Z)("span", {
+                target: "eczjsme13"
             })((e => {
                 let {
                     isActive: t,
                     theme: n
                 } = e;
+                const r = (0, Ae.Iy)(n),
+                    o = r ? n.colors.gray80 : n.colors.gray50,
+                    i = r ? n.colors.gray90 : n.colors.gray10;
                 return {
-                    color: t ? n.colors.bodyText : n.colors.fadedText60,
+                    color: t ? i : o,
                     overflow: "hidden",
                     whiteSpace: "nowrap",
                     textOverflow: "ellipsis",
                     display: "table-cell"
                 }
             }), ""),
-            Va = (0, et.Z)("div", {
-                target: "eczjsme9"
+            ja = (0, et.Z)("div", {
+                target: "eczjsme12"
             })((e => {
                 let {
-                    theme: t
+                    hasPageNavAbove: t,
+                    theme: n
                 } = e;
                 return {
-                    paddingTop: t.spacing.lg,
-                    paddingBottom: t.sizes.sidebarTopSpace,
-                    paddingLeft: t.spacing.twoXL,
-                    paddingRight: t.spacing.twoXL,
-                    ...(0, Ae.XE)(t)
+                    paddingTop: t ? n.spacing.twoXL : 0,
+                    paddingBottom: n.sizes.sidebarTopSpace,
+                    paddingLeft: n.spacing.twoXL,
+                    paddingRight: n.spacing.twoXL,
+                    ...(0, Ae.XE)(n)
                 }
             }), ""),
-            Ha = (0, et.Z)("div", {
-                target: "eczjsme8"
+            Fa = (0, et.Z)("div", {
+                target: "eczjsme11"
             })((e => {
-                let {
-                    hideScrollbar: t
-                } = e;
+                let {} = e;
                 return {
                     position: "relative",
                     height: "100%",
                     width: "100%",
-                    overflow: t ? "hidden" : ["auto", "overlay"]
+                    overflow: ["auto", "overlay"]
                 }
             }), ""),
-            Xa = (0, et.Z)("div", {
-                target: "eczjsme7"
+            Ua = (0, et.Z)("div", {
+                target: "eczjsme10"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
                     width: "8px",
@@ -121989,60 +122166,60 @@
                     cursor: "col-resize",
                     zIndex: t.zIndices.sidebarMobile,
                     "&:hover": {
                         backgroundImage: "linear-gradient(to right, transparent 20%, ".concat(t.colors.fadedText20, " 28%, transparent 36%)")
                     }
                 }
             }), ""),
-            Ga = (0, et.Z)("div", {
-                target: "eczjsme6"
+            Va = (0, et.Z)("div", {
+                target: "eczjsme9"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "start",
                     padding: "".concat(t.spacing.xl, " ").concat(t.spacing.twoXL, " ").concat(t.spacing.twoXL, " ").concat(t.spacing.twoXL)
                 }
             }), ""),
-            $a = (0, et.Z)("a", {
-                target: "eczjsme5"
+            Ha = (0, et.Z)("a", {
+                target: "eczjsme8"
             })((e => {
                 let {} = e;
                 return {
                     "&:hover": {
                         opacity: "0.7"
                     }
                 }
             }), ""),
-            Ka = (0, et.Z)("img", {
-                target: "eczjsme4"
+            Xa = (0, et.Z)("img", {
+                target: "eczjsme7"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     height: "1.5rem",
                     maxWidth: "15rem",
                     margin: "0.25rem 0.5rem 0.25rem 0",
                     zIndex: t.zIndices.header
                 }
             }), ""),
-            Ya = (0, et.Z)("div", {
-                target: "eczjsme3"
+            Ga = (0, et.Z)("div", {
+                target: "eczjsme6"
             })((e => {
                 let {} = e;
                 return {
                     height: "2.0rem"
                 }
             }), ""),
-            Za = (0, et.Z)("div", {
-                target: "eczjsme2"
+            $a = (0, et.Z)("div", {
+                target: "eczjsme5"
             })((e => {
                 let {
                     theme: t,
                     chevronDownshift: n,
                     isCollapsed: r
                 } = e;
                 return {
@@ -122056,16 +122233,16 @@
                     transition: "left 300ms",
                     transitionDelay: "left 300ms",
                     "@media print": {
                         position: "static"
                     }
                 }
             }), ""),
-            Ja = (0, et.Z)("div", {
-                target: "eczjsme1"
+            Ka = (0, et.Z)("div", {
+                target: "eczjsme4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 const n = (0, Ae.Iy)(t);
                 return {
                     zIndex: t.zIndices.header,
@@ -122076,109 +122253,195 @@
                         }
                     },
                     "@media print": {
                         display: "none"
                     }
                 }
             }), ""),
-            Qa = (0, et.Z)("div", {
-                target: "eczjsme0"
+            Ya = (0, et.Z)("div", {
+                target: "eczjsme3"
             })((e => {
                 let {
-                    theme: t
+                    showSidebarCollapse: t,
+                    theme: n
                 } = e;
                 return {
-                    display: "auto",
+                    display: t ? "inline" : "none",
                     transition: "left 300ms",
                     transitionDelay: "left 300ms",
-                    color: (0, Ae.Iy)(t) ? t.colors.gray70 : t.colors.bodyText,
+                    color: (0, Ae.Iy)(n) ? n.colors.gray70 : n.colors.bodyText,
                     lineHeight: "0",
-                    button: {
-                        padding: "0.25rem",
-                        "&:hover": {
-                            backgroundColor: t.colors.darkenedBgMix25
-                        }
-                    },
                     "@media print": {
                         display: "none"
+                    },
+                    ["@media (max-width: ".concat(n.breakpoints.sm, ")")]: {
+                        display: "inline"
                     }
                 }
+            }), ""),
+            Za = (0, et.Z)("header", {
+                target: "eczjsme2"
+            })((e => {
+                let {
+                    theme: t
+                } = e;
+                const n = (0, Ae.Iy)(t);
+                return {
+                    fontSize: t.fontSizes.sm,
+                    fontWeight: t.fontWeights.bold,
+                    color: n ? t.colors.gray80 : t.colors.gray60,
+                    lineHeight: t.lineHeights.table,
+                    paddingRight: t.spacing.sm,
+                    marginLeft: t.spacing.twoXL,
+                    marginRight: t.spacing.twoXL,
+                    marginTop: t.spacing.sm,
+                    marginBottom: t.spacing.twoXS
+                }
+            }), ""),
+            Ja = (0, et.Z)("button", {
+                target: "eczjsme1"
+            })((e => {
+                let {
+                    theme: t
+                } = e;
+                const n = (0, Ae.Iy)(t);
+                return {
+                    fontSize: t.fontSizes.sm,
+                    lineHeight: "1.4rem",
+                    color: n ? t.colors.gray90 : t.colors.gray10,
+                    backgroundColor: t.colors.transparent,
+                    border: "none",
+                    borderRadius: t.radii.lg,
+                    marginTop: t.spacing.twoXS,
+                    marginLeft: t.spacing.xl,
+                    padding: "".concat(t.spacing.threeXS, " ").concat(t.spacing.sm),
+                    "&:hover, &:active, &:focus": {
+                        border: "none",
+                        outline: "none",
+                        boxShadow: "none"
+                    },
+                    "&:hover": {
+                        backgroundColor: n ? t.colors.darkenedBgMix15 : (0, xe.DZ)(t.colors.gray100, .6)
+                    }
+                }
+            }), ""),
+            Qa = (0, et.Z)("div", {
+                target: "eczjsme0"
+            })((e => {
+                let {
+                    theme: t
+                } = e;
+                return {
+                    paddingTop: t.spacing.lg,
+                    borderBottom: "1px solid ".concat(t.colors.fadedText10)
+                }
             }), "");
-        var es = __webpack_require__(91706),
-            ts = __webpack_require__(88235);
-        const ns = e => {
-            let {
-                endpoints: t,
-                appPages: r,
-                collapseSidebar: o,
-                currentPageScriptHash: i,
-                hasSidebarElements: a,
-                hideParentScrollbar: s,
-                onPageChange: l
-            } = e;
-            const {
-                pageLinkBaseUrl: c
-            } = n.useContext(Fe), [u, p] = (0, n.useState)(!1), d = (0, n.useRef)(null), b = (0, ts.d)(d, u), f = (0, n.useCallback)((() => {
-                b && s(!0)
-            }), [b, s]), h = (0, n.useCallback)((() => s(!1)), [s]), m = (0, n.useCallback)((() => {
-                !u && b ? p(!0) : u && p(!1)
-            }), [u, b]);
-            return r.length < 2 ? null : (0, ze.jsxs)(Ia, {
-                "data-testid": "stSidebarNav",
-                children: [(0, ze.jsx)(Pa, {
-                    ref: d,
-                    isExpanded: u,
-                    isOverflowing: b,
+        var es = __webpack_require__(76236),
+            ts = __webpack_require__.n(es),
+            ns = __webpack_require__(91706),
+            rs = __webpack_require__(88235);
+        const os = e => {
+                let {
+                    header: t = "",
+                    children: n
+                } = e;
+                return (0, ze.jsxs)(ze.Fragment, {
+                    children: [t && (0, ze.jsx)(Za, {
+                        children: t
+                    }), n]
+                })
+            },
+            is = e => {
+                let {
+                    isActive: t,
+                    pageUrl: n,
+                    icon: r,
+                    onClick: o,
+                    children: i
+                } = e;
+                return (0, ze.jsx)(Pa, {
+                    children: (0, ze.jsxs)(Da, {
+                        "data-testid": "stSidebarNavLink",
+                        isActive: t,
+                        href: n,
+                        onClick: o,
+                        children: [r && r.length && (0, ze.jsx)(Mn.p, {
+                            size: "md",
+                            iconValue: r
+                        }), (0, ze.jsx)(Ba, {
+                            isActive: t,
+                            children: i
+                        })]
+                    })
+                })
+            },
+            as = e => {
+                let {
+                    endpoints: t,
+                    appPages: r,
+                    collapseSidebar: o,
+                    currentPageScriptHash: i,
                     hasSidebarElements: a,
-                    onMouseOver: f,
-                    onMouseOut: h,
-                    "data-testid": "stSidebarNavItems",
-                    children: r.map(((e, n) => {
-                        const r = t.buildAppPageURL(c, e, n),
-                            a = e.pageName,
-                            s = a.replace(/_/g, " "),
-                            u = e.pageScriptHash === i;
-                        return (0, ze.jsx)("li", {
-                            children: (0, ze.jsx)(ja, {
-                                children: (0, ze.jsxs)(Fa, {
-                                    "data-testid": "stSidebarNavLink",
-                                    isActive: u,
-                                    href: r,
-                                    onClick: t => {
-                                        t.preventDefault(), l(e.pageScriptHash), es.tq && o()
-                                    },
-                                    children: [e.icon && e.icon.length && (0, ze.jsx)(mn.S, {
-                                        size: "lg",
-                                        children: e.icon
-                                    }), (0, ze.jsx)(Ua, {
-                                        isActive: u,
-                                        children: s
-                                    })]
-                                })
-                            })
-                        }, a)
+                    navSections: s,
+                    onPageChange: l
+                } = e;
+                const [c, u] = (0, n.useState)(!1), p = (0, n.useRef)(null), d = (0, rs.d)(p, c), {
+                    pageLinkBaseUrl: b
+                } = (0, n.useContext)(Fe), f = (0, n.useCallback)((() => {
+                    u(!c)
+                }), [c]), h = (0, n.useCallback)((e => {
+                    const n = t.buildAppPageURL(b, e),
+                        r = e.pageName,
+                        a = r.replace(/_/g, " "),
+                        s = e.pageScriptHash === i;
+                    return (0, ze.jsx)("li", {
+                        children: (0, ze.jsx)(is, {
+                            isActive: s,
+                            pageUrl: n,
+                            icon: e.icon,
+                            onClick: t => {
+                                t.preventDefault(), l(e.pageScriptHash), ns.tq && o()
+                            },
+                            children: a
+                        })
+                    }, r)
+                }), [o, i, t, l, b]);
+                let m = null;
+                if (s.length > 0) {
+                    const e = ts()(r, (e => e.sectionHeader || ""));
+                    m = s.map((t => {
+                        var n;
+                        return (0, ze.jsx)(os, {
+                            header: t,
+                            children: (null !== (n = e[t]) && void 0 !== n ? n : []).map(h)
+                        }, t)
                     }))
-                }), a && (0, ze.jsxs)(Ba, {
-                    "data-testid": "stSidebarNavSeparator",
-                    isExpanded: u,
-                    isOverflowing: b,
-                    onClick: m,
-                    children: [b && !u && (0, ze.jsx)(mn.Z, {
-                        content: rn,
-                        size: "md",
-                        testid: "stSidebarNavExpandIcon"
-                    }), u && (0, ze.jsx)(mn.Z, {
-                        content: nn,
-                        size: "md",
-                        testid: "stSidebarNavCollapseIcon"
+                } else m = r.map(h);
+                const M = !a || c,
+                    O = a && d || c;
+                return (0, ze.jsxs)(La, {
+                    "data-testid": "stSidebarNav",
+                    children: [(0, ze.jsx)(Ia, {
+                        ref: p,
+                        isExpanded: M,
+                        hasSidebarElements: a,
+                        "data-testid": "stSidebarNavItems",
+                        children: m
+                    }), a && (0, ze.jsxs)(ze.Fragment, {
+                        children: [O && (0, ze.jsx)(Ja, {
+                            onClick: f,
+                            "data-testid": "stSidebarNavViewButton",
+                            children: c ? "View less" : "View more"
+                        }), (0, ze.jsx)(Qa, {
+                            "data-testid": "stSidebarNavSeparator"
+                        })]
                     })]
-                })]
-            })
-        };
-        class rs extends n.PureComponent {
+                })
+            };
+        class ss extends n.PureComponent {
             static calculateMaxBreakpoint(e) {
                 return parseInt(e, 10) - .02
             }
             constructor(e) {
                 super(e), this.mediumBreakpointPx = void 0, this.sidebarRef = n.createRef(), this.handleClickOutside = e => {
                     if (this.sidebarRef && window) {
                         const {
@@ -122190,19 +122453,19 @@
                             collapsedSidebar: !0
                         })
                     }
                 }, this.setSidebarWidth = e => {
                     const t = e.toString();
                     this.setState({
                         sidebarWidth: t
-                    }), (0, Wa.V)() && window.localStorage.setItem("sidebarWidth", t)
+                    }), (0, Ca.V)() && window.localStorage.setItem("sidebarWidth", t)
                 }, this.resetSidebarWidth = e => {
                     2 === e.detail && (this.setState({
-                        sidebarWidth: rs.minWidth
-                    }), (0, Wa.V)() && window.localStorage.setItem("sidebarWidth", rs.minWidth))
+                        sidebarWidth: ss.minWidth
+                    }), (0, Ca.V)() && window.localStorage.setItem("sidebarWidth", ss.minWidth))
                 }, this.checkMobileOnResize = () => {
                     if (!window) return !1;
                     const {
                         innerWidth: e
                     } = window;
                     return e < this.state.lastInnerWidth && e <= this.mediumBreakpointPx && this.setState({
                         collapsedSidebar: !0
@@ -122212,30 +122475,34 @@
                 }, this.toggleCollapse = () => {
                     const {
                         collapsedSidebar: e
                     } = this.state;
                     this.setState({
                         collapsedSidebar: !e
                     })
-                }, this.hideScrollbar = e => {
+                }, this.onMouseOver = () => {
                     this.setState({
-                        hideScrollbar: e
+                        showSidebarCollapse: !0
                     })
-                }, this.mediumBreakpointPx = rs.calculateMaxBreakpoint(e.theme.breakpoints.md);
-                const t = (0, Wa.V)() ? localStorage.getItem("sidebarWidth") : void 0;
+                }, this.onMouseOut = () => {
+                    this.setState({
+                        showSidebarCollapse: !1
+                    })
+                }, this.mediumBreakpointPx = ss.calculateMaxBreakpoint(e.theme.breakpoints.md);
+                const t = (0, Ca.V)() ? localStorage.getItem("sidebarWidth") : void 0;
                 this.state = {
-                    collapsedSidebar: rs.shouldCollapse(e, this.mediumBreakpointPx),
-                    sidebarWidth: t || rs.minWidth,
+                    collapsedSidebar: ss.shouldCollapse(e, this.mediumBreakpointPx),
+                    sidebarWidth: t || ss.minWidth,
                     lastInnerWidth: window ? window.innerWidth : 1 / 0,
-                    hideScrollbar: !1
+                    showSidebarCollapse: !1
                 }
             }
             componentDidUpdate(e) {
-                this.mediumBreakpointPx = rs.calculateMaxBreakpoint(this.props.theme.breakpoints.md), this.props.initialSidebarState === e.initialSidebarState && this.props.hasElements === e.hasElements || this.setState({
-                    collapsedSidebar: rs.shouldCollapse(this.props, this.mediumBreakpointPx)
+                this.mediumBreakpointPx = ss.calculateMaxBreakpoint(this.props.theme.breakpoints.md), this.props.initialSidebarState === e.initialSidebarState && this.props.hasElements === e.hasElements || this.setState({
+                    collapsedSidebar: ss.shouldCollapse(this.props, this.mediumBreakpointPx)
                 })
             }
             static shouldCollapse(e, t) {
                 switch (e.initialSidebarState) {
                     case je.Pz.SidebarState.EXPANDED:
                         return !1;
                     case je.Pz.SidebarState.COLLAPSED:
@@ -122264,65 +122531,66 @@
                 }
                 return e
             }
             renderLogo(e) {
                 const {
                     appLogo: t
                 } = this.props;
-                if (!t) return (0, ze.jsx)(Ya, {
+                if (!t) return (0, ze.jsx)(Ga, {
                     "data-testid": "stLogoSpacer"
                 });
                 const n = e && t.iconImage ? t.iconImage : t.image,
                     r = this.props.endpoints.buildMediaURL(n);
-                return t.link ? (0, ze.jsx)($a, {
+                return t.link ? (0, ze.jsx)(Ha, {
                     href: t.link,
                     target: "_blank",
                     rel: "noreferrer",
                     "data-testid": "stLogoLink",
-                    children: (0, ze.jsx)(Ka, {
+                    children: (0, ze.jsx)(Xa, {
                         src: r,
                         alt: "Logo",
                         "data-testid": "stLogo"
                     })
-                }) : (0, ze.jsx)(Ka, {
+                }) : (0, ze.jsx)(Xa, {
                     src: r,
                     alt: "Logo",
                     "data-testid": "stLogo"
                 })
             }
             render() {
                 const {
                     collapsedSidebar: e,
                     sidebarWidth: t,
-                    hideScrollbar: n
+                    showSidebarCollapse: n
                 } = this.state, {
                     appPages: r,
                     chevronDownshift: o,
                     children: i,
                     hasElements: a,
                     onPageChange: s,
                     currentPageScriptHash: l,
-                    hideSidebarNav: c
-                } = this.props, u = !((0, Xe.P2)() && !(0, Xe.av)()) && this.headerDecorationVisible();
+                    hideSidebarNav: c,
+                    navSections: u
+                } = this.props, p = r.length > 1 && !c, d = !((0, Xe.P2)() && !(0, Xe.av)()) && this.headerDecorationVisible();
                 return (0, ze.jsxs)(ze.Fragment, {
-                    children: [e && (0, ze.jsxs)(Za, {
+                    children: [e && (0, ze.jsxs)($a, {
                         chevronDownshift: o,
                         isCollapsed: e,
                         "data-testid": "collapsedControl",
-                        children: [this.renderLogo(!0), (0, ze.jsx)(Ja, {
+                        children: [this.renderLogo(!0), (0, ze.jsx)(Ka, {
                             children: (0, ze.jsx)(sn.ZP, {
                                 kind: ln.nW.HEADER_NO_PADDING,
                                 onClick: this.toggleCollapse,
                                 children: (0, ze.jsx)(mn.Z, {
-                                    content: Ta._,
+                                    content: Ra._,
                                     size: "xl"
                                 })
                             })
                         })]
-                    }), (0, ze.jsx)(Ca.e, {
+                    }), (0, ze.jsx)(ka.e, {
                         "data-testid": "stSidebar",
                         "aria-expanded": !e,
                         enable: {
                             top: !1,
                             right: !0,
                             bottom: !1,
                             left: !1
@@ -122330,74 +122598,77 @@
                         handleStyles: {
                             right: {
                                 width: "8px",
                                 right: "-6px"
                             }
                         },
                         handleComponent: {
-                            right: (0, ze.jsx)(Xa, {
+                            right: (0, ze.jsx)(Ua, {
                                 onClick: this.resetSidebarWidth
                             })
                         },
                         size: {
                             width: t,
-                            height: u ? window.innerHeight - 2 : "100%"
+                            height: "auto"
                         },
-                        as: La,
+                        as: Na,
                         onResizeStop: (e, n, r, o) => {
                             const i = parseInt(t, 10) + o.width;
                             this.setSidebarWidth(i)
                         },
                         isCollapsed: e,
-                        adjustTop: u,
+                        adjustTop: d,
                         sidebarWidth: t,
-                        children: (0, ze.jsxs)(Ha, {
+                        children: (0, ze.jsxs)(Fa, {
                             "data-testid": "stSidebarContent",
-                            hideScrollbar: n,
                             ref: this.sidebarRef,
-                            children: [(0, ze.jsxs)(Ga, {
+                            onMouseOver: this.onMouseOver,
+                            onMouseOut: this.onMouseOut,
+                            children: [(0, ze.jsxs)(Va, {
                                 "data-testid": "stSidebarHeader",
-                                children: [this.renderLogo(!1), (0, ze.jsx)(Qa, {
+                                children: [this.renderLogo(!1), (0, ze.jsx)(Ya, {
+                                    showSidebarCollapse: n,
                                     "data-testid": "stSidebarCollapseButton",
                                     children: (0, ze.jsx)(sn.ZP, {
-                                        kind: ln.nW.HEADER_BUTTON,
+                                        kind: ln.nW.HEADER_NO_PADDING,
                                         onClick: this.toggleCollapse,
                                         children: (0, ze.jsx)(mn.Z, {
-                                            content: ka.x,
-                                            size: "lg"
+                                            content: Ta.s,
+                                            size: "xl"
                                         })
                                     })
                                 })]
-                            }), !c && (0, ze.jsx)(ns, {
+                            }), p && (0, ze.jsx)(as, {
                                 endpoints: this.props.endpoints,
                                 appPages: r,
                                 collapseSidebar: this.toggleCollapse,
                                 currentPageScriptHash: l,
+                                navSections: u,
                                 hasSidebarElements: a,
-                                hideParentScrollbar: this.hideScrollbar,
                                 onPageChange: s
-                            }), (0, ze.jsx)(Va, {
+                            }), (0, ze.jsx)(ja, {
+                                hasPageNavAbove: p,
                                 "data-testid": "stSidebarUserContent",
                                 children: i
                             })]
                         })
                     })]
                 })
             }
         }
-        rs.minWidth = "336";
-        const os = (0, _e.b)((function(e) {
+        ss.minWidth = "336";
+        const ls = (0, _e.b)((function(e) {
                 return (0, ze.jsx)(cn.Z.Provider, {
                     value: !0,
-                    children: (0, ze.jsx)(rs, {
+                    children: (0, ze.jsx)(ss, {
                         ...e
                     })
                 })
             })),
-            is = e => {
+            cs = e => {
                 let {
                     children: t,
                     ...r
                 } = e;
                 const {
                     sidebarChevronDownshift: o
                 } = n.useContext(Fe), {
@@ -122407,37 +122678,37 @@
                     backgroundColor: e.emotion.colors.secondaryBg,
                     bodyFont: e.emotion.genericFonts.bodyFont,
                     codeFont: e.emotion.genericFonts.codeFont
                 }, e, !0))(i);
                 return (0, ze.jsx)(xa, {
                     theme: a.emotion,
                     baseuiTheme: a.basewebTheme,
-                    children: (0, ze.jsx)(os, {
+                    children: (0, ze.jsx)(ls, {
                         ...r,
                         chevronDownshift: o,
                         children: t
                     })
                 })
             };
-        var as = __webpack_require__(69021),
-            ss = __webpack_require__(92775);
-        const ls = function(e) {
+        var us = __webpack_require__(69021),
+            ps = __webpack_require__(92775);
+        const ds = function(e) {
                 let {
                     scriptRunId: t,
                     children: r
                 } = e;
                 const {
                     sizes: o
                 } = (0, _e.u)();
                 return (0, n.useEffect)((() => {
                     var e;
-                    null === (e = as.Z.getRef()) || void 0 === e || e.clearAll()
+                    null === (e = us.Z.getRef()) || void 0 === e || e.clearAll()
                 }), [t]), (0, ze.jsxs)(ze.Fragment, {
-                    children: [(0, ze.jsx)(as.w, {
-                        placement: ss.r4.topRight,
+                    children: [(0, ze.jsx)(us.w, {
+                        placement: ps.r4.topRight,
                         autoHideDuration: 4e3,
                         overrides: {
                             Root: {
                                 style: {
                                     top: o.headerHeight,
                                     zIndex: 100
                                 },
@@ -122445,15 +122716,15 @@
                                     "data-testid": "toastContainer"
                                 }
                             }
                         }
                     }), r]
                 })
             },
-            cs = (0, et.Z)("div", {
+            bs = (0, et.Z)("div", {
                 target: "ea3mdgi9"
             })((() => ({
                 display: "flex",
                 flexDirection: "row",
                 justifyContent: "flex-start",
                 alignItems: "stretch",
                 alignContent: "flex-start",
@@ -122463,15 +122734,15 @@
                 right: 0,
                 bottom: 0,
                 overflow: "hidden",
                 "@media print": {
                     overflow: "visible"
                 }
             })), ""),
-            us = (0, et.Z)("section", {
+            fs = (0, et.Z)("section", {
                 target: "ea3mdgi8"
             })((e => {
                 let {
                     disableScrolling: t,
                     theme: n
                 } = e;
                 return {
@@ -122493,23 +122764,23 @@
                         }
                     },
                     "@media print": {
                         overflow: "visible"
                     }
                 }
             }), ""),
-            ps = (0, et.Z)("div", {
+            hs = (0, et.Z)("div", {
                 target: "ea3mdgi7"
             })((() => ({
                 position: "sticky",
                 left: 0,
                 bottom: 0,
                 width: "100%"
             })), ""),
-            ds = (0, et.Z)("div", {
+            ms = (0, et.Z)("div", {
                 target: "ea3mdgi6"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "relative",
@@ -122519,15 +122790,15 @@
                     backgroundColor: t.colors.bgColor,
                     display: "flex",
                     flexDirection: "column",
                     alignItems: "center",
                     zIndex: t.zIndices.bottom
                 }
             }), ""),
-            bs = (0, et.Z)("div", {
+            Ms = (0, et.Z)("div", {
                 target: "ea3mdgi5"
             })((e => {
                 let {
                     hasSidebar: t,
                     hasBottom: n,
                     isEmbedded: r,
                     isWideMode: o,
@@ -122560,30 +122831,30 @@
                     maxWidth: o ? "initial" : l.sizes.contentMaxWidth,
                     ...b,
                     "@media print": {
                         paddingTop: c
                     }
                 }
             }), ""),
-            fs = (0, et.Z)("div", {
+            Os = (0, et.Z)("div", {
                 target: "ea3mdgi4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full
                 }
             }), ""),
-            hs = (0, et.Z)("div", {
+            gs = (0, et.Z)("div", {
                 target: "ea3mdgi3"
             })((() => ({
                 display: "none"
             })), ""),
-            ms = (0, et.Z)("div", {
+            zs = (0, et.Z)("div", {
                 target: "ea3mdgi2"
             })((e => {
                 let {
                     isWideMode: t,
                     showPadding: n,
                     theme: r
                 } = e;
@@ -122601,239 +122872,241 @@
                     minWidth: t ? "auto" : void 0,
                     maxWidth: t ? "initial" : r.sizes.contentMaxWidth,
                     "@media print": {
                         paddingTop: 0
                     }
                 }
             }), ""),
-            Ms = (0, et.Z)("div", {
+            ys = (0, et.Z)("div", {
                 target: "ea3mdgi1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     flexGrow: 1
                 }
             }), ""),
-            Os = (0, et.Z)("div", {
+            As = (0, et.Z)("div", {
                 target: "ea3mdgi0"
             })((() => ({
                 position: "relative",
                 bottom: "0"
             })), "");
 
-        function gs(e) {
+        function vs(e) {
             const {
                 className: t,
                 tabIndex: n,
                 children: r,
                 isEmbedded: o,
                 disableScrolling: i
             } = e, a = kr();
-            return (0, ze.jsx)(us, {
+            return (0, ze.jsx)(fs, {
                 tabIndex: n,
                 className: t,
                 isEmbedded: o,
                 disableScrolling: i,
                 ref: a,
                 "data-testid": "ScrollToBottomContainer",
                 children: r
             })
         }
-        const zs = function(e) {
+        const ws = function(e) {
             const {
                 elements: t,
                 sessionInfo: r,
                 scriptRunId: o,
                 scriptRunState: i,
                 widgetMgr: a,
                 widgetsDisabled: s,
                 uploadClient: l,
                 componentRegistry: c,
                 formsData: u,
                 appLogo: p,
                 appPages: d,
-                onPageChange: b,
-                currentPageScriptHash: f,
-                hideSidebarNav: h,
-                sendMessageToHost: m,
-                endpoints: M
+                navSections: b,
+                onPageChange: f,
+                currentPageScriptHash: h,
+                hideSidebarNav: m,
+                sendMessageToHost: M,
+                endpoints: O
             } = e;
             n.useEffect((() => {
                 const e = () => {
-                    m({
+                    M({
                         type: "UPDATE_HASH",
                         hash: window.location.hash
                     })
                 };
                 return window.addEventListener("hashchange", e, !1), () => window.removeEventListener("hashchange", e, !1)
-            }), [m]);
+            }), [M]);
             const {
-                wideMode: O,
-                initialSidebarState: g,
-                embedded: z,
-                showPadding: y,
-                disableScrolling: A,
-                showToolbar: v,
-                showColoredLine: w,
-                sidebarChevronDownshift: S
+                wideMode: g,
+                initialSidebarState: z,
+                embedded: y,
+                showPadding: A,
+                disableScrolling: v,
+                showToolbar: w,
+                showColoredLine: S,
+                sidebarChevronDownshift: q
             } = n.useContext(Fe), {
-                addScriptFinishedHandler: q,
-                removeScriptFinishedHandler: E,
-                libConfig: _
-            } = n.useContext(Ue.E), x = O ? "wide" : "narrow", R = !t.sidebar.isEmpty, T = !t.event.isEmpty, k = !t.bottom.isEmpty, [C, W] = n.useState(!1), N = R || !h && d.length > 1 || C;
+                addScriptFinishedHandler: E,
+                removeScriptFinishedHandler: _,
+                libConfig: x
+            } = n.useContext(Ue.E), R = g ? "wide" : "narrow", T = !t.sidebar.isEmpty, k = !t.event.isEmpty, C = !t.bottom.isEmpty, [W, N] = n.useState(!1), L = T || !m && d.length > 1 || W;
             n.useEffect((() => {
-                N && h && !C && W(!0)
-            }), [N, h, C]);
-            const L = n.useCallback((() => {
-                !R && C && W(!1)
-            }), [R, C]);
-            n.useEffect((() => (q(L), () => {
-                E(L)
-            })), [L, q, E]);
-            const I = k ? gs : us,
-                P = e => (0, ze.jsx)(Ea, {
+                L && m && !W && N(!0)
+            }), [L, m, W]);
+            const I = n.useCallback((() => {
+                !T && W && N(!1)
+            }), [T, W]);
+            n.useEffect((() => (E(I), () => {
+                _(I)
+            })), [I, E, _]);
+            const P = C ? vs : fs,
+                D = e => (0, ze.jsx)(Ea, {
                     node: e,
-                    endpoints: M,
+                    endpoints: O,
                     sessionInfo: r,
                     scriptRunId: o,
                     scriptRunState: i,
                     widgetMgr: a,
                     widgetsDisabled: s,
                     uploadClient: l,
                     componentRegistry: c,
                     formsData: u
                 });
-            return (0, ze.jsxs)(cs, {
+            return (0, ze.jsxs)(bs, {
                 className: "appview-container",
                 "data-testid": "stAppViewContainer",
-                "data-layout": x,
-                children: [N && (0, ze.jsx)(is, {
-                    endpoints: M,
-                    initialSidebarState: g,
+                "data-layout": R,
+                children: [L && (0, ze.jsx)(cs, {
+                    endpoints: O,
+                    initialSidebarState: z,
                     appLogo: p,
                     appPages: d,
-                    hasElements: R,
-                    onPageChange: b,
-                    currentPageScriptHash: f,
-                    hideSidebarNav: h,
-                    children: (0, ze.jsx)(fs, {
-                        children: P(t.sidebar)
+                    navSections: b,
+                    hasElements: T,
+                    onPageChange: f,
+                    currentPageScriptHash: h,
+                    hideSidebarNav: m,
+                    children: (0, ze.jsx)(Os, {
+                        children: D(t.sidebar)
                     })
-                }), !N && p && (0, ze.jsx)(Za, {
-                    chevronDownshift: S,
+                }), !L && p && (0, ze.jsx)($a, {
+                    chevronDownshift: q,
                     isCollapsed: !0,
                     "data-testid": "collapsedControl",
                     children: (e => {
                         const t = e.iconImage ? e.iconImage : e.image,
-                            n = M.buildMediaURL(t);
-                        return e.link ? (0, ze.jsx)($a, {
+                            n = O.buildMediaURL(t);
+                        return e.link ? (0, ze.jsx)(Ha, {
                             href: e.link,
                             target: "_blank",
                             rel: "noreferrer",
                             "data-testid": "stLogoLink",
-                            children: (0, ze.jsx)(Ka, {
+                            children: (0, ze.jsx)(Xa, {
                                 src: n,
                                 alt: "Logo",
                                 "data-testid": "stLogo"
                             })
-                        }) : (0, ze.jsx)(Ka, {
+                        }) : (0, ze.jsx)(Xa, {
                             src: n,
                             alt: "Logo",
                             "data-testid": "stLogo"
                         })
                     })(p)
-                }), (0, ze.jsxs)(I, {
+                }), (0, ze.jsxs)(P, {
                     tabIndex: 0,
-                    isEmbedded: z,
-                    disableScrolling: A,
+                    isEmbedded: y,
+                    disableScrolling: v,
                     className: "main",
-                    children: [(0, ze.jsx)(bs, {
+                    children: [(0, ze.jsx)(Ms, {
                         className: "block-container",
                         "data-testid": "stAppViewBlockContainer",
-                        isWideMode: O,
-                        showPadding: y,
-                        addPaddingForHeader: v || w,
-                        hasBottom: k,
-                        isEmbedded: z,
-                        hasSidebar: N,
-                        disableFullscreenMode: Boolean(_.disableFullscreenMode),
-                        children: P(t.main)
-                    }), !k && (0, ze.jsx)(Os, {
+                        isWideMode: g,
+                        showPadding: A,
+                        addPaddingForHeader: w || S,
+                        hasBottom: C,
+                        isEmbedded: y,
+                        hasSidebar: L,
+                        disableFullscreenMode: Boolean(x.disableFullscreenMode),
+                        children: D(t.main)
+                    }), !C && (0, ze.jsx)(As, {
                         "data-testid": "IframeResizerAnchor",
                         "data-iframe-height": !0
-                    }), k && (0, ze.jsxs)(ze.Fragment, {
-                        children: [(0, ze.jsx)(Ms, {}), (0, ze.jsx)(ps, {
+                    }), C && (0, ze.jsxs)(ze.Fragment, {
+                        children: [(0, ze.jsx)(ys, {}), (0, ze.jsx)(hs, {
                             "data-testid": "stBottom",
-                            children: (0, ze.jsx)(ds, {
-                                children: (0, ze.jsx)(ms, {
+                            children: (0, ze.jsx)(ms, {
+                                children: (0, ze.jsx)(zs, {
                                     "data-testid": "stBottomBlockContainer",
-                                    isWideMode: O,
-                                    showPadding: y,
-                                    children: P(t.bottom)
+                                    isWideMode: g,
+                                    showPadding: A,
+                                    children: D(t.bottom)
                                 })
                             })
                         })]
                     })]
-                }), T && (0, ze.jsx)(ls, {
+                }), k && (0, ze.jsx)(ds, {
                     scriptRunId: t.event.scriptRunId,
-                    children: (0, ze.jsx)(hs, {
-                        children: P(t.event)
+                    children: (0, ze.jsx)(gs, {
+                        children: D(t.event)
                     })
                 })]
             })
         };
-        var ys = n.forwardRef((function(e, t) {
+        var Ss = n.forwardRef((function(e, t) {
             return n.createElement(tn.D, (0, en.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 8 8"
             }, e, {
                 ref: t
             }), n.createElement("path", {
                 d: "M5 0c-.55 0-1 .45-1 1s.45 1 1 1 1-.45 1-1-.45-1-1-1zM3.5 2.5C2.67 2.5 2 3.17 2 4h1c0-.28.22-.5.5-.5s.5.22.5.5-1 1.64-1 2.5C3 7.36 3.67 8 4.5 8S6 7.33 6 6.5H5c0 .28-.22.5-.5.5S4 6.78 4 6.5C4 6.14 5 4.66 5 4c0-.81-.67-1.5-1.5-1.5z"
             }))
         }));
-        ys.displayName = "Info";
-        var As = n.forwardRef((function(e, t) {
+        Ss.displayName = "Info";
+        var qs = n.forwardRef((function(e, t) {
             return n.createElement(tn.D, (0, en.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 8 8"
             }, e, {
                 ref: t
             }), n.createElement("path", {
                 d: "M0 3v2h2V3H0zm3 0v2h2V3H3zm3 0v2h2V3H6z"
             }))
         }));
-        As.displayName = "Ellipses";
-        var vs = n.forwardRef((function(e, t) {
+        qs.displayName = "Ellipses";
+        var Es = n.forwardRef((function(e, t) {
             return n.createElement(tn.D, (0, en.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 8 8"
             }, e, {
                 ref: t
             }), n.createElement("path", {
                 d: "M3.09 0c-.06 0-.1.04-.13.09L.02 6.9c-.02.05-.03.13-.03.19v.81c0 .05.04.09.09.09h6.81c.05 0 .09-.04.09-.09v-.81c0-.05-.01-.14-.03-.19L4.01.09A.142.142 0 003.88 0h-.81zM3 3h1v2H3V3zm0 3h1v1H3V6z"
             }))
         }));
-        vs.displayName = "Warning";
-        class ws {
+        Es.displayName = "Warning";
+        class _s {
             constructor() {
                 this.timerHandle = void 0, this.duration = 0, this.startTime = 0, this.running = !1
             }
             get isRunning() {
                 return this.running
             }
             get remainingTime() {
@@ -122846,116 +123119,116 @@
                     this.running = !1, e()
                 }), t)
             }
             cancel() {
                 void 0 !== this.timerHandle && (window.clearTimeout(this.timerHandle), this.timerHandle = void 0, this.running = !1)
             }
         }
-        var Ss = __webpack_require__(68785),
-            qs = __webpack_require__(30808),
-            Es = __webpack_require__(93219);
+        var xs = __webpack_require__(68785),
+            Rs = __webpack_require__(30808),
+            Ts = __webpack_require__(93219);
 
-        function _s(e, t) {
+        function ks(e, t) {
             return e.replace(new RegExp("(^|\\s)" + t + "(?:\\s|$)", "g"), "$1").replace(/\s+/g, " ").replace(/^\s*|\s*$/g, "")
         }
-        const xs = !1,
-            Rs = n.createContext(null);
-        var Ts = function(e) {
+        const Cs = !1,
+            Ws = n.createContext(null);
+        var Ns = function(e) {
                 return e.scrollTop
             },
-            ks = "unmounted",
-            Cs = "exited",
-            Ws = "entering",
-            Ns = "entered",
-            Ls = "exiting",
-            Is = function(e) {
+            Ls = "unmounted",
+            Is = "exited",
+            Ps = "entering",
+            Ds = "entered",
+            Bs = "exiting",
+            js = function(e) {
                 function t(t, n) {
                     var r;
                     r = e.call(this, t, n) || this;
                     var o, i = n && !n.isMounting ? t.enter : t.appear;
-                    return r.appearStatus = null, t.in ? i ? (o = Cs, r.appearStatus = Ws) : o = Ns : o = t.unmountOnExit || t.mountOnEnter ? ks : Cs, r.state = {
+                    return r.appearStatus = null, t.in ? i ? (o = Is, r.appearStatus = Ps) : o = Ds : o = t.unmountOnExit || t.mountOnEnter ? Ls : Is, r.state = {
                         status: o
                     }, r.nextCallback = null, r
-                }(0, Es.Z)(t, e), t.getDerivedStateFromProps = function(e, t) {
-                    return e.in && t.status === ks ? {
-                        status: Cs
+                }(0, Ts.Z)(t, e), t.getDerivedStateFromProps = function(e, t) {
+                    return e.in && t.status === Ls ? {
+                        status: Is
                     } : null
                 };
                 var o = t.prototype;
                 return o.componentDidMount = function() {
                     this.updateStatus(!0, this.appearStatus)
                 }, o.componentDidUpdate = function(e) {
                     var t = null;
                     if (e !== this.props) {
                         var n = this.state.status;
-                        this.props.in ? n !== Ws && n !== Ns && (t = Ws) : n !== Ws && n !== Ns || (t = Ls)
+                        this.props.in ? n !== Ps && n !== Ds && (t = Ps) : n !== Ps && n !== Ds || (t = Bs)
                     }
                     this.updateStatus(!1, t)
                 }, o.componentWillUnmount = function() {
                     this.cancelNextCallback()
                 }, o.getTimeouts = function() {
                     var e, t, n, r = this.props.timeout;
                     return e = t = n = r, null != r && "number" !== typeof r && (e = r.exit, t = r.enter, n = void 0 !== r.appear ? r.appear : t), {
                         exit: e,
                         enter: t,
                         appear: n
                     }
                 }, o.updateStatus = function(e, t) {
                     if (void 0 === e && (e = !1), null !== t)
-                        if (this.cancelNextCallback(), t === Ws) {
+                        if (this.cancelNextCallback(), t === Ps) {
                             if (this.props.unmountOnExit || this.props.mountOnEnter) {
                                 var n = this.props.nodeRef ? this.props.nodeRef.current : r.findDOMNode(this);
-                                n && Ts(n)
+                                n && Ns(n)
                             }
                             this.performEnter(e)
                         } else this.performExit();
-                    else this.props.unmountOnExit && this.state.status === Cs && this.setState({
-                        status: ks
+                    else this.props.unmountOnExit && this.state.status === Is && this.setState({
+                        status: Ls
                     })
                 }, o.performEnter = function(e) {
                     var t = this,
                         n = this.props.enter,
                         o = this.context ? this.context.isMounting : e,
                         i = this.props.nodeRef ? [o] : [r.findDOMNode(this), o],
                         a = i[0],
                         s = i[1],
                         l = this.getTimeouts(),
                         c = o ? l.appear : l.enter;
-                    !e && !n || xs ? this.safeSetState({
-                        status: Ns
+                    !e && !n || Cs ? this.safeSetState({
+                        status: Ds
                     }, (function() {
                         t.props.onEntered(a)
                     })) : (this.props.onEnter(a, s), this.safeSetState({
-                        status: Ws
+                        status: Ps
                     }, (function() {
                         t.props.onEntering(a, s), t.onTransitionEnd(c, (function() {
                             t.safeSetState({
-                                status: Ns
+                                status: Ds
                             }, (function() {
                                 t.props.onEntered(a, s)
                             }))
                         }))
                     })))
                 }, o.performExit = function() {
                     var e = this,
                         t = this.props.exit,
                         n = this.getTimeouts(),
                         o = this.props.nodeRef ? void 0 : r.findDOMNode(this);
-                    t && !xs ? (this.props.onExit(o), this.safeSetState({
-                        status: Ls
+                    t && !Cs ? (this.props.onExit(o), this.safeSetState({
+                        status: Bs
                     }, (function() {
                         e.props.onExiting(o), e.onTransitionEnd(n.exit, (function() {
                             e.safeSetState({
-                                status: Cs
+                                status: Is
                             }, (function() {
                                 e.props.onExited(o)
                             }))
                         }))
                     }))) : this.safeSetState({
-                        status: Cs
+                        status: Is
                     }, (function() {
                         e.props.onExited(o)
                     }))
                 }, o.cancelNextCallback = function() {
                     null !== this.nextCallback && (this.nextCallback.cancel(), this.nextCallback = null)
                 }, o.safeSetState = function(e, t) {
                     t = this.setNextCallback(t), this.setState(e, t)
@@ -122978,47 +123251,47 @@
                                 s = i[1];
                             this.props.addEndListener(a, s)
                         }
                         null != e && setTimeout(this.nextCallback, e)
                     } else setTimeout(this.nextCallback, 0)
                 }, o.render = function() {
                     var e = this.state.status;
-                    if (e === ks) return null;
+                    if (e === Ls) return null;
                     var t = this.props,
                         r = t.children,
-                        o = (t.in, t.mountOnEnter, t.unmountOnExit, t.appear, t.enter, t.exit, t.timeout, t.addEndListener, t.onEnter, t.onEntering, t.onEntered, t.onExit, t.onExiting, t.onExited, t.nodeRef, (0, qs.Z)(t, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
-                    return n.createElement(Rs.Provider, {
+                        o = (t.in, t.mountOnEnter, t.unmountOnExit, t.appear, t.enter, t.exit, t.timeout, t.addEndListener, t.onEnter, t.onEntering, t.onEntered, t.onExit, t.onExiting, t.onExited, t.nodeRef, (0, Rs.Z)(t, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
+                    return n.createElement(Ws.Provider, {
                         value: null
                     }, "function" === typeof r ? r(e, o) : n.cloneElement(n.Children.only(r), o))
                 }, t
             }(n.Component);
 
-        function Ps() {}
-        Is.contextType = Rs, Is.propTypes = {}, Is.defaultProps = {
+        function Fs() {}
+        js.contextType = Ws, js.propTypes = {}, js.defaultProps = {
             in: !1,
             mountOnEnter: !1,
             unmountOnExit: !1,
             appear: !1,
             enter: !0,
             exit: !0,
-            onEnter: Ps,
-            onEntering: Ps,
-            onEntered: Ps,
-            onExit: Ps,
-            onExiting: Ps,
-            onExited: Ps
-        }, Is.UNMOUNTED = ks, Is.EXITED = Cs, Is.ENTERING = Ws, Is.ENTERED = Ns, Is.EXITING = Ls;
-        const Ds = Is;
-        var Bs = function(e, t) {
+            onEnter: Fs,
+            onEntering: Fs,
+            onEntered: Fs,
+            onExit: Fs,
+            onExiting: Fs,
+            onExited: Fs
+        }, js.UNMOUNTED = Ls, js.EXITED = Is, js.ENTERING = Ps, js.ENTERED = Ds, js.EXITING = Bs;
+        const Us = js;
+        var Vs = function(e, t) {
                 return e && t && t.split(" ").forEach((function(t) {
-                    return r = t, void((n = e).classList ? n.classList.remove(r) : "string" === typeof n.className ? n.className = _s(n.className, r) : n.setAttribute("class", _s(n.className && n.className.baseVal || "", r)));
+                    return r = t, void((n = e).classList ? n.classList.remove(r) : "string" === typeof n.className ? n.className = ks(n.className, r) : n.setAttribute("class", ks(n.className && n.className.baseVal || "", r)));
                     var n, r
                 }))
             },
-            js = function(e) {
+            Hs = function(e) {
                 function t() {
                     for (var t, n = arguments.length, r = new Array(n), o = 0; o < n; o++) r[o] = arguments[o];
                     return (t = e.call.apply(e, [this].concat(r)) || this).appliedClasses = {
                         appear: {},
                         enter: {},
                         exit: {}
                     }, t.onEnter = function(e, n) {
@@ -123053,69 +123326,69 @@
                             o = r ? "" + (r && n ? n + "-" : "") + e : n[e];
                         return {
                             baseClassName: o,
                             activeClassName: r ? o + "-active" : n[e + "Active"],
                             doneClassName: r ? o + "-done" : n[e + "Done"]
                         }
                     }, t
-                }(0, Es.Z)(t, e);
+                }(0, Ts.Z)(t, e);
                 var r = t.prototype;
                 return r.addClass = function(e, t, n) {
                     var r = this.getClassNames(t)[n + "ClassName"],
                         o = this.getClassNames("enter").doneClassName;
-                    "appear" === t && "done" === n && o && (r += " " + o), "active" === n && e && Ts(e), r && (this.appliedClasses[t][n] = r, function(e, t) {
+                    "appear" === t && "done" === n && o && (r += " " + o), "active" === n && e && Ns(e), r && (this.appliedClasses[t][n] = r, function(e, t) {
                         e && t && t.split(" ").forEach((function(t) {
                             return r = t, void((n = e).classList ? n.classList.add(r) : function(e, t) {
                                 return e.classList ? !!t && e.classList.contains(t) : -1 !== (" " + (e.className.baseVal || e.className) + " ").indexOf(" " + t + " ")
                             }(n, r) || ("string" === typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)));
                             var n, r
                         }))
                     }(e, r))
                 }, r.removeClasses = function(e, t) {
                     var n = this.appliedClasses[t],
                         r = n.base,
                         o = n.active,
                         i = n.done;
-                    this.appliedClasses[t] = {}, r && Bs(e, r), o && Bs(e, o), i && Bs(e, i)
+                    this.appliedClasses[t] = {}, r && Vs(e, r), o && Vs(e, o), i && Vs(e, i)
                 }, r.render = function() {
                     var e = this.props,
-                        t = (e.classNames, (0, qs.Z)(e, ["classNames"]));
-                    return n.createElement(Ds, (0, en.Z)({}, t, {
+                        t = (e.classNames, (0, Rs.Z)(e, ["classNames"]));
+                    return n.createElement(Us, (0, en.Z)({}, t, {
                         onEnter: this.onEnter,
                         onEntered: this.onEntered,
                         onEntering: this.onEntering,
                         onExit: this.onExit,
                         onExiting: this.onExiting,
                         onExited: this.onExited
                     }))
                 }, t
             }(n.Component);
-        js.defaultProps = {
+        Hs.defaultProps = {
             classNames: ""
-        }, js.propTypes = {};
-        const Fs = js;
-        let Us;
+        }, Hs.propTypes = {};
+        const Xs = Hs;
+        let Gs;
         ! function(e) {
             e.CONNECTED = "CONNECTED", e.DISCONNECTED_FOREVER = "DISCONNECTED_FOREVER", e.INITIAL = "INITIAL", e.PINGING_SERVER = "PINGING_SERVER", e.CONNECTING = "CONNECTING"
-        }(Us || (Us = {}));
-        const Vs = __webpack_require__.p + "static/media/fireworks.0906f02ea43f1018a6d2.gif",
-            Hs = (0, et.Z)("div", {
+        }(Gs || (Gs = {}));
+        const $s = __webpack_require__.p + "static/media/fireworks.0906f02ea43f1018a6d2.gif",
+            Ks = (0, et.Z)("div", {
                 target: "en6cib67"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     alignItems: "center",
                     justifyContent: "center",
                     color: t.colors.gray
                 }
             }), ""),
-            Xs = (0, et.Z)("label", {
+            Ys = (0, et.Z)("label", {
                 target: "en6cib66"
             })((e => {
                 let {
                     isMinimized: t,
                     theme: n
                 } = e;
                 return {
@@ -123130,15 +123403,15 @@
                     maxWidth: t ? "0" : "20rem",
                     transition: "opacity 500ms 0ms, clip 500ms 0ms, max-width 500ms 0ms, margin 500ms 0ms, visibility 0ms 500ms",
                     opacity: t ? 0 : 1,
                     visibility: t ? "hidden" : "visible",
                     lineHeight: 1
                 }
             }), ""),
-            Gs = (0, et.Z)("div", {
+            Zs = (0, et.Z)("div", {
                 target: "en6cib65"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
@@ -123146,23 +123419,23 @@
                     justifyContent: "center",
                     borderRadius: t.radii.md,
                     margin: "0 ".concat(t.spacing.sm, " 0 0"),
                     paddingLeft: t.spacing.sm,
                     height: "1.6rem"
                 }
             }), ""),
-            $s = e => ({
+            Js = e => ({
                 opacity: 0,
                 padding: e.spacing.none,
                 margin: e.spacing.none,
                 maxWidth: 0,
                 minWidth: 0,
                 border: 0
             }),
-            Ks = (0, et.Z)("label", {
+            Qs = (0, et.Z)("label", {
                 target: "en6cib64"
             })((e => {
                 let {
                     isPrompt: t,
                     isMinimized: n,
                     theme: r
                 } = e;
@@ -123171,32 +123444,32 @@
                     color: t ? r.colors.bodyText : r.colors.gray,
                     textTransform: t ? "none" : "uppercase",
                     margin: "0 0 0 ".concat(r.spacing.lg),
                     whiteSpace: "nowrap",
                     maxWidth: "20rem",
                     borderRadius: t ? r.radii.md : void 0,
                     transition: "opacity 200ms ease-out 0s,\n  clip 200ms ease-out 0s, min-width 200ms ease-out 0s,\n  max-width 200ms ease-out 0s, padding 200ms ease-out 0s",
-                    ...n ? $s(r) : {}
+                    ...n ? Js(r) : {}
                 }
             }), ""),
-            Ys = (0, et.Z)("span", {
+            el = (0, et.Z)("span", {
                 target: "en6cib63"
             })((e => {
                 let {
                     isMinimized: t,
                     theme: n
                 } = e;
                 return {
                     marginLeft: n.spacing.sm,
                     whiteSpace: "nowrap",
                     transition: "opacity 200ms ease-out 0s,\n  clip 200ms ease-out 0s, min-width 200ms ease-out 0s,\n  max-width 200ms ease-out 0s, padding 200ms ease-out 0s",
-                    ...t ? $s(n) : {}
+                    ...t ? Js(n) : {}
                 }
             }), ""),
-            Zs = (0, et.Z)("img", {
+            tl = (0, et.Z)("img", {
                 target: "en6cib62"
             })((e => {
                 let {
                     isNewYears: t,
                     theme: n
                 } = e;
                 const r = (0, Ae.Iy)(n) ? "" : "invert(1)";
@@ -123204,15 +123477,15 @@
                     opacity: t ? 1 : .4,
                     width: t ? "2.2rem" : "1.6rem",
                     height: t ? "2.2rem" : "1.6rem",
                     marginRight: "-".concat(n.spacing.sm),
                     filter: t ? "" : r
                 }
             }), ""),
-            Js = (0, et.Z)("div", {
+            nl = (0, et.Z)("div", {
                 target: "en6cib61"
             })((() => ({
                 "&.StatusWidget-appear": {
                     opacity: 0
                 },
                 "&.StatusWidget-appear-active": {
                     opacity: 1,
@@ -123229,26 +123502,26 @@
                     opacity: 1
                 },
                 "&.StatusWidget-exit-active": {
                     opacity: 0,
                     transition: "opacity 200ms ease-out"
                 }
             })), ""),
-            Qs = (0, et.Z)("div", {
+            rl = (0, et.Z)("div", {
                 target: "en6cib60"
             })((() => ({
                 "&::first-letter": {
                     textDecoration: "underline"
                 }
             })), "");
-        class el extends n.PureComponent {
+        class ol extends n.PureComponent {
             constructor(e) {
-                super(e), this.sessionEventConn = void 0, this.curView = void 0, this.minimizePromptTimer = new ws, this.keyHandlers = void 0, this.handleScroll = () => {
+                super(e), this.sessionEventConn = void 0, this.curView = void 0, this.minimizePromptTimer = new _s, this.keyHandlers = void 0, this.handleScroll = () => {
                     this.setState({
-                        statusMinimized: el.shouldMinimize()
+                        statusMinimized: ol.shouldMinimize()
                     })
                 }, this.onAppPromptHover = () => {
                     this.setState({
                         promptHovered: !0
                     })
                 }, this.onAppPromptUnhover = () => {
                     this.setState({
@@ -123258,15 +123531,15 @@
                 }, this.handleStopScriptClick = () => {
                     this.props.stopScript()
                 }, this.handleRerunClick = () => {
                     this.props.rerunScript(!1)
                 }, this.handleAlwaysRerunClick = () => {
                     this.props.allowRunOnSave && this.props.rerunScript(!0)
                 }, this.state = {
-                    statusMinimized: el.shouldMinimize(),
+                    statusMinimized: ol.shouldMinimize(),
                     promptMinimized: !1,
                     scriptChangedOnDisk: !1,
                     promptHovered: !1
                 }, this.keyHandlers = {
                     a: this.handleAlwaysRerunClick
                 }
             }
@@ -123279,15 +123552,15 @@
             componentDidMount() {
                 this.sessionEventConn = this.props.sessionEventDispatcher.onSessionEvent.connect((e => this.handleSessionEvent(e))), window.addEventListener("scroll", this.handleScroll)
             }
             componentWillUnmount() {
                 void 0 !== this.sessionEventConn && (this.sessionEventConn.disconnect(), this.sessionEventConn = void 0), this.minimizePromptTimer.cancel(), window.removeEventListener("scroll", this.handleScroll)
             }
             isConnected() {
-                return this.props.connectionState === Us.CONNECTED
+                return this.props.connectionState === Gs.CONNECTED
             }
             handleSessionEvent(e) {
                 "scriptChangedOnDisk" === e.type && (this.setState({
                     scriptChangedOnDisk: !0,
                     promptMinimized: !1
                 }), this.minimizePromptAfterTimeout(15e3))
             }
@@ -123301,44 +123574,44 @@
             static shouldMinimize() {
                 return window.scrollY > 32
             }
             render() {
                 const e = this.curView;
                 if (this.curView = this.renderWidget(), null == e && null == this.curView) return null;
                 let t, n;
-                return null != this.curView ? (t = !0, n = this.curView) : (t = !1, n = e), (0, ze.jsx)(Fs, {
+                return null != this.curView ? (t = !0, n = this.curView) : (t = !1, n = e), (0, ze.jsx)(Xs, {
                     appear: !0,
                     in: t,
                     timeout: 200,
                     unmountOnExit: !0,
                     classNames: "StatusWidget",
-                    children: (0, ze.jsx)(Js, {
+                    children: (0, ze.jsx)(nl, {
                         "data-testid": "stStatusWidget",
                         children: n
                     }, "StatusWidget")
                 })
             }
             renderWidget() {
                 if (this.isConnected()) {
                     if (this.props.scriptRunState === Qe.RUNNING || this.props.scriptRunState === Qe.RERUN_REQUESTED) return this.renderScriptIsRunning();
-                    if (!Ss.B && this.state.scriptChangedOnDisk) return this.renderRerunScriptPrompt()
+                    if (!xs.B && this.state.scriptChangedOnDisk) return this.renderRerunScriptPrompt()
                 }
                 return this.renderConnectionStatus()
             }
             renderConnectionStatus() {
-                const e = el.getConnectionStateUI(this.props.connectionState);
+                const e = ol.getConnectionStateUI(this.props.connectionState);
                 return void 0 === e ? null : (0, ze.jsx)(_o.Z, {
                     content: e.tooltip,
                     placement: _o.u.BOTTOM,
-                    children: (0, ze.jsxs)(Hs, {
+                    children: (0, ze.jsxs)(Ks, {
                         "data-testid": "stConnectionStatus",
                         children: [(0, ze.jsx)(mn.Z, {
                             size: "sm",
                             content: e.icon
-                        }), (0, ze.jsx)(Xs, {
+                        }), (0, ze.jsx)(Ys, {
                             isMinimized: this.state.statusMinimized,
                             children: e.label
                         })]
                     })
                 })
             }
             static isNewYears() {
@@ -123346,28 +123619,28 @@
                     t = e.getMonth(),
                     n = e.getDate();
                 return 11 === t && 31 === n || 0 === t && n <= 6
             }
             renderScriptIsRunning() {
                 const e = this.state.statusMinimized,
                     t = this.props.scriptRunState === Qe.STOP_REQUESTED,
-                    n = el.promptButton(t ? "Stopping..." : "Stop", t, this.handleStopScriptClick, e),
-                    r = el.isNewYears(),
-                    o = r ? Vs : "data:image/gif;base64,R0lGODlhgACAAPAAAAAAAAAAACH5BAkUAAEAIf8LTkVUU0NBUEUyLjADAQAAACwAAAAAgACAAAAC/oyPqcvtD6OctNqLs968+w+G4kiW5omm6sq27gvH8kzX9o3nKcD3vA5s+Ia9oNFATAKOQKWSiXM6oTbpkzqzTrEx7ZX78ibBYfGYzDKf0So1kZ12/+Ar+Zy+s+Pr7j1f7ffnFRinRegiddg1pNho5OMIKbhGZpXXl6N3YrdlwvlF8ik6SioZWoqaauap2ur6xvoqm4oya1t6easL2Lbra1j2+5sp3ApWjKmI7Bghy1zh/DwRLd38Wi1Bje2gvc3Q7a0AHo4wTo50fb5gfs5O7h4O7y2/TY9tX40vrf/Mz+wfKZ26BAAbFVQmcOCBg4cYEnIYCKIfiXso4rFIByMcnY1sOKLxWCmhwgCWhCQaufDkN5UoS67s1JKlOJkKXa6jOdDmTJgjdRLEqc5nOaDtiJI0Gs+o0KBKkc5ryrMmVFA9p1KqGnVoVqZb0XV9ZxUWyqNflxYt67ReWEZjyVL9+TUp2rhP577NudZUTLtXpfIVu/duSrpq/7Id6zRtYcAvGQfWy60vYsgPDre9jDmz5s2cO3v+DDq06NEnCgAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4P1AGGxGGwV0wSjzmlE8C0PZ/R2XRahV2vWdcW22V9qeHV2FlWnclp0xrddr+T8dN8WZff8/o5v3/2BzgmOMhVaAiHaAe2qEbnGCk56XBHSLlgaYl5oOmJ6Rk6GUoaSVrqeIpaqLoq2OqaBxtbNyv6eljZyprbAMvL5vuLG8wwTKxofIxcBLGM2Oz8zKm8S/0wfZ0wq62r2i1sDa6QPc49Ti6O3lkObFR9Opq8rc6sBB/v3kj/rb/PXi/Om0wB2/jh10/WQQTtumxCaGsekocMI2758QmixfZiNxbi28ixxpoIIC91NCmtZC+RXyiobCkFpsuX/2TIrEAz5IubOHNK3Hkxg897NIJuGIrHptGjSIuubPLUS9STNaVWpapTzFWsP1tM5UpUadaYW82U1bA05dhHa4V+JXg2RVoPc721RVGXQ96PkMTetbAX7t9EST8EFtzV69sLh9PFlbu4Z2SNff0OVps43GXChd1OphzNaWNsPEl+xotS8umKj9mOdvwadGcrqUnXlhAbciDbt3Gv1j0QoEfVmbUMRfvbtUqmm82+7NDaOEjDYSdaDBEayPV1wmlxz8dd88jwvnOTP48+vfr17Nu7fw8/vnz4BQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/IG1PaMc/a+537FC9Z+xIfwWEwmjkylkgl1FqFN6Y9atc6wWW2Mi/TKwELxmMwzf9E99YvddrvgQ/kcbofh828yf431FxK2ECjowcVAeKgDxsjC9phCJ2lCV1c5eImZ2bEZ16nxmRaaMRpUenFaljqxutja8NoVqzAbVWt7i5trsJuYOxuAVivsS1xqfBDZqYxAKfkquyko7TDKtxpxasctge3m7foZTq56KUdtCq2G3ojcvofomC4PQpVtr0ma594ryu4fBn8CB+orCOQgwnHMYuH7ppAGLxQRn1WkcFGiuv5p8Axu9GRNUcOE2t450+UH4y6AvwBcSwmx5bmWnFAa2kazJoScoGxOfMnTZUxgPn8uuQkUqUV6RpQmpXXUaFFWOB9yhFoV6zKpS7U+hRUVLEOvw8g6HUt1as+ZadXq7IpKo1ircuMW8srVAt1jYte1hcvP7T1aeT3+5Xu4bGKWacn6tRsWMuAbIrr0BXlYquPH/DZzXqs482WTpEZjDrx17uJ5cU2TXmvUM+MesmdTnnw7NeoRGU/Dhur69V4SYGOv/tCxRHHgx1kTtfTXuGTiMKFPl76bd3Xl0ZlP187U+m7soCtvp37de3bz4bmnX/6dfXvw49WXH1wmuO3ciK/fx0fOin6fvaVZc3VRVhtboBX4n29tJEhSfH1BqBJVFGa1Xn9CiWSgXosUZliGEYoYImoXfnXfiCR62J2AO53IYYcYZgfiUDLOuCKO/OnmoltvHZjjVZed9WKNJTYo5HHPFQmjjin6uONdRPJo5ICmzZckTRQF9WOWK00SlIK33CHTkeK0UOZ+H5FZknMEnWGOfOf5EJB7VeKw5EJ67slnn37+CWiggg5KaKGGMlIAACH5BAkUAAEALAAAAACAAIAAAAL+jI+py+0Po5y02ouz3rz7D4biSJbmiabqyrbuC8cyBNT2jHP2vud+xQvefsSG8AgoKhFI5HLZPD6LUefUV5Vec1nhFtfVfmFh75hc5p3R6do61na/X/HknJ6+s8P6fbUPlwUo8zc4I2aYqLjI2Ehk5rhSGGlSRilSd+lRJ6eZwdnjCQQaJCpBimi6gNqkqsAq6GoAG6tKy2d6aymqi6vZu3sJ7BuZN0sr3JWgSzm5zOwYxTAc3bpKzSh9ja2o/To8ZOj9DB7eN34AGtAGiH6cyXnnvp75Hj82f5+u/pVfz8TviruAAPU9GWiwYJwtCBc6+HfQmkJjD9gJtELOYoTpYFMw7oO40VlHSBMpjiLZL9Q3hxtUZgMpa0LCmCFh0qw48+ZDgjp3kuqJExXQaciGZmRltKTQpPSgGf3DsmcsjVLHUb0p0iTWhsqqSlTq8Y1LCrWOfj0zj+hZs6lSElsZFm5chjBFbpt7sZw5I2vz6rVDo+/Iv4CDtqX795TgwXoV4/XLLfBjyL1kLkbrtObhdj/JXhanVTPKX5/5TvZUGENappI3szY8+nXr2LJ9uq59lzbu3KV2i+7tGzbw4KZvE29qnPjq48h1M19+HLry0sGlV6d+3Tnz5mO3y+3kvWL48eTLmz8PoQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4PDAqHQ4DRWDseiQalc8l6PoXSKgBllQKz1RJX2/taRWLwrjz2oM25dbfjdvLibAxdrrvXK3pou49nAeiHM6h0YXiVl4jEZxjG6Dj4EzmRSARo+cgUoCdxydlEFwEa2jn6UGp66gYxuYqA2vAKeyDL0FercLtwp9sb5+D7uxs820oMjHz8lSxs/PzmHL32STjNDI0Nl7vNseltpxquWUluzdh4npp+uJ7drv4eGz81b1u/R56fts6f5e8fwHACm20rKAYbwjLOulFD03BZOYYRDYqzOI3Lt/aB++x98HgvpMiRJEuaPIkypcqKIDVw3NDPBUREMwVRTDEMnUR22khk4ukJKK+P4/AVFQWO28KlP2EyferwItSpPSVRvXqTJtatGjNw/RrTZldltBKYKzZWa1iyQ9EGfdhSbFx4NUm1xSXNZSAK1dRinCjvxlqpc1caPow4seLFjBs7hqTP7169kXFm5VsXc0IVb13dxVs1RFO6oc1GBXGW3lFWZTeCBav0NWzKsl/Trv31Nu6tundf7V2Y9WjVrYkPBhzcaGfQy9kmt1vZbV+d0z1HB0w4rebNVgPbOC73+ePx5MubP48+vfr17Nu7fw8/vvzGBQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJphPAAuoLI+3cxrZJ5+7Ne/q/6wkvQN3wSCn+kEyHEtiMJp5LqZVqtEaxVS2Sm/UewTnxlzwzn9HqNbk9RgfhPTY9jr27n3omv99UBKiVNmh4iJiouMjY6FhX9hijJJnCVVnyhhkit/khx+LJARoqmkFaY0qEOqcqwVrq+gobK+tEW2u7gJuqu8ub62sA3Cs8TBxsi1wovMys7PysGh05TV29eQ1Vqf2H2N35jXyMKg4sw3o4jl5ueK4Aq07bEO+efts+eI9PKp/PUM/eP3j7BPYDWFDcAU0EBzZiyO4gNzC/JE681DBcNvCKGSFi8kgO5MU8HUmaEmnHGsYpHF2hXOmyZURKul7S/JjM5raRrUJSqdjlUZiZ3ohKY7TTqKCSyRTdVJp0ITakRaXCtNrUXFWsWwMUo3qV69OFkjSyNLnRLNShZR36HPsw4NmfQuchROs07Aq9+vjuxdsX8CrBd2RuMFzYLwbEbRiPcutH8WHIQxx/ogyJ7omEeOBmwmxDswrOmaOOBv3C82mLQkzDkNt6amjYpXvOpm1srcjcXnnxZopa1rrfvd8RL47ruNjg0HATd36ceW5Qyh+krE5PMva3Qbfz6+79O43wSdiShyD7PPqv6tsbKgAAOw==",
-                    i = (0, ze.jsx)(Zs, {
+                    n = ol.promptButton(t ? "Stopping..." : "Stop", t, this.handleStopScriptClick, e),
+                    r = ol.isNewYears(),
+                    o = r ? $s : "data:image/gif;base64,R0lGODlhgACAAPAAAAAAAAAAACH5BAkUAAEAIf8LTkVUU0NBUEUyLjADAQAAACwAAAAAgACAAAAC/oyPqcvtD6OctNqLs968+w+G4kiW5omm6sq27gvH8kzX9o3nKcD3vA5s+Ia9oNFATAKOQKWSiXM6oTbpkzqzTrEx7ZX78ibBYfGYzDKf0So1kZ12/+Ar+Zy+s+Pr7j1f7ffnFRinRegiddg1pNho5OMIKbhGZpXXl6N3YrdlwvlF8ik6SioZWoqaauap2ur6xvoqm4oya1t6easL2Lbra1j2+5sp3ApWjKmI7Bghy1zh/DwRLd38Wi1Bje2gvc3Q7a0AHo4wTo50fb5gfs5O7h4O7y2/TY9tX40vrf/Mz+wfKZ26BAAbFVQmcOCBg4cYEnIYCKIfiXso4rFIByMcnY1sOKLxWCmhwgCWhCQaufDkN5UoS67s1JKlOJkKXa6jOdDmTJgjdRLEqc5nOaDtiJI0Gs+o0KBKkc5ryrMmVFA9p1KqGnVoVqZb0XV9ZxUWyqNflxYt67ReWEZjyVL9+TUp2rhP577NudZUTLtXpfIVu/duSrpq/7Id6zRtYcAvGQfWy60vYsgPDre9jDmz5s2cO3v+DDq06NEnCgAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4P1AGGxGGwV0wSjzmlE8C0PZ/R2XRahV2vWdcW22V9qeHV2FlWnclp0xrddr+T8dN8WZff8/o5v3/2BzgmOMhVaAiHaAe2qEbnGCk56XBHSLlgaYl5oOmJ6Rk6GUoaSVrqeIpaqLoq2OqaBxtbNyv6eljZyprbAMvL5vuLG8wwTKxofIxcBLGM2Oz8zKm8S/0wfZ0wq62r2i1sDa6QPc49Ti6O3lkObFR9Opq8rc6sBB/v3kj/rb/PXi/Om0wB2/jh10/WQQTtumxCaGsekocMI2758QmixfZiNxbi28ixxpoIIC91NCmtZC+RXyiobCkFpsuX/2TIrEAz5IubOHNK3Hkxg897NIJuGIrHptGjSIuubPLUS9STNaVWpapTzFWsP1tM5UpUadaYW82U1bA05dhHa4V+JXg2RVoPc721RVGXQ96PkMTetbAX7t9EST8EFtzV69sLh9PFlbu4Z2SNff0OVps43GXChd1OphzNaWNsPEl+xotS8umKj9mOdvwadGcrqUnXlhAbciDbt3Gv1j0QoEfVmbUMRfvbtUqmm82+7NDaOEjDYSdaDBEayPV1wmlxz8dd88jwvnOTP48+vfr17Nu7fw8/vnz4BQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/IG1PaMc/a+537FC9Z+xIfwWEwmjkylkgl1FqFN6Y9atc6wWW2Mi/TKwELxmMwzf9E99YvddrvgQ/kcbofh828yf431FxK2ECjowcVAeKgDxsjC9phCJ2lCV1c5eImZ2bEZ16nxmRaaMRpUenFaljqxutja8NoVqzAbVWt7i5trsJuYOxuAVivsS1xqfBDZqYxAKfkquyko7TDKtxpxasctge3m7foZTq56KUdtCq2G3ojcvofomC4PQpVtr0ma594ryu4fBn8CB+orCOQgwnHMYuH7ppAGLxQRn1WkcFGiuv5p8Axu9GRNUcOE2t450+UH4y6AvwBcSwmx5bmWnFAa2kazJoScoGxOfMnTZUxgPn8uuQkUqUV6RpQmpXXUaFFWOB9yhFoV6zKpS7U+hRUVLEOvw8g6HUt1as+ZadXq7IpKo1ircuMW8srVAt1jYte1hcvP7T1aeT3+5Xu4bGKWacn6tRsWMuAbIrr0BXlYquPH/DZzXqs482WTpEZjDrx17uJ5cU2TXmvUM+MesmdTnnw7NeoRGU/Dhur69V4SYGOv/tCxRHHgx1kTtfTXuGTiMKFPl76bd3Xl0ZlP187U+m7soCtvp37de3bz4bmnX/6dfXvw49WXH1wmuO3ciK/fx0fOin6fvaVZc3VRVhtboBX4n29tJEhSfH1BqBJVFGa1Xn9CiWSgXosUZliGEYoYImoXfnXfiCR62J2AO53IYYcYZgfiUDLOuCKO/OnmoltvHZjjVZed9WKNJTYo5HHPFQmjjin6uONdRPJo5ICmzZckTRQF9WOWK00SlIK33CHTkeK0UOZ+H5FZknMEnWGOfOf5EJB7VeKw5EJ67slnn37+CWiggg5KaKGGMlIAACH5BAkUAAEALAAAAACAAIAAAAL+jI+py+0Po5y02ouz3rz7D4biSJbmiabqyrbuC8cyBNT2jHP2vud+xQvefsSG8AgoKhFI5HLZPD6LUefUV5Vec1nhFtfVfmFh75hc5p3R6do61na/X/HknJ6+s8P6fbUPlwUo8zc4I2aYqLjI2Ehk5rhSGGlSRilSd+lRJ6eZwdnjCQQaJCpBimi6gNqkqsAq6GoAG6tKy2d6aymqi6vZu3sJ7BuZN0sr3JWgSzm5zOwYxTAc3bpKzSh9ja2o/To8ZOj9DB7eN34AGtAGiH6cyXnnvp75Hj82f5+u/pVfz8TviruAAPU9GWiwYJwtCBc6+HfQmkJjD9gJtELOYoTpYFMw7oO40VlHSBMpjiLZL9Q3hxtUZgMpa0LCmCFh0qw48+ZDgjp3kuqJExXQaciGZmRltKTQpPSgGf3DsmcsjVLHUb0p0iTWhsqqSlTq8Y1LCrWOfj0zj+hZs6lSElsZFm5chjBFbpt7sZw5I2vz6rVDo+/Iv4CDtqX795TgwXoV4/XLLfBjyL1kLkbrtObhdj/JXhanVTPKX5/5TvZUGENappI3szY8+nXr2LJ9uq59lzbu3KV2i+7tGzbw4KZvE29qnPjq48h1M19+HLry0sGlV6d+3Tnz5mO3y+3kvWL48eTLmz8PoQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4PDAqHQ4DRWDseiQalc8l6PoXSKgBllQKz1RJX2/taRWLwrjz2oM25dbfjdvLibAxdrrvXK3pou49nAeiHM6h0YXiVl4jEZxjG6Dj4EzmRSARo+cgUoCdxydlEFwEa2jn6UGp66gYxuYqA2vAKeyDL0FercLtwp9sb5+D7uxs820oMjHz8lSxs/PzmHL32STjNDI0Nl7vNseltpxquWUluzdh4npp+uJ7drv4eGz81b1u/R56fts6f5e8fwHACm20rKAYbwjLOulFD03BZOYYRDYqzOI3Lt/aB++x98HgvpMiRJEuaPIkypcqKIDVw3NDPBUREMwVRTDEMnUR22khk4ukJKK+P4/AVFQWO28KlP2EyferwItSpPSVRvXqTJtatGjNw/RrTZldltBKYKzZWa1iyQ9EGfdhSbFx4NUm1xSXNZSAK1dRinCjvxlqpc1caPow4seLFjBs7hqTP7169kXFm5VsXc0IVb13dxVs1RFO6oc1GBXGW3lFWZTeCBav0NWzKsl/Trv31Nu6tundf7V2Y9WjVrYkPBhzcaGfQy9kmt1vZbV+d0z1HB0w4rebNVgPbOC73+ePx5MubP48+vfr17Nu7fw8/vvzGBQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJphPAAuoLI+3cxrZJ5+7Ne/q/6wkvQN3wSCn+kEyHEtiMJp5LqZVqtEaxVS2Sm/UewTnxlzwzn9HqNbk9RgfhPTY9jr27n3omv99UBKiVNmh4iJiouMjY6FhX9hijJJnCVVnyhhkit/khx+LJARoqmkFaY0qEOqcqwVrq+gobK+tEW2u7gJuqu8ub62sA3Cs8TBxsi1wovMys7PysGh05TV29eQ1Vqf2H2N35jXyMKg4sw3o4jl5ueK4Aq07bEO+efts+eI9PKp/PUM/eP3j7BPYDWFDcAU0EBzZiyO4gNzC/JE681DBcNvCKGSFi8kgO5MU8HUmaEmnHGsYpHF2hXOmyZURKul7S/JjM5raRrUJSqdjlUZiZ3ohKY7TTqKCSyRTdVJp0ITakRaXCtNrUXFWsWwMUo3qV69OFkjSyNLnRLNShZR36HPsw4NmfQuchROs07Aq9+vjuxdsX8CrBd2RuMFzYLwbEbRiPcutH8WHIQxx/ogyJ7omEeOBmwmxDswrOmaOOBv3C82mLQkzDkNt6amjYpXvOpm1srcjcXnnxZopa1rrfvd8RL47ruNjg0HATd36ceW5Qyh+krE5PMva3Qbfz6+79O43wSdiShyD7PPqv6tsbKgAAOw==",
+                    i = (0, ze.jsx)(tl, {
                         isNewYears: r,
                         src: o,
                         alt: "Running..."
                     });
-                return (0, ze.jsxs)(Gs, {
+                return (0, ze.jsxs)(Zs, {
                     children: [e ? (0, ze.jsx)(_o.Z, {
                         placement: _o.u.BOTTOM,
                         content: "This script is currently running",
                         children: i
-                    }) : i, (0, ze.jsx)(Ks, {
+                    }) : i, (0, ze.jsx)(Qs, {
                         isMinimized: this.state.statusMinimized,
                         isPrompt: !1,
                         children: "Running..."
                     }), n]
                 })
             }
             renderRerunScriptPrompt() {
@@ -123379,66 +123652,66 @@
                 return (0, ze.jsx)(Ie.HotKeys, {
                     handlers: this.keyHandlers,
                     attach: window,
                     focused: !0,
                     children: (0, ze.jsx)("div", {
                         onMouseEnter: this.onAppPromptHover,
                         onMouseLeave: this.onAppPromptUnhover,
-                        children: (0, ze.jsxs)(Gs, {
+                        children: (0, ze.jsxs)(Zs, {
                             children: [(0, ze.jsx)(mn.Z, {
-                                content: ys,
+                                content: Ss,
                                 margin: "0 sm 0 0",
                                 color: n.bodyText
-                            }), (0, ze.jsx)(Ks, {
+                            }), (0, ze.jsx)(Qs, {
                                 isMinimized: t,
                                 isPrompt: !0,
                                 children: "Source file changed."
-                            }), el.promptButton((0, ze.jsx)(Qs, {
+                            }), ol.promptButton((0, ze.jsx)(rl, {
                                 children: "Rerun"
-                            }), e, this.handleRerunClick, t), this.props.allowRunOnSave && el.promptButton((0, ze.jsx)(Qs, {
+                            }), e, this.handleRerunClick, t), this.props.allowRunOnSave && ol.promptButton((0, ze.jsx)(rl, {
                                 children: "Always rerun"
                             }), e, this.handleAlwaysRerunClick, t)]
                         })
                     })
                 })
             }
             static promptButton(e, t, n, r) {
-                return (0, ze.jsx)(Ys, {
+                return (0, ze.jsx)(el, {
                     isMinimized: r,
                     children: (0, ze.jsx)(sn.ZP, {
                         kind: ln.nW.HEADER_BUTTON,
                         disabled: t,
                         fluidWidth: !0,
                         onClick: n,
                         children: e
                     })
                 })
             }
             static getConnectionStateUI(e) {
                 switch (e) {
-                    case Us.INITIAL:
-                    case Us.PINGING_SERVER:
-                    case Us.CONNECTING:
+                    case Gs.INITIAL:
+                    case Gs.PINGING_SERVER:
+                    case Gs.CONNECTING:
                         return {
-                            icon: As, label: "Connecting", tooltip: "Connecting to Streamlit server"
+                            icon: qs, label: "Connecting", tooltip: "Connecting to Streamlit server"
                         };
-                    case Us.CONNECTED:
+                    case Gs.CONNECTED:
                         return;
-                    case Us.DISCONNECTED_FOREVER:
+                    case Gs.DISCONNECTED_FOREVER:
                     default:
                         return {
-                            icon: vs, label: "Error", tooltip: "Unable to connect to Streamlit server"
+                            icon: Es, label: "Error", tooltip: "Unable to connect to Streamlit server"
                         }
                 }
             }
         }
-        const tl = (0, _e.b)(el);
-        var nl = __webpack_require__(37701),
-            rl = __webpack_require__(96386),
-            ol = n.forwardRef((function(e, t) {
+        const il = (0, _e.b)(ol);
+        var al = __webpack_require__(37701),
+            sl = __webpack_require__(96386),
+            ll = n.forwardRef((function(e, t) {
                 return n.createElement(tn.D, (0, en.Z)({
                     iconAttrs: {
                         fill: "currentColor",
                         xmlns: "http://www.w3.org/2000/svg"
                     },
                     iconVerticalAlign: "middle",
                     iconViewBox: "0 0 24 24"
@@ -123447,20 +123720,20 @@
                 }), n.createElement("path", {
                     fill: "none",
                     d: "M0 0h24v24H0V0z"
                 }), n.createElement("path", {
                     d: "M12 8c1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2 .9 2 2 2zm0 2c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2zm0 6c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2z"
                 }))
             }));
-        ol.displayName = "MoreVert";
-        const il = "video/webm";
-        const al = class {
+        ll.displayName = "MoreVert";
+        const cl = "video/webm";
+        const ul = class {
             static isSupportedBrowser() {
                 try {
-                    return null != navigator.mediaDevices && null != navigator.mediaDevices.getUserMedia && null != navigator.mediaDevices.getDisplayMedia && MediaRecorder.isTypeSupported(il)
+                    return null != navigator.mediaDevices && null != navigator.mediaDevices.getUserMedia && null != navigator.mediaDevices.getDisplayMedia && MediaRecorder.isTypeSupported(cl)
                 } catch (e) {
                     return !1
                 }
             }
             constructor(e) {
                 let {
                     recordAudio: t,
@@ -123476,15 +123749,15 @@
                     const t = await navigator.mediaDevices.getUserMedia({
                         video: !1,
                         audio: !0
                     });
                     e = e.concat(t.getAudioTracks())
                 }
                 this.recordedChunks = [], this.inputStream = new MediaStream(e), this.mediaRecorder = new MediaRecorder(this.inputStream, {
-                    mimeType: il
+                    mimeType: cl
                 }), this.mediaRecorder.ondataavailable = e => this.recordedChunks.push(e.data)
             }
             getState() {
                 return this.mediaRecorder ? this.mediaRecorder.state : "inactive"
             }
             start() {
                 if (!this.mediaRecorder) return (0, ui.KE)("ScreenCastRecorder.start: mediaRecorder is null"), !1;
@@ -123507,65 +123780,65 @@
                 const t = new Promise((t => {
                     e = t
                 }));
                 return this.mediaRecorder.onstop = () => e(), this.mediaRecorder.stop(), this.inputStream && (this.inputStream.getTracks().forEach((e => e.stop())), this.inputStream = null), t.then((() => this.buildOutputBlob()))
             }
             buildOutputBlob() {
                 return new Blob(this.recordedChunks, {
-                    type: il
+                    type: cl
                 })
             }
         };
-        var sl;
-        const ll = e => (0, ge.F4)(sl || (sl = (0, Na.Z)(["\n0% {\n  box-shadow: 0 0 ", " ", ";\n}\n50% {\n  box-shadow: 0 0 ", " ", " ", ";\n}\n100% {\n  box-shadow: 0 0 ", " ", ";\n}"])), e.spacing.twoXS, e.colors.red, e.spacing.sm, e.spacing.twoXS, e.colors.red, e.spacing.twoXS, e.colors.red),
-            cl = (0, et.Z)("div", {
+        var pl, dl = __webpack_require__(50669);
+        const bl = e => (0, ge.F4)(pl || (pl = (0, dl.Z)(["\n0% {\n  box-shadow: 0 0 ", " ", ";\n}\n50% {\n  box-shadow: 0 0 ", " ", " ", ";\n}\n100% {\n  box-shadow: 0 0 ", " ", ";\n}"])), e.spacing.twoXS, e.colors.red, e.spacing.sm, e.spacing.twoXS, e.colors.red, e.spacing.twoXS, e.colors.red),
+            fl = (0, et.Z)("div", {
                 target: "e16jpq808"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
                     bottom: t.spacing.lg,
                     right: t.spacing.sm,
                     width: t.spacing.sm,
                     height: t.spacing.sm,
                     backgroundColor: "red",
                     borderRadius: t.radii.full,
                     boxShadow: "0 0 ".concat(t.spacing.twoXS, " ").concat(t.colors.red),
-                    animation: "".concat(ll(t), " 2s linear infinite")
+                    animation: "".concat(bl(t), " 2s linear infinite")
                 }
             }), ""),
-            ul = (0, et.Z)("div", {
+            hl = (0, et.Z)("div", {
                 target: "e16jpq807"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     borderTop: "1px solid ".concat(t.colors.fadedText10),
                     margin: "".concat(t.spacing.sm, " ").concat(t.spacing.none)
                 }
             }), ""),
-            pl = (0, et.Z)("span", {
+            ml = (0, et.Z)("span", {
                 target: "e16jpq806"
             })((e => {
                 let {
                     isRecording: t,
                     theme: n
                 } = e;
                 return {
                     color: t ? n.colors.red : n.colors.fadedText60,
                     fontSize: n.fontSizes.sm,
                     marginTop: n.spacing.twoXS,
                     fontVariant: "small-caps",
                     textTransform: "uppercase"
                 }
             }), ""),
-            dl = (0, et.Z)("ul", {
+            Ml = (0, et.Z)("ul", {
                 target: "e16jpq805"
             })((e => {
                 let {
                     isDisabled: t,
                     isRecording: n,
                     theme: r
                 } = e;
@@ -123574,15 +123847,15 @@
                     color: r.colors.fadedText60,
                     cursor: "not-allowed"
                 } : {
                     "&:active": {
                         backgroundColor: r.colors.primary,
                         color: r.colors.white,
                         outline: "none",
-                        [pl]: {
+                        [ml]: {
                             color: r.colors.white
                         }
                     },
                     "&:focus": {
                         backgroundColor: r.colors.primary,
                         color: r.colors.white
                     }
@@ -123598,15 +123871,15 @@
                     } || {},
                     ...o,
                     "@media print": {
                         display: "none !important"
                     }
                 }
             }), ""),
-            bl = (0, et.Z)("li", {
+            Ol = (0, et.Z)("li", {
                 target: "e16jpq804"
             })((e => {
                 let {
                     isHighlighted: t,
                     styleProps: n,
                     theme: r
                 } = e;
@@ -123620,15 +123893,15 @@
                     padding: (null === n || void 0 === n ? void 0 : n.padding) || "".concat(r.spacing.twoXS, " ").concat(r.spacing.twoXL),
                     backgroundColor: (null === n || void 0 === n ? void 0 : n.backgroundColor) || r.colors.primaryBg,
                     fontSize: (null === n || void 0 === n ? void 0 : n.fontSize) || r.fontSizes.md,
                     ...o || {},
                     display: "block"
                 }
             }), ""),
-            fl = (0, et.Z)("li", {
+            gl = (0, et.Z)("li", {
                 target: "e16jpq803"
             })((e => {
                 let {
                     isHighlighted: t,
                     styleProps: n,
                     theme: r
                 } = e;
@@ -123642,27 +123915,27 @@
                     padding: (null === n || void 0 === n ? void 0 : n.padding) || "".concat(r.spacing.twoXS, " ").concat(r.spacing.twoXL),
                     backgroundColor: (null === n || void 0 === n ? void 0 : n.backgroundColor) || r.colors.secondaryBg,
                     fontSize: (null === n || void 0 === n ? void 0 : n.fontSize) || r.fontSizes.md,
                     ...o || {},
                     display: "block"
                 }
             }), ""),
-            hl = (0, et.Z)("span", {
+            zl = (0, et.Z)("span", {
                 target: "e16jpq802"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginRight: t.spacing.md,
                     flexGrow: 1,
                     fontFamily: t.fonts.sansSerif
                 }
             }), ""),
-            ml = (0, et.Z)("div", {
+            yl = (0, et.Z)("div", {
                 target: "e16jpq801"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     ul: {
@@ -123679,29 +123952,29 @@
                         borderTop: "none"
                     },
                     "@media print": {
                         display: "none"
                     }
                 }
             }), ""),
-            Ml = (0, et.Z)("span", {
+            Al = (0, et.Z)("span", {
                 target: "e16jpq800"
             })((() => ({
                 lineHeight: "initial"
             })), ""),
-            Ol = {
+            vl = {
                 COUNTDOWN: "Cancel screencast",
                 RECORDING: "Stop recording"
             },
-            gl = e => () => {
+            wl = e => () => {
                 window.open(e, "_blank")
             },
-            zl = () => "localhost" === window.location.hostname || "127.0.0.1" === window.location.hostname;
+            Sl = () => "localhost" === window.location.hostname || "127.0.0.1" === window.location.hostname;
 
-        function yl(e, t) {
+        function ql(e, t) {
             const r = (0, n.forwardRef)(((n, r) => {
                 let {
                     item: o,
                     "aria-selected": i,
                     onClick: a,
                     onMouseEnter: s,
                     $disabled: l,
@@ -123725,52 +123998,52 @@
                         t.enqueue("menuClick", {
                             label: u
                         }), a(e)
                     },
                     onMouseEnter: s
                 });
                 return (0, ze.jsxs)(ze.Fragment, {
-                    children: [d && (0, ze.jsx)(ul, {
+                    children: [d && (0, ze.jsx)(hl, {
                         "data-testid": "main-menu-divider"
-                    }), (0, ze.jsx)(dl, {
+                    }), (0, ze.jsx)(Ml, {
                         ref: r,
                         role: "option",
                         "aria-selected": i,
                         "aria-disabled": l,
                         ...m,
                         ...O,
                         children: (0, ze.jsxs)(e, {
                             ...M,
-                            children: [(0, ze.jsx)(hl, {
+                            children: [(0, ze.jsx)(zl, {
                                 ...m,
                                 children: u
-                            }), p && (0, ze.jsx)(pl, {
+                            }), p && (0, ze.jsx)(ml, {
                                 ...m,
                                 children: p
                             })]
                         })
                     })]
                 })
             }));
             return r.displayName = "MenuItem", r
         }
-        const Al = e => {
+        const El = e => {
             const {
                 colors: t
-            } = (0, _e.u)(), n = e.isDevMenu ? fl : bl;
-            return (0, ze.jsx)(nl.Z, {
+            } = (0, _e.u)(), n = e.isDevMenu ? gl : Ol;
+            return (0, ze.jsx)(al.Z, {
                 items: e.menuItems,
                 onItemSelect: t => {
                     let {
                         item: n
                     } = t;
                     n.onClick(), e.closeMenu()
                 },
                 overrides: {
-                    Option: yl(n, e.metricsMgr),
+                    Option: ql(n, e.metricsMgr),
                     List: {
                         props: {
                             "data-testid": "main-menu-list"
                         },
                         style: {
                             backgroundColor: "inherit",
                             borderBottomRadius: 0,
@@ -123783,15 +124056,15 @@
                             border: "1px solid ".concat(t.fadedText10)
                         }
                     }
                 }
             })
         };
 
-        function vl(e) {
+        function _l(e) {
             var t, n, r, o, i, a, s;
             const l = !e.isServerConnected,
                 c = e.toolbarMode != je.De.ToolbarMode.MINIMAL || e.toolbarMode == je.De.ToolbarMode.MINIMAL && (null === (t = e.menuItems) || void 0 === t ? void 0 : t.aboutSectionMd),
                 u = {
                     DIVIDER: {
                         isDivider: !0
                     },
@@ -123803,31 +124076,31 @@
                     },
                     print: {
                         onClick: e.printCallback,
                         label: "Print"
                     },
                     recordScreencast: {
                         onClick: e.screencastCallback,
-                        label: Ol[e.screenCastState] || "Record a screencast",
-                        shortcut: Ol[e.screenCastState] ? "esc" : "",
-                        stopRecordingIndicator: Boolean(Ol[e.screenCastState])
+                        label: vl[e.screenCastState] || "Record a screencast",
+                        shortcut: vl[e.screenCastState] ? "esc" : "",
+                        stopRecordingIndicator: Boolean(vl[e.screenCastState])
                     },
                     saveSnapshot: {
                         disabled: l,
                         label: "Save a snapshot"
                     },
                     ...!(null !== (n = e.menuItems) && void 0 !== n && n.hideGetHelp) && (null === (r = e.menuItems) || void 0 === r ? void 0 : r.getHelpUrl) && {
                         community: {
-                            onClick: gl(null === (o = e.menuItems) || void 0 === o ? void 0 : o.getHelpUrl),
+                            onClick: wl(null === (o = e.menuItems) || void 0 === o ? void 0 : o.getHelpUrl),
                             label: "Get help"
                         }
                     },
                     ...!(null !== (i = e.menuItems) && void 0 !== i && i.hideReportABug) && (null === (a = e.menuItems) || void 0 === a ? void 0 : a.reportABugUrl) && {
                         report: {
-                            onClick: gl(null === (s = e.menuItems) || void 0 === s ? void 0 : s.reportABugUrl),
+                            onClick: wl(null === (s = e.menuItems) || void 0 === s ? void 0 : s.reportABugUrl),
                             label: "Report a bug"
                         }
                     },
                     settings: {
                         onClick: e.settingsCallback,
                         label: "Settings"
                     },
@@ -123876,15 +124149,15 @@
                 b = function(e, t, n) {
                     let r;
                     if (e.toolbarMode == je.De.ToolbarMode.MINIMAL) {
                         for (r = [n.report, n.community, n.DIVIDER, ...t.length > 0 ? t : [n.DIVIDER], n.about], r = r.filter((e => e)); r.length > 0 && r[0] == n.DIVIDER;) r.shift();
                         for (; r.length > 0 && r.at(r.length - 1) == n.DIVIDER;) r.pop();
                         return r
                     }
-                    return [n.rerun, n.settings, n.DIVIDER, n.print, ...al.isSupportedBrowser() ? [n.recordScreencast] : [], n.DIVIDER, n.report, n.community, ...t.length > 0 ? t : [n.DIVIDER], n.about]
+                    return [n.rerun, n.settings, n.DIVIDER, n.print, ...ul.isSupportedBrowser() ? [n.recordScreencast] : [], n.DIVIDER, n.report, n.community, ...t.length > 0 ? t : [n.DIVIDER], n.about]
                 }(e, d, u),
                 f = [];
             let h = null;
             for (const M of b) M && (M !== u.DIVIDER && (h === u.DIVIDER ? f.push({
                 ...M,
                 hasDividerAbove: !0
             }) : f.push(M)), h = M);
@@ -123897,180 +124170,180 @@
                     hasDividerAbove: !0
                 }) : t.push(o)), r = o);
                 return null != r && (r.styleProps = {
                     margin: "0 0 -.5rem 0",
                     padding: ".25rem 0 .25rem 1.5rem"
                 }), t
             }(p) : [];
-            return 0 == f.length && 0 == m.length ? (0, ze.jsx)(ze.Fragment, {}) : (0, ze.jsx)(rl.Z, {
+            return 0 == f.length && 0 == m.length ? (0, ze.jsx)(ze.Fragment, {}) : (0, ze.jsx)(sl.Z, {
                 focusLock: !0,
                 placement: pn.r4.bottomRight,
                 content: t => {
                     let {
                         close: n
                     } = t;
-                    return (0, ze.jsxs)(ml, {
-                        children: [0 != f.length && (0, ze.jsx)(Al, {
+                    return (0, ze.jsxs)(yl, {
+                        children: [0 != f.length && (0, ze.jsx)(El, {
                             menuItems: f,
                             closeMenu: n,
                             isDevMenu: !1,
                             metricsMgr: e.metricsMgr
-                        }), 0 != m.length && (0, ze.jsx)(Al, {
+                        }), 0 != m.length && (0, ze.jsx)(El, {
                             menuItems: m,
                             closeMenu: n,
                             isDevMenu: !0,
                             metricsMgr: e.metricsMgr
                         })]
                     })
                 },
                 overrides: {
                     Body: {
                         props: {
                             "data-testid": "stMainMenuPopover"
                         }
                     }
                 },
-                children: (0, ze.jsxs)(Ml, {
+                children: (0, ze.jsxs)(Al, {
                     id: "MainMenu",
                     "data-testid": "stMainMenu",
                     children: [(0, ze.jsx)(sn.ZP, {
                         kind: ln.nW.HEADER_NO_PADDING,
                         children: (0, ze.jsx)(mn.Z, {
-                            content: ol,
+                            content: ll,
                             size: "lg"
                         })
-                    }), "RECORDING" === e.screenCastState && (0, ze.jsx)(cl, {})]
+                    }), "RECORDING" === e.screenCastState && (0, ze.jsx)(fl, {})]
                 })
             })
         }
-        const wl = (0, n.memo)(vl),
-            Sl = (0, et.Z)("div", {
+        const xl = (0, n.memo)(_l),
+            Rl = (0, et.Z)("div", {
                 target: "e3g6aar2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     gap: t.spacing.sm,
                     alignItems: "center",
                     lineHeight: t.iconSizes.md
                 }
             }), ""),
-            ql = (0, et.Z)("div", {
+            Tl = (0, et.Z)("div", {
                 target: "e3g6aar1"
             })((e => {
                 let {
                     icon: t
                 } = e;
                 return {
                     background: 'url("'.concat(t, '") no-repeat center / contain'),
                     width: "1rem",
                     height: "1rem"
                 }
             }), ""),
-            El = (0, et.Z)("div", {
+            kl = (0, et.Z)("div", {
                 target: "e3g6aar0"
             })((e => {
                 let {} = e;
                 return {
                     display: "flex",
                     alignItems: "center",
                     flexDirection: "row"
                 }
             }), "");
 
-        function _l(e) {
+        function Cl(e) {
             let {
                 label: t,
                 icon: n,
                 onClick: r
             } = e;
             return (0, ze.jsx)("div", {
                 className: "stActionButton",
                 "data-testid": "stActionButton",
                 children: (0, ze.jsx)(sn.ZP, {
                     onClick: r,
                     kind: ln.nW.HEADER_BUTTON,
-                    children: (0, ze.jsxs)(Sl, {
-                        children: [n && (0, ze.jsx)(ql, {
+                    children: (0, ze.jsxs)(Rl, {
+                        children: [n && (0, ze.jsx)(Tl, {
                             "data-testid": "stActionButtonIcon",
                             icon: n
                         }), t && (0, ze.jsx)("span", {
                             "data-testid": "stActionButtonLabel",
                             children: t
                         })]
                     })
                 })
             })
         }
-        const xl = function(e) {
+        const Wl = function(e) {
                 let {
                     sendMessageToHost: t,
                     hostToolbarItems: n,
                     metricsMgr: r
                 } = e;
-                return (0, ze.jsx)(El, {
+                return (0, ze.jsx)(kl, {
                     "data-testid": "stToolbarActions",
                     children: n.map((e => {
                         let {
                             key: n,
                             label: o,
                             icon: i
                         } = e;
-                        return (0, ze.jsx)(_l, {
+                        return (0, ze.jsx)(Cl, {
                             label: o,
                             icon: i,
                             onClick: () => {
                                 r.enqueue("menuClick", {
                                     key: n
                                 }), t({
                                     type: "TOOLBAR_ITEM_CALLBACK",
                                     key: n
                                 })
                             }
                         }, n)
                     }))
                 })
             },
-            Rl = (0, et.Z)("div", {
+            Nl = (0, et.Z)("div", {
                 target: "e17vllj40"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     gap: t.spacing.sm,
                     alignItems: "center",
                     lineHeight: t.iconSizes.md
                 }
             }), "");
-        class Tl extends n.Component {
+        class Ll extends n.Component {
             render() {
                 const {
                     onClick: e
                 } = this.props;
                 return (0, ze.jsx)("div", {
                     className: "stDeployButton",
                     "data-testid": "stDeployButton",
                     children: (0, ze.jsx)(sn.ZP, {
                         kind: ln.nW.HEADER_BUTTON,
                         onClick: e,
-                        children: (0, ze.jsx)(Rl, {
+                        children: (0, ze.jsx)(Nl, {
                             children: (0, ze.jsx)("span", {
                                 children: "Deploy"
                             })
                         })
                     })
                 })
             }
         }
-        const kl = Tl,
-            Cl = (0, et.Z)("header", {
+        const Il = Ll,
+            Pl = (0, et.Z)("header", {
                 target: "ezrtsby2"
             })((e => {
                 let {
                     showHeader: t,
                     theme: n
                 } = e;
                 return {
@@ -124084,15 +124357,15 @@
                     zIndex: n.zIndices.header,
                     display: t ? "block" : "none",
                     "@media print": {
                         display: "none"
                     }
                 }
             }), ""),
-            Wl = (0, et.Z)("div", {
+            Dl = (0, et.Z)("div", {
                 target: "ezrtsby1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
@@ -124100,180 +124373,180 @@
                     right: t.spacing.none,
                     left: t.spacing.none,
                     height: "0.125rem",
                     backgroundImage: "linear-gradient(90deg, ".concat(t.colors.red70, ", #fffd80)"),
                     zIndex: t.zIndices.header
                 }
             }), ""),
-            Nl = (0, et.Z)("div", {
+            Bl = (0, et.Z)("div", {
                 target: "ezrtsby0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
                     top: t.spacing.xl,
                     right: t.spacing.xl,
                     display: "flex",
                     flexDirection: "row",
                     alignItems: "center"
                 }
             }), "");
-        const Ll = function(e) {
+        const jl = function(e) {
             let {
                 isStale: t,
                 children: r
             } = e;
             const {
                 wideMode: o,
                 embedded: i,
                 showToolbar: a,
                 showColoredLine: s
             } = n.useContext(Fe);
             let l = !0;
-            return i && (l = a || s), (0, ze.jsxs)(Cl, {
+            return i && (l = a || s), (0, ze.jsxs)(Pl, {
                 showHeader: l,
                 isWideMode: o,
                 tabIndex: -1,
                 isStale: t,
                 "data-testid": "stHeader",
-                children: [s && (0, ze.jsx)(Wl, {
+                children: [s && (0, ze.jsx)(Dl, {
                     "data-testid": "stDecoration",
                     id: "stDecoration"
-                }), a && (0, ze.jsx)(Nl, {
+                }), a && (0, ze.jsx)(Bl, {
                     "data-testid": "stToolbar",
                     children: r
                 })]
             })
         };
-        var Il = __webpack_require__(8984),
-            Pl = __webpack_require__.n(Il);
+        var Fl = __webpack_require__(8984),
+            Ul = __webpack_require__.n(Fl);
 
-        function Dl() {
-            return Dl = Object.assign || function(e) {
+        function Vl() {
+            return Vl = Object.assign || function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
-            }, Dl.apply(this, arguments)
+            }, Vl.apply(this, arguments)
         }
 
-        function Bl(e, t) {
+        function Hl(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     i = Object.keys(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var i = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
         }
-        var jl = (0, n.forwardRef)((function(e, t) {
+        var Xl = (0, n.forwardRef)((function(e, t) {
             var r = e.color,
                 o = void 0 === r ? "currentColor" : r,
                 i = e.size,
                 a = void 0 === i ? 24 : i,
-                s = Bl(e, ["color", "size"]);
-            return n.createElement("svg", Dl({
+                s = Hl(e, ["color", "size"]);
+            return n.createElement("svg", Vl({
                 ref: t,
                 xmlns: "http://www.w3.org/2000/svg",
                 width: a,
                 height: a,
                 viewBox: "0 0 24 24",
                 fill: "none",
                 stroke: o,
                 strokeWidth: "2",
                 strokeLinecap: "round",
                 strokeLinejoin: "round"
             }, s), n.createElement("polyline", {
                 points: "15 18 9 12 15 6"
             }))
         }));
-        jl.propTypes = {
-            color: Pl().string,
-            size: Pl().oneOfType([Pl().string, Pl().number])
-        }, jl.displayName = "ChevronLeft";
-        const Fl = jl;
-        var Ul = __webpack_require__(33746);
-        const Vl = (0, et.Z)("div", {
+        Xl.propTypes = {
+            color: Ul().string,
+            size: Ul().oneOfType([Ul().string, Ul().number])
+        }, Xl.displayName = "ChevronLeft";
+        const Gl = Xl;
+        var $l = __webpack_require__(33746);
+        const Kl = (0, et.Z)("div", {
                 target: "e1x90zqc14"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginBottom: t.spacing.sm
                 }
             }), ""),
-            Hl = (0, et.Z)("textarea", {
+            Yl = (0, et.Z)("textarea", {
                 target: "e1x90zqc13"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     fontFamily: t.genericFonts.codeFont,
                     fontSize: t.fontSizes.sm,
                     height: "6rem"
                 }
             }), ""),
-            Xl = (0, et.Z)("span", {
+            Zl = (0, et.Z)("span", {
                 target: "e1x90zqc12"
             })((() => ({
                 "&::first-letter": {
                     textDecoration: "underline"
                 }
             })), ""),
-            Gl = (0, et.Z)(Fl, {
+            Jl = (0, et.Z)(Gl, {
                 target: "e1x90zqc11"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     cursor: "pointer",
                     marginRight: t.spacing.lg
                 }
             }), ""),
-            $l = (0, et.Z)("div", {
+            Ql = (0, et.Z)("div", {
                 target: "e1x90zqc10"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "grid",
                     gap: t.spacing.twoXL,
                     gridTemplateColumns: "1fr 1fr",
                     margin: 0,
                     padding: 0
                 }
             }), ""),
-            Kl = (0, et.Z)("div", {
+            ec = (0, et.Z)("div", {
                 target: "e1x90zqc9"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     gridColumnStart: 1,
                     gridColumnEnd: -1,
                     display: "grid",
                     gap: t.spacing.xs
                 }
             }), ""),
-            Yl = (0, et.Z)("h2", {
+            tc = (0, et.Z)("h2", {
                 target: "e1x90zqc8"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingBottom: 0,
@@ -124288,50 +124561,50 @@
                     gridAutoFlow: "row",
                     gap: t.spacing.xs,
                     "&:first-of-type": {
                         marginTop: 0
                     }
                 }
             }), ""),
-            Zl = (0, et.Z)("label", {
+            nc = (0, et.Z)("label", {
                 target: "e1x90zqc7"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingBottom: 0,
                     paddingTop: 0,
                     marginBottom: 0,
                     marginTop: 0,
                     lineHeight: 1.25,
                     fontSize: t.fontSizes.sm
                 }
             }), ""),
-            Jl = (0, et.Z)(Ul.x, {
+            rc = (0, et.Z)($l.x, {
                 target: "e1x90zqc6"
             })((() => ({
                 display: "block",
                 paddingBottom: 0,
                 paddingTop: 0,
                 marginBottom: 0,
                 marginTop: 0,
                 lineHeight: 1.5
             })), ""),
-            Ql = (0, et.Z)("div", {
+            oc = (0, et.Z)("div", {
                 target: "e1x90zqc4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.md
                 }
             }), ""),
-            ec = (0, et.Z)("input", {
+            ic = (0, et.Z)("input", {
                 target: "e1x90zqc3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginRight: t.spacing.xs,
@@ -124360,41 +124633,41 @@
                         }
                     },
                     "&:disabled": {
                         backgroundColor: t.colors.secondaryBg
                     }
                 }
             }), ""),
-            tc = (0, et.Z)("div", {
+            ac = (0, et.Z)("div", {
                 target: "e1x90zqc2"
             })((() => ({
                 "& > ul": {
                     paddingLeft: "1.4rem"
                 }
             })), ""),
-            nc = (0, et.Z)("div", {
+            sc = (0, et.Z)("div", {
                 target: "e1x90zqc1"
             })((() => ({
                 padding: "0 0 1rem 0",
                 overflowY: "scroll"
             })), ""),
-            rc = (0, et.Z)("a", {
+            lc = (0, et.Z)("a", {
                 target: "e1x90zqc0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: "".concat(t.colors.linkText, " !important"),
                     "&:hover": {
                         color: "".concat((0, xe._j)(t.colors.linkText, .15), " !important")
                     }
                 }
             }), "");
-        class oc extends n.PureComponent {
+        class cc extends n.PureComponent {
             constructor(e) {
                 super(e), this.keyHandlers = void 0, this.rerun = () => {
                     this.props.onRerun(!1)
                 }, this.alwaysRerun = () => {
                     this.props.onRerun(!0)
                 }, this.keyHandlers = {
                     a: this.alwaysRerun
@@ -124414,36 +124687,36 @@
                             children: (0, ze.jsx)("div", {
                                 children: "The source files for this app have changed on disk."
                             })
                         }), (0, ze.jsxs)(sr, {
                             children: [this.props.allowRunOnSave ? (0, ze.jsx)(lr, {
                                 kind: ln.nW.TERTIARY,
                                 onClick: this.alwaysRerun,
-                                children: (0, ze.jsx)(Xl, {
+                                children: (0, ze.jsx)(Zl, {
                                     children: "Always rerun"
                                 })
                             }) : null, (0, ze.jsx)(lr, {
                                 kind: ln.nW.SECONDARY,
                                 onClick: this.rerun,
-                                children: (0, ze.jsx)(Xl, {
+                                children: (0, ze.jsx)(Zl, {
                                     children: "Rerun"
                                 })
                             })]
                         })]
                     })
                 })
             }
         }
-        const ic = "https://streamlit.io",
-            ac = "https://docs.streamlit.io/streamlit-community-cloud/get-started",
-            sc = "https://docs.streamlit.io/knowledge-base/tutorials/deploy";
-        var lc = __webpack_require__(97965);
-        class cc extends n.PureComponent {
+        const uc = "https://streamlit.io",
+            pc = "https://docs.streamlit.io/streamlit-community-cloud/get-started",
+            dc = "https://docs.streamlit.io/knowledge-base/tutorials/deploy";
+        var bc = __webpack_require__(97965);
+        class fc extends n.PureComponent {
             constructor(e) {
-                super(e), this.activeSettings = void 0, this.context = void 0, this.renderThemeCreatorButton = () => this.props.developerMode && (0, ze.jsx)(Ql, {
+                super(e), this.activeSettings = void 0, this.context = void 0, this.renderThemeCreatorButton = () => this.props.developerMode && (0, ze.jsx)(oc, {
                     "data-testid": "edit-theme",
                     children: (0, ze.jsx)(sn.ZP, {
                         onClick: this.props.openThemeCreator,
                         kind: ln.nW.SECONDARY,
                         children: "Edit active theme"
                     })
                 }), this.changeSingleSetting = (e, t) => {
@@ -124479,48 +124752,48 @@
                 return (0, ze.jsxs)(cr, {
                     animate: this.props.animateModal,
                     isOpen: !0,
                     onClose: this.handleCancelButtonClick,
                     children: [(0, ze.jsx)(ir, {
                         children: "Settings"
                     }), (0, ze.jsx)(ar, {
-                        children: (0, ze.jsxs)($l, {
+                        children: (0, ze.jsxs)(Ql, {
                             children: [this.props.allowRunOnSave && (0, ze.jsx)(n.Fragment, {
-                                children: (0, ze.jsxs)(Kl, {
-                                    children: [(0, ze.jsx)(Yl, {
+                                children: (0, ze.jsxs)(ec, {
+                                    children: [(0, ze.jsx)(tc, {
                                         children: "Development"
                                     }), (0, ze.jsxs)("label", {
-                                        children: [(0, ze.jsx)(ec, {
+                                        children: [(0, ze.jsx)(ic, {
                                             disabled: !this.props.isServerConnected,
                                             type: "checkbox",
                                             name: "runOnSave",
                                             checked: this.state.runOnSave && this.props.isServerConnected,
                                             onChange: this.handleCheckboxChange
                                         }), " ", "Run on save"]
-                                    }), (0, ze.jsx)(Jl, {
+                                    }), (0, ze.jsx)(rc, {
                                         children: "Automatically updates the app when the underlying code is updated."
                                     })]
                                 })
-                            }), (0, ze.jsxs)(Kl, {
-                                children: [(0, ze.jsx)(Yl, {
+                            }), (0, ze.jsxs)(ec, {
+                                children: [(0, ze.jsx)(tc, {
                                     children: "Appearance"
                                 }), (0, ze.jsxs)("label", {
-                                    children: [(0, ze.jsx)(ec, {
+                                    children: [(0, ze.jsx)(ic, {
                                         type: "checkbox",
                                         name: "wideMode",
                                         checked: this.state.wideMode,
                                         onChange: this.handleCheckboxChange
                                     }), " ", "Wide mode"]
-                                }), (0, ze.jsx)(Jl, {
+                                }), (0, ze.jsx)(rc, {
                                     children: "Turn on to make this app occupy the entire width of the screen"
                                 })]
-                            }), this.context.availableThemes.length && (0, ze.jsxs)(Kl, {
-                                children: [(0, ze.jsx)(Zl, {
+                            }), this.context.availableThemes.length && (0, ze.jsxs)(ec, {
+                                children: [(0, ze.jsx)(nc, {
                                     children: "Choose app theme, colors and fonts"
-                                }), (0, ze.jsx)(lc.ZP, {
+                                }), (0, ze.jsx)(bc.ZP, {
                                     options: this.context.availableThemes.map((e => e.name)),
                                     disabled: !1,
                                     onChange: this.handleThemeChange,
                                     value: e
                                 }), this.renderThemeCreatorButton()]
                             })]
                         })
@@ -124529,92 +124802,92 @@
             }
             componentDidMount() {
                 this.setState({
                     ...this.activeSettings
                 })
             }
         }
-        cc.contextType = Ue.E;
-        var uc = __webpack_require__(26218),
-            pc = __webpack_require__.n(uc),
-            dc = __webpack_require__(97910),
-            bc = __webpack_require__.n(dc),
-            fc = __webpack_require__(74516),
-            hc = __webpack_require__(44722);
-        const mc = (e, t) => (0, xe.NC)(e).toUpperCase(),
-            Mc = e => pc()(je.MA.FontFamily[e]),
-            Oc = {
+        fc.contextType = Ue.E;
+        var hc = __webpack_require__(26218),
+            mc = __webpack_require__.n(hc),
+            Mc = __webpack_require__(97910),
+            Oc = __webpack_require__.n(Mc),
+            gc = __webpack_require__(74516),
+            zc = __webpack_require__(44722);
+        const yc = (e, t) => (0, xe.NC)(e).toUpperCase(),
+            Ac = e => mc()(je.MA.FontFamily[e]),
+            vc = {
                 primaryColor: {
                     help: "Primary accent color for interactive elements.",
                     title: "Primary color",
-                    component: fc.Z,
-                    getValue: mc
+                    component: gc.Z,
+                    getValue: yc
                 },
                 backgroundColor: {
                     help: "Background color for the main content area.",
                     title: "Background color",
-                    component: fc.Z,
-                    getValue: mc
+                    component: gc.Z,
+                    getValue: yc
                 },
                 secondaryBackgroundColor: {
                     help: "Background color used for the sidebar and most interactive widgets.",
                     title: "Secondary background color",
-                    component: fc.Z,
-                    getValue: mc
+                    component: gc.Z,
+                    getValue: yc
                 },
                 textColor: {
                     help: "Color used for almost all text.",
                     title: "Text color",
-                    component: fc.Z,
-                    getValue: mc
+                    component: gc.Z,
+                    getValue: yc
                 },
                 font: {
                     help: "Font family for all text in the app, except code blocks.",
                     title: "Font family",
-                    options: Object.keys(je.MA.FontFamily).map((e => pc()(e))),
-                    getValue: (e, t) => t.options && t.options.findIndex((t => t === Mc(e))) || 0,
-                    component: lc.ZP
+                    options: Object.keys(je.MA.FontFamily).map((e => mc()(e))),
+                    getValue: (e, t) => t.options && t.options.findIndex((t => t === Ac(e))) || 0,
+                    component: bc.ZP
                 }
             },
-            gc = (e, t) => {
+            wc = (e, t) => {
                 const n = e => "string" === typeof e ? e.toLowerCase() : e,
-                    r = bc()((0, Ae.Zf)(t), n),
+                    r = Oc()((0, Ae.Zf)(t), n),
                     o = [];
-                return (e = bc()(e, n)).primaryColor !== r.primaryColor && o.push('primaryColor="'.concat(e.primaryColor, '"')), e.backgroundColor !== r.backgroundColor && o.push('backgroundColor="'.concat(e.backgroundColor, '"')), e.secondaryBackgroundColor !== r.secondaryBackgroundColor && o.push('secondaryBackgroundColor="'.concat(e.secondaryBackgroundColor, '"')), e.textColor !== r.textColor && o.push('textColor="'.concat(e.textColor, '"')), o
+                return (e = Oc()(e, n)).primaryColor !== r.primaryColor && o.push('primaryColor="'.concat(e.primaryColor, '"')), e.backgroundColor !== r.backgroundColor && o.push('backgroundColor="'.concat(e.backgroundColor, '"')), e.secondaryBackgroundColor !== r.secondaryBackgroundColor && o.push('secondaryBackgroundColor="'.concat(e.secondaryBackgroundColor, '"')), e.textColor !== r.textColor && o.push('textColor="'.concat(e.textColor, '"')), o
             },
-            zc = e => {
+            Sc = e => {
                 const [t, r] = n.useState(!1), {
                     activeTheme: o,
                     addThemes: i,
                     setTheme: a
                 } = n.useContext(Ue.E), s = (0, Ae.Zf)(o.emotion), l = (e, t) => {
                     (e => {
                         i([e]), a(e)
                     })((0, Ae.jG)(Ae.UO, {
                         ...s,
                         [e]: t
                     })), r(!1)
                 }, c = (e => {
                     const t = ["[theme]"],
-                        n = gc(e, hc.Wb.emotion),
-                        r = gc(e, hc.$_.emotion),
+                        n = wc(e, zc.Wb.emotion),
+                        r = wc(e, zc.$_.emotion),
                         o = n.length,
                         i = r.length;
                     if (o === i ? t.push(...n) : o < i ? t.push('base="light"', ...n) : t.push('base="dark"', ...r), e.font) {
-                        const n = Mc(e.font).toLowerCase();
+                        const n = Ac(e.font).toLowerCase();
                         t.push('font="'.concat(n, '"'))
                     }
                     return [...t, ""].join("\n")
                 })(s), u = e => {
                     let {
                         name: t,
                         value: r
                     } = e;
-                    const o = Oc[t],
-                        i = o.component === fc.Z,
+                    const o = vc[t],
+                        i = o.component === gc.Z,
                         a = {
                             options: o.options || void 0,
                             showValue: i,
                             value: o.getValue(r, o)
                         };
                     return (0, ze.jsx)(n.Fragment, {
                         children: (0, ze.jsx)(o.component, {
@@ -124634,53 +124907,53 @@
                     secondaryBackgroundColor: f
                 } = s;
                 return (0, ze.jsxs)(cr, {
                     animate: !1,
                     isOpen: !0,
                     onClose: e.onClose,
                     children: [(0, ze.jsxs)(ir, {
-                        children: [(0, ze.jsx)(Gl, {
+                        children: [(0, ze.jsx)(Jl, {
                             onClick: () => {
                                 e.backToSettings(!1)
                             },
                             "data-testid": "stThemeCreatorBack"
                         }), "Edit active theme"]
                     }), (0, ze.jsx)(ar, {
-                        children: (0, ze.jsxs)($l, {
+                        children: (0, ze.jsxs)(Ql, {
                             "data-testid": "stThemeCreatorDialog",
-                            children: [(0, ze.jsx)(Kl, {
-                                children: (0, ze.jsx)(Jl, {
+                            children: [(0, ze.jsx)(ec, {
+                                children: (0, ze.jsx)(rc, {
                                     children: "Changes made to the active theme will exist for the duration of a session. To discard changes and recover the original theme, refresh the page."
                                 })
                             }), (0, ze.jsx)(u, {
                                 name: "primaryColor",
                                 value: p
                             }), (0, ze.jsx)(u, {
                                 name: "backgroundColor",
                                 value: b
                             }), (0, ze.jsx)(u, {
                                 name: "textColor",
                                 value: d
                             }), (0, ze.jsx)(u, {
                                 name: "secondaryBackgroundColor",
                                 value: f
-                            }), (0, ze.jsx)(Kl, {
+                            }), (0, ze.jsx)(ec, {
                                 children: (0, ze.jsx)(u, {
                                     name: "font",
                                     value: String(s.font)
                                 })
-                            }), (0, ze.jsx)(Kl, {
-                                children: (0, ze.jsxs)(Jl, {
+                            }), (0, ze.jsx)(ec, {
+                                children: (0, ze.jsxs)(rc, {
                                     children: ["To save your changes, copy your custom theme into the clipboard and paste it into the", (0, ze.jsx)("code", {
                                         children: "[theme]"
                                     }), " section of your", " ", (0, ze.jsx)("code", {
                                         children: ".streamlit/config.toml"
                                     }), " file."]
                                 })
-                            }), (0, ze.jsx)(Kl, {
+                            }), (0, ze.jsx)(ec, {
                                 children: (0, ze.jsx)("div", {
                                     children: (0, ze.jsx)(sn.ZP, {
                                         onClick: () => {
                                             navigator.clipboard.writeText(c), r(!0)
                                         },
                                         kind: ln.nW.SECONDARY,
                                         children: t ? (0, ze.jsxs)(n.Fragment, {
@@ -124693,80 +124966,80 @@
                                     })
                                 })
                             })]
                         })
                     })]
                 })
             };
-        var yc = __webpack_require__(30067);
+        var qc = __webpack_require__(30067);
 
-        function Ac(e, t) {
+        function Ec(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function vc(e) {
+        function _c(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ac(Object(n), !0).forEach((function(t) {
-                    wc(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ac(Object(n)).forEach((function(t) {
+                t % 2 ? Ec(Object(n), !0).forEach((function(t) {
+                    xc(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ec(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
 
-        function wc(e, t, n) {
+        function xc(e, t, n) {
             return t in e ? Object.defineProperty(e, t, {
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
-        var Sc = (0, st.zo)("div", (function(e) {
-            return vc({}, e.$theme.typography.LabelMedium)
+        var Rc = (0, st.zo)("div", (function(e) {
+            return _c({}, e.$theme.typography.LabelMedium)
         }));
-        Sc.displayName = "Action", Sc.displayName = "Action";
-        var qc = (0, st.zo)("div", (function(e) {
+        Rc.displayName = "Action", Rc.displayName = "Action";
+        var Tc = (0, st.zo)("div", (function(e) {
             var t = e.$theme;
-            return vc({
+            return _c({
                 marginBottom: t.sizing.scale600,
                 color: t.colors.contentPrimary
             }, t.typography.ParagraphMedium)
         }));
-        qc.displayName = "Body", qc.displayName = "Body";
-        var Ec = (0, st.zo)("div", (function(e) {
+        Tc.displayName = "Body", Tc.displayName = "Body";
+        var kc = (0, st.zo)("div", (function(e) {
             var t = e.$theme;
             return {
                 marginLeft: t.sizing.scale600,
                 marginTop: t.sizing.scale600,
                 marginRight: t.sizing.scale600,
                 marginBottom: t.sizing.scale600
             }
         }));
-        Ec.displayName = "Contents", Ec.displayName = "Contents";
-        var _c = (0, st.zo)("img", (function(e) {
+        kc.displayName = "Contents", kc.displayName = "Contents";
+        var Cc = (0, st.zo)("img", (function(e) {
             var t = e.$theme;
             return {
                 borderTopLeftRadius: t.borders.surfaceBorderRadius,
                 borderTopRightRadius: t.borders.surfaceBorderRadius,
                 objectFit: "contain",
                 maxWidth: "100%"
             }
         }));
-        _c.displayName = "HeaderImage", _c.displayName = "HeaderImage";
-        var xc = (0, st.zo)("section", (function(e) {
+        Cc.displayName = "HeaderImage", Cc.displayName = "HeaderImage";
+        var Wc = (0, st.zo)("section", (function(e) {
             var t = e.$theme;
             return {
                 borderLeftWidth: "2px",
                 borderTopWidth: "2px",
                 borderRightWidth: "2px",
                 borderBottomWidth: "2px",
                 borderLeftStyle: "solid",
@@ -124781,89 +125054,89 @@
                 borderTopRightRadius: t.borders.radius400,
                 borderBottomLeftRadius: t.borders.radius400,
                 borderBottomRightRadius: t.borders.radius400,
                 backgroundColor: t.colors.backgroundPrimary,
                 overflow: "hidden"
             }
         }));
-        xc.displayName = "Root", xc.displayName = "Root";
-        var Rc = (0, st.zo)("img", (function(e) {
+        Wc.displayName = "Root", Wc.displayName = "Root";
+        var Nc = (0, st.zo)("img", (function(e) {
             var t = e.$theme;
-            return vc(vc({
+            return _c(_c({
                 float: "right",
                 height: t.sizing.scale2400,
                 width: t.sizing.scale2400,
                 objectFit: "cover",
                 borderTopLeftRadius: t.borders.surfaceBorderRadius,
                 borderTopRightRadius: t.borders.surfaceBorderRadius,
                 borderBottomLeftRadius: t.borders.surfaceBorderRadius,
                 borderBottomRightRadius: t.borders.surfaceBorderRadius
-            }, (0, yc.Qj)(t.borders.border200)), {}, {
+            }, (0, qc.Qj)(t.borders.border200)), {}, {
                 margin: "0 0 ".concat(t.sizing.scale500, " ").concat(t.sizing.scale500)
             })
         }));
-        Rc.displayName = "Thumbnail", Rc.displayName = "Thumbnail";
-        var Tc = (0, st.zo)("h1", (function(e) {
+        Nc.displayName = "Thumbnail", Nc.displayName = "Thumbnail";
+        var Lc = (0, st.zo)("h1", (function(e) {
             var t = e.$theme;
-            return vc(vc({}, t.typography.HeadingSmall), {}, {
+            return _c(_c({}, t.typography.HeadingSmall), {}, {
                 color: t.colors.contentPrimary,
                 marginLeft: 0,
                 marginTop: 0,
                 marginRight: 0,
                 marginBottom: t.sizing.scale500,
                 paddingLeft: 0,
                 paddingTop: 0,
                 paddingRight: 0,
                 paddingBottom: 0
             })
         }));
-        Tc.displayName = "Title", Tc.displayName = "Title";
-        const kc = __webpack_require__.p + "static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg";
-        const Cc = __webpack_require__.p + "static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg";
-        const Wc = function() {
+        Lc.displayName = "Title", Lc.displayName = "Title";
+        const Ic = __webpack_require__.p + "static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg";
+        const Pc = __webpack_require__.p + "static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg";
+        const Dc = function() {
                 return {
                     title: "Unable to deploy",
                     body: (0, ze.jsxs)(ze.Fragment, {
                         children: [(0, ze.jsx)("p", {
                             children: "This Git tree is in a detached HEAD state."
                         }), (0, ze.jsx)("p", {
                             children: "Please commit the latest changes and push to GitHub to continue."
                         })]
                     })
                 }
             },
-            Nc = (0, et.Z)("p", {
+            Bc = (0, et.Z)("p", {
                 target: "epbg7au0"
             })((() => ({
                 textAlign: "justify"
             })), "");
-        const Lc = function(e) {
+        const jc = function(e) {
             return {
                 title: "Unable to deploy",
-                body: (0, ze.jsxs)(Nc, {
+                body: (0, ze.jsxs)(Bc, {
                     children: ["The app\u2019s main file ", (0, ze.jsx)("code", {
                         children: e
                     }), " has not been pushed to GitHub. Please add it to continue."]
                 })
             }
         };
-        const Ic = function() {
+        const Fc = function() {
             return {
                 title: "Unable to deploy",
-                body: (0, ze.jsxs)(Nc, {
+                body: (0, ze.jsxs)(Bc, {
                     children: ["The app\u2019s code is not connected to a remote GitHub repository. To deploy on Streamlit Community Cloud, please put your code in a GitHub repository and publish the current branch. Read more in", " ", (0, ze.jsx)("a", {
-                        href: ac,
+                        href: pc,
                         rel: "noopener noreferrer",
                         target: "_blank",
                         children: "our documentation"
                     }), "."]
                 })
             }
         };
-        const Pc = function(e) {
+        const Uc = function(e) {
             const {
                 children: t,
                 onClose: n
             } = e;
             return (0, ze.jsxs)(cr, {
                 isOpen: !0,
                 closeable: !0,
@@ -124878,108 +125151,108 @@
                 children: [(0, ze.jsx)(ir, {
                     children: "Deploy this app"
                 }), (0, ze.jsx)(ar, {
                     children: t
                 })]
             })
         };
-        var Dc = n.createContext(0);
-        var Bc = ["children"],
-            jc = ["action", "children", "hasThumbnail", "headerImage", "thumbnail", "title", "overrides"];
+        var Vc = n.createContext(0);
+        var Hc = ["children"],
+            Xc = ["action", "children", "hasThumbnail", "headerImage", "thumbnail", "title", "overrides"];
 
-        function Fc() {
-            return Fc = Object.assign ? Object.assign.bind() : function(e) {
+        function Gc() {
+            return Gc = Object.assign ? Object.assign.bind() : function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
-            }, Fc.apply(this, arguments)
+            }, Gc.apply(this, arguments)
         }
 
-        function Uc(e, t) {
+        function $c(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     i = Object.keys(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var i = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
         }
-        var Vc = function(e) {
+        var Kc = function(e) {
             var t = e.children,
-                r = Uc(e, Bc),
+                r = $c(e, Hc),
                 o = ["", "h1", "h2", "h3", "h4", "h5", "h6"];
-            return n.createElement(Dc.Consumer, null, (function(e) {
-                return n.createElement(Tc, Fc({
+            return n.createElement(Vc.Consumer, null, (function(e) {
+                return n.createElement(Lc, Gc({
                     $as: o[e]
                 }, r), t)
             }))
         };
 
-        function Hc(e) {
+        function Yc(e) {
             var t = e.action,
                 r = e.children,
                 o = e.hasThumbnail,
                 i = e.headerImage,
                 a = e.thumbnail,
                 s = e.title,
                 l = e.overrides,
-                c = Uc(e, jc),
+                c = $c(e, Xc),
                 u = l.Action,
                 p = l.Body,
                 d = l.Contents,
                 b = l.HeaderImage,
                 f = l.Root,
                 h = l.Thumbnail,
                 m = l.Title,
-                M = (0, lt.XG)(u) || Sc,
-                O = (0, lt.XG)(p) || qc,
-                g = (0, lt.XG)(d) || Ec,
-                z = (0, lt.XG)(b) || _c,
-                y = (0, lt.XG)(f) || xc,
-                A = (0, lt.XG)(h) || Rc,
-                v = (0, lt.XG)(m) || Vc,
+                M = (0, lt.XG)(u) || Rc,
+                O = (0, lt.XG)(p) || Tc,
+                g = (0, lt.XG)(d) || kc,
+                z = (0, lt.XG)(b) || Cc,
+                y = (0, lt.XG)(f) || Wc,
+                A = (0, lt.XG)(h) || Nc,
+                v = (0, lt.XG)(m) || Kc,
                 w = "string" === typeof i ? {
                     src: i
                 } : i,
                 S = o(e);
-            return n.createElement(y, Fc({
+            return n.createElement(y, Gc({
                 "data-baseweb": "card"
-            }, c, (0, lt.ch)(f)), i && n.createElement(z, Fc({}, w, (0, lt.ch)(b))), n.createElement(g, (0, lt.ch)(d), a && n.createElement(A, Fc({
+            }, c, (0, lt.ch)(f)), i && n.createElement(z, Gc({}, w, (0, lt.ch)(b))), n.createElement(g, (0, lt.ch)(d), a && n.createElement(A, Gc({
                 src: a
-            }, (0, lt.ch)(h))), s && n.createElement(v, Fc({
+            }, (0, lt.ch)(h))), s && n.createElement(v, Gc({
                 $hasThumbnail: S
             }, (0, lt.ch)(m)), s), n.createElement(O, (0, lt.ch)(p), r), t && n.createElement(M, (0, lt.ch)(u), t)))
         }
-        Hc.defaultProps = {
+        Yc.defaultProps = {
             action: null,
             children: null,
             hasThumbnail: function(e) {
                 return !!e.thumbnail
             },
             overrides: {}
         };
-        const Xc = Hc;
-        const Gc = function(e) {
+        const Zc = Yc;
+        const Jc = function(e) {
                 const {
                     colors: t,
                     spacing: n,
                     radii: r,
                     breakpoints: o
                 } = (0, _e.u)(), {
                     children: i
                 } = e;
-                return (0, ze.jsx)(Xc, {
+                return (0, ze.jsx)(Zc, {
                     overrides: {
                         Root: {
                             style: {
                                 borderTopWidth: "1px",
                                 borderBottomWidth: "1px",
                                 borderLeftWidth: "1px",
                                 borderRightWidth: "1px",
@@ -125017,15 +125290,15 @@
                                 }
                             }
                         }
                     },
                     children: i
                 })
             },
-            $c = (0, et.Z)("div", {
+            Qc = (0, et.Z)("div", {
                 target: "e97l2ve3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontFamily: t.fonts.sansSerif,
@@ -125035,30 +125308,30 @@
                     marginTop: t.spacing.twoXL,
                     marginBottom: t.spacing.md,
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         marginTop: t.spacing.md
                     }
                 }
             }), ""),
-            Kc = (0, et.Z)("div", {
+            eu = (0, et.Z)("div", {
                 target: "e97l2ve2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "grid",
                     gridTemplateColumns: "1fr 1fr",
                     gridGap: t.spacing.twoXL,
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         gridTemplateColumns: "1fr"
                     }
                 }
             }), ""),
-            Yc = (0, et.Z)("div", {
+            tu = (0, et.Z)("div", {
                 target: "e97l2ve1"
             })((e => {
                 let {
                     theme: t,
                     extraSpacing: n
                 } = e;
                 return {
@@ -125073,15 +125346,15 @@
                     },
                     "& > img": {
                         position: "absolute",
                         marginTop: t.spacing.sm
                     }
                 }
             }), ""),
-            Zc = (0, et.Z)("div", {
+            nu = (0, et.Z)("div", {
                 target: "e97l2ve0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
@@ -125090,174 +125363,174 @@
                         marginRight: t.spacing.twoXL
                     },
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         marginTop: t.spacing.xl
                     }
                 }
             }), "");
-        const Jc = __webpack_require__.p + "static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg";
-        const Qc = function(e) {
+        const ru = __webpack_require__.p + "static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg";
+        const ou = function(e) {
                 const {
                     children: t,
                     extraSpacing: n
                 } = e;
-                return (0, ze.jsxs)(Yc, {
+                return (0, ze.jsxs)(tu, {
                     extraSpacing: n,
                     children: [(0, ze.jsx)("img", {
-                        src: Jc,
+                        src: ru,
                         alt: "Checkmark"
                     }), (0, ze.jsx)("span", {
                         children: t
                     })]
                 })
             },
             {
-                GitStates: eu
+                GitStates: iu
             } = je.ef,
-            tu = e => {
+            au = e => {
                 window.open(e, "_blank")
             },
-            nu = e => {
+            su = e => {
                 if (e) {
                     const t = new URL("https://share.streamlit.io/deploy");
                     return t.searchParams.set("repository", e.repository || ""), t.searchParams.set("branch", e.branch || ""), t.searchParams.set("mainModule", e.module || ""), t.toString()
                 }
                 return "https://streamlit.io/cloud"
             };
 
-        function ru(e) {
+        function lu(e) {
             const {
                 gitInfo: t
             } = (0, n.useContext)(Fe), {
                 onClose: r,
                 metricsMgr: o
             } = e, i = (0, n.useCallback)((() => {
                 const {
                     showDeployError: n,
                     isDeployErrorModalOpen: o,
                     metricsMgr: i
                 } = e;
                 if (i.enqueue("menuClick", {
                         label: "deployButtonInDialog"
                     }), !t) {
-                    const e = Ic();
+                    const e = Fc();
                     return void n(e.title, e.body)
                 }
                 const {
                     repository: a,
                     branch: s,
                     module: l,
                     untrackedFiles: c,
                     state: u
                 } = t;
-                if ((!a || !s || !l) && u === eu.DEFAULT) {
-                    const e = Ic();
+                if ((!a || !s || !l) && u === iu.DEFAULT) {
+                    const e = Fc();
                     n(e.title, e.body)
-                } else if (u !== eu.HEAD_DETACHED)
+                } else if (u !== iu.HEAD_DETACHED)
                     if (l && null !== c && void 0 !== c && c.includes(l)) {
-                        const e = Lc(l);
+                        const e = jc(l);
                         n(e.title, e.body)
-                    } else o && r(), tu(nu(t));
+                    } else o && r(), au(su(t));
                 else {
-                    const e = Wc();
+                    const e = Dc();
                     n(e.title, e.body)
                 }
             }), [e, r, t]);
-            return (0, ze.jsx)(Pc, {
+            return (0, ze.jsx)(Uc, {
                 onClose: r,
-                children: (0, ze.jsxs)(Kc, {
-                    children: [(0, ze.jsxs)(Gc, {
-                        children: [(0, ze.jsxs)(qc, {
+                children: (0, ze.jsxs)(eu, {
+                    children: [(0, ze.jsxs)(Jc, {
+                        children: [(0, ze.jsxs)(Tc, {
                             children: [(0, ze.jsx)("img", {
-                                src: kc,
+                                src: Ic,
                                 alt: "Streamlit Logo",
                                 "data-testid": "stDeployDialogCommunityCloudIcon"
-                            }), (0, ze.jsx)($c, {
-                                children: "Streamlit Community Cloud"
                             }), (0, ze.jsx)(Qc, {
+                                children: "Streamlit Community Cloud"
+                            }), (0, ze.jsx)(ou, {
                                 extraSpacing: !0,
                                 children: "For the community"
-                            }), (0, ze.jsx)(Qc, {
+                            }), (0, ze.jsx)(ou, {
                                 extraSpacing: !0,
                                 children: "Deploy unlimited public apps for free"
-                            }), (0, ze.jsx)(Qc, {
+                            }), (0, ze.jsx)(ou, {
                                 extraSpacing: !0,
                                 children: "Apps are discoverable through the Streamlit gallery and search engines"
                             })]
-                        }), (0, ze.jsx)(Sc, {
-                            children: (0, ze.jsxs)(Zc, {
+                        }), (0, ze.jsx)(Rc, {
+                            children: (0, ze.jsxs)(nu, {
                                 children: [(0, ze.jsx)(sn.ZP, {
                                     kind: ln.nW.SECONDARY,
                                     onClick: i,
                                     children: "Deploy now"
                                 }), (0, ze.jsx)(sn.ZP, {
                                     onClick: () => {
                                         o.enqueue("menuClick", {
                                             label: "readMoreCommunityCloudInDeployDialog"
-                                        }), tu(ac)
+                                        }), au(pc)
                                     },
                                     kind: ln.nW.MINIMAL,
                                     children: "Read more"
                                 })]
                             })
                         })]
-                    }), (0, ze.jsxs)(Gc, {
-                        children: [(0, ze.jsxs)(qc, {
+                    }), (0, ze.jsxs)(Jc, {
+                        children: [(0, ze.jsxs)(Tc, {
                             children: [(0, ze.jsx)("img", {
-                                src: Cc,
+                                src: Pc,
                                 alt: "Rocket",
                                 "data-testid": "stDeployDialogCustomDeploymentIcon"
-                            }), (0, ze.jsx)($c, {
-                                children: "Custom deployment"
                             }), (0, ze.jsx)(Qc, {
+                                children: "Custom deployment"
+                            }), (0, ze.jsx)(ou, {
                                 children: "For companies"
-                            }), (0, ze.jsx)(Qc, {
+                            }), (0, ze.jsx)(ou, {
                                 children: "Deploy on your own hardware or in the cloud, with Docker, Kubernetes, etc"
-                            }), (0, ze.jsx)(Qc, {
+                            }), (0, ze.jsx)(ou, {
                                 children: "Set up your own authentication"
                             })]
-                        }), (0, ze.jsx)(Sc, {
-                            children: (0, ze.jsx)(Zc, {
+                        }), (0, ze.jsx)(Rc, {
+                            children: (0, ze.jsx)(nu, {
                                 children: (0, ze.jsx)(sn.ZP, {
                                     onClick: () => {
                                         o.enqueue("menuClick", {
                                             label: "readMoreDeployTutorialInDeployDialog"
-                                        }), tu(sc)
+                                        }), au(dc)
                                     },
                                     kind: ln.nW.MINIMAL,
                                     children: "Read more"
                                 })
                             })
                         })]
                     })]
                 })
             })
         }
-        let ou;
+        let cu;
 
-        function iu(e) {
+        function uu(e) {
             switch (e.type) {
-                case ou.ABOUT:
+                case cu.ABOUT:
                     return function(e) {
                         if (e.aboutSectionMd) {
                             const t = {
                                     overflowY: "auto",
                                     overflowX: "hidden",
                                     maxHeight: "35vh"
                                 },
                                 n = "  \n",
-                                r = ["Made with Streamlit v".concat(e.sessionInfo.current.streamlitVersion), ic, "Copyright ".concat((new Date).getFullYear(), " Snowflake Inc. All rights reserved.")].join(n),
+                                r = ["Made with Streamlit v".concat(e.sessionInfo.current.streamlitVersion), uc, "Copyright ".concat((new Date).getFullYear(), " Snowflake Inc. All rights reserved.")].join(n),
                                 o = "".concat(e.aboutSectionMd, " ").concat(n, " ").concat(n, " ").concat(r);
                             return (0, ze.jsxs)(cr, {
                                 isOpen: !0,
                                 onClose: e.onClose,
                                 children: [(0, ze.jsx)(ir, {
                                     children: "About"
                                 }), (0, ze.jsx)(ar, {
-                                    children: (0, ze.jsx)(nc, {
+                                    children: (0, ze.jsx)(sc, {
                                         children: (0, ze.jsx)(Zt.ZP, {
                                             source: o,
                                             allowHTML: !1,
                                             style: t
                                         })
                                     })
                                 })]
@@ -125268,23 +125541,23 @@
                             onClose: e.onClose,
                             children: [(0, ze.jsx)(ir, {
                                 children: "Made with"
                             }), (0, ze.jsx)(ar, {
                                 children: (0, ze.jsxs)("div", {
                                     children: [e.sessionInfo.isSet && (0, ze.jsxs)(ze.Fragment, {
                                         children: ["Streamlit v", e.sessionInfo.current.streamlitVersion, (0, ze.jsx)("br", {})]
-                                    }), (0, ze.jsx)(rc, {
-                                        href: ic,
-                                        children: ic
+                                    }), (0, ze.jsx)(lc, {
+                                        href: uc,
+                                        children: uc
                                     }), (0, ze.jsx)("br", {}), "Copyright ", (new Date).getFullYear(), " Snowflake Inc. All rights reserved."]
                                 })
                             })]
                         })
                     }(e);
-                case ou.CLEAR_CACHE:
+                case cu.CLEAR_CACHE:
                     return function(e) {
                         const t = {
                             enter: () => e.defaultAction()
                         };
                         return (0, ze.jsx)(Ie.HotKeys, {
                             handlers: t,
                             attach: window,
@@ -125319,30 +125592,30 @@
                                             children: "Clear caches"
                                         })]
                                     })]
                                 })
                             })
                         })
                     }(e);
-                case ou.RERUN_SCRIPT:
+                case cu.RERUN_SCRIPT:
                     return function(e) {
                         const t = {
                             enter: () => e.defaultAction()
                         };
                         return (0, ze.jsx)(Ie.HotKeys, {
                             handlers: t,
                             attach: window,
                             children: (0, ze.jsxs)(cr, {
                                 isOpen: !0,
                                 onClose: e.onClose,
                                 children: [(0, ze.jsxs)(ar, {
-                                    children: [(0, ze.jsx)(Vl, {
+                                    children: [(0, ze.jsx)(Kl, {
                                         children: "Command line:"
                                     }), (0, ze.jsx)("div", {
-                                        children: (0, ze.jsx)(Hl, {
+                                        children: (0, ze.jsx)(Yl, {
                                             autoFocus: !0,
                                             className: "command-line",
                                             value: e.getCommandLine(),
                                             onChange: t => e.setCommandLine(t.target.value)
                                         })
                                     })]
                                 }), (0, ze.jsxs)(sr, {
@@ -125355,23 +125628,23 @@
                                         onClick: () => e.rerunCallback(),
                                         children: "Rerun"
                                     })]
                                 })]
                             })
                         })
                     }(e);
-                case ou.SETTINGS:
-                    return t = e, (0, ze.jsx)(cc, {
+                case cu.SETTINGS:
+                    return t = e, (0, ze.jsx)(fc, {
                         ...t
                     });
-                case ou.SCRIPT_CHANGED:
-                    return (0, ze.jsx)(oc, {
+                case cu.SCRIPT_CHANGED:
+                    return (0, ze.jsx)(cc, {
                         ...e
                     });
-                case ou.SCRIPT_COMPILE_ERROR:
+                case cu.SCRIPT_COMPILE_ERROR:
                     return function(e) {
                         return (0, ze.jsxs)(cr, {
                             isOpen: !0,
                             onClose: e.onClose,
                             size: "auto",
                             autoFocus: !1,
                             children: [(0, ze.jsx)(ir, {
@@ -125389,35 +125662,35 @@
                                     kind: ln.nW.SECONDARY,
                                     onClick: e.onClose,
                                     children: "Close"
                                 })
                             })]
                         })
                     }(e);
-                case ou.THEME_CREATOR:
-                    return (0, ze.jsx)(zc, {
+                case cu.THEME_CREATOR:
+                    return (0, ze.jsx)(Sc, {
                         ...e
                     });
-                case ou.WARNING:
+                case cu.WARNING:
                     return function(e) {
                         return (0, ze.jsxs)(cr, {
                             isOpen: !0,
                             onClose: e.onClose,
                             children: [(0, ze.jsx)(ir, {
                                 children: e.title
                             }), (0, ze.jsx)(ar, {
                                 children: e.msg
                             })]
                         })
                     }(e);
-                case ou.DEPLOY_DIALOG:
-                    return (0, ze.jsx)(ru, {
+                case cu.DEPLOY_DIALOG:
+                    return (0, ze.jsx)(lu, {
                         ...e
                     });
-                case ou.DEPLOY_ERROR:
+                case cu.DEPLOY_ERROR:
                     return function(e) {
                         let {
                             title: t,
                             msg: n,
                             onClose: r,
                             onContinue: o,
                             onTryAgain: i
@@ -125427,15 +125700,15 @@
                         };
                         return (0, ze.jsxs)(cr, {
                             isOpen: !0,
                             onClose: r,
                             children: [(0, ze.jsx)(ir, {
                                 children: t
                             }), (0, ze.jsx)(ar, {
-                                children: (0, ze.jsx)(tc, {
+                                children: (0, ze.jsx)(ac, {
                                     children: n
                                 })
                             }), (0, ze.jsxs)(sr, {
                                 children: [(0, ze.jsx)(lr, {
                                     kind: ln.nW.TERTIARY,
                                     onClick: i,
                                     children: "Try again"
@@ -125467,28 +125740,28 @@
                             })
                         })
                     }(e)
             }
             var t
         }! function(e) {
             e.ABOUT = "about", e.CLEAR_CACHE = "clearCache", e.RERUN_SCRIPT = "rerunScript", e.SETTINGS = "settings", e.SCRIPT_CHANGED = "scriptChanged", e.SCRIPT_COMPILE_ERROR = "scriptCompileError", e.THEME_CREATOR = "themeCreator", e.WARNING = "warning", e.DEPLOY_ERROR = "deployError", e.DEPLOY_DIALOG = "deployDialog"
-        }(ou || (ou = {}));
-        var au = __webpack_require__(16840),
-            su = __webpack_require__.n(au);
-        const lu = /\/+$/,
-            cu = /^\/+/;
+        }(cu || (cu = {}));
+        var pu = __webpack_require__(16840),
+            du = __webpack_require__.n(pu);
+        const bu = /\/+$/,
+            fu = /^\/+/;
 
-        function uu() {
+        function hu() {
             const e = function() {
                     const e = window.location.hostname;
                     let t;
-                    return t = Ss.td ? Ss.Id : window.location.port ? Number(window.location.port) : bu() ? 443 : 80, {
+                    return t = xs.td ? xs.Id : window.location.port ? Number(window.location.port) : Ou() ? 443 : 80, {
                         host: e,
                         port: t,
-                        basePath: window.location.pathname.replace(lu, "").replace(cu, "")
+                        basePath: window.location.pathname.replace(bu, "").replace(fu, "")
                     }
                 }(),
                 {
                     basePath: t
                 } = e;
             if (!t) return [e];
             const n = t.split("/"),
@@ -125496,45 +125769,45 @@
             for (; n.length > 0;) r.push({
                 ...e,
                 basePath: n.join("/")
             }), n.pop();
             return r.push({
                 ...e,
                 basePath: ""
-            }), su()(r, 2)
+            }), du()(r, 2)
         }
 
-        function pu(e, t) {
+        function mu(e, t) {
             let {
                 host: n,
                 port: r,
                 basePath: o
             } = e;
-            const i = bu() ? "https" : "http",
-                a = du(o, t);
+            const i = Ou() ? "https" : "http",
+                a = Mu(o, t);
             return "".concat(i, "://").concat(n, ":").concat(r, "/").concat(a)
         }
 
-        function du(e, t) {
-            return e = e.replace(lu, "").replace(cu, ""), t = t.replace(lu, "").replace(cu, ""), 0 === e.length ? t : "".concat(e, "/").concat(t)
+        function Mu(e, t) {
+            return e = e.replace(bu, "").replace(fu, ""), t = t.replace(bu, "").replace(fu, ""), 0 === e.length ? t : "".concat(e, "/").concat(t)
         }
 
-        function bu() {
+        function Ou() {
             return window.location.href.startsWith("https://")
         }
-        var fu = __webpack_require__(18080);
-        class hu {
+        var gu = __webpack_require__(18080);
+        class zu {
             getAge(e) {
                 return e - this.scriptRunCount
             }
             constructor(e, t) {
                 this.encodedMsg = void 0, this.scriptRunCount = 0, this.encodedMsg = e, this.scriptRunCount = t
             }
         }
-        class mu {
+        class yu {
             constructor(e) {
                 this.messages = new Map, this.endpoints = void 0, this.scriptRunCount = 0, this.endpoints = e
             }
             incrementRunCount(e) {
                 this.scriptRunCount += 1, this.messages.forEach(((t, n) => {
                     t.getAge(this.scriptRunCount) > e && ((0, ui.ji)("Removing expired ForwardMsg [hash=".concat(n, "]")), this.messages.delete(n))
                 }))
@@ -125553,212 +125826,212 @@
                     }
                     this.maybeCacheMessage(n, t)
                 }
                 if (!e.metadata) throw new Error("ForwardMsg has no metadata");
                 return n.metadata = je.eI.decode(t).metadata, n
             }
             maybeCacheMessage(e, t) {
-                "refHash" !== e.type && e.metadata && e.metadata.cacheable && void 0 === this.getCachedMessage(e.hash, !0) && ((0, ui.ji)("Caching ForwardMsg [hash=".concat(e.hash, "]")), this.messages.set(e.hash, new hu(t, this.scriptRunCount)))
+                "refHash" !== e.type && e.metadata && e.metadata.cacheable && void 0 === this.getCachedMessage(e.hash, !0) && ((0, ui.ji)("Caching ForwardMsg [hash=".concat(e.hash, "]")), this.messages.set(e.hash, new zu(t, this.scriptRunCount)))
             }
             getCachedMessage(e, t) {
                 const n = this.messages.get(e);
                 if (null != n) return t && (n.scriptRunCount = this.scriptRunCount), je.eI.decode(n.encodedMsg)
             }
         }
 
-        function Mu(e, t, n) {
+        function Au(e, t, n) {
             for (let r = "number" === typeof t ? t : e.indexOf(t); r < e.length; ++r)
                 if (n(e[r])) return r
         }
 
-        function Ou(e, t, n) {
+        function vu(e, t, n) {
             for (let r = "number" === typeof t ? t : e.indexOf(t); r >= 0; --r) {
                 if (n(e[r])) return r
             }
         }
 
-        function gu(e) {
+        function wu(e) {
             return void 0 !== e.messageIndex
         }
 
-        function zu(e, t) {
+        function Su(e, t) {
             return Math.abs(t.timestamp - e.timestamp)
         }
-        class yu {
+        class qu {
             constructor(e, t) {
                 this.rerunEvents = void 0, this.requestedRerun = void 0, this.getResults = () => {
                     const e = new Set;
                     if (this.rerunEvents.forEach((t => {
-                            gu(t) && e.add(t.messageIndex)
+                            wu(t) && e.add(t.messageIndex)
                         })), 0 === e.size) return "No rerun messages found!";
-                    const t = Array.from(e).sort(Au),
+                    const t = Array.from(e).sort(Eu),
                         n = this.rerunEvents[this.rerunEvents.length - 1],
                         r = this.rerunEvents[0],
                         o = {
                             messages: t.map(this.getMessageAnalysis),
-                            rerunDuration: zu(r, n)
+                            rerunDuration: Su(r, n)
                         };
-                    return void 0 !== this.requestedRerun && (o.requestedRerun = !0, o.scriptRunStateAtStart = this.requestedRerun.scriptRunState, o.requestToRerunStart = zu(this.requestedRerun, r)), o
+                    return void 0 !== this.requestedRerun && (o.requestedRerun = !0, o.scriptRunStateAtStart = this.requestedRerun.scriptRunState, o.requestToRerunStart = Su(this.requestedRerun, r)), o
                 }, this.getMessageAnalysis = e => {
                     const t = [];
                     let n = 0;
                     for (; n < this.rerunEvents.length;) {
-                        const r = vu(this.rerunEvents, n, e);
+                        const r = _u(this.rerunEvents, n, e);
                         if (void 0 === r) break;
                         t.push(this.rerunEvents[r]), n = r + 1
                     }
                     if (0 === t.length) throw new Error("No messages for the given index: ".concat(e));
                     const r = {
                         messageIndex: e,
-                        duration: zu(t[0], t[t.length - 1]),
+                        duration: Su(t[0], t[t.length - 1]),
                         steps: []
                     };
                     for (let o = 1; o < t.length; ++o) {
                         const e = t[o - 1],
                             n = t[o];
                         "DecodedMessage" === n.name && (r.messageType = n.messageType, r.len = n.len), r.steps.push({
                             name: n.name,
-                            duration: zu(e, n)
+                            duration: Su(e, n)
                         })
                     }
                     return r
                 };
                 const n = function(e, t) {
-                    const n = Ou(e, t - 1, (e => "DecodedMessage" === e.name && "newSession" === e.messageType));
+                    const n = vu(e, t - 1, (e => "DecodedMessage" === e.name && "newSession" === e.messageType));
                     if (void 0 === n) return;
                     const {
                         messageIndex: r
                     } = e[n];
-                    return Ou(e, n, (e => "BeginHandleMessage" === e.name && e.messageIndex === r))
+                    return vu(e, n, (e => "BeginHandleMessage" === e.name && e.messageIndex === r))
                 }(e, t);
                 if (void 0 === n) throw new Error("Unable to find run start!");
                 this.rerunEvents = e.slice(n, t + 1), this.requestedRerun = function(e, t, n) {
-                    const r = Ou(e, t, n);
+                    const r = vu(e, t, n);
                     return void 0 !== r ? e[r] : void 0
                 }(e, n - 1, (e => "RequestedRerun" === e.name))
             }
         }
 
-        function Au(e, t) {
+        function Eu(e, t) {
             return e < t ? -1 : e > t ? 1 : 0
         }
 
-        function vu(e, t, n) {
-            return Mu(e, t, (e => gu(e) && e.messageIndex === n))
+        function _u(e, t, n) {
+            return Au(e, t, (e => wu(e) && e.messageIndex === n))
         }
-        class wu {
+        class xu {
             static record(e) {
                 var t, n;
-                this.enabled && (e.timestamp = performance.now(), this.events.push(e), "DispatchedMessage" === e.name && "scriptFinished" === e.messageType && ((0, ui.ji)("Rerun results", (t = this.events, new yu(t, null !== n && void 0 !== n ? n : t.length - 1).getResults())), this.events = []))
+                this.enabled && (e.timestamp = performance.now(), this.events.push(e), "DispatchedMessage" === e.name && "scriptFinished" === e.messageType && ((0, ui.ji)("Rerun results", (t = this.events, new qu(t, null !== n && void 0 !== n ? n : t.length - 1).getResults())), this.events = []))
             }
         }
-        wu.enabled = !1, wu.events = [];
-        class Su {
+        xu.enabled = !1, xu.events = [];
+        class Ru {
             constructor() {
                 this.resolve = void 0, this.reject = void 0, this.promise = void 0, this.resolve = () => {}, this.reject = () => {}, this.promise = new Promise(((e, t) => {
                     this.resolve = e, this.reject = t
                 }))
             }
         }
-        const qu = "WebsocketConnection",
-            Eu = "_stcore/health",
-            _u = "_stcore/host-config",
-            xu = 15e3,
-            Ru = "https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS";
-        class Tu {
+        const Tu = "WebsocketConnection",
+            ku = "_stcore/health",
+            Cu = "_stcore/host-config",
+            Wu = 15e3,
+            Nu = "https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS";
+        class Lu {
             constructor(e) {
-                this.args = void 0, this.cache = void 0, this.uriIndex = 0, this.lastDispatchedMessageIndex = -1, this.nextMessageIndex = 0, this.messageQueue = {}, this.state = Us.INITIAL, this.websocket = void 0, this.wsConnectionTimeoutId = void 0, this.args = e, this.cache = new mu(e.endpoints), this.stepFsm("INITIALIZED")
+                this.args = void 0, this.cache = void 0, this.uriIndex = 0, this.lastDispatchedMessageIndex = -1, this.nextMessageIndex = 0, this.messageQueue = {}, this.state = Gs.INITIAL, this.websocket = void 0, this.wsConnectionTimeoutId = void 0, this.args = e, this.cache = new yu(e.endpoints), this.stepFsm("INITIALIZED")
             }
             getBaseUriParts() {
-                if (this.state === Us.CONNECTED) return this.args.baseUriPartsList[this.uriIndex]
+                if (this.state === Gs.CONNECTED) return this.args.baseUriPartsList[this.uriIndex]
             }
             disconnect() {
-                this.setFsmState(Us.DISCONNECTED_FOREVER)
+                this.setFsmState(Gs.DISCONNECTED_FOREVER)
             }
             setFsmState(e, t) {
-                if ((0, ui.ji)(qu, "New state: ".concat(e)), this.state = e, this.state === Us.PINGING_SERVER) this.pingServer();
+                if ((0, ui.ji)(Tu, "New state: ".concat(e)), this.state = e, this.state === Gs.PINGING_SERVER) this.pingServer();
                 switch (this.args.onConnectionStateChange(e, t), this.state) {
-                    case Us.CONNECTING:
+                    case Gs.CONNECTING:
                         this.connectToWebSocket();
                         break;
-                    case Us.DISCONNECTED_FOREVER:
+                    case Gs.DISCONNECTED_FOREVER:
                         this.closeConnection()
                 }
             }
             stepFsm(e, t) {
-                if ((0, ui.ji)(qu, "State: ".concat(this.state, "; Event: ").concat(e)), "FATAL_ERROR" !== e || this.state === Us.DISCONNECTED_FOREVER) {
+                if ((0, ui.ji)(Tu, "State: ".concat(this.state, "; Event: ").concat(e)), "FATAL_ERROR" !== e || this.state === Gs.DISCONNECTED_FOREVER) {
                     switch (this.state) {
-                        case Us.INITIAL:
-                            if ("INITIALIZED" === e) return void this.setFsmState(Us.PINGING_SERVER);
+                        case Gs.INITIAL:
+                            if ("INITIALIZED" === e) return void this.setFsmState(Gs.PINGING_SERVER);
                             break;
-                        case Us.CONNECTING:
-                            if ("CONNECTION_SUCCEEDED" === e) return void this.setFsmState(Us.CONNECTED);
-                            if ("CONNECTION_TIMED_OUT" === e || "CONNECTION_ERROR" === e || "CONNECTION_CLOSED" === e) return void this.setFsmState(Us.PINGING_SERVER);
+                        case Gs.CONNECTING:
+                            if ("CONNECTION_SUCCEEDED" === e) return void this.setFsmState(Gs.CONNECTED);
+                            if ("CONNECTION_TIMED_OUT" === e || "CONNECTION_ERROR" === e || "CONNECTION_CLOSED" === e) return void this.setFsmState(Gs.PINGING_SERVER);
                             break;
-                        case Us.CONNECTED:
-                            if ("CONNECTION_CLOSED" === e || "CONNECTION_ERROR" === e) return void this.setFsmState(Us.PINGING_SERVER);
+                        case Gs.CONNECTED:
+                            if ("CONNECTION_CLOSED" === e || "CONNECTION_ERROR" === e) return void this.setFsmState(Gs.PINGING_SERVER);
                             break;
-                        case Us.PINGING_SERVER:
-                            if ("SERVER_PING_SUCCEEDED" === e) return void this.setFsmState(Us.CONNECTING);
+                        case Gs.PINGING_SERVER:
+                            if ("SERVER_PING_SUCCEEDED" === e) return void this.setFsmState(Gs.CONNECTING);
                             break;
-                        case Us.DISCONNECTED_FOREVER:
-                            return void(0, ui.KE)(qu, "Discarding ".concat(e, " while in ").concat(Us.DISCONNECTED_FOREVER))
+                        case Gs.DISCONNECTED_FOREVER:
+                            return void(0, ui.KE)(Tu, "Discarding ".concat(e, " while in ").concat(Gs.DISCONNECTED_FOREVER))
                     }
                     throw new Error("Unsupported state transition.\n" + "State: ".concat(this.state, "\n") + "Event: ".concat(e))
                 }
-                this.setFsmState(Us.DISCONNECTED_FOREVER, t)
+                this.setFsmState(Gs.DISCONNECTED_FOREVER, t)
             }
             async pingServer() {
                 this.uriIndex = await
                 function(e, t, r, o, i) {
-                    const a = new Su;
+                    const a = new Ru;
                     let s = 0,
                         l = 0,
                         c = () => {};
                     const u = () => {
                             l++, l >= e.length && (l = 0), c()
                         },
                         p = e => {
                             const n = .4 * Math.random() - .2,
                                 i = 1 === s ? t : t * 2 ** (s - 1) * (1 + n),
                                 a = Math.min(r, i);
                             o(s, e, a), window.setTimeout(u, a)
                         },
                         d = () => {
                             const t = e[l];
-                            "localhost" === new URL(pu(t, "")).hostname ? p((0, ze.jsxs)(n.Fragment, {
+                            "localhost" === new URL(mu(t, "")).hostname ? p((0, ze.jsxs)(n.Fragment, {
                                 children: [(0, ze.jsx)("p", {
                                     children: "Is Streamlit still running? If you accidentally stopped Streamlit, just restart it in your terminal:"
                                 }), (0, ze.jsx)("pre", {
-                                    children: (0, ze.jsx)(ku, {
+                                    children: (0, ze.jsx)(Iu, {
                                         children: "streamlit run yourscript.py"
                                     })
                                 })]
                             })) : p("Connection failed with status 0.")
                         },
                         b = () => {
                             p((0, ze.jsxs)(n.Fragment, {
                                 children: [(0, ze.jsx)("p", {
                                     children: "Cannot connect to Streamlit (HTTP status: 403)."
                                 }), (0, ze.jsxs)("p", {
                                     children: ["If you are trying to access a Streamlit app running on another server, this could be due to the app's", " ", (0, ze.jsx)("a", {
-                                        href: Ru,
+                                        href: Nu,
                                         children: "CORS"
                                     }), " settings."]
                                 })]
                             }))
                         };
                     return c = () => {
                         const t = e[l],
-                            n = pu(t, Eu),
-                            r = pu(t, _u);
-                        (0, ui.ji)(qu, "Attempting to connect to ".concat(n, ".")), 0 === l && s++, Promise.all([fu.Z.get(n, {
-                            timeout: xu
-                        }), fu.Z.get(r, {
-                            timeout: xu
+                            n = mu(t, ku),
+                            r = mu(t, Cu);
+                        (0, ui.ji)(Tu, "Attempting to connect to ".concat(n, ".")), 0 === l && s++, Promise.all([gu.Z.get(n, {
+                            timeout: Wu
+                        }), gu.Z.get(r, {
+                            timeout: Wu
                         })]).then((e => {
                             let [t, n] = e;
                             i(n.data), a.resolve(l)
                         })).catch((e => {
                             if ("ECONNABORTED" === e.code) return p("Connection timed out.");
                             if (e.response) {
                                 const {
@@ -125780,148 +126053,148 @@
             async connectToWebSocket() {
                 const e = function(e, t) {
                     let {
                         host: n,
                         port: r,
                         basePath: o
                     } = e;
-                    const i = bu() ? "wss" : "ws",
-                        a = du(o, t);
+                    const i = Ou() ? "wss" : "ws",
+                        a = Mu(o, t);
                     return "".concat(i, "://").concat(n, ":").concat(r, "/").concat(a)
                 }(this.args.baseUriPartsList[this.uriIndex], "_stcore/stream");
                 if (null != this.websocket) throw new Error("Websocket already exists");
-                (0, ui.ji)(qu, "creating WebSocket");
+                (0, ui.ji)(Tu, "creating WebSocket");
                 const t = await this.getSessionTokens();
                 this.websocket = new WebSocket(e, ["streamlit", ...t]), this.websocket.binaryType = "arraybuffer", this.setConnectionTimeout(e);
                 const n = this.websocket,
                     r = () => n === this.websocket;
                 this.websocket.onmessage = e => {
                     r() && this.handleMessage(e.data).catch((e => {
                         const t = "Failed to process a Websocket message (".concat(e, ")");
-                        (0, ui.H)(qu, t), this.stepFsm("FATAL_ERROR", t)
+                        (0, ui.H)(Tu, t), this.stepFsm("FATAL_ERROR", t)
                     }))
                 }, this.websocket.onopen = () => {
-                    r() && ((0, ui.ji)(qu, "WebSocket onopen"), this.stepFsm("CONNECTION_SUCCEEDED"))
+                    r() && ((0, ui.ji)(Tu, "WebSocket onopen"), this.stepFsm("CONNECTION_SUCCEEDED"))
                 }, this.websocket.onclose = () => {
-                    r() && ((0, ui.KE)(qu, "WebSocket onclose"), this.closeConnection(), this.stepFsm("CONNECTION_CLOSED"))
+                    r() && ((0, ui.KE)(Tu, "WebSocket onclose"), this.closeConnection(), this.stepFsm("CONNECTION_CLOSED"))
                 }, this.websocket.onerror = () => {
-                    r() && ((0, ui.H)(qu, "WebSocket onerror"), this.closeConnection(), this.stepFsm("CONNECTION_ERROR"))
+                    r() && ((0, ui.H)(Tu, "WebSocket onerror"), this.closeConnection(), this.stepFsm("CONNECTION_ERROR"))
                 }
             }
             setConnectionTimeout(e) {
                 if (null != this.wsConnectionTimeoutId) throw new Error("WS timeout is already set");
                 const t = this.websocket;
                 this.wsConnectionTimeoutId = window.setTimeout((() => {
                     if (t === this.websocket) {
-                        if (null != this.wsConnectionTimeoutId) return null == this.websocket ? (this.closeConnection(), void this.stepFsm("FATAL_ERROR", "Null Websocket in setConnectionTimeout")) : void(0 === this.websocket.readyState && ((0, ui.ji)(qu, "".concat(e, " timed out")), this.closeConnection(), this.stepFsm("CONNECTION_TIMED_OUT")));
-                        (0, ui.KE)(qu, "Timeout fired after cancellation")
+                        if (null != this.wsConnectionTimeoutId) return null == this.websocket ? (this.closeConnection(), void this.stepFsm("FATAL_ERROR", "Null Websocket in setConnectionTimeout")) : void(0 === this.websocket.readyState && ((0, ui.ji)(Tu, "".concat(e, " timed out")), this.closeConnection(), this.stepFsm("CONNECTION_TIMED_OUT")));
+                        (0, ui.KE)(Tu, "Timeout fired after cancellation")
                     }
-                }), 15e3), (0, ui.ji)(qu, "Set WS timeout ".concat(this.wsConnectionTimeoutId))
+                }), 15e3), (0, ui.ji)(Tu, "Set WS timeout ".concat(this.wsConnectionTimeoutId))
             }
             closeConnection() {
-                this.websocket && (this.websocket.close(), this.websocket = void 0), null != this.wsConnectionTimeoutId && ((0, ui.ji)(qu, "Clearing WS timeout ".concat(this.wsConnectionTimeoutId)), window.clearTimeout(this.wsConnectionTimeoutId), this.wsConnectionTimeoutId = void 0)
+                this.websocket && (this.websocket.close(), this.websocket = void 0), null != this.wsConnectionTimeoutId && ((0, ui.ji)(Tu, "Clearing WS timeout ".concat(this.wsConnectionTimeoutId)), window.clearTimeout(this.wsConnectionTimeoutId), this.wsConnectionTimeoutId = void 0)
             }
             sendMessage(e) {
                 if (!this.websocket) return;
                 const t = je._b.create(e),
                     n = je._b.encode(t).finish();
                 this.websocket.send(n)
             }
             incrementMessageCacheRunCount(e) {
                 this.cache.incrementRunCount(e)
             }
             async handleMessage(e) {
                 const t = this.nextMessageIndex;
-                this.nextMessageIndex += 1, wu.record({
+                this.nextMessageIndex += 1, xu.record({
                     name: "BeginHandleMessage",
                     messageIndex: t
                 });
                 const n = new Uint8Array(e),
                     r = je.eI.decode(n);
-                for (wu.record({
+                for (xu.record({
                         name: "DecodedMessage",
                         messageIndex: t,
                         messageType: r.type,
                         len: e.byteLength
-                    }), this.messageQueue[t] = await this.cache.processMessagePayload(r, n), wu.record({
+                    }), this.messageQueue[t] = await this.cache.processMessagePayload(r, n), xu.record({
                         name: "GotCachedPayload",
                         messageIndex: t
                     }); this.lastDispatchedMessageIndex + 1 in this.messageQueue;) {
                     const e = this.lastDispatchedMessageIndex + 1;
-                    this.args.onMessage(this.messageQueue[e]), wu.record({
+                    this.args.onMessage(this.messageQueue[e]), xu.record({
                         name: "DispatchedMessage",
                         messageIndex: e,
                         messageType: this.messageQueue[e].type
                     }), delete this.messageQueue[e], this.lastDispatchedMessageIndex = e
                 }
             }
         }
-        const ku = (0, et.Z)("code", {
+        const Iu = (0, et.Z)("code", {
             target: "e1xobb530"
         })({
             name: "28m1rt",
             styles: '&::before{content:"$";margin-right:1ex;}'
         });
-        class Cu {
+        class Pu {
             constructor(e) {
-                this.props = void 0, this.connection = void 0, this.connectionState = Us.INITIAL, this.setConnectionState = (e, t) => {
+                this.props = void 0, this.connection = void 0, this.connectionState = Gs.INITIAL, this.setConnectionState = (e, t) => {
                     this.connectionState !== e && (this.connectionState = e, this.props.connectionStateChanged(e)), t && this.props.onConnectionError(t)
                 }, this.showRetryError = (e, t, n) => {
                     6 === e && this.props.onConnectionError(t)
                 }, this.props = e, this.connect()
             }
             isConnected() {
-                return this.connectionState === Us.CONNECTED
+                return this.connectionState === Gs.CONNECTED
             }
             getBaseUriParts() {
-                if (this.connection instanceof Tu) return this.connection.getBaseUriParts()
+                if (this.connection instanceof Lu) return this.connection.getBaseUriParts()
             }
             sendMessage(e) {
-                this.connection instanceof Tu && this.isConnected() ? this.connection.sendMessage(e) : (0, ui.H)("Cannot send message when server is disconnected: ".concat(e))
+                this.connection instanceof Lu && this.isConnected() ? this.connection.sendMessage(e) : (0, ui.H)("Cannot send message when server is disconnected: ".concat(e))
             }
             incrementMessageCacheRunCount(e) {
-                this.connection instanceof Tu && this.connection.incrementMessageCacheRunCount(e)
+                this.connection instanceof Lu && this.connection.incrementMessageCacheRunCount(e)
             }
             async connect() {
                 try {
                     this.connection = await this.connectToRunningServer()
                 } catch (e) {
                     const t = (0, He.b)(e);
-                    (0, ui.H)(t.message), this.setConnectionState(Us.DISCONNECTED_FOREVER, t.message)
+                    (0, ui.H)(t.message), this.setConnectionState(Gs.DISCONNECTED_FOREVER, t.message)
                 }
             }
             disconnect() {
                 var e;
                 null === (e = this.connection) || void 0 === e || e.disconnect()
             }
             connectToRunningServer() {
-                const e = uu();
-                return new Tu({
+                const e = hu();
+                return new Lu({
                     sessionInfo: this.props.sessionInfo,
                     endpoints: this.props.endpoints,
                     baseUriPartsList: e,
                     onMessage: this.props.onMessage,
                     onConnectionStateChange: this.setConnectionState,
                     onRetry: this.showRetryError,
                     claimHostAuthToken: this.props.claimHostAuthToken,
                     resetHostAuthToken: this.props.resetHostAuthToken,
                     onHostConfigResp: this.props.onHostConfigResp
                 })
             }
         }
-        var Wu = __webpack_require__(54735);
-        class Nu {
+        var Du = __webpack_require__(54735);
+        class Bu {
             constructor() {
-                this.onSessionEvent = new Wu.MZ
+                this.onSessionEvent = new Du.MZ
             }
             handleSessionEventMsg(e) {
                 this.onSessionEvent.emit(e)
             }
         }
-        class Lu {
+        class ju {
             constructor() {
                 this._current = void 0, this._last = void 0
             }
             get current() {
                 if (!this._current) throw new Error("Tried to use SessionInfo before it was initialized");
                 return this._current
             }
@@ -125957,60 +126230,60 @@
                     installationId: r.installationId,
                     installationIdV3: r.installationIdV3,
                     maxCachedMessageAge: n.maxCachedMessageAge,
                     isHello: t.isHello
                 }
             }
         }
-        var Iu = __webpack_require__(76005),
-            Pu = __webpack_require__.n(Iu);
-        const Du = /\uFE0F/g,
-            Bu = String.fromCharCode(8205);
+        var Fu = __webpack_require__(76005),
+            Uu = __webpack_require__.n(Fu);
+        const Vu = /\uFE0F/g,
+            Hu = String.fromCharCode(8205);
 
-        function ju(e, t, n) {
+        function Xu(e, t, n) {
             const r = function(e) {
                 const t = e.replace("-", "_");
-                if (Pu().hasEmoji(Pu().get(t))) return Pu().get(t);
-                if (Pu().hasEmoji(e)) return e;
+                if (Uu().hasEmoji(Uu().get(t))) return Uu().get(t);
+                if (Uu().hasEmoji(e)) return e;
                 return ""
             }(e);
             let o;
             if (r && !e.startsWith(":material")) {
                 const e = function(e, t) {
                     const n = [];
                     let r = 0,
                         o = 0,
                         i = 0;
                     for (; i < e.length;) r = e.charCodeAt(i++), o ? (n.push((65536 + (o - 55296 << 10) + (r - 56320)).toString(16)), o = 0) : 55296 <= r && r <= 56319 ? o = r : n.push(r.toString(16));
                     return n.join(t || "-")
-                }((i = r).indexOf(Bu) < 0 ? i.replace(Du, "") : i);
+                }((i = r).indexOf(Hu) < 0 ? i.replace(Vu, "") : i);
                 o = "https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/".concat(e, ".png")
             } else o = e.startsWith(":material") ? function(e) {
                 const t = e.match(/^:(.+)\/(.+):$/);
                 return null === t ? "" : "https://fonts.gstatic.com/s/i/short-term/release/materialsymbolsoutlined/".concat(t[2], "/default/24px.svg")
             }(e) : n.buildMediaURL(e);
             var i;
             ! function(e) {
                 const t = document.querySelector("link[rel='shortcut icon']");
                 t && (t.href = e)
             }(o), t({
                 type: "SET_PAGE_FAVICON",
                 favicon: o
             })
         }
-        var Fu = __webpack_require__(43396);
+        var Gu = __webpack_require__(43396);
 
-        function Uu() {
+        function $u() {
             return {
                 formsWithPendingChanges: new Set,
                 formsWithUploads: new Set,
                 submitButtons: new Map
             }
         }
-        class Vu {
+        class Ku {
             constructor() {
                 this.widgetStates = new Map
             }
             createState(e) {
                 const t = new je.KR({
                     id: e
                 });
@@ -126042,25 +126315,25 @@
                     this.widgetStates.set(t, e)
                 }))
             }
             forEach(e) {
                 this.widgetStates.forEach(e)
             }
         }
-        class Hu {
+        class Yu {
             constructor() {
-                this.widgetStates = new Vu, this.clearOnSubmit = !1, this.formCleared = new Wu.MZ
+                this.widgetStates = new Ku, this.clearOnSubmit = !1, this.formCleared = new Du.MZ
             }
             get hasPendingChanges() {
                 return !this.widgetStates.isEmpty
             }
         }
-        class Xu {
+        class Zu {
             constructor(e) {
-                this.props = void 0, this.widgetStates = new Vu, this.forms = new Map, this.formsData = void 0, this.elementStates = new Map, this.props = e, this.formsData = Uu()
+                this.props = void 0, this.widgetStates = new Ku, this.forms = new Map, this.formsData = void 0, this.elementStates = new Map, this.props = e, this.formsData = $u()
             }
             addFormClearedListener(e, t) {
                 return this.getOrCreateFormState(e).formCleared.connect(t)
             }
             setFormClearOnSubmit(e, t) {
                 this.getOrCreateFormState(e).clearOnSubmit = t
             }
@@ -126087,15 +126360,15 @@
                 if (null != t && "boolValue" === t.value) return t.boolValue
             }
             setBoolValue(e, t, n, r) {
                 this.createWidgetState(e, n).boolValue = t, this.onWidgetValueChanged(e.formId, n, r)
             }
             getIntValue(e) {
                 const t = this.getWidgetState(e);
-                if (null != t && "intValue" === t.value) return Gu(t.intValue)
+                if (null != t && "intValue" === t.value) return Ju(t.intValue)
             }
             setIntValue(e, t, n, r) {
                 this.createWidgetState(e, n).intValue = t, this.onWidgetValueChanged(e.formId, n, r)
             }
             getDoubleValue(e) {
                 const t = this.getWidgetState(e);
                 if (null != t && "doubleValue" === t.value) return t.doubleValue
@@ -126126,15 +126399,15 @@
             setDoubleArrayValue(e, t, n, r) {
                 this.createWidgetState(e, n).doubleArrayValue = new je.qj({
                     data: t
                 }), this.onWidgetValueChanged(e.formId, n, r)
             }
             getIntArrayValue(e) {
                 const t = this.getWidgetState(e);
-                if (null != t && "intArrayValue" === t.value && null != t.intArrayValue && null != t.intArrayValue.data) return t.intArrayValue.data.map(Gu)
+                if (null != t && "intArrayValue" === t.value && null != t.intArrayValue && null != t.intArrayValue.data) return t.intArrayValue.data.map(Ju)
             }
             setIntArrayValue(e, t, n, r) {
                 this.createWidgetState(e, n).intArrayValue = new je.Zh({
                     data: t
                 }), this.onWidgetValueChanged(e.formId, n, r)
             }
             getJsonValue(e) {
@@ -126175,14 +126448,20 @@
                 })), this.updateFormsData((t => {
                     t.formsWithPendingChanges = e
                 }))
             }
             sendUpdateWidgetsMessage(e) {
                 this.props.sendRerunBackMsg(this.widgetStates.createWidgetStatesMsg(), e)
             }
+            getActiveWidgetStates(e) {
+                const t = new je.iE;
+                return this.widgetStates.forEach((n => {
+                    e.has(n.id) && t.widgets.push(n)
+                })), t
+            }
             removeInactive(e) {
                 this.widgetStates.removeInactive(e), this.forms.forEach((t => t.widgetStates.removeInactive(e))), this.elementStates.forEach(((t, n) => {
                     e.has(n) || this.deleteElementState(n)
                 }))
             }
             createWidgetState(e, t) {
                 return ((0, Xe.bM)(e.formId) && t.fromUi ? this.getOrCreateFormState(e.formId).widgetStates : this.widgetStates).createState(e.id)
@@ -126196,15 +126475,15 @@
                 return this.widgetStates.getState(e.id)
             }
             deleteWidgetState(e) {
                 this.widgetStates.deleteState(e)
             }
             getOrCreateFormState(e) {
                 let t = this.forms.get(e);
-                return null != t || (t = new Hu, this.forms.set(e, t)), t
+                return null != t || (t = new Yu, this.forms.set(e, t)), t
             }
             setFormsWithUploads(e) {
                 this.updateFormsData((t => {
                     t.formsWithUploads = e
                 }))
             }
             addSubmitButton(e, t) {
@@ -126242,30 +126521,30 @@
             }
             deleteElementState(e, t) {
                 var n;
                 (0, Xe.bb)(t) ? null === (n = this.elementStates.get(e)) || void 0 === n || n.delete(t): this.elementStates.delete(e)
             }
         }
 
-        function Gu(e) {
+        function Ju(e) {
             if ("number" === typeof e) return e;
-            const t = Fu.util.LongBits.from(e).toNumber();
+            const t = Gu.util.LongBits.from(e).toNumber();
             if (Number.isSafeInteger(t)) return t;
             throw new Error("value ".concat(e, " cannot be converted to number without a loss of precision!"))
         }
-        class $u {
+        class Qu {
             constructor(e) {
                 this.props = void 0, this.allowedOrigins = void 0, this.deferredAuthToken = void 0, this.openHostCommunication = () => {
                     window.addEventListener("message", this.receiveHostMessage), this.sendMessageToHost({
                         type: "GUEST_READY"
                     })
                 }, this.closeHostCommunication = () => {
                     window.removeEventListener("message", this.receiveHostMessage)
                 }, this.resetAuthToken = () => {
-                    this.deferredAuthToken = new Su
+                    this.deferredAuthToken = new Ru
                 }, this.claimAuthToken = () => this.deferredAuthToken.promise, this.setAllowedOrigins = e => {
                     let {
                         allowedOrigins: t,
                         useExternalAuthToken: n
                     } = e;
                     n || this.deferredAuthToken.resolve(void 0), null !== t && void 0 !== t && t.length && (this.allowedOrigins = t, this.openHostCommunication())
                 }, this.sendMessageToHost = e => {
@@ -126289,60 +126568,60 @@
                             hostname: i
                         } = r;
                         if (o === i) return !0;
                         const a = o.replace(/%2A/g, "*").split("."),
                             s = i.split(".");
                         return a.length === s.length && a.every(((e, t) => "*" === e || e === s[t]))
                     }(t, e.origin))) && ("CLOSE_MODAL" === t.type && this.props.closeModal(), "STOP_SCRIPT" === t.type && this.props.stopScript(), "RERUN_SCRIPT" === t.type && this.props.rerunScript(), "CLEAR_CACHE" === t.type && this.props.clearCache(), "REQUEST_PAGE_CHANGE" === t.type && this.props.pageChanged(t.pageScriptHash), "SEND_APP_HEARTBEAT" === t.type && this.props.sendAppHeartbeat(), "SET_INPUTS_DISABLED" === t.type && this.props.setInputsDisabled(t.disabled), "SET_AUTH_TOKEN" === t.type && (this.deferredAuthToken.resolve(t.authToken), void 0 !== t.jwtHeaderName && this.props.jwtHeaderChanged(t)), "SET_IS_OWNER" === t.type && this.props.isOwnerChanged(t.isOwner), "SET_MENU_ITEMS" === t.type && this.props.hostMenuItemsChanged(t.items), "SET_METADATA" === t.type && this.props.deployedAppMetadataChanged(t.metadata), "SET_PAGE_LINK_BASE_URL" === t.type && this.props.pageLinkBaseUrlChanged(t.pageLinkBaseUrl), "SET_SIDEBAR_CHEVRON_DOWNSHIFT" === t.type && this.props.sidebarChevronDownshiftChanged(t.sidebarChevronDownshift), "SET_SIDEBAR_NAV_VISIBILITY" === t.type && this.props.hostHideSidebarNavChanged(t.hidden), "SET_TOOLBAR_ITEMS" === t.type && this.props.hostToolbarItemsChanged(t.items), "UPDATE_FROM_QUERY_PARAMS" === t.type && (this.props.queryParamsChanged(t.queryParams), this.props.sendRerunBackMsg()), "UPDATE_HASH" === t.type && (window.location.hash = t.hash), "SET_CUSTOM_THEME_CONFIG" === t.type && this.props.themeChanged(t.themeInfo))
-                }, this.props = e, this.allowedOrigins = [], this.deferredAuthToken = new Su
+                }, this.props = e, this.allowedOrigins = [], this.deferredAuthToken = new Ru
             }
         }
-        var Ku = __webpack_require__(62813),
-            Yu = __webpack_require__.n(Ku);
-        const Zu = {
+        var ep = __webpack_require__(62813),
+            tp = __webpack_require__.n(ep);
+        const np = {
             randomUUID: "undefined" !== typeof crypto && crypto.randomUUID && crypto.randomUUID.bind(crypto)
         };
-        let Ju;
-        const Qu = new Uint8Array(16);
+        let rp;
+        const op = new Uint8Array(16);
 
-        function ep() {
-            if (!Ju && (Ju = "undefined" !== typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto), !Ju)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
-            return Ju(Qu)
+        function ip() {
+            if (!rp && (rp = "undefined" !== typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto), !rp)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
+            return rp(op)
         }
-        const tp = [];
-        for (let Up = 0; Up < 256; ++Up) tp.push((Up + 256).toString(16).slice(1));
+        const ap = [];
+        for (let Jp = 0; Jp < 256; ++Jp) ap.push((Jp + 256).toString(16).slice(1));
 
-        function np(e) {
+        function sp(e) {
             let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
-            return (tp[e[t + 0]] + tp[e[t + 1]] + tp[e[t + 2]] + tp[e[t + 3]] + "-" + tp[e[t + 4]] + tp[e[t + 5]] + "-" + tp[e[t + 6]] + tp[e[t + 7]] + "-" + tp[e[t + 8]] + tp[e[t + 9]] + "-" + tp[e[t + 10]] + tp[e[t + 11]] + tp[e[t + 12]] + tp[e[t + 13]] + tp[e[t + 14]] + tp[e[t + 15]]).toLowerCase()
+            return (ap[e[t + 0]] + ap[e[t + 1]] + ap[e[t + 2]] + ap[e[t + 3]] + "-" + ap[e[t + 4]] + ap[e[t + 5]] + "-" + ap[e[t + 6]] + ap[e[t + 7]] + "-" + ap[e[t + 8]] + ap[e[t + 9]] + "-" + ap[e[t + 10]] + ap[e[t + 11]] + ap[e[t + 12]] + ap[e[t + 13]] + ap[e[t + 14]] + ap[e[t + 15]]).toLowerCase()
         }
-        const rp = function(e, t, n) {
-            if (Zu.randomUUID && !t && !e) return Zu.randomUUID();
-            const r = (e = e || {}).random || (e.rng || ep)();
+        const lp = function(e, t, n) {
+            if (np.randomUUID && !t && !e) return np.randomUUID();
+            const r = (e = e || {}).random || (e.rng || ip)();
             if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, t) {
                 n = n || 0;
                 for (let e = 0; e < 16; ++e) t[n + e] = r[e];
                 return t
             }
-            return np(r)
+            return sp(r)
         };
-        class op {
+        class cp {
             constructor(e) {
                 this.sessionInfo = void 0, this.endpoints = void 0, this.formsWithPendingRequests = new Map, this.pendingFormUploadsChanged = void 0, this.requestFileURLs = void 0, this.pendingFileURLsRequests = new Map, this.sessionInfo = e.sessionInfo, this.endpoints = e.endpoints, this.pendingFormUploadsChanged = e.formsWithPendingRequestsChanged, this.requestFileURLs = e.requestFileURLs
             }
             async uploadFile(e, t, n, r, o) {
                 return this.offsetPendingRequestCount(e.formId, 1), this.endpoints.uploadFileUploaderFile(t, n, this.sessionInfo.current.sessionId, r, o).finally((() => this.offsetPendingRequestCount(e.formId, -1)))
             }
             deleteFile(e) {
                 return this.endpoints.deleteFileAtURL ? this.endpoints.deleteFileAtURL(e, this.sessionInfo.current.sessionId) : Promise.resolve()
             }
             fetchFileURLs(e) {
                 if (!this.requestFileURLs) return Promise.resolve([]);
-                const t = new Su,
-                    n = rp();
+                const t = new Ru,
+                    n = lp();
                 return this.pendingFileURLsRequests.set(n, t), this.requestFileURLs(n, e), t.promise
             }
             onFileURLsResponse(e) {
                 const t = e.responseId,
                     n = this.pendingFileURLsRequests.get(t);
                 n ? (e.errorMsg ? n.reject(e.errorMsg) : n.resolve(e.fileUrls || []), this.pendingFileURLsRequests.delete(t)) : (0, ui.KE)("fileURLsResponse received for nonexistent request, ignoring.")
             }
@@ -126355,18 +126634,18 @@
                 if (!(0, Xe.bM)(e)) return;
                 const r = null !== (n = this.formsWithPendingRequests.get(e)) && void 0 !== n ? n : 0,
                     o = r + t;
                 if (o < 0) throw new Error("Can't offset pendingRequestCount below 0 (formId=".concat(e, ", curCount=").concat(r, ", offset=").concat(t, ")"));
                 const i = this.getFormIdSet();
                 0 === o ? this.formsWithPendingRequests.delete(e) : this.formsWithPendingRequests.set(e, o);
                 const a = this.getFormIdSet();
-                Yu()(a, i) || this.pendingFormUploadsChanged(a)
+                tp()(a, i) || this.pendingFormUploadsChanged(a)
             }
         }
-        class ip {
+        class up {
             constructor(e) {
                 this.endpoints = void 0, this.msgListeners = new Map, this.registerListener = (e, t) => {
                     this.msgListeners.has(e) && (0, ui.KE)("MessageEventSource registered multiple times!", e), this.msgListeners.set(e, t)
                 }, this.deregisterListener = e => {
                     this.msgListeners.delete(e) || (0, ui.KE)("Could not deregister unregistered MessageEventSource!")
                 }, this.getComponentURL = (e, t) => this.endpoints.buildComponentURL(e, t), this.onMessageEvent = e => {
                     if (null == e.data || !e.data.hasOwnProperty("isStreamlitMessage")) return;
@@ -126376,35 +126655,36 @@
                     const {
                         type: n
                     } = e.data;
                     null != n ? t(n, e.data) : (0, ui.KE)("Received Streamlit message with no type!", e.data)
                 }, this.endpoints = e, window.addEventListener("message", this.onMessageEvent)
             }
         }
-        var ap = __webpack_require__(81810),
-            sp = __webpack_require__.n(ap);
-        class lp {
+        var pp = __webpack_require__(81810),
+            dp = __webpack_require__.n(pp);
+        class bp {
             constructor(e) {
                 this.getServerUri = void 0, this.csrfEnabled = void 0, this.cachedServerUri = void 0, this.jwtHeader = void 0, this.getServerUri = e.getServerUri, this.csrfEnabled = e.csrfEnabled
             }
             buildComponentURL(e, t) {
-                return pu(this.requireServerUri(), "".concat("/component", "/").concat(e, "/").concat(t))
+                return mu(this.requireServerUri(), "".concat("/component", "/").concat(e, "/").concat(t))
             }
             setJWTHeader(e) {
                 this.jwtHeader = e
             }
             buildMediaURL(e) {
-                return e.startsWith("/media") ? pu(this.requireServerUri(), e) : e
+                return e.startsWith("/media") ? mu(this.requireServerUri(), e) : e
             }
             buildFileUploadURL(e) {
-                return e.startsWith("/_stcore/upload_file") ? pu(this.requireServerUri(), e) : e
+                return e.startsWith("/_stcore/upload_file") ? mu(this.requireServerUri(), e) : e
             }
-            buildAppPageURL(e, t, n) {
-                const r = t.pageName,
-                    o = 0 === n ? "" : r;
+            buildAppPageURL(e, t) {
+                const n = t.pageName,
+                    r = t.urlPathname || n,
+                    o = t.isDefault ? "" : r;
                 if (null != e && e.length > 0) return "".concat(e, "/").concat(o);
                 const {
                     port: i,
                     protocol: a
                 } = window.location, {
                     basePath: s,
                     host: l
@@ -126430,16 +126710,16 @@
                     data: {
                         sessionId: t
                     }
                 }).then((() => {}))
             }
             async fetchCachedForwardMsg(e) {
                 const t = this.requireServerUri(),
-                    n = await fu.Z.request({
-                        url: pu(t, "".concat("/_stcore/message", "?hash=").concat(e)),
+                    n = await gu.Z.request({
+                        url: mu(t, "".concat("/_stcore/message", "?hash=").concat(e)),
                         method: "GET",
                         responseType: "arraybuffer"
                     });
                 return new Uint8Array(n.data)
             }
             requireServerUri() {
                 const e = this.getServerUri();
@@ -126451,20 +126731,20 @@
                 if (t.url = e, this.csrfEnabled) {
                     const e = (0, Xe.ej)("_streamlit_xsrf");
                     null != e && (t.headers = {
                         "X-Xsrftoken": e,
                         ...t.headers || {}
                     }, t.withCredentials = !0)
                 }
-                return fu.Z.request(t)
+                return gu.Z.request(t)
             }
         }
-        var cp = __webpack_require__(1866),
-            up = __webpack_require__.n(cp);
-        class pp {
+        var fp = __webpack_require__(1866),
+            hp = __webpack_require__.n(fp);
+        class mp {
             constructor(e) {
                 this.sessionInfo = void 0, this.initialized = !1, this.actuallySendMetrics = !1, this.pendingEvents = [], this.pendingCustomComponentCounter = {}, this.appHash = "Not initialized", this.metadata = {}, this.setAppHash = e => {
                     this.appHash = e
                 }, this.sessionInfo = e
             }
             initialize(e) {
                 let {
@@ -126521,20 +126801,20 @@
             }
             send(e) {
                 const t = {
                     ...arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                     ...this.getHostTrackingData(),
                     ...this.getInstallationData(),
                     reportHash: this.appHash,
-                    dev: Ss.td,
+                    dev: xs.td,
                     source: "browser",
                     streamlitVersion: this.sessionInfo.current.streamlitVersion,
                     isHello: this.sessionInfo.isHello
                 };
-                Ss.td ? (0, ui.up)("[Dev mode] Not tracking stat datapoint: ", e, t) : this.track(e, t, {
+                xs.td ? (0, ui.up)("[Dev mode] Not tracking stat datapoint: ", e, t) : this.track(e, t, {
                     context: {
                         ip: "0.0.0.0"
                     }
                 })
             }
             sendPendingEvents() {
                 this.pendingEvents.forEach((e => {
@@ -126550,18 +126830,18 @@
                     machineIdV3: this.sessionInfo.current.installationIdV3
                 }
             }
             setMetadata(e) {
                 this.metadata = e
             }
             getHostTrackingData() {
-                return this.metadata ? up()(this.metadata, ["hostedAt", "owner", "repo", "branch", "mainModule", "creatorId"]) : {}
+                return this.metadata ? hp()(this.metadata, ["hostedAt", "owner", "repo", "branch", "mainModule", "creatorId"]) : {}
             }
         }
-        const dp = (0, et.Z)("div", {
+        const Mp = (0, et.Z)("div", {
                 target: "erw9t6i1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 const n = (0, Ae.Iy)(t);
                 return {
@@ -126578,41 +126858,41 @@
                         float: "none",
                         height: t.sizes.full,
                         position: "static",
                         overflow: "visible"
                     }
                 }
             }), ""),
-            bp = (0, et.Z)("div", {
+            Op = (0, et.Z)("div", {
                 target: "erw9t6i0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "fixed",
                     top: 0,
                     left: 0,
                     zIndex: t.zIndices.tablePortal,
                     lineHeight: "100%"
                 }
             }), "");
-        const fp = (0, et.Z)("label", {
+        const gp = (0, et.Z)("label", {
                 target: "emfz9mr1"
             })({
                 name: "ti75j2",
                 styles: "margin:0"
             }),
-            hp = (0, et.Z)("p", {
+            zp = (0, et.Z)("p", {
                 target: "emfz9mr0"
             })({
                 name: "ti75j2",
                 styles: "margin:0"
             });
-        class mp extends n.PureComponent {
+        class yp extends n.PureComponent {
             constructor() {
                 super(...arguments), this.state = {
                     recordAudio: this.props.recordAudio
                 }, this.handleRecordAudioCheckbox = e => {
                     const {
                         checked: t
                     } = e.target, {
@@ -126642,24 +126922,24 @@
                     onClose: t,
                     children: [(0, ze.jsx)(ir, {
                         children: "Record a screencast"
                     }), (0, ze.jsxs)(ar, {
                         children: [(0, ze.jsx)("p", {
                             children: "This will record a video with the contents of your screen, so you can easily share what you're seeing with others."
                         }), (0, ze.jsx)("p", {
-                            children: (0, ze.jsxs)(fp, {
+                            children: (0, ze.jsxs)(gp, {
                                 "data-testid": "stScreencastAudioCheckbox",
                                 children: [(0, ze.jsx)("input", {
                                     type: "checkbox",
                                     name: "recordAudio",
                                     checked: e,
                                     onChange: this.handleRecordAudioCheckbox
                                 }), " ", "Also record audio"]
                             })
-                        }), (0, ze.jsxs)(hp, {
+                        }), (0, ze.jsxs)(zp, {
                             "data-testid": "stScreencastInstruction",
                             children: ["Press ", (0, ze.jsx)("kbd", {
                                 children: "Esc"
                             }), " any time to stop recording."]
                         })]
                     }), (0, ze.jsx)(sr, {
                         children: (0, ze.jsx)(lr, {
@@ -126667,103 +126947,103 @@
                             onClick: this.handleStartButton,
                             children: "Start recording!"
                         })
                     })]
                 })
             }
         }
-        const Mp = mp,
-            Op = (0, et.Z)("video", {
+        const Ap = yp,
+            vp = (0, et.Z)("video", {
                 target: "ecutw1r6"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     borderRadius: t.radii.md
                 }
             }), ""),
-            gp = (0, et.Z)("div", {
+            wp = (0, et.Z)("div", {
                 target: "ecutw1r5"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     flexDirection: "column",
                     width: t.sizes.full
                 }
             }), ""),
-            zp = (0, et.Z)("div", {
+            Sp = (0, et.Z)("div", {
                 target: "ecutw1r4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     flexDirection: "row",
                     paddingTop: t.spacing.md,
                     paddingBottom: t.spacing.md
                 }
             }), ""),
-            yp = (0, et.Z)("div", {
+            qp = (0, et.Z)("div", {
                 target: "ecutw1r3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingRight: t.spacing.lg,
                     textAlign: "right",
                     color: t.colors.gray,
                     fontWeight: t.fontWeights.bold,
                     width: "6em"
                 }
             }), ""),
-            Ap = (0, et.Z)("div", {
+            Ep = (0, et.Z)("div", {
                 target: "ecutw1r2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     flex: 1,
                     paddingRight: t.spacing.lg,
                     marginRight: "6em",
                     ["@media (max-width: ".concat(t.breakpoints.sm, ")")]: {
                         marginRight: t.spacing.none
                     }
                 }
             }), ""),
-            vp = (0, et.Z)("p", {
+            _p = (0, et.Z)("p", {
                 target: "ecutw1r1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.sm,
                     marginBottom: t.spacing.none,
                     fontSize: t.fontSizes.sm
                 }
             }), ""),
-            wp = (0, et.Z)("div", {
+            xp = (0, et.Z)("div", {
                 target: "ecutw1r0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.twoXS
                 }
             }), ""),
-            Sp = e => {
+            Rp = e => {
                 let {
                     onClose: t,
                     videoBlob: n,
                     fileName: r
                 } = e;
                 const o = URL.createObjectURL(n);
                 return (0, ze.jsxs)(cr, {
@@ -126775,118 +127055,118 @@
                                 width: "80vw"
                             }
                         }
                     },
                     children: [(0, ze.jsx)(ir, {
                         children: "Next steps"
                     }), (0, ze.jsx)(ar, {
-                        children: (0, ze.jsxs)(gp, {
+                        children: (0, ze.jsxs)(wp, {
                             "data-testid": "stVideoRecordedDialog",
-                            children: [(0, ze.jsxs)(zp, {
-                                children: [(0, ze.jsx)(yp, {
+                            children: [(0, ze.jsxs)(Sp, {
+                                children: [(0, ze.jsx)(qp, {
                                     children: "Step 1"
-                                }), (0, ze.jsxs)(Ap, {
+                                }), (0, ze.jsxs)(Ep, {
                                     children: [(0, ze.jsx)("p", {
                                         children: "Preview your video below:"
-                                    }), (0, ze.jsx)(Op, {
+                                    }), (0, ze.jsx)(vp, {
                                         src: o,
                                         controls: !0
                                     })]
                                 })]
-                            }), (0, ze.jsxs)(zp, {
-                                children: [(0, ze.jsx)(yp, {
+                            }), (0, ze.jsxs)(Sp, {
+                                children: [(0, ze.jsx)(qp, {
                                     children: "Step 2"
-                                }), (0, ze.jsxs)(Ap, {
-                                    children: [(0, ze.jsx)(wp, {
+                                }), (0, ze.jsxs)(Ep, {
+                                    children: [(0, ze.jsx)(xp, {
                                         children: (0, ze.jsx)(sn.ZP, {
                                             kind: ln.nW.SECONDARY,
                                             onClick: () => {
                                                 const e = document.createElement("a");
                                                 e.setAttribute("href", o), e.setAttribute("download", "".concat(r, ".webm")), e.click(), t()
                                             },
                                             children: "Save video to disk"
                                         })
-                                    }), (0, ze.jsxs)(vp, {
+                                    }), (0, ze.jsxs)(_p, {
                                         children: ["This video is encoded in the", " ", (0, ze.jsx)("a", {
                                             href: "https://www.webmproject.org/",
                                             children: "WebM format"
                                         }), ", which is only supported by newer video players. You can also play it by dragging the file directly into your browser."]
                                     })]
                                 })]
-                            }), (0, ze.jsxs)(zp, {
-                                children: [(0, ze.jsx)(yp, {
+                            }), (0, ze.jsxs)(Sp, {
+                                children: [(0, ze.jsx)(qp, {
                                     children: "Step 3"
-                                }), (0, ze.jsxs)(Ap, {
+                                }), (0, ze.jsxs)(Ep, {
                                     children: ["Share your video with the world on Twitter, LinkedIn, YouTube, or just plain email!", " ", (0, ze.jsx)("span", {
                                         role: "img",
                                         "aria-label": "Happy",
                                         children: "\ud83d\ude00"
                                     })]
                                 })]
                             })]
                         })
                     })]
                 })
             },
-            qp = (0, et.Z)("div", {
+            Tp = (0, et.Z)("div", {
                 target: "e16i1uly2"
             })((() => ({
                 display: "flex"
             })), ""),
-            Ep = (0, et.Z)("div", {
+            kp = (0, et.Z)("div", {
                 target: "e16i1uly1"
             })((() => ({
                 display: "flex",
                 alignItems: "center",
                 justifyItems: "center",
                 marginRight: "26px",
                 marginLeft: "10px",
                 fontSize: "50px"
             })), ""),
-            _p = (0, et.Z)("p", {
+            Cp = (0, et.Z)("p", {
                 target: "e16i1uly0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     margin: t.spacing.none
                 }
             }), "");
-        class xp extends n.PureComponent {
+        class Wp extends n.PureComponent {
             render() {
                 const {
                     onClose: e
                 } = this.props;
                 return (0, ze.jsxs)(cr, {
                     isOpen: !0,
                     onClose: e,
                     children: [(0, ze.jsx)(ir, {
                         children: "Record a screencast"
                     }), (0, ze.jsx)(ar, {
-                        children: (0, ze.jsxs)(qp, {
+                        children: (0, ze.jsxs)(Tp, {
                             "data-testid": "stUnsupportedBrowserDialog",
-                            children: [(0, ze.jsx)(Ep, {
+                            children: [(0, ze.jsx)(kp, {
                                 children: (0, ze.jsx)("span", {
                                     role: "img",
                                     "aria-label": "Alien Monster",
                                     children: "\ud83d\udc7e"
                                 })
-                            }), (0, ze.jsx)(_p, {
+                            }), (0, ze.jsx)(Cp, {
                                 children: "Due to limitations with some browsers, this feature is only supported on recent desktop versions of Chrome, Firefox, and Edge."
                             })]
                         })
                     })]
                 })
             }
         }
-        const Rp = xp;
-        var Tp;
-        const kp = (0, ge.F4)(Tp || (Tp = (0, Na.Z)(["\n0% {\n  opacity: 0;\n}\n25% {\n  opacity: 1;\n}\n100% {\n  opacity: 0;\n}"]))),
-            Cp = (0, et.Z)("div", {
+        const Np = Wp;
+        var Lp;
+        const Ip = (0, ge.F4)(Lp || (Lp = (0, dl.Z)(["\n0% {\n  opacity: 0;\n}\n25% {\n  opacity: 1;\n}\n100% {\n  opacity: 0;\n}"]))),
+            Pp = (0, et.Z)("div", {
                 target: "e7qru6u0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "fixed",
@@ -126900,18 +127180,18 @@
                     fontSize: "40vh",
                     color: t.colors.red,
                     fontWeight: t.fontWeights.bold,
                     opacity: "0.8",
                     textShadow: "1px 1px 10px ".concat(t.colors.darkGray),
                     transition: "opacity 0.3s ease-in-out",
                     fontFamily: 'Helvetica, Calibri, Roboto, "Open Sans", Arial, sans-serif',
-                    animation: "".concat(kp, " 1s")
+                    animation: "".concat(Ip, " 1s")
                 }
             }), "");
-        class Wp extends n.PureComponent {
+        class Dp extends n.PureComponent {
             constructor() {
                 super(...arguments), this.state = {
                     countdown: this.props.countdown
                 }, this.onAnimationEnd = async () => {
                     const {
                         countdown: e
                     } = this.state, {
@@ -126922,163 +127202,331 @@
                     }), 0 === n && t()
                 }
             }
             render() {
                 const {
                     countdown: e
                 } = this.state;
-                return (0, ze.jsx)(Cp, {
+                return (0, ze.jsx)(Pp, {
                     "data-testid": "stCountdown",
                     onAnimationEnd: this.onAnimationEnd,
                     children: (0, ze.jsx)("span", {
                         children: e
                     })
                 }, "frame".concat(e))
             }
         }
-        Wp.defaultProps = {
+        Dp.defaultProps = {
             endCallback: () => {}
         };
-        const Np = Wp;
-        const Lp = function(e) {
-                class t extends n.PureComponent {
-                    constructor() {
-                        super(...arguments), this.recorder = void 0, this.state = {
-                            fileName: "streamlit-screencast",
-                            recordAudio: !1,
-                            currentState: this.props.testOverride || "OFF"
-                        }, this.toggleRecordAudio = () => {
-                            const {
-                                recordAudio: e
-                            } = this.state;
-                            this.setState({
-                                recordAudio: !e
-                            })
-                        }, this.showDialog = e => {
-                            const {
-                                currentState: t
-                            } = this.state;
-                            al.isSupportedBrowser() ? "OFF" === t ? this.setState({
-                                fileName: e,
-                                currentState: "SETUP"
-                            }) : this.stopRecording().catch((e => (0, ui.KE)("withScreencast.stopRecording threw an error: ".concat(e)))) : this.setState({
+        const Bp = Dp;
+        const jp = function(e) {
+            class t extends n.PureComponent {
+                constructor() {
+                    super(...arguments), this.recorder = void 0, this.state = {
+                        fileName: "streamlit-screencast",
+                        recordAudio: !1,
+                        currentState: this.props.testOverride || "OFF"
+                    }, this.toggleRecordAudio = () => {
+                        const {
+                            recordAudio: e
+                        } = this.state;
+                        this.setState({
+                            recordAudio: !e
+                        })
+                    }, this.showDialog = e => {
+                        const {
+                            currentState: t
+                        } = this.state;
+                        ul.isSupportedBrowser() ? "OFF" === t ? this.setState({
+                            fileName: e,
+                            currentState: "SETUP"
+                        }) : this.stopRecording().catch((e => (0, ui.KE)("withScreencast.stopRecording threw an error: ".concat(e)))) : this.setState({
+                            currentState: "UNSUPPORTED"
+                        })
+                    }, this.startRecording = async () => {
+                        const {
+                            recordAudio: e
+                        } = this.state;
+                        this.recorder = new ul({
+                            recordAudio: e,
+                            onErrorOrStop: () => this.stopRecording()
+                        });
+                        try {
+                            await this.recorder.initialize()
+                        } catch (t) {
+                            return (0, ui.KE)("ScreenCastRecorder.initialize error: ".concat(t)), void this.setState({
                                 currentState: "UNSUPPORTED"
                             })
-                        }, this.startRecording = async () => {
-                            const {
-                                recordAudio: e
-                            } = this.state;
-                            this.recorder = new al({
-                                recordAudio: e,
-                                onErrorOrStop: () => this.stopRecording()
-                            });
-                            try {
-                                await this.recorder.initialize()
-                            } catch (t) {
-                                return (0, ui.KE)("ScreenCastRecorder.initialize error: ".concat(t)), void this.setState({
-                                    currentState: "UNSUPPORTED"
-                                })
-                            }
-                            this.setState({
-                                currentState: "COUNTDOWN"
-                            })
-                        }, this.stopRecording = async () => {
-                            let e;
-                            const {
-                                currentState: t
-                            } = this.state;
-                            "OFF" !== t && null != this.recorder && ("COUNTDOWN" === t && this.setState({
-                                currentState: "OFF"
-                            }), "RECORDING" === t && ("inactive" === this.recorder.getState() ? this.setState({
-                                currentState: "OFF"
-                            }) : (e = await this.recorder.stop(), this.setState({
-                                outputBlob: e,
-                                currentState: "PREVIEW_FILE"
-                            }))))
-                        }, this.onCountdownEnd = async () => {
-                            if (null == this.recorder) throw new Error("Countdown finished but recorder is null");
-                            this.recorder.start() ? this.setState({
-                                currentState: "RECORDING"
-                            }) : this.stopRecording().catch((e => (0, ui.KE)("withScreencast.stopRecording threw an error: ".concat(e))))
-                        }, this.getScreenCastProps = () => ({
-                            currentState: this.state.currentState,
-                            toggleRecordAudio: this.toggleRecordAudio,
-                            startRecording: this.showDialog,
-                            stopRecording: this.stopRecording
-                        }), this.closeDialog = () => {
-                            this.setState({
-                                currentState: "OFF"
-                            })
-                        }, this.render = () => {
-                            const {
-                                outputBlob: t,
-                                fileName: n,
-                                recordAudio: r,
-                                currentState: o
-                            } = this.state;
-                            return (0, ze.jsxs)("div", {
-                                className: "withScreencast",
-                                "data-testid": "stScreencast",
-                                children: [(0, ze.jsx)(e, {
-                                    ...this.props,
-                                    screenCast: this.getScreenCastProps()
-                                }), "UNSUPPORTED" === o && (0, ze.jsx)(Rp, {
-                                    onClose: this.closeDialog
-                                }), "SETUP" === o && (0, ze.jsx)(Mp, {
-                                    recordAudio: r,
-                                    onClose: this.closeDialog,
-                                    startRecording: this.startRecording,
-                                    toggleRecordAudio: this.toggleRecordAudio
-                                }), "COUNTDOWN" === o && (0, ze.jsx)(Np, {
-                                    countdown: 3,
-                                    endCallback: this.onCountdownEnd
-                                }), "PREVIEW_FILE" === o && t && (0, ze.jsx)(Sp, {
-                                    onClose: this.closeDialog,
-                                    videoBlob: t,
-                                    fileName: n
-                                })]
-                            })
                         }
+                        this.setState({
+                            currentState: "COUNTDOWN"
+                        })
+                    }, this.stopRecording = async () => {
+                        let e;
+                        const {
+                            currentState: t
+                        } = this.state;
+                        "OFF" !== t && null != this.recorder && ("COUNTDOWN" === t && this.setState({
+                            currentState: "OFF"
+                        }), "RECORDING" === t && ("inactive" === this.recorder.getState() ? this.setState({
+                            currentState: "OFF"
+                        }) : (e = await this.recorder.stop(), this.setState({
+                            outputBlob: e,
+                            currentState: "PREVIEW_FILE"
+                        }))))
+                    }, this.onCountdownEnd = async () => {
+                        if (null == this.recorder) throw new Error("Countdown finished but recorder is null");
+                        this.recorder.start() ? this.setState({
+                            currentState: "RECORDING"
+                        }) : this.stopRecording().catch((e => (0, ui.KE)("withScreencast.stopRecording threw an error: ".concat(e))))
+                    }, this.getScreenCastProps = () => ({
+                        currentState: this.state.currentState,
+                        toggleRecordAudio: this.toggleRecordAudio,
+                        startRecording: this.showDialog,
+                        stopRecording: this.stopRecording
+                    }), this.closeDialog = () => {
+                        this.setState({
+                            currentState: "OFF"
+                        })
+                    }, this.render = () => {
+                        const {
+                            outputBlob: t,
+                            fileName: n,
+                            recordAudio: r,
+                            currentState: o
+                        } = this.state;
+                        return (0, ze.jsxs)("div", {
+                            className: "withScreencast",
+                            "data-testid": "stScreencast",
+                            children: [(0, ze.jsx)(e, {
+                                ...this.props,
+                                screenCast: this.getScreenCastProps()
+                            }), "UNSUPPORTED" === o && (0, ze.jsx)(Np, {
+                                onClose: this.closeDialog
+                            }), "SETUP" === o && (0, ze.jsx)(Ap, {
+                                recordAudio: r,
+                                onClose: this.closeDialog,
+                                startRecording: this.startRecording,
+                                toggleRecordAudio: this.toggleRecordAudio
+                            }), "COUNTDOWN" === o && (0, ze.jsx)(Bp, {
+                                countdown: 3,
+                                endCallback: this.onCountdownEnd
+                            }), "PREVIEW_FILE" === o && t && (0, ze.jsx)(Rp, {
+                                onClose: this.closeDialog,
+                                videoBlob: t,
+                                fileName: n
+                            })]
+                        })
                     }
                 }
-                return t.displayName = "withScreencast(".concat(e.displayName || e.name, ")"), Lr()(t, e)
-            },
-            Ip = "<null>",
-            Pp = (e, t) => t == je.De.ToolbarMode.DEVELOPER || je.De.ToolbarMode.VIEWER != t && je.De.ToolbarMode.MINIMAL != t && (e || zl());
-        class Dp extends n.PureComponent {
+            }
+            return t.displayName = "withScreencast(".concat(e.displayName || e.name, ")"), Lr()(t, e)
+        };
+
+        function Fp(e) {
+            return e ? "".concat(e, " \xb7 Streamlit") : "Streamlit"
+        }
+        class Up {
             constructor(e) {
+                this.appPages = void 0, this.currentPageScriptHash = void 0, this.hideSidebarNav = void 0, this.appNav = void 0, this.appNav = e, this.appPages = [], this.currentPageScriptHash = null, this.hideSidebarNav = null
+            }
+            handleNewSession(e) {
+                var t, n, r, o, i;
+                this.appPages = e.appPages, this.currentPageScriptHash = e.pageScriptHash, this.hideSidebarNav = null !== (t = null === (n = e.config) || void 0 === n ? void 0 : n.hideSidebarNav) && void 0 !== t && t;
+                const a = this.appPages[0],
+                    s = null !== (r = a.pageName) && void 0 !== r ? r : "",
+                    l = null !== (o = null === (i = this.appPages.find((e => e.pageScriptHash === this.currentPageScriptHash))) || void 0 === i ? void 0 : i.pageName) && void 0 !== o ? o : "",
+                    c = a.pageScriptHash === this.currentPageScriptHash;
+                return this.appNav.onUpdatePageUrl(s, l, c), document.title = Fp(null !== l && void 0 !== l ? l : ""), [{
+                    hideSidebarNav: this.hideSidebarNav,
+                    appPages: this.appPages,
+                    currentPageScriptHash: this.currentPageScriptHash
+                }, () => {
+                    this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_APP_PAGES",
+                        appPages: this.appPages
+                    }), this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_CURRENT_PAGE_NAME",
+                        currentPageName: c ? "" : l,
+                        currentPageScriptHash: this.currentPageScriptHash
+                    })
+                }]
+            }
+            handlePagesChanged(e) {
+                const {
+                    appPages: t
+                } = e;
+                return [{
+                    appPages: t
+                }, () => {
+                    this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_APP_PAGES",
+                        appPages: t
+                    })
+                }]
+            }
+            handlePageNotFound(e) {
+                var t, n;
+                const {
+                    pageName: r
+                } = e;
+                this.appNav.onPageNotFound(r);
+                const o = null !== (t = null === (n = this.appPages[0]) || void 0 === n ? void 0 : n.pageScriptHash) && void 0 !== t ? t : "";
+                return this.currentPageScriptHash = o, [{
+                    currentPageScriptHash: o
+                }, () => {
+                    this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_CURRENT_PAGE_NAME",
+                        currentPageName: "",
+                        currentPageScriptHash: o
+                    })
+                }]
+            }
+            handleNavigation(e) {}
+            findPageByUrlPath(e) {
                 var t;
-                super(e), t = this, this.endpoints = void 0, this.sessionInfo = new Lu, this.metricsMgr = new pp(this.sessionInfo), this.sessionEventDispatcher = new Nu, this.connectionManager = void 0, this.widgetMgr = void 0, this.hostCommunicationMgr = void 0, this.uploadClient = void 0, this.pendingElementsBuffer = void 0, this.pendingElementsTimerRunning = void 0, this.componentRegistry = void 0, this.embeddingId = (0, Xe.D)(), this.keyMap = {
+                return 0 === this.appPages.length ? null : null !== (t = this.appPages.find((t => e.endsWith("/" + t.pageName)))) && void 0 !== t ? t : this.appPages[0]
+            }
+            clearPageElements(e, t, n) {
+                return Ye.empty(t, !1, n)
+            }
+        }
+        class Vp {
+            constructor(e) {
+                this.appNav = void 0, this.mainScriptHash = void 0, this.appPages = void 0, this.mainPage = void 0, this.hideSidebarNav = void 0, this.appNav = e, this.mainScriptHash = null, this.appPages = [], this.mainPage = null, this.hideSidebarNav = null
+            }
+            handleNewSession(e) {
+                var t, n, r;
+                (this.mainScriptHash = e.mainScriptHash, null === this.hideSidebarNav) && (this.hideSidebarNav = null !== (n = null === (r = e.config) || void 0 === r ? void 0 : r.hideSidebarNav) && void 0 !== n ? n : null);
+                return document.title = Fp(""), [{
+                    hideSidebarNav: null !== (t = this.hideSidebarNav) && void 0 !== t && t
+                }, () => {}]
+            }
+            handlePagesChanged(e) {}
+            handlePageNotFound(e) {
+                var t;
+                const {
+                    pageName: n
+                } = e;
+                return this.appNav.onPageNotFound(n), [{
+                    currentPageScriptHash: null !== (t = this.mainScriptHash) && void 0 !== t ? t : ""
+                }, () => {
+                    var e;
+                    this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_CURRENT_PAGE_NAME",
+                        currentPageName: "",
+                        currentPageScriptHash: null !== (e = this.mainScriptHash) && void 0 !== e ? e : ""
+                    })
+                }]
+            }
+            handleNavigation(e) {
+                var t, n;
+                const {
+                    sections: r,
+                    position: o,
+                    appPages: i
+                } = e;
+                this.appPages = i, this.hideSidebarNav = o === je.uh.Position.HIDDEN;
+                const a = e.pageScriptHash,
+                    s = i.find((e => e.pageScriptHash === a)),
+                    l = i.find((e => e.isDefault));
+                this.mainPage = l;
+                const c = s.urlPathname;
+                if (!this.appNav.isPageTitleSet) {
+                    var u;
+                    const e = Fp(s.pageName);
+                    document.title = e, this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_PAGE_TITLE",
+                        title: null !== (u = s.pageName) && void 0 !== u ? u : ""
+                    })
+                }
+                return !this.appNav.isPageIconSet && s.icon && this.appNav.onPageIconChange(s.icon), this.appNav.onUpdatePageUrl(null !== (t = l.urlPathname) && void 0 !== t ? t : "", c, null !== (n = s.isDefault) && void 0 !== n && n), [{
+                    appPages: i,
+                    navSections: r,
+                    hideSidebarNav: this.hideSidebarNav,
+                    currentPageScriptHash: a
+                }, () => {
+                    this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_APP_PAGES",
+                        appPages: i
+                    }), this.appNav.hostCommunicationMgr.sendMessageToHost({
+                        type: "SET_CURRENT_PAGE_NAME",
+                        currentPageName: s.isDefault ? "" : c,
+                        currentPageScriptHash: a
+                    })
+                }]
+            }
+            findPageByUrlPath(e) {
+                var t;
+                return null !== (t = this.appPages.find((t => e.endsWith("/" + t.urlPathname)))) && void 0 !== t ? t : this.mainPage
+            }
+            clearPageElements(e, t, n) {
+                return e.filterMainScriptElements(t)
+            }
+        }
+        class Hp {
+            constructor(e, t, n, r) {
+                this.hostCommunicationMgr = void 0, this.onUpdatePageUrl = void 0, this.onPageNotFound = void 0, this.onPageIconChange = void 0, this.isPageTitleSet = void 0, this.isPageIconSet = void 0, this.strategy = void 0, this.hostCommunicationMgr = e, this.onUpdatePageUrl = t, this.onPageNotFound = n, this.onPageIconChange = r, this.isPageIconSet = !1, this.isPageTitleSet = !1, this.strategy = new Up(this)
+            }
+            handleNewSession(e) {
+                return this.isPageTitleSet = !1, this.isPageIconSet = !1, this.strategy.handleNewSession(e)
+            }
+            handleNavigation(e) {
+                return this.strategy instanceof Up && (this.strategy = new Vp(this)), this.strategy.handleNavigation(e)
+            }
+            handlePagesChanged(e) {
+                return this.strategy.handlePagesChanged(e)
+            }
+            handlePageNotFound(e) {
+                return this.strategy.handlePageNotFound(e)
+            }
+            findPageByUrlPath(e) {
+                return this.strategy.findPageByUrlPath(e)
+            }
+            handlePageConfigChanged(e) {
+                this.isPageIconSet = Boolean(e.favicon), this.isPageTitleSet = Boolean(e.title)
+            }
+            clearPageElements(e, t, n) {
+                return this.strategy.clearPageElements(e, t, n)
+            }
+        }
+        const Xp = "<null>",
+            Gp = (e, t) => t == je.De.ToolbarMode.DEVELOPER || je.De.ToolbarMode.VIEWER != t && je.De.ToolbarMode.MINIMAL != t && (e || Sl());
+        class $p extends n.PureComponent {
+            constructor(e) {
+                var t;
+                super(e), t = this, this.endpoints = void 0, this.sessionInfo = new ju, this.metricsMgr = new mp(this.sessionInfo), this.sessionEventDispatcher = new Bu, this.connectionManager = void 0, this.widgetMgr = void 0, this.hostCommunicationMgr = void 0, this.uploadClient = void 0, this.pendingElementsBuffer = void 0, this.pendingElementsTimerRunning = void 0, this.componentRegistry = void 0, this.embeddingId = (0, Xe.D)(), this.appNavigation = void 0, this.keyMap = {
                     RERUN: "r",
                     CLEAR_CACHE: "c",
                     STOP_RECORDING: {
                         sequence: "esc",
                         action: "keyup"
                     }
                 }, this.keyHandlers = {
                     RERUN: () => {
                         this.rerunScript()
                     },
                     CLEAR_CACHE: () => {
-                        Pp(this.state.isOwner, this.state.toolbarMode) && this.openClearCacheDialog()
+                        Gp(this.state.isOwner, this.state.toolbarMode) && this.openClearCacheDialog()
                     },
                     STOP_RECORDING: this.props.screenCast.stopRecording
                 }, this.showDeployError = (e, t, n) => {
                     this.openDialog({
-                        type: ou.DEPLOY_ERROR,
+                        type: cu.DEPLOY_ERROR,
                         title: e,
                         msg: t,
                         onContinue: n,
                         onClose: () => {},
                         onTryAgain: this.sendLoadGitInfoBackMsg
                     })
                 }, this.handleConnectionStateChanged = e => {
                     (0, ui.ji)("Connection state changed from ".concat(this.state.connectionState, " to ").concat(e)), this.setState({
                         connectionState: e
-                    }), e === Us.CONNECTED ? ((0, ui.ji)("Reconnected to server; requesting a script run"), this.widgetMgr.sendUpdateWidgetsMessage(void 0), this.setState({
+                    }), e === Gs.CONNECTED ? ((0, ui.ji)("Reconnected to server; requesting a script run"), this.widgetMgr.sendUpdateWidgetsMessage(void 0), this.setState({
                         dialog: null
                     })) : ((0, Xe.d8)("_streamlit_xsrf", ""), this.sessionInfo.isSet && this.sessionInfo.clearCurrent())
                 }, this.handleGitInfoChanged = e => {
                     this.setState({
                         gitInfo: e
                     })
                 }, this.handleCustomParentMessage = e => {
@@ -127103,34 +127551,39 @@
                             pageNotFound: e => this.handlePageNotFound(e),
                             gitInfoChanged: e => this.handleGitInfoChanged(e),
                             scriptFinished: e => this.handleScriptFinished(e),
                             pageProfile: e => this.handlePageProfileMsg(e),
                             autoRerun: e => this.handleAutoRerun(e),
                             fileUrlsResponse: e => this.uploadClient.onFileURLsResponse(e),
                             parentMessage: e => this.handleCustomParentMessage(e),
-                            logo: e => this.setState({
-                                appLogo: e
-                            })
+                            logo: t => this.handleLogo(t, e.metadata),
+                            navigation: e => this.handleNavigation(e)
                         })
                     } catch (t) {
                         const e = (0, He.b)(t);
                         (0, ui.H)(e), this.showError("Bad message format", e.message)
                     }
+                }, this.handleLogo = (e, t) => {
+                    this.setState({
+                        elements: this.pendingElementsBuffer.appRootWithLogo(e, t)
+                    }, (() => {
+                        this.pendingElementsBuffer = this.state.elements
+                    }))
                 }, this.handlePageConfigChanged = e => {
                     const {
                         title: t,
                         favicon: n,
                         layout: r,
                         initialSidebarState: o,
                         menuItems: i
                     } = e;
-                    t && (this.hostCommunicationMgr.sendMessageToHost({
+                    this.appNavigation.handlePageConfigChanged(e), t && (this.hostCommunicationMgr.sendMessageToHost({
                         type: "SET_PAGE_TITLE",
                         title: t
-                    }), document.title = t), n && ju(n, this.hostCommunicationMgr.sendMessageToHost, this.endpoints), r !== this.state.layout && this.setState((e => ({
+                    }), document.title = t), n && this.onPageIconChanged(n), r !== this.state.layout && this.setState((e => ({
                         layout: r,
                         userSettings: {
                             ...e.userSettings,
                             wideMode: r === je.Pz.Layout.WIDE
                         }
                     }))), o !== this.state.initialSidebarState && this.setState((() => ({
                         initialSidebarState: o
@@ -127145,41 +127598,21 @@
                         type: "SET_QUERY_PARAM",
                         queryParams: t ? "?".concat(t) : ""
                     })
                 }, this.onPageNotFound = e => {
                     const t = e ? "You have requested page /".concat(e, ", but no corresponding file was found in the app's pages/ directory") : "The page that you have requested does not seem to exist";
                     this.showError("Page not found", "".concat(t, ". Running the app's main page."))
                 }, this.handlePageNotFound = e => {
-                    var t;
-                    const {
-                        pageName: n
-                    } = e;
-                    this.onPageNotFound(n);
-                    const r = (null === (t = this.state.appPages[0]) || void 0 === t ? void 0 : t.pageScriptHash) || "";
-                    this.setState({
-                        currentPageScriptHash: r
-                    }, (() => {
-                        this.hostCommunicationMgr.sendMessageToHost({
-                            type: "SET_CURRENT_PAGE_NAME",
-                            currentPageName: "",
-                            currentPageScriptHash: r
-                        })
-                    }))
+                    this.maybeSetState(this.appNavigation.handlePageNotFound(e))
+                }, this.onPageIconChanged = e => {
+                    Xu(e, this.hostCommunicationMgr.sendMessageToHost, this.endpoints)
                 }, this.handlePagesChanged = e => {
-                    const {
-                        appPages: t
-                    } = e;
-                    this.setState({
-                        appPages: t
-                    }, (() => {
-                        this.hostCommunicationMgr.sendMessageToHost({
-                            type: "SET_APP_PAGES",
-                            appPages: t
-                        })
-                    }))
+                    this.maybeSetState(this.appNavigation.handlePagesChanged(e))
+                }, this.handleNavigation = e => {
+                    this.maybeSetState(this.appNavigation.handleNavigation(e))
                 }, this.handlePageProfileMsg = e => {
                     var t, n, r;
                     const o = je.AG.toObject(e);
                     this.metricsMgr.enqueue("pageProfile", {
                         ...o,
                         isFragmentRun: Boolean(o.isFragmentRun),
                         appId: this.sessionInfo.current.appId,
@@ -127200,15 +127633,15 @@
                 }, this.handleSessionStatusChanged = e => {
                     this.setState((t => {
                         let {
                             scriptRunState: n
                         } = t, {
                             dialog: r
                         } = t;
-                        if (e.scriptIsRunning && t.scriptRunState !== Qe.STOP_REQUESTED) n = Qe.RUNNING, null != r && r.type === ou.SCRIPT_COMPILE_ERROR && (r = void 0);
+                        if (e.scriptIsRunning && t.scriptRunState !== Qe.STOP_REQUESTED) n = Qe.RUNNING, null != r && r.type === cu.SCRIPT_COMPILE_ERROR && (r = void 0);
                         else if (!e.scriptIsRunning && t.scriptRunState !== Qe.RERUN_REQUESTED && t.scriptRunState !== Qe.COMPILATION_ERROR) {
                             n = Qe.NOT_RUNNING;
                             const e = this.metricsMgr.getAndResetCustomComponentCounter();
                             Object.entries(e).forEach((e => {
                                 let [t, n] = e;
                                 this.metricsMgr.enqueue("customComponentStats", {
                                     name: t,
@@ -127227,22 +127660,22 @@
                     }))
                 }, this.handleSessionEvent = e => {
                     if (this.sessionEventDispatcher.handleSessionEventMsg(e), "scriptCompilationException" === e.type) {
                         this.setState({
                             scriptRunState: Qe.COMPILATION_ERROR
                         });
                         const t = {
-                            type: ou.SCRIPT_COMPILE_ERROR,
+                            type: cu.SCRIPT_COMPILE_ERROR,
                             exception: e.scriptCompilationException,
                             onClose: () => {}
                         };
                         this.openDialog(t)
-                    } else if (Ss.B && "scriptChangedOnDisk" === e.type) {
+                    } else if (xs.B && "scriptChangedOnDisk" === e.type) {
                         const e = {
-                            type: ou.SCRIPT_CHANGED,
+                            type: cu.SCRIPT_CHANGED,
                             onRerun: this.rerunScript,
                             onClose: () => {},
                             allowRunOnSave: this.state.allowRunOnSave
                         };
                         this.openDialog(e)
                     }
                 }, this.maybeUpdatePageUrl = (e, t, n) => {
@@ -127257,79 +127690,63 @@
                                 i = r ? "?".concat(r) : "",
                                 a = o ? "/".concat(o) : "",
                                 s = "".concat(a, "/").concat(e).concat(i);
                             window.history.pushState({}, "", s)
                         }
                     }
                 }, this.handleNewSession = e => {
-                    var t;
-                    const n = e.initialize;
-                    if (this.hasStreamlitVersionChanged(n)) return void window.location.reload();
+                    const t = e.initialize;
+                    if (this.hasStreamlitVersionChanged(t)) return void window.location.reload();
                     this.sessionInfo.isSet || this.handleOneTimeInitialization(e);
                     const {
-                        appHash: r,
-                        currentPageScriptHash: o
+                        appHash: n,
+                        currentPageScriptHash: r
                     } = this.state, {
-                        scriptRunId: i,
-                        name: a,
-                        mainScriptPath: s,
-                        fragmentIdsThisRun: l,
-                        pageScriptHash: c
-                    } = e, u = e.appPages[0], p = null === (t = e.appPages.find((e => e.pageScriptHash === c))) || void 0 === t ? void 0 : t.pageName, d = c === u.pageScriptHash;
-                    if (l.length) this.setState({
-                        fragmentIdsThisRun: l,
+                        scriptRunId: o,
+                        name: i,
+                        mainScriptPath: a,
+                        fragmentIdsThisRun: s,
+                        pageScriptHash: l,
+                        mainScriptHash: c
+                    } = e;
+                    if (s.length) this.setState({
+                        fragmentIdsThisRun: s,
                         latestRunTime: performance.now()
                     });
                     else {
                         this.state.autoReruns.forEach((e => {
                             clearInterval(e)
                         })), this.setState({
                             autoReruns: []
                         });
                         const t = e.config,
                             n = e.customTheme;
-                        this.maybeUpdatePageUrl(u.pageName, p, d), this.processThemeInput(n), this.setState({
+                        this.processThemeInput(n), this.setState({
                             allowRunOnSave: t.allowRunOnSave,
                             hideTopBar: t.hideTopBar,
                             toolbarMode: t.toolbarMode,
                             latestRunTime: performance.now(),
-                            fragmentIdsThisRun: l
-                        }), this.setState({
-                            hideSidebarNav: t.hideSidebarNav,
-                            appPages: e.appPages,
-                            currentPageScriptHash: c
-                        }, (() => {
-                            this.hostCommunicationMgr.sendMessageToHost({
-                                type: "SET_APP_PAGES",
-                                appPages: e.appPages
-                            }), this.hostCommunicationMgr.sendMessageToHost({
-                                type: "SET_CURRENT_PAGE_NAME",
-                                currentPageName: d ? "" : p,
-                                currentPageScriptHash: c
-                            })
-                        })), document.title = "".concat(p, " \xb7 Streamlit"), ju("".concat(".", "/favicon.png"), this.hostCommunicationMgr.sendMessageToHost, this.endpoints)
-                    }
-                    const b = (0, Xe.Wu)(this.sessionInfo.current.installationId + s);
-                    this.metricsMgr.setMetadata(this.state.deployedAppMetadata), this.metricsMgr.setAppHash(b), this.metricsMgr.enqueue("updateReport", {
-                        numPages: e.appPages.length,
-                        isMainPage: d
-                    }), r === b && o === c ? this.setState({
-                        scriptRunId: i
-                    }) : this.clearAppState(b, i, a)
+                            mainScriptHash: c,
+                            fragmentIdsThisRun: s
+                        }), this.maybeSetState(this.appNavigation.handleNewSession(e)), this.onPageIconChanged("".concat(".", "/favicon.png"))
+                    }
+                    const u = (0, Xe.Wu)(this.sessionInfo.current.installationId + a);
+                    this.metricsMgr.setMetadata(this.state.deployedAppMetadata), this.metricsMgr.setAppHash(u), this.metricsMgr.enqueue("updateReport"), n === u && r === l ? this.setState({
+                        scriptRunId: o
+                    }) : this.clearAppState(u, o, i, c)
                 }, this.handleOneTimeInitialization = e => {
                     const t = e.initialize,
                         n = e.config;
-                    this.sessionInfo.setCurrent(Lu.propsFromNewSessionMessage(e)), this.metricsMgr.initialize({
+                    this.sessionInfo.setCurrent(ju.propsFromNewSessionMessage(e)), this.metricsMgr.initialize({
                         gatherUsageStats: n.gatherUsageStats
                     }), this.handleSessionStatusChanged(t.sessionStatus)
                 }, this.onHistoryChange = () => {
-                    var e;
-                    const t = null !== (e = this.state.appPages.find((e => document.location.pathname.endsWith("/" + e.pageName)))) && void 0 !== e ? e : this.state.appPages[0],
-                        n = document.location.toString().includes("#"),
-                        r = (null === t || void 0 === t ? void 0 : t.pageScriptHash) === this.state.currentPageScriptHash;
+                    const {
+                        currentPageScriptHash: e
+                    } = this.state, t = this.appNavigation.findPageByUrlPath(document.location.pathname), n = document.location.toString().includes("#"), r = (null === t || void 0 === t ? void 0 : t.pageScriptHash) === e;
                     null == t || n && r || this.onPageChange(t.pageScriptHash)
                 }, this.setAndSendTheme = e => {
                     this.props.theme.setTheme(e), this.hostCommunicationMgr.sendMessageToHost({
                         type: "SET_THEME_CONFIG",
                         themeInfo: (0, Ae.ol)(e.emotion)
                     })
                 }, this.createThemeHash = e => {
@@ -127376,32 +127793,34 @@
                         const e = new je._b({
                             debugDisconnectWebsocket: !0
                         });
                         e.type = "debugDisconnectWebsocket", this.sendBackMsg(e)
                     }
                 }, this.debugClearForwardMsgCache = () => {
                     var e, t;
-                    zl() && (null === (e = this.connectionManager) || void 0 === e || null === (t = e.connection) || void 0 === t || t.cache.messages.clear())
+                    Sl() && (null === (e = this.connectionManager) || void 0 === e || null === (t = e.connection) || void 0 === t || t.cache.messages.clear())
                 }, this.rerunScript = function() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                     t.closeDialog(), t.isServerConnected() ? t.state.scriptRunState !== Qe.RUNNING && t.state.scriptRunState !== Qe.RERUN_REQUESTED && (t.metricsMgr.enqueue("rerunScript"), t.setState({
                         scriptRunState: Qe.RERUN_REQUESTED
                     }), !0 === e && t.saveSettings({
                         ...t.state.userSettings,
                         runOnSave: !0
                     }), t.widgetMgr.sendUpdateWidgetsMessage(void 0)) : (0, ui.H)("Cannot rerun script when disconnected from server.")
                 }, this.sendLoadGitInfoBackMsg = () => {
                     this.isServerConnected() ? this.sendBackMsg(new je._b({
                         loadGitInfo: !0
                     })) : (0, ui.H)("Cannot load git information when disconnected from server.")
                 }, this.onPageChange = e => {
-                    this.setState({
-                        appLogo: null
-                    }), this.sendRerunBackMsg(void 0, void 0, e)
-                }, this.isAppInReadyState = e => this.state.connectionState === Us.CONNECTED && this.state.scriptRunState === Qe.NOT_RUNNING && e.scriptRunState === Qe.RUNNING && e.connectionState === Us.CONNECTED, this.sendRerunBackMsg = (e, t, n) => {
+                    const {
+                        elements: t,
+                        mainScriptHash: n
+                    } = this.state, r = this.appNavigation.clearPageElements(t, n, void 0), o = new Set(Array.from(r.getElements()).map((e => (0, Xe.po)(e))).filter(Xe.Av));
+                    this.sendRerunBackMsg(this.widgetMgr.getActiveWidgetStates(o), void 0, e)
+                }, this.isAppInReadyState = e => this.state.connectionState === Gs.CONNECTED && this.state.scriptRunState === Qe.NOT_RUNNING && e.scriptRunState === Qe.RUNNING && e.connectionState === Gs.CONNECTED, this.sendRerunBackMsg = (e, t, n) => {
                     const r = this.getBaseUriParts();
                     if (!r) return void(0, ui.H)("Cannot send rerun backMessage when disconnected from server.");
                     const {
                         currentPageScriptHash: o
                     } = this.state, {
                         basePath: i
                     } = r;
@@ -127414,15 +127833,15 @@
                         rerunScript: {
                             queryString: a,
                             widgetStates: e,
                             pageScriptHash: n,
                             pageName: s,
                             fragmentId: t
                         }
-                    })), wu.record({
+                    })), xu.record({
                         name: "RequestedRerun",
                         scriptRunState: this.state.scriptRunState
                     })
                 }, this.stopScript = () => {
                     if (!this.isServerConnected()) return void(0, ui.H)("Cannot stop app when disconnected from server.");
                     if (this.state.scriptRunState === Qe.NOT_RUNNING || this.state.scriptRunState === Qe.STOP_REQUESTED) return;
                     const e = new je._b({
@@ -127430,34 +127849,34 @@
                     });
                     e.type = "stopScript", this.sendBackMsg(e), this.setState({
                         scriptRunState: Qe.STOP_REQUESTED
                     })
                 }, this.openClearCacheDialog = () => {
                     if (this.isServerConnected()) {
                         const e = {
-                            type: ou.CLEAR_CACHE,
+                            type: cu.CLEAR_CACHE,
                             confirmCallback: this.clearCache,
                             defaultAction: this.clearCache,
                             onClose: () => {}
                         };
                         this.openDialog(e)
                     } else(0, ui.H)("Cannot clear cache: disconnected from server")
                 }, this.openDeployDialog = () => {
                     var e;
                     const t = {
-                        type: ou.DEPLOY_DIALOG,
+                        type: cu.DEPLOY_DIALOG,
                         onClose: this.closeDialog,
                         showDeployError: this.showDeployError,
-                        isDeployErrorModalOpen: (null === (e = this.state.dialog) || void 0 === e ? void 0 : e.type) === ou.DEPLOY_ERROR,
+                        isDeployErrorModalOpen: (null === (e = this.state.dialog) || void 0 === e ? void 0 : e.type) === cu.DEPLOY_ERROR,
                         metricsMgr: this.metricsMgr
                     };
                     this.openDialog(t)
                 }, this.openThemeCreatorDialog = () => {
                     const e = {
-                        type: ou.THEME_CREATOR,
+                        type: cu.THEME_CREATOR,
                         backToSettings: this.settingsCallback,
                         onClose: this.closeDialog
                     };
                     this.openDialog(e)
                 }, this.clearCache = () => {
                     if (this.closeDialog(), this.isServerConnected()) {
                         this.metricsMgr.enqueue("clearCache");
@@ -127476,31 +127895,31 @@
                 }, this.sendBackMsg = e => {
                     this.connectionManager ? ((0, ui.ji)(e), this.connectionManager.sendMessage(e)) : (0, ui.H)("Not connected. Cannot send back message: ".concat(e))
                 }, this.handleConnectionError = e => {
                     this.showError("Connection error", e)
                 }, this.isServerConnected = () => !!this.connectionManager && this.connectionManager.isConnected(), this.settingsCallback = function() {
                     let e = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0];
                     const n = {
-                        type: ou.SETTINGS,
+                        type: cu.SETTINGS,
                         isServerConnected: t.isServerConnected(),
                         settings: t.state.userSettings,
                         allowRunOnSave: t.state.allowRunOnSave,
                         onSave: t.saveSettings,
                         onClose: () => {},
-                        developerMode: Pp(t.state.isOwner, t.state.toolbarMode),
+                        developerMode: Gp(t.state.isOwner, t.state.toolbarMode),
                         openThemeCreator: t.openThemeCreatorDialog,
                         animateModal: e,
                         metricsMgr: t.metricsMgr
                     };
                     t.openDialog(n)
                 }, this.aboutCallback = () => {
                     const {
                         menuItems: e
                     } = this.state, t = {
-                        type: ou.ABOUT,
+                        type: cu.ABOUT,
                         sessionInfo: this.sessionInfo,
                         onClose: this.closeDialog,
                         aboutSectionMd: null === e || void 0 === e ? void 0 : e.aboutSectionMd
                     };
                     this.openDialog(t)
                 }, this.printCallback = () => {
                     const {
@@ -127537,27 +127956,27 @@
                     })
                 }, this.addScriptFinishedHandler = e => {
                     this.setState(((t, n) => ({
                         scriptFinishedHandlers: t.scriptFinishedHandlers.concat(e)
                     })))
                 }, this.removeScriptFinishedHandler = e => {
                     this.setState(((t, n) => ({
-                        scriptFinishedHandlers: sp()(t.scriptFinishedHandlers, e)
+                        scriptFinishedHandlers: dp()(t.scriptFinishedHandlers, e)
                     })))
                 }, this.getBaseUriParts = () => this.connectionManager ? this.connectionManager.getBaseUriParts() : void 0, this.getQueryString = () => {
                     const {
                         queryParams: e
                     } = this.state, t = e && e.length > 0 ? e : document.location.search;
                     return t.startsWith("?") ? t.substring(1) : t
                 }, this.isInCloudEnvironment = () => {
                     const {
                         hostMenuItems: e
                     } = this.state;
                     return e && (null === e || void 0 === e ? void 0 : e.length) > 0
-                }, this.showDeployButton = () => Pp(this.state.isOwner, this.state.toolbarMode) && !this.isInCloudEnvironment() && this.sessionInfo.isSet && !this.sessionInfo.isHello, this.deployButtonClicked = () => {
+                }, this.showDeployButton = () => Gp(this.state.isOwner, this.state.toolbarMode) && !this.isInCloudEnvironment() && this.sessionInfo.isSet && !this.sessionInfo.isHello, this.deployButtonClicked = () => {
                     this.metricsMgr.enqueue("menuClick", {
                         label: "deployButtonInApp"
                     }), this.sendLoadGitInfoBackMsg(), this.openDeployDialog()
                 }, this.requestFileURLs = (e, t) => {
                     if (this.isServerConnected()) {
                         const n = new je._b({
                             fileUrlsRequest: {
@@ -127565,36 +127984,37 @@
                                 fileNames: t.map((e => e.name)),
                                 sessionId: this.sessionInfo.current.sessionId
                             }
                         });
                         n.type = "fileUrlsRequest", this.sendBackMsg(n)
                     }
                 }, (0, Pe.GP)(), this.state = {
-                    connectionState: Us.INITIAL,
-                    elements: Ye.empty(!0),
+                    connectionState: Gs.INITIAL,
+                    elements: Ye.empty("", !0),
                     isFullScreen: !1,
                     scriptName: "",
-                    scriptRunId: Ip,
+                    scriptRunId: Xp,
                     appHash: null,
                     scriptRunState: Qe.NOT_RUNNING,
                     userSettings: {
                         wideMode: !1,
                         runOnSave: !1
                     },
                     layout: je.Pz.Layout.CENTERED,
                     initialSidebarState: je.Pz.SidebarState.AUTO,
                     menuItems: void 0,
                     allowRunOnSave: !0,
                     scriptFinishedHandlers: [],
                     themeHash: this.createThemeHash(),
                     gitInfo: null,
-                    formsData: Uu(),
-                    appLogo: null,
+                    formsData: $u(),
                     appPages: [],
+                    navSections: [],
                     currentPageScriptHash: "",
+                    mainScriptHash: "",
                     hideTopBar: !0,
                     hideSidebarNav: !0,
                     toolbarMode: je.De.ToolbarMode.MINIMAL,
                     latestRunTime: performance.now(),
                     fragmentIdsThisRun: [],
                     isOwner: !1,
                     hostMenuItems: [],
@@ -127604,20 +128024,20 @@
                     pageLinkBaseUrl: "",
                     queryParams: "",
                     deployedAppMetadata: {},
                     libConfig: {},
                     appConfig: {},
                     autoReruns: [],
                     inputsDisabled: !1
-                }, this.connectionManager = null, this.widgetMgr = new Xu({
+                }, this.connectionManager = null, this.widgetMgr = new Zu({
                     sendRerunBackMsg: this.sendRerunBackMsg,
                     formsDataChanged: e => this.setState({
                         formsData: e
                     })
-                }), this.hostCommunicationMgr = new $u({
+                }), this.hostCommunicationMgr = new Qu({
                     sendRerunBackMsg: this.sendRerunBackMsg,
                     closeModal: this.closeDialog,
                     stopScript: this.stopScript,
                     rerunScript: this.rerunScript,
                     clearCache: this.clearCache,
                     sendAppHeartbeat: this.sendAppHeartbeat,
                     setInputsDisabled: e => {
@@ -127671,30 +128091,30 @@
                         })
                     },
                     deployedAppMetadataChanged: e => {
                         this.setState({
                             deployedAppMetadata: e
                         })
                     }
-                }), this.endpoints = new lp({
+                }), this.endpoints = new bp({
                     getServerUri: this.getBaseUriParts,
                     csrfEnabled: !0
-                }), this.uploadClient = new op({
+                }), this.uploadClient = new cp({
                     sessionInfo: this.sessionInfo,
                     endpoints: this.endpoints,
                     formsWithPendingRequestsChanged: e => this.widgetMgr.setFormsWithUploads(e),
                     requestFileURLs: this.requestFileURLs
-                }), this.componentRegistry = new ip(this.endpoints), this.pendingElementsTimerRunning = !1, this.pendingElementsBuffer = this.state.elements, window.streamlitDebug = {
+                }), this.componentRegistry = new up(this.endpoints), this.pendingElementsTimerRunning = !1, this.pendingElementsBuffer = this.state.elements, this.appNavigation = new Hp(this.hostCommunicationMgr, this.maybeUpdatePageUrl, this.onPageNotFound, this.onPageIconChanged), window.streamlitDebug = {
                     clearForwardMsgCache: this.debugClearForwardMsgCache,
                     disconnectWebsocket: this.debugDisconnectWebsocket,
                     shutdownRuntime: this.debugShutdownRuntime
                 }
             }
             componentDidMount() {
-                this.connectionManager = new Cu({
+                this.connectionManager = new Pu({
                     sessionInfo: this.sessionInfo,
                     endpoints: this.endpoints,
                     onMessage: this.handleMessage,
                     onConnectionError: this.handleConnectionError,
                     connectionStateChanged: this.handleConnectionStateChanged,
                     claimHostAuthToken: this.hostCommunicationMgr.claimAuthToken,
                     resetHostAuthToken: this.hostCommunicationMgr.resetAuthToken,
@@ -127740,15 +128160,15 @@
             componentWillUnmount() {
                 var e;
                 null === (e = this.connectionManager) || void 0 === e || e.disconnect(), this.hostCommunicationMgr.closeHostCommunication(), window.removeEventListener("popstate", this.onHistoryChange, !1)
             }
             showError(e, t) {
                 (0, ui.H)(t);
                 const n = {
-                    type: ou.WARNING,
+                    type: cu.WARNING,
                     title: e,
                     msg: t,
                     onClose: () => {}
                 };
                 this.openDialog(n)
             }
             hasStreamlitVersionChanged(e) {
@@ -127757,14 +128177,20 @@
                         {
                             environmentInfo: n
                         } = e;
                     if (null != n && null != n.streamlitVersion) return t != n.streamlitVersion
                 }
                 return !1
             }
+            maybeSetState(e) {
+                if (e) {
+                    const [t, n] = e;
+                    this.setState(t, n)
+                }
+            }
             processThemeInput(e) {
                 const t = this.createThemeHash(e);
                 if (t === this.state.themeHash) return;
                 this.setState({
                     themeHash: t
                 });
                 const n = !(0, Ae.MJ)(this.props.theme.activeTheme);
@@ -127791,26 +128217,28 @@
                         })), e === je.eI.ScriptFinishedStatus.FINISHED_SUCCESSFULLY || e === je.eI.ScriptFinishedStatus.FINISHED_FRAGMENT_RUN_SUCCESSFULLY) {
                         const e = new Set(Array.from(this.state.elements.getElements()).map((e => (0, Xe.po)(e))).filter(Xe.Av));
                         this.widgetMgr.removeInactive(e)
                     }
                     null !== this.connectionManager && e !== je.eI.ScriptFinishedStatus.FINISHED_EARLY_FOR_RERUN && this.sessionInfo.isSet && this.connectionManager.incrementMessageCacheRunCount(this.sessionInfo.current.maxCachedMessageAge)
                 }
             }
-            clearAppState(e, t, n) {
+            clearAppState(e, t, n, r) {
                 const {
-                    hideSidebarNav: r,
-                    elements: o
-                } = this.state, i = r && o.sidebar || void 0;
+                    hideSidebarNav: o,
+                    elements: i
+                } = this.state, a = o && i.sidebar || void 0;
                 this.setState({
                     scriptRunId: t,
                     scriptName: n,
                     appHash: e,
-                    elements: Ye.empty(!1, i)
+                    elements: this.appNavigation.clearPageElements(this.pendingElementsBuffer, r, a)
                 }, (() => {
-                    this.pendingElementsBuffer = this.state.elements, this.widgetMgr.removeInactive(new Set([]))
+                    this.pendingElementsBuffer = this.state.elements;
+                    const e = new Set(Array.from(this.state.elements.getElements()).map((e => (0, Xe.po)(e))).filter(Xe.Av));
+                    this.widgetMgr.removeInactive(e)
                 }))
             }
             openDialog(e) {
                 this.setState({
                     dialog: e
                 })
             }
@@ -127832,22 +128260,24 @@
                     hostHideSidebarNav: b,
                     pageLinkBaseUrl: f,
                     sidebarChevronDownshift: h,
                     hostMenuItems: m,
                     hostToolbarItems: M,
                     libConfig: O,
                     appConfig: g,
-                    inputsDisabled: z
-                } = this.state, y = Pp(this.state.isOwner, this.state.toolbarMode), A = Be()("stApp", (0, Xe.l7)(this.embeddingId), {
+                    inputsDisabled: z,
+                    appPages: y,
+                    navSections: A
+                } = this.state, v = Gp(this.state.isOwner, this.state.toolbarMode), w = Be()("stApp", (0, Xe.l7)(this.embeddingId), {
                     "streamlit-embedded": (0, Xe.P2)(),
                     "streamlit-wide": c.wideMode
-                }), v = n ? iu({
+                }), S = n ? uu({
                     ...n,
                     onClose: this.closeDialog
-                }) : null, w = z || t !== Us.CONNECTED;
+                }) : null, q = z || t !== Gs.CONNECTED;
                 return (0, ze.jsx)(Fe.Provider, {
                     value: {
                         initialSidebarState: o,
                         wideMode: c.wideMode,
                         embedded: (0, Xe.P2)(),
                         showPadding: !(0, Xe.P2)() || (0, Xe._A)(),
                         disableScrolling: (0, Xe.G$)(),
@@ -127874,76 +128304,77 @@
                             fragmentIdsThisRun: this.state.fragmentIdsThisRun
                         },
                         children: (0, ze.jsx)(Ie.HotKeys, {
                             keyMap: this.keyMap,
                             handlers: this.keyHandlers,
                             attach: window,
                             focused: !0,
-                            children: (0, ze.jsxs)(dp, {
-                                className: A,
+                            children: (0, ze.jsxs)(Mp, {
+                                className: w,
                                 "data-testid": "stApp",
-                                "data-teststate": s == Ip ? "initial" : l,
-                                children: [(0, ze.jsxs)(Ll, {
+                                "data-teststate": s == Xp ? "initial" : l,
+                                children: [(0, ze.jsxs)(jl, {
                                     children: [!u && (0, ze.jsxs)(ze.Fragment, {
-                                        children: [(0, ze.jsx)(tl, {
+                                        children: [(0, ze.jsx)(il, {
                                             connectionState: t,
                                             sessionEventDispatcher: this.sessionEventDispatcher,
                                             scriptRunState: l,
                                             rerunScript: this.rerunScript,
                                             stopScript: this.stopScript,
                                             allowRunOnSave: e
-                                        }), (0, ze.jsx)(xl, {
+                                        }), (0, ze.jsx)(Wl, {
                                             hostToolbarItems: M,
                                             sendMessageToHost: this.hostCommunicationMgr.sendMessageToHost,
                                             metricsMgr: this.metricsMgr
                                         })]
-                                    }), this.showDeployButton() && (0, ze.jsx)(kl, {
+                                    }), this.showDeployButton() && (0, ze.jsx)(Il, {
                                         onClick: this.deployButtonClicked.bind(this)
-                                    }), (0, ze.jsx)(wl, {
+                                    }), (0, ze.jsx)(xl, {
                                         isServerConnected: this.isServerConnected(),
                                         quickRerunCallback: this.rerunScript,
                                         clearCacheCallback: this.openClearCacheDialog,
                                         settingsCallback: this.settingsCallback,
                                         aboutCallback: this.aboutCallback,
                                         printCallback: this.printCallback,
                                         screencastCallback: this.screencastCallback,
                                         screenCastState: this.props.screenCast.currentState,
                                         hostMenuItems: m,
-                                        developmentMode: y,
+                                        developmentMode: v,
                                         sendMessageToHost: this.hostCommunicationMgr.sendMessageToHost,
                                         menuItems: i,
                                         metricsMgr: this.metricsMgr,
                                         toolbarMode: this.state.toolbarMode
                                     })]
-                                }), (0, ze.jsx)(zs, {
+                                }), (0, ze.jsx)(ws, {
                                     endpoints: this.endpoints,
                                     sessionInfo: this.sessionInfo,
                                     sendMessageToHost: this.hostCommunicationMgr.sendMessageToHost,
                                     elements: r,
                                     scriptRunId: s,
                                     scriptRunState: l,
                                     widgetMgr: this.widgetMgr,
-                                    widgetsDisabled: w,
+                                    widgetsDisabled: q,
                                     uploadClient: this.uploadClient,
                                     componentRegistry: this.componentRegistry,
                                     formsData: this.state.formsData,
-                                    appLogo: this.state.appLogo,
-                                    appPages: this.state.appPages,
+                                    appLogo: r.logo,
+                                    appPages: y,
+                                    navSections: A,
                                     onPageChange: this.onPageChange,
                                     currentPageScriptHash: d,
                                     hideSidebarNav: p || b
-                                }), v]
+                                }), S]
                             })
                         })
                     })
                 })
             }
         }
-        const Bp = Lp(Dp);
-        const jp = () => {
+        const Kp = jp($p);
+        const Yp = () => {
                 const [e, t] = function() {
                     const e = (0, Ae.Vx)(),
                         [t, r] = (0, n.useState)(e),
                         [o, i] = (0, n.useState)([]),
                         [a, s] = (0, n.useState)([...(0, Ae.Uy)(), ...(0, Ae.MJ)(e) ? [] : [e]]),
                         l = (0, n.useCallback)((e => {
                             e !== t && (r(e), e.name === Ae.oo ? (0, Ae.rk)() : (0, Ae.b3)(e))
@@ -127976,24 +128407,24 @@
                 }(), {
                     activeTheme: r
                 } = e, o = r.name === Ae.UO && t.length > 0;
                 return (0, ze.jsxs)(We, {
                     theme: r,
                     children: [o && (0, ze.jsx)(ye, {
                         fontFaces: t
-                    }), (0, ze.jsx)(Bp, {
+                    }), (0, ze.jsx)(Kp, {
                         theme: e
-                    }), (0, ze.jsx)(bp, {
+                    }), (0, ze.jsx)(Op, {
                         id: "portal",
                         "data-testid": "portal"
                     })]
                 })
             },
-            Fp = new Me({
+            Zp = new Me({
                 prefix: "st-"
             });
         r.render((0, ze.jsx)(Oe.zt, {
-            value: Fp,
-            children: (0, ze.jsx)(jp, {})
+            value: Zp,
+            children: (0, ze.jsx)(Yp, {})
         }), document.getElementById("root"))
     })()
 })();
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/js/main.9978e612.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/js/main.707da454.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.35.1.dev20240531/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/string_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/temporary_directory.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/testing/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/app_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from streamlit.proto.WidgetStates_pb2 import WidgetStates
 from streamlit.runtime import Runtime
 from streamlit.runtime.caching.storage.dummy_cache_storage import (
     MemoryCacheStorageManager,
 )
 from streamlit.runtime.media_file_manager import MediaFileManager
 from streamlit.runtime.memory_media_file_storage import MemoryMediaFileStorage
+from streamlit.runtime.pages_manager import PagesManager
 from streamlit.runtime.secrets import Secrets
 from streamlit.runtime.state.common import TESTING_KEY
 from streamlit.runtime.state.safe_session_state import SafeSessionState
 from streamlit.runtime.state.session_state import SessionState
 from streamlit.testing.v1.element_tree import (
     Block,
     Button,
@@ -317,27 +318,32 @@
         # setup
         mock_runtime = MagicMock(spec=Runtime)
         mock_runtime.media_file_mgr = MediaFileManager(
             MemoryMediaFileStorage("/mock/media")
         )
         mock_runtime.cache_storage_manager = MemoryCacheStorageManager()
         Runtime._instance = mock_runtime
+        pages_manager = PagesManager(self._script_path, setup_watcher=False)
         with source_util._pages_cache_lock:
             saved_cached_pages = source_util._cached_pages
             source_util._cached_pages = None
 
         saved_secrets: Secrets = st.secrets
         # Only modify global secrets stuff if we have been given secrets
         if self.secrets:
             new_secrets = Secrets([])
             new_secrets._secrets = self.secrets
             st.secrets = new_secrets
 
         script_runner = LocalScriptRunner(
-            self._script_path, self.session_state, args=self.args, kwargs=self.kwargs
+            self._script_path,
+            self.session_state,
+            pages_manager,
+            args=self.args,
+            kwargs=self.kwargs,
         )
         with patch_config_options({"global.appTest": True}):
             self._tree = script_runner.run(
                 widget_state, self.query_params, timeout, self._page_hash
             )
             self._tree._runner = self
         # Last event is SHUTDOWN, so the corresponding data includes query string
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/local_script_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,37 +12,41 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import os
 import time
 import types
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from urllib import parse
 
 from streamlit import runtime
 from streamlit.proto.ForwardMsg_pb2 import ForwardMsg
 from streamlit.proto.WidgetStates_pb2 import WidgetStates
 from streamlit.runtime.forward_msg_queue import ForwardMsgQueue
 from streamlit.runtime.fragment import MemoryFragmentStorage
 from streamlit.runtime.memory_uploaded_file_manager import MemoryUploadedFileManager
 from streamlit.runtime.scriptrunner import RerunData, ScriptRunner, ScriptRunnerEvent
 from streamlit.runtime.scriptrunner.script_cache import ScriptCache
 from streamlit.runtime.scriptrunner.script_run_context import ScriptRunContext
 from streamlit.runtime.state.safe_session_state import SafeSessionState
 from streamlit.testing.v1.element_tree import ElementTree, parse_tree_from_messages
 
+if TYPE_CHECKING:
+    from streamlit.runtime.pages_manager import PagesManager
+
 
 class LocalScriptRunner(ScriptRunner):
     """Subclasses ScriptRunner to provide some testing features."""
 
     def __init__(
         self,
         script_path: str,
         session_state: SafeSessionState,
+        pages_manager: "PagesManager",
         args=None,
         kwargs=None,
     ):
         """Initializes the ScriptRunner for the given script_path."""
 
         assert os.path.isfile(script_path), f"File not found at {script_path}"
 
@@ -57,14 +61,15 @@
             main_script_path=script_path,
             session_state=self.session_state._state,
             uploaded_file_mgr=MemoryUploadedFileManager("/mock/upload"),
             script_cache=ScriptCache(),
             initial_rerun_data=RerunData(),
             user_info={"email": "test@test.com"},
             fragment_storage=MemoryFragmentStorage(),
+            pages_manager=pages_manager,
         )
 
         # Accumulates all ScriptRunnerEvents emitted by us.
         self.events: list[ScriptRunnerEvent] = []
         self.event_data: list[Any] = []
 
         def record_event(
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/testing/v1/util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/time_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/type_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/url_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/user_info.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/version.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/local_sources_watcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,37 +15,40 @@
 from __future__ import annotations
 
 import collections
 import os
 import sys
 import types
 from pathlib import Path
-from typing import Callable, Final
+from typing import TYPE_CHECKING, Callable, Final
 
 from streamlit import config, file_util
 from streamlit.folder_black_list import FolderBlackList
 from streamlit.logger import get_logger
-from streamlit.source_util import get_pages
 from streamlit.watcher.path_watcher import (
     NoOpPathWatcher,
     get_default_path_watcher_class,
 )
 
+if TYPE_CHECKING:
+    from streamlit.runtime.pages_manager import PagesManager
+
 _LOGGER: Final = get_logger(__name__)
 
 WatchedModule = collections.namedtuple("WatchedModule", ["watcher", "module_name"])
 
 # This needs to be initialized lazily to avoid calling config.get_option() and
 # thus initializing config options when this file is first imported.
 PathWatcher = None
 
 
 class LocalSourcesWatcher:
-    def __init__(self, main_script_path: str):
-        self._main_script_path = os.path.abspath(main_script_path)
+    def __init__(self, pages_manager: "PagesManager"):
+        self._pages_manager = pages_manager
+        self._main_script_path = os.path.abspath(self._pages_manager.main_script_path)
         self._script_folder = os.path.dirname(self._main_script_path)
         self._on_file_changed: list[Callable[[str], None]] = []
         self._is_closed = False
         self._cached_sys_modules: set[str] = set()
 
         # Blacklist for folders that should not be watched
         self._folder_black_list = FolderBlackList(
@@ -54,30 +57,37 @@
 
         self._watched_modules: dict[str, WatchedModule] = {}
         self._watched_pages: set[str] = set()
 
         self.update_watched_pages()
 
     def update_watched_pages(self) -> None:
-        old_watched_pages = self._watched_pages
+        old_page_paths = self._watched_pages.copy()
         new_pages_paths: set[str] = set()
 
-        for page_info in get_pages(self._main_script_path).values():
+        for page_info in self._pages_manager.get_pages().values():
+            if not page_info["script_path"]:
+                continue
+
             new_pages_paths.add(page_info["script_path"])
-            if page_info["script_path"] not in old_watched_pages:
+            if page_info["script_path"] not in self._watched_pages:
                 self._register_watcher(
                     page_info["script_path"],
                     module_name=None,
                 )
 
-        for old_page_path in old_watched_pages:
-            if old_page_path not in new_pages_paths:
+        for old_page_path in old_page_paths:
+            # Only remove pages that are no longer valid files
+            if old_page_path not in new_pages_paths and not os.path.isfile(
+                old_page_path
+            ):
                 self._deregister_watcher(old_page_path)
+                self._watched_pages.remove(old_page_path)
 
-        self._watched_pages = new_pages_paths
+        self._watched_pages = self._watched_pages.union(new_pages_paths)
 
     def register_file_change_callback(self, cb: Callable[[str], None]) -> None:
         self._on_file_changed.append(cb)
 
     def on_file_changed(self, filepath):
         if filepath not in self._watched_modules:
             _LOGGER.error("Received event for non-watched file: %s", filepath)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/watcher/util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/bootstrap.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from __future__ import annotations
 
 import asyncio
 import os
 import signal
 import sys
-from pathlib import Path
 from typing import Any, Final
 
 from streamlit import (
     cli_util,
     config,
     env_util,
     file_util,
@@ -30,16 +29,15 @@
     secrets,
     util,
     version,
 )
 from streamlit.config import CONFIG_FILENAMES
 from streamlit.git_util import MIN_GIT_VERSION, GitRepo
 from streamlit.logger import get_logger
-from streamlit.source_util import invalidate_pages_cache
-from streamlit.watcher import report_watchdog_availability, watch_dir, watch_file
+from streamlit.watcher import report_watchdog_availability, watch_file
 from streamlit.web.server import Server, server_address_is_unix_socket, server_util
 
 _LOGGER: Final = get_logger(__name__)
 
 
 # The maximum possible total size of a static directory.
 # We agreed on these limitations for the initial release of static file sharing,
@@ -344,29 +342,14 @@
         load_config_options(flag_options)
 
     for filename in CONFIG_FILENAMES:
         if os.path.exists(filename):
             watch_file(filename, on_config_changed)
 
 
-def _install_pages_watcher(main_script_path_str: str) -> None:
-    def _on_pages_changed(_path: str) -> None:
-        invalidate_pages_cache()
-
-    main_script_path = Path(main_script_path_str)
-    pages_dir = main_script_path.parent / "pages"
-
-    watch_dir(
-        str(pages_dir),
-        _on_pages_changed,
-        glob_pattern="*.py",
-        allow_nonexistent=True,
-    )
-
-
 def run(
     main_script_path: str,
     is_hello: bool,
     args: list[str],
     flag_options: dict[str, Any],
 ) -> None:
     """Run a script in a separate thread and start a server for the app.
@@ -375,15 +358,14 @@
     """
     _fix_sys_path(main_script_path)
     _fix_tornado_crash()
     _fix_sys_argv(main_script_path, args)
     _fix_pydeck_mapbox_api_warning()
     _fix_pydantic_duplicate_validators_error()
     _install_config_watchers(flag_options)
-    _install_pages_watcher(main_script_path)
 
     # Create the server. It won't start running yet.
     server = Server(main_script_path, is_hello)
 
     async def run_server() -> None:
         # Start the server
         await server.start()
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/cli.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/__init__.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/routes.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/routes.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,54 +37,52 @@
     """
     return not config.get_option("server.enableCORS") or config.get_option(
         "global.developmentMode"
     )
 
 
 class StaticFileHandler(tornado.web.StaticFileHandler):
-    def initialize(self, path, default_filename, get_pages):
-        self._pages = get_pages()
+    def initialize(
+        self,
+        path: str,
+        default_filename: str | None = None,
+        reserved_paths: list[str] = [],
+    ):
+        self._reserved_paths = reserved_paths
 
-        super().initialize(path=path, default_filename=default_filename)
+        super().initialize(path, default_filename)
 
     def set_extra_headers(self, path: str) -> None:
         """Disable cache for HTML files.
 
         Other assets like JS and CSS are suffixed with their hash, so they can
         be cached indefinitely.
         """
         is_index_url = len(path) == 0
 
         if is_index_url or path.endswith(".html"):
             self.set_header("Cache-Control", "no-cache")
         else:
             self.set_header("Cache-Control", "public")
 
-    def parse_url_path(self, url_path: str) -> str:
-        url_parts = url_path.split("/")
+    def validate_absolute_path(self, root: str, absolute_path: str) -> str | None:
+        try:
+            return super().validate_absolute_path(root, absolute_path)
+        except tornado.web.HTTPError as e:
+            # If the file is not found, and there are no reserved paths,
+            # we try to serve the default file and allow the frontend to handle the issue.
+            if e.status_code == 404:
+                if any([self.path.endswith(x) for x in self._reserved_paths]):
+                    raise e
+
+                self.path = self.parse_url_path(self.default_filename or "index.html")
+                absolute_path = self.get_absolute_path(self.root, self.path)
+                return super().validate_absolute_path(root, absolute_path)
 
-        maybe_page_name = url_parts[0]
-        if maybe_page_name in self._pages:
-            # If we're trying to navigate to a page, we return "index.html"
-            # directly here instead of deferring to the superclass below after
-            # modifying the url_path. The reason why is that tornado handles
-            # requests to "directories" (which is what navigating to a page
-            # looks like) by appending a trailing '/' if there is none and
-            # redirecting.
-            #
-            # This would work, but it
-            #   * adds an unnecessary redirect+roundtrip
-            #   * adds a trailing '/' to the URL appearing in the browser, which
-            #     looks bad
-            if len(url_parts) == 1:
-                return "index.html"
-
-            url_path = "/".join(url_parts[1:])
-
-        return super().parse_url_path(url_path)
+            raise e
 
     def write_error(self, status_code: int, **kwargs) -> None:
         if status_code == 404:
             index_file = os.path.join(file_util.get_static_dir(), "index.html")
             self.render(index_file)
         else:
             super().write_error(status_code, **kwargs)
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/server.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import tornado.concurrent
 import tornado.locks
 import tornado.netutil
 import tornado.web
 import tornado.websocket
 from tornado.httpserver import HTTPServer
 
-from streamlit import cli_util, config, file_util, source_util, util
+from streamlit import cli_util, config, file_util, util
 from streamlit.config_option import ConfigOption
 from streamlit.logger import get_logger
 from streamlit.runtime import Runtime, RuntimeConfig, RuntimeState
 from streamlit.runtime.memory_media_file_storage import MemoryMediaFileStorage
 from streamlit.runtime.memory_uploaded_file_manager import MemoryUploadedFileManager
 from streamlit.runtime.runtime_util import get_max_message_size_bytes
 from streamlit.web.cache_storage_manager_config import (
@@ -82,15 +82,16 @@
 UNIX_SOCKET_PREFIX: Final = "unix://"
 
 MEDIA_ENDPOINT: Final = "/media"
 UPLOAD_FILE_ENDPOINT: Final = "/_stcore/upload_file"
 STREAM_ENDPOINT: Final = r"_stcore/stream"
 METRIC_ENDPOINT: Final = r"(?:st-metrics|_stcore/metrics)"
 MESSAGE_ENDPOINT: Final = r"_stcore/message"
-HEALTH_ENDPOINT: Final = r"(?:healthz|_stcore/health)"
+NEW_HEALTH_ENDPOINT: Final = "_stcore/health"
+HEALTH_ENDPOINT: Final = rf"(?:healthz|{NEW_HEALTH_ENDPOINT})"
 HOST_CONFIG_ENDPOINT: Final = r"_stcore/host-config"
 SCRIPT_HEALTH_CHECK_ENDPOINT: Final = (
     r"(?:script-health-check|_stcore/script-health-check)"
 )
 
 
 class RetriesExceeded(Exception):
@@ -364,20 +365,20 @@
                 [
                     (
                         make_url_path_regex(base, "(.*)"),
                         StaticFileHandler,
                         {
                             "path": "%s/" % static_path,
                             "default_filename": "index.html",
-                            "get_pages": lambda: {
-                                page_info["page_name"]
-                                for page_info in source_util.get_pages(
-                                    self.main_script_path
-                                ).values()
-                            },
+                            "reserved_paths": [
+                                # These paths are required for identifying
+                                # the base url path.
+                                NEW_HEALTH_ENDPOINT,
+                                HOST_CONFIG_ENDPOINT,
+                            ],
                         },
                     ),
                     (make_url_path_regex(base, trailing_slash=False), AddSlashHandler),
                 ]
             )
 
         return tornado.web.Application(
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/server_util.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.35.1.dev20240531/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.35.1.dev20240530
+Version: 1.35.1.dev20240531
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.35.1.dev20240531/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 streamlit/user_info.py
 streamlit/util.py
 streamlit/version.py
 streamlit/commands/__init__.py
 streamlit/commands/execution_control.py
 streamlit/commands/experimental_query_params.py
 streamlit/commands/logo.py
+streamlit/commands/navigation.py
 streamlit/commands/page_config.py
 streamlit/components/__init__.py
 streamlit/components/lib/__init__.py
 streamlit/components/lib/local_component_registry.py
 streamlit/components/types/__init__.py
 streamlit/components/types/base_component_registry.py
 streamlit/components/types/base_custom_component.py
@@ -128,14 +129,16 @@
 streamlit/hello/Hello.py
 streamlit/hello/__init__.py
 streamlit/hello/utils.py
 streamlit/hello/pages/0_Animation_Demo.py
 streamlit/hello/pages/1_Plotting_Demo.py
 streamlit/hello/pages/2_Mapping_Demo.py
 streamlit/hello/pages/3_DataFrame_Demo.py
+streamlit/navigation/__init__.py
+streamlit/navigation/page.py
 streamlit/proto/Alert_pb2.py
 streamlit/proto/Alert_pb2.pyi
 streamlit/proto/AppPage_pb2.py
 streamlit/proto/AppPage_pb2.pyi
 streamlit/proto/ArrowNamedDataSet_pb2.py
 streamlit/proto/ArrowNamedDataSet_pb2.pyi
 streamlit/proto/ArrowVegaLiteChart_pb2.py
@@ -220,14 +223,16 @@
 streamlit/proto/Markdown_pb2.pyi
 streamlit/proto/Metric_pb2.py
 streamlit/proto/Metric_pb2.pyi
 streamlit/proto/MultiSelect_pb2.py
 streamlit/proto/MultiSelect_pb2.pyi
 streamlit/proto/NamedDataSet_pb2.py
 streamlit/proto/NamedDataSet_pb2.pyi
+streamlit/proto/Navigation_pb2.py
+streamlit/proto/Navigation_pb2.pyi
 streamlit/proto/NewSession_pb2.py
 streamlit/proto/NewSession_pb2.pyi
 streamlit/proto/NumberInput_pb2.py
 streamlit/proto/NumberInput_pb2.pyi
 streamlit/proto/PageConfig_pb2.py
 streamlit/proto/PageConfig_pb2.pyi
 streamlit/proto/PageInfo_pb2.py
@@ -292,14 +297,15 @@
 streamlit/runtime/fragment.py
 streamlit/runtime/media_file_manager.py
 streamlit/runtime/media_file_storage.py
 streamlit/runtime/memory_media_file_storage.py
 streamlit/runtime/memory_session_storage.py
 streamlit/runtime/memory_uploaded_file_manager.py
 streamlit/runtime/metrics_util.py
+streamlit/runtime/pages_manager.py
 streamlit/runtime/runtime.py
 streamlit/runtime/runtime_util.py
 streamlit/runtime/script_data.py
 streamlit/runtime/secrets.py
 streamlit/runtime/session_manager.py
 streamlit/runtime/stats.py
 streamlit/runtime/uploaded_file_manager.py
@@ -365,26 +371,23 @@
 streamlit/static/static/js/4177.69f9f18d.chunk.js
 streamlit/static/static/js/4319.bf1c86bf.chunk.js
 streamlit/static/static/js/4477.1bd49702.chunk.js
 streamlit/static/static/js/4500.b6f348d1.chunk.js
 streamlit/static/static/js/4666.c4b22a63.chunk.js
 streamlit/static/static/js/474.7eb0c6cd.chunk.js
 streamlit/static/static/js/5106.44f0ff51.chunk.js
-streamlit/static/static/js/5117.04bfe5d3.chunk.js
 streamlit/static/static/js/5249.f2f4070d.chunk.js
 streamlit/static/static/js/5345.73d26e5d.chunk.js
 streamlit/static/static/js/5379.f08eddd1.chunk.js
 streamlit/static/static/js/5441.1b94928f.chunk.js
 streamlit/static/static/js/5791.9a42fb4b.chunk.js
 streamlit/static/static/js/6013.4ba2d616.chunk.js
 streamlit/static/static/js/6405.ac5a6f23.chunk.js
 streamlit/static/static/js/6718.802da17e.chunk.js
 streamlit/static/static/js/6853.93dd1c4c.chunk.js
-streamlit/static/static/js/6950.70fe55c2.chunk.js
-streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
 streamlit/static/static/js/7142.83028745.chunk.js
 streamlit/static/static/js/7175.583ff733.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
 streamlit/static/static/js/7483.64f23be7.chunk.js
 streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
 streamlit/static/static/js/7602.e8abc06b.chunk.js
@@ -392,23 +395,26 @@
 streamlit/static/static/js/8005.43974a35.chunk.js
 streamlit/static/static/js/8148.293984e0.chunk.js
 streamlit/static/static/js/8427.bd0a7cf3.chunk.js
 streamlit/static/static/js/8477.de889fe5.chunk.js
 streamlit/static/static/js/8492.0d93bd08.chunk.js
 streamlit/static/static/js/8536.f8de3d9a.chunk.js
 streamlit/static/static/js/8570.6de19120.chunk.js
+streamlit/static/static/js/8571.cfc22b99.chunk.js
 streamlit/static/static/js/8691.4211c305.chunk.js
 streamlit/static/static/js/9330.2b4c99e0.chunk.js
 streamlit/static/static/js/9336.3e046ad7.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.9978e612.js
-streamlit/static/static/js/main.9978e612.js.LICENSE.txt
+streamlit/static/static/js/9945.47d54f35.chunk.js
+streamlit/static/static/js/9945.47d54f35.chunk.js.LICENSE.txt
+streamlit/static/static/js/main.707da454.js
+streamlit/static/static/js/main.707da454.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.35.1.dev20240530/tests/testutil.py` & `streamlit_nightly-1.35.1.dev20240531/tests/testutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 from contextlib import contextmanager
 from typing import TYPE_CHECKING
 
 from streamlit import config
 from streamlit.runtime.fragment import MemoryFragmentStorage
 from streamlit.runtime.memory_uploaded_file_manager import MemoryUploadedFileManager
+from streamlit.runtime.pages_manager import PagesManager
 from streamlit.runtime.scriptrunner import ScriptRunContext
 from streamlit.runtime.state import SafeSessionState, SessionState
 from tests.constants import SNOWFLAKE_CREDENTIAL_FILE
 
 if TYPE_CHECKING:
     from snowflake.snowpark import Session
 
@@ -49,17 +50,17 @@
     return ScriptRunContext(
         session_id="mock_session_id",
         _enqueue=lambda msg: None,
         query_string="mock_query_string",
         session_state=SafeSessionState(SessionState(), lambda: None),
         uploaded_file_mgr=MemoryUploadedFileManager("/mock/upload"),
         main_script_path="",
-        page_script_hash="mock_page_script_hash",
         user_info={"email": "mock@test.com"},
         fragment_storage=MemoryFragmentStorage(),
+        pages_manager=PagesManager(""),
     )
 
 
 def build_mock_config_is_manually_set(overrides_dict):
     orig_is_manually_set = config.is_manually_set
 
     def mock_config_is_manually_set(name):
```

