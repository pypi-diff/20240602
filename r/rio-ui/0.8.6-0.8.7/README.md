# Comparing `tmp/rio_ui-0.8.6.tar.gz` & `tmp/rio_ui-0.8.7.tar.gz`

## Comparing `rio_ui-0.8.6.tar` & `rio_ui-0.8.7.tar`

### file list

```diff
@@ -1,385 +1,392 @@
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.prettierrc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.sassrc
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.8.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 rio_ui-0.8.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 rio_ui-0.8.6/SECURITY.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 rio_ui-0.8.6/changelog.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 rio_ui-0.8.6/package.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 rio_ui-0.8.6/vite.config.js
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/DISCUSSION_TEMPLATE/feature-requests.yml
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/index.html
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20719 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/eventRateLimiter.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/layouting.ts
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/rippleEffect.ts
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/utils.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/button.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/card.ts
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/codeBlock.ts
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/devToolsConnector.ts
--rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/html.ts
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/code/components/website.ts
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    51597 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/style.scss
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.8.6/frontend/css/switcheroos.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.8.6/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/__main__.py
--rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/app.py
--rw-r--r--   0        0        0    33083 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/app_server.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/byte_serving.py
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/color.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cursor_style.py
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/dataclass.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/deprecations.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/errors.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/event.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/global_state.py
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/icon_registry.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/inspection.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/py.typed
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/self_serializing.py
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/serialization.py
--rw-r--r--   0        0        0    89510 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/session.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/session_attachments.py
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/state_properties.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/testing.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/text_style.py
--rw-r--r--   0        0        0    30066 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/theme.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/user_settings_module.py
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/utils.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/world_units.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/hosted/README.md
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/project.py
--rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    26835 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/__init__.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/app_root.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/auto_form.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/banner.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/build_failed.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/button.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/card.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/class_container.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/code_block.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/color_picker.py
--rw-r--r--   0        0        0    30717 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/component.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/component_tree.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/dev_tools_connector.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/devel_component.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/drawer.py
--rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/dropdown.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/flow_container.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/grid.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/html.py
--rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/icon.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/image.py
--rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/labeled_column.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/linear_containers.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/link.py
--rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/list_items.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/list_view.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/markdown.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/media_player.py
--rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/node_input.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/node_output.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/number_input.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/overlay.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/page_view.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/plot.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/popup.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/progress_circle.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/rectangle.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/revealer.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/root_components.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/scroll_container.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/separator.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/slider.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/slideshow.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/spacer.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/stack.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/switch.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/switcher.py
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/table.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/text.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/text_input.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/tooltip.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/__init__.py
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/component_details.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/deploy_page.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/dev_tools_sidebar.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/docs_page.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/icons_page.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/project_page.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/sample_icons_grid.py
--rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/debug/dev_tools/tree_page.py
--rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/docs/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/frontend files/index.html
--rw-r--r--   0        0        0   361140 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/frontend files/assets/index-8ca8e5f1.js
--rw-r--r--   0        0        0    57852 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/frontend files/assets/index-9eba151c.css
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/README.md
--rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/core-classes.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/debugging-setup.md
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/deployment.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-custom-events.md
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-install.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/persistent-settings.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/project-setup.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/run-project.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos/theming.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/custom-events.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/force-refresh.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/layouting.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/README.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
--rw-r--r--   0        0        0   209356 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/README.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/data_models.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/meta.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/root_init.py
--rw-r--r--   0        0        0   136134 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/benchmark.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/build_frontend.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/code_coverage.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 rio_ui-0.8.6/scripts/publish_new_release.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_app_build.py
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_attribute_bindings.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_custom_components.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_documentation.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_project_templates.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_reconciliation.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_refresh.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_session.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_testing_tools.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_user_settings.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 rio_ui-0.8.6/tests/utils.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rio_ui-0.8.6/.gitignore
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.8.6/LICENSE.txt
--rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 rio_ui-0.8.6/README.md
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.8.6/pyproject.toml
--rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 rio_ui-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.sassrc
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.8.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 rio_ui-0.8.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 rio_ui-0.8.7/SECURITY.md
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 rio_ui-0.8.7/changelog.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 rio_ui-0.8.7/devel.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 rio_ui-0.8.7/package.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio.toml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 rio_ui-0.8.7/vite.config.mjs
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.github/DISCUSSION_TEMPLATE/feature-requests.yml
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/index.html
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    21076 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/eventRateLimiter.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/popupManager.ts
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/button.ts
+-rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/calendar.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/codeBlock.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13511 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/devToolsConnector.ts
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/code/components/website.ts
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    54086 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.8.7/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.8.7/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/__main__.py
+-rw-r--r--   0        0        0    20286 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/app.py
+-rw-r--r--   0        0        0    36117 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/app_server.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/byte_serving.py
+-rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/color.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cursor_style.py
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/dataclass.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/deprecations.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/errors.py
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/event.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/global_state.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/inspection.py
+-rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/language_info.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/py.typed
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/self_serializing.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/serialization.py
+-rw-r--r--   0        0        0    90687 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/session.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/session_attachments.py
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/state_properties.py
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/testing.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/text_style.py
+-rw-r--r--   0        0        0    30066 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/theme.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/user_settings_module.py
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/utils.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/world_units.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/project.py
+-rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    26840 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/__init__.py
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/app_root.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/auto_form.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/banner.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/build_failed.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/button.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/calendar.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/card.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/class_container.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/code_block.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/color_picker.py
+-rw-r--r--   0        0        0    30717 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/component.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/container.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/date_input.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/dev_tools_connector.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/drawer.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/grid.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/html.py
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/icon.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/image.py
+-rw-r--r--   0        0        0    14214 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/labeled_column.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/link.py
+-rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/list_items.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/list_view.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/markdown.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/media_player.py
+-rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/node_output.py
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/number_input.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/overlay.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/page_view.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/plot.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/popup.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/rectangle.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/revealer.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/root_components.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/separator.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/slider.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/spacer.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/stack.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/switch.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/switcher.py
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/table.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/text.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/text_input.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/tooltip.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/__init__.py
+-rw-r--r--   0        0        0    12408 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/component_details.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/deploy_page.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/dev_tools_sidebar.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/icons_page.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/sample_icons_grid.py
+-rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/theme_picker_page.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/debug/dev_tools/tree_page.py
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/docs/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/frontend files/index.html
+-rw-r--r--   0        0        0   102203 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/frontend files/assets/index-BqnRx0kk.js.gz
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/frontend files/assets/index-CVJ3BDCx.css.gz
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/README.md
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/README.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
+-rw-r--r--   0        0        0   209356 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/README.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/data_models.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/meta.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/root_init.py
+-rw-r--r--   0        0        0   136134 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.8.7/scripts/benchmark.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 rio_ui-0.8.7/scripts/build_frontend.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.8.7/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.8.7/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.8.7/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 rio_ui-0.8.7/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_app_build.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_custom_components.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_documentation.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_project_templates.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_refresh.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_session.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_testing_tools.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_user_settings.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 rio_ui-0.8.7/tests/utils.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 rio_ui-0.8.7/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.8.7/LICENSE.txt
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 rio_ui-0.8.7/README.md
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 rio_ui-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 rio_ui-0.8.7/PKG-INFO
```

### Comparing `rio_ui-0.8.6/CODE_OF_CONDUCT.md` & `rio_ui-0.8.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/CONTRIBUTING.md` & `rio_ui-0.8.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/.github/PULL_REQUEST_TEMPLATE.md` & `rio_ui-0.8.7/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/.github/DISCUSSION_TEMPLATE/feature-requests.yml` & `rio_ui-0.8.7/.github/DISCUSSION_TEMPLATE/feature-requests.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/.github/ISSUE_TEMPLATE/bug_report.yml` & `rio_ui-0.8.7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/.github/ISSUE_TEMPLATE/config.yml` & `rio_ui-0.8.7/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/index.html` & `rio_ui-0.8.7/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/app.ts` & `rio_ui-0.8.7/frontend/code/app.ts`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         //
         // NOTE: If we send a `onUrlChange` message to the server, it'll cause a
         // rebuild of all PageViews and scroll to the top of the page. This is
         // why we *EITHER* send a `onUrlChange` message *OR* scroll to the
         // ScrollTarget, but not both.
 
         // FIXME: Find a way to tell whether only the url fragment changed
-        console.trace(`URL changed to ${window.location.href}`);
+        console.debug(`URL changed to ${window.location.href}`);
         callRemoteMethodDiscardResponse('onUrlChange', {
             newUrl: window.location.href.toString(),
         });
     });
 
     // Listen for resize events
     window.addEventListener('resize', (event) => {
```

### Comparing `rio_ui-0.8.6/frontend/code/colorConversion.ts` & `rio_ui-0.8.7/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/componentManagement.ts` & `rio_ui-0.8.7/frontend/code/componentManagement.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import { AlignComponent } from './components/align';
 import { BuildFailedComponent } from './components/buildFailed';
 import { ButtonComponent } from './components/button';
+import { CalendarComponent } from './components/calendar';
 import { CardComponent } from './components/card';
 import { ClassContainerComponent } from './components/classContainer';
 import { CodeBlockComponent } from './components/codeBlock';
 import { CodeExplorerComponent } from './components/codeExplorer';
 import { ColorPickerComponent } from './components/colorPicker';
 import { ColumnComponent, RowComponent } from './components/linearContainers';
 import { ComponentBase, ComponentState } from './components/componentBase';
@@ -57,14 +58,15 @@
 import { TooltipComponent } from './components/tooltip';
 import { updateLayout } from './layouting';
 
 const COMPONENT_CLASSES = {
     'Align-builtin': AlignComponent,
     'BuildFailed-builtin': BuildFailedComponent,
     'Button-builtin': ButtonComponent,
+    'Calendar-builtin': CalendarComponent,
     'Card-builtin': CardComponent,
     'ClassContainer-builtin': ClassContainerComponent,
     'CodeBlock-builtin': CodeBlockComponent,
     'CodeExplorer-builtin': CodeExplorerComponent,
     'ColorPicker-builtin': ColorPickerComponent,
     'Column-builtin': ColumnComponent,
     'ComponentTree-builtin': ComponentTreeComponent,
@@ -467,15 +469,15 @@
         // If the component's width or height has changed, request a re-layout.
         let width_changed =
             Math.abs(deltaState._size_![0] - component.state._size_[0]) > 1e-6;
         let height_changed =
             Math.abs(deltaState._size_![1] - component.state._size_[1]) > 1e-6;
 
         if (width_changed || height_changed) {
-            console.trace(
+            console.debug(
                 `Triggering re-layout because component #${id} changed size: ${component.state._size_} -> ${deltaState._size_}`
             );
             component.makeLayoutDirty();
         }
 
         // Update the component's state
         component.state = {
@@ -513,14 +515,22 @@
     updateLayout();
 
     // If this is the first time, check if there's an #url-fragment and scroll
     // to it
     if (rootComponentId !== null) {
         scrollToUrlFragment('instant');
     }
+
+    // Notify the dev tools, if any
+    if (globalThis.RIO_DEV_TOOLS !== null) {
+        let devToolsComponent =
+            globalThis.RIO_DEV_TOOLS as DevToolsConnectorComponent;
+
+        devToolsComponent.afterComponentStateChange(deltaStates);
+    }
 }
 
 function canHaveKeyboardFocus(instance: ComponentBase): boolean {
     // @ts-expect-error
     return typeof instance.grabKeyboardFocus === 'function';
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/cssUtils.ts` & `rio_ui-0.8.7/frontend/code/cssUtils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/dataModels.ts` & `rio_ui-0.8.7/frontend/code/dataModels.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/designApplication.ts` & `rio_ui-0.8.7/frontend/code/designApplication.ts`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,14 @@
     const pattern = document.createElementNS(
         'http://www.w3.org/2000/svg',
         'pattern'
     );
     pattern.setAttribute('id', patternId);
     pattern.setAttribute('width', '100%');
     pattern.setAttribute('height', '100%');
-    pattern.setAttribute('preserveAspectRatio', aspectRatio);
 
     // Create an image
     const image = document.createElementNS(
         'http://www.w3.org/2000/svg',
         'image'
     );
     image.setAttribute('href', imageUrl);
@@ -256,15 +255,15 @@
     cssColor: string
 ): Promise<void> {
     // Is the icon already in the cache?
     let promise = ICON_PROMISE_CACHE[iconName];
 
     // No, load it from the server
     if (promise === undefined) {
-        console.trace(`Fetching icon ${iconName} from server`);
+        console.debug(`Fetching icon ${iconName} from server`);
 
         promise = fetch(`/rio/icon/${iconName}`).then((response) =>
             response.text()
         );
 
         ICON_PROMISE_CACHE[iconName] = promise;
     }
```

### Comparing `rio_ui-0.8.6/frontend/code/easeFunctions.ts` & `rio_ui-0.8.7/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/eventHandling.ts` & `rio_ui-0.8.7/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/eventRateLimiter.ts` & `rio_ui-0.8.7/frontend/code/eventRateLimiter.ts`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     // Create a closure over the state
     return (...args: any[]) => {
         // Store the arguments, so future calls can use them
         lastArgs = args;
 
         // If a timeout is already set, do nothing
         if (timeout) {
-            console.trace('Eating');
             return;
         }
 
         // Set a timeout to call the function
         timeout = window.setTimeout(() => {
             timeout = null;
             callback(...lastArgs);
```

### Comparing `rio_ui-0.8.6/frontend/code/inputBoxTools.ts` & `rio_ui-0.8.7/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/layoutHelpers.ts` & `rio_ui-0.8.7/frontend/code/layoutHelpers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/layouting.ts` & `rio_ui-0.8.7/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/rippleEffect.ts` & `rio_ui-0.8.7/frontend/code/rippleEffect.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/rpc.ts` & `rio_ui-0.8.7/frontend/code/rpc.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import { goingAway, pixelsPerRem } from './app';
-import { DevToolsConnectorComponent } from './components/devToolsConnector';
 import { componentsById, updateComponentStates } from './componentManagement';
 import {
     requestFileUpload,
     registerFont,
     closeSession,
     setTitle,
 } from './rpcFunctions';
-import { setClipboard, getClipboard, ClipboardError } from './utils';
+import {
+    setClipboard,
+    getClipboard,
+    ClipboardError,
+    getPreferredPythonDateFormatString,
+} from './utils';
 import { AsyncQueue, commitCss } from './utils';
 
 let websocket: WebSocket | null = null;
 let connectionAttempt: number = 1;
 let pingPongHandlerId: number;
 let incomingMessageQueue: AsyncQueue<JsonRpcMessage> = new AsyncQueue();
 
@@ -127,29 +131,57 @@
                 localStorage[key]
             );
         } catch (e) {
             console.warn(`Failed to parse user setting ${key}: ${e}`);
         }
     }
 
-    // Locale information:
-    // - Decimal separator
-    // - Thousands separator
+    // The names of all months
+    const monthFormatter = new Intl.DateTimeFormat('default', {
+        month: 'long',
+    });
+    const monthNamesLong: string[] = [];
+
+    for (let month = 0; month < 12; month++) {
+        const date = new Date(2000, month, 1);
+        monthNamesLong.push(monthFormatter.format(date));
+    }
+
+    // The names of all days
+    const dayFormatter = new Intl.DateTimeFormat('default', {
+        weekday: 'long',
+    });
+    const dayNamesLong: string[] = [];
+
+    for (let day = 0; day < 7; day++) {
+        const date = new Date(2000, 0, day + 3);
+        dayNamesLong.push(dayFormatter.format(date));
+    }
+
+    // Date format string
+    let dateFormatString = getPreferredPythonDateFormatString('default');
+
+    // Decimal separator
     let decimalSeparator = (1.1).toLocaleString().replace(/1/g, '');
+
+    // Thousands separator
     let thousandsSeparator = (1111).toLocaleString().replace(/1/g, '');
 
     sendMessageOverWebsocket({
         websiteUrl: window.location.href,
+        userSettings: userSettings,
+        prefersLightTheme: !window.matchMedia('(prefers-color-scheme: dark)')
+            .matches,
         preferredLanguages: navigator.languages,
+        monthNamesLong: monthNamesLong,
+        dayNamesLong: dayNamesLong,
+        dateFormatString: dateFormatString,
         timezone: Intl.DateTimeFormat().resolvedOptions().timeZone,
         decimalSeparator: decimalSeparator,
         thousandsSeparator: thousandsSeparator,
-        userSettings: userSettings,
-        prefersLightTheme: !window.matchMedia('(prefers-color-scheme: dark)')
-            .matches,
         windowWidth: window.innerWidth / pixelsPerRem,
         windowHeight: window.innerHeight / pixelsPerRem,
     });
 }
 
 function onOpen(): void {
     console.log('Websocket connection opened');
@@ -171,15 +203,15 @@
 
 function onMessage(event: MessageEvent<string>) {
     // Parse the message JSON
     let message = JSON.parse(event.data);
 
     // Print a copy of the message because some messages are modified in-place
     // when they're processed
-    console.trace('Received message: ', JSON.parse(event.data));
+    console.debug('Received message: ', JSON.parse(event.data));
 
     // Push it into the queue, to be processed as soon as the previous message
     // has been processed
     incomingMessageQueue.push(message);
 }
 
 function onError(event: Event) {
@@ -231,15 +263,15 @@
     if (!websocket) {
         console.error(
             `Attempted to send message, but the websocket is not connected: ${message}`
         );
         return;
     }
 
-    console.trace('Sending message: ', message);
+    console.debug('Sending message: ', message);
 
     websocket.send(JSON.stringify(message));
 }
 
 export function callRemoteMethodDiscardResponse(
     method: string,
     params: object
@@ -267,25 +299,14 @@
         case 'updateComponentStates':
             // The component states have changed, and new components may have been
             // introduced.
             updateComponentStates(
                 message.params.deltaStates,
                 message.params.rootComponentId
             );
-
-            // Notify the dev tools, if any
-            if (globalThis.RIO_DEV_TOOLS !== null) {
-                let devToolsComponent =
-                    globalThis.RIO_DEV_TOOLS as DevToolsConnectorComponent;
-
-                devToolsComponent.afterComponentStateChange(
-                    message.params.deltaStates
-                );
-            }
-
             response = null;
             break;
 
         case 'evaluateJavaScript':
         case 'evaluateJavaScriptAndGetResult':
             // Allow the server to run JavaScript
             //
```

### Comparing `rio_ui-0.8.6/frontend/code/rpcFunctions.ts` & `rio_ui-0.8.7/frontend/code/rpcFunctions.ts`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         }
 
         numSuccesses++;
         document.fonts.add(fontFace);
     }
 
     if (numFailures === 0) {
-        console.trace(
+        console.debug(
             `Successfully registered all ${numSuccesses} variations of font ${name}`
         );
     } else if (numSuccesses === 0) {
         console.warn(
             `Failed to register all ${numFailures} variations of font ${name}`
         );
     } else {
```

### Comparing `rio_ui-0.8.6/frontend/code/utils.ts` & `rio_ui-0.8.7/frontend/code/utils.ts`

 * *Files 17% similar despite different names*

```diff
@@ -279,7 +279,30 @@
             event.preventDefault();
 
             navigateToUrl(linkElement.href, openInNewTab);
         },
         true
     );
 }
+
+/// Determines the preferred format string for dates in the given locale. The
+/// string is suitable for use with Python's `strftime` function.
+export function getPreferredPythonDateFormatString(locale: string): string {
+    /// Format an already known date
+    let formattedDate = new Date(3333, 2, 1).toLocaleDateString(locale, {
+        year: 'numeric',
+        month: 'numeric',
+        day: 'numeric',
+    });
+
+    /// Parse the format string
+    formattedDate = formattedDate.replace('3333', '%Y');
+    formattedDate = formattedDate.replace('33', '%y');
+
+    formattedDate = formattedDate.replace('03', '%m');
+    formattedDate = formattedDate.replace('3', '%-m');
+
+    formattedDate = formattedDate.replace('01', '%d');
+    formattedDate = formattedDate.replace('1', '%-d');
+
+    return formattedDate;
+}
```

### Comparing `rio_ui-0.8.6/frontend/code/components/align.ts` & `rio_ui-0.8.7/frontend/code/components/align.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/buildFailed.ts` & `rio_ui-0.8.7/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/button.ts` & `rio_ui-0.8.7/frontend/code/components/button.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/card.ts` & `rio_ui-0.8.7/frontend/code/components/card.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/classContainer.ts` & `rio_ui-0.8.7/frontend/code/components/classContainer.ts`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         deltaState: ClassContainerState,
         latentComponents: Set<ComponentBase>
     ): void {
         this.replaceOnlyChild(latentComponents, deltaState.content);
 
         if (deltaState.classes !== undefined) {
             // Remove all old values
-            this.element.className = '';
+            this.element.className = 'rio-component';
 
             // Add all new values
             this.element.classList.add(...deltaState.classes);
         }
     }
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/codeBlock.ts` & `rio_ui-0.8.7/frontend/code/components/codeBlock.ts`

 * *Files 6% similar despite different names*

```diff
@@ -178,25 +178,19 @@
         this.naturalWidth = getElementWidth(this.element);
 
         // Any previously calculated height request is no longer valid
         this.heightRequestAssumesWidth = -1;
         this.makeLayoutDirty();
     }
 
-    updateNaturalWidth(ctx: LayoutContext): void {}
-
-    updateAllocatedWidth(ctx: LayoutContext): void {}
-
     updateNaturalHeight(ctx: LayoutContext): void {
         // Is the previous height request still value?
         if (this.heightRequestAssumesWidth === this.allocatedWidth) {
             return;
         }
 
         // No, re-layout
         this.element.style.height = 'min-content';
         this.naturalHeight = getElementHeight(this.element);
         this.heightRequestAssumesWidth = this.allocatedWidth;
     }
-
-    updateAllocatedHeight(ctx: LayoutContext): void {}
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/codeExplorer.ts` & `rio_ui-0.8.7/frontend/code/components/codeExplorer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/colorPicker.ts` & `rio_ui-0.8.7/frontend/code/components/colorPicker.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/componentBase.ts` & `rio_ui-0.8.7/frontend/code/components/componentBase.ts`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     // still references the *last* parent component. `null` is only for newly
     // created components and the root component.
     parent: ComponentBase | null = null;
     children = new Set<ComponentBase>();
 
     isLayoutDirty: boolean;
 
-    naturalWidth: number;
-    naturalHeight: number;
+    naturalWidth: number = 0;
+    naturalHeight: number = 0;
 
     requestedWidth: number;
     requestedHeight: number;
 
     allocatedWidth: number;
     allocatedHeight: number;
 
@@ -353,52 +353,47 @@
         this.updateElement(deltaState, null as any as Set<ComponentBase>);
 
         // Set the state
         this.state = {
             ...this.state,
             ...deltaState,
         };
+
+        // Notify the dev tools, if any
+        if (globalThis.RIO_DEV_TOOLS !== null) {
+            let devToolsComponent =
+                globalThis.RIO_DEV_TOOLS as DevToolsConnectorComponent;
+
+            devToolsComponent.afterComponentStateChange({
+                [this.id]: deltaState,
+            });
+        }
     }
 
     setStateAndNotifyBackend(deltaState: object): void {
         // Set the state. This also updates the component
         this._setStateDontNotifyBackend(deltaState);
 
         // Notify the backend
         callRemoteMethodDiscardResponse('componentStateUpdate', {
             componentId: this.id,
             deltaState: deltaState,
         });
-
-        // Notify the dev tools, if any
-        if (globalThis.RIO_DEV_TOOLS !== null) {
-            let devToolsComponent =
-                globalThis.RIO_DEV_TOOLS as DevToolsConnectorComponent;
-
-            devToolsComponent.afterComponentStateChange({
-                componentIdString: deltaState,
-            });
-        }
     }
 
     addClickHandler(args: ClickHandlerArguments): ClickHandler {
         return new ClickHandler(this, args);
     }
 
     addDragHandler(args: DragHandlerArguments): DragHandler {
         return new DragHandler(this, args);
     }
 
-    updateNaturalWidth(ctx: LayoutContext): void {
-        this.naturalWidth = 0;
-    }
-
-    updateNaturalHeight(ctx: LayoutContext): void {
-        this.naturalHeight = 0;
-    }
+    updateNaturalWidth(ctx: LayoutContext): void {}
+    updateNaturalHeight(ctx: LayoutContext): void {}
 
     updateAllocatedWidth(ctx: LayoutContext): void {}
     updateAllocatedHeight(ctx: LayoutContext): void {}
 
     toString(): string {
         let class_name = this.constructor.name;
         return `<${class_name} id:${this.id}>`;
```

### Comparing `rio_ui-0.8.6/frontend/code/components/componentTree.ts` & `rio_ui-0.8.7/frontend/code/components/componentTree.ts`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     state: Required<ComponentTreeState>;
 
     /// When a component should be highlighted to the user, this HTML element
     /// does the highlighting.
     private highlighterElement: HTMLElement;
 
     private selectedComponentId: ComponentId | null = null;
+    private nodesByComponent: WeakMap<ComponentBase, HTMLElement> =
+        new WeakMap();
+
+    // FIXME: Dead entries are never removed from `nodesByComponentId`
 
     createElement(): HTMLElement {
         // Register this component with the global dev tools component, so it
         // receives updates when a component's state changes.
         let dbg: DevToolsConnectorComponent = globalThis.RIO_DEV_TOOLS;
         console.assert(dbg !== null);
         dbg.componentTree = this;
@@ -134,20 +138,16 @@
         return userRoot;
     }
 
     buildTree(): void {
         // Get the rootmost displayed component
         let rootComponent = this.getDisplayedRootComponent();
 
-        // Clear the tree
-        let element = this.element;
-        element.innerHTML = '';
-
-        // Build a fresh one
-        this.buildNode(element, rootComponent, 0);
+        // Build a node for it
+        this.element.appendChild(this.getNodeFor(rootComponent));
 
         // Attempting to immediately access the just spawned items fails,
         // apparently because the browser needs to get control first. Any
         // further actions will happen with a delay.
         setTimeout(() => {
             // Don't start off with a fully collapsed tree
             if (!this.getNodeExpanded(rootComponent)) {
@@ -155,59 +155,67 @@
             }
 
             // Highlight the selected component
             this.highlightSelectedComponent();
         }, 0);
     }
 
-    buildNode(
-        parentElement: HTMLElement,
-        component: ComponentBase,
-        level: number
-    ) {
+    getNodeFor(component: ComponentBase): HTMLElement {
+        let node = this.nodesByComponent.get(component);
+        if (node !== undefined) {
+            return node;
+        }
+
+        node = this.buildNode(component);
+        this.nodesByComponent.set(component, node);
+        return node;
+    }
+
+    buildNode(component: ComponentBase): HTMLElement {
         // Create the element for this item
-        let element = document.createElement('div');
-        element.id = `rio-dev-tools-component-tree-item-${component.id}`;
-        element.classList.add('rio-dev-tools-component-tree-item');
-        parentElement.appendChild(element);
+        let node = document.createElement('div');
+        node.id = `rio-dev-tools-component-tree-item-${component.id}`;
+        node.classList.add('rio-dev-tools-component-tree-item');
 
         // Create the header
         let children = this.getDisplayableChildren(component);
         let header = document.createElement('div');
         header.classList.add('rio-dev-tools-component-tree-item-header');
         header.textContent = component.state._python_type_;
 
+        // Expander arrow, or at least a placeholder for it
         let iconElement = document.createElement('div');
+        iconElement.style.display = 'flex'; // Centers the SVG vertically
         header.insertBefore(iconElement, header.firstChild);
 
         if (children.length > 0) {
             applyIcon(
                 iconElement,
                 'material/keyboard-arrow-right',
                 'currentColor'
             );
         }
 
-        element.appendChild(header);
+        node.appendChild(header);
 
         // Add the children
-        let childElement = document.createElement('div');
-        childElement.classList.add(
+        let childrenContainer = document.createElement('div');
+        childrenContainer.classList.add(
             'rio-dev-tools-component-tree-item-children'
         );
-        element.appendChild(childElement);
+        node.appendChild(childrenContainer);
 
         for (let childInfo of children) {
-            this.buildNode(childElement, childInfo, level + 1);
+            childrenContainer.appendChild(this.getNodeFor(childInfo));
         }
 
         // Expand the node, or not
         let expanded = this.getNodeExpanded(component);
-        element.dataset.expanded = `${expanded}`;
-        element.dataset.hasChildren = `${children.length > 0}`;
+        node.dataset.expanded = `${expanded}`;
+        node.dataset.hasChildren = `${children.length > 0}`;
 
         // Add icons to give additional information
         let icons: string[] = [];
 
         // Icon: Container
         if (children.length <= 1) {
         } else if (children.length > 9) {
@@ -223,14 +231,15 @@
 
         let spacer = document.createElement('div');
         spacer.style.flexGrow = '1';
         header.appendChild(spacer);
 
         for (let icon of icons) {
             let iconElement = document.createElement('div');
+            iconElement.style.display = 'flex'; // Centers the SVG vertically
             header.appendChild(iconElement);
             applyIcon(iconElement, icon, 'currentColor');
         }
 
         // Click...
         header.addEventListener('click', (event) => {
             event.stopPropagation();
@@ -257,18 +266,20 @@
         // Highlight the actual component when the element is hovered
         header.addEventListener('mouseover', (event) => {
             this.moveHighlighterTo(component);
             event.stopPropagation();
         });
 
         // Remove any highlighters when the element is unhovered
-        element.addEventListener('mouseout', (event) => {
+        node.addEventListener('mouseout', (event) => {
             this.moveHighlighterTo(null);
             event.stopPropagation();
         });
+
+        return node;
     }
 
     /// Transition the highlighter to the given component. If the component is
     /// `null`, transition it out.
     moveHighlighterTo(component: ComponentBase | null) {
         // If no component is to be highlighted, make the highlighter the size
         // of the window, effectively hiding it. Overshoot by a bit to make sure
@@ -378,22 +389,62 @@
         for (let i = 1; i < treeItems.length; i++) {
             treeItems[i].classList.add(
                 'rio-dev-tools-component-tree-item-header-weakly-selected'
             );
         }
     }
 
+    nodeNeedsRebuild(
+        component: ComponentBase,
+        deltaState: ComponentState
+    ): boolean {
+        if ('key' in deltaState) {
+            return true;
+        }
+
+        let propertyNamesWithChildren: string[] =
+            globalThis.CHILD_ATTRIBUTE_NAMES[component.state['_type_']!] || [];
+
+        for (let propertyName of propertyNamesWithChildren) {
+            if (propertyName in deltaState) {
+                return true;
+            }
+        }
+
+        return false;
+    }
+
+    rebuildNode(node: HTMLElement, component: ComponentBase): void {
+        let newNode = this.buildNode(component);
+        this.nodesByComponent.set(component, newNode);
+
+        node.parentElement!.insertBefore(newNode, node);
+        node.remove();
+    }
+
     public afterComponentStateChange(deltaStates: {
-        [key: string]: { [key: string]: any };
+        [componentId: string]: { [key: string]: any };
     }) {
-        // Some components have had their state changed. This may affect the
-        // tree, as their children may have changed.
-        //
-        // Rebuild the tree
-        this.buildTree();
+        // Look for components whose children changed and rebuild their nodes
+        for (let [componentIdString, deltaState] of Object.entries(
+            deltaStates
+        )) {
+            let component = componentsById[componentIdString]!;
+
+            // If we haven't created a node for this component yet, there's no
+            // need to update it
+            let node = this.nodesByComponent.get(component);
+            if (node === undefined) {
+                continue;
+            }
+
+            if (this.nodeNeedsRebuild(component, deltaState)) {
+                this.rebuildNode(node, component);
+            }
+        }
 
         // The component tree has been modified. Browsers struggle to retrieve
         // the new elements immediately, so wait a bit.
         setTimeout(() => {
             // Flash all changed components
             for (let componentId in deltaStates) {
                 // Get the element. Not everything will show up, since some
```

### Comparing `rio_ui-0.8.6/frontend/code/components/customListItem.ts` & `rio_ui-0.8.7/frontend/code/components/customListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/devToolsConnector.ts` & `rio_ui-0.8.7/frontend/code/components/devToolsConnector.ts`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         // Create the element
         let element = document.createElement('a');
         element.href = 'https://rio.dev';
         element.target = '_blank';
         element.classList.add('rio-dev-tools-connector');
         element.innerHTML = `
-            <img src="/rio/asset/rio-logos/rio-logo-square.png">
+            <img src="/rio/asset/hosted/rio-logos/rio-logo-square.png">
             <div style="font-size: 1.2rem">Rio</div>
             <!-- <div style="font-size: 0.9rem">Dev Tools</div> -->
         `;
         return element;
     }
 
     updateElement(
```

### Comparing `rio_ui-0.8.6/frontend/code/components/drawer.ts` & `rio_ui-0.8.7/frontend/code/components/drawer.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import { pixelsPerRem } from '../app';
 import { commitCss } from '../utils';
 import { componentsById } from '../componentManagement';
 import { ComponentBase, ComponentState } from './componentBase';
 import { LayoutContext } from '../layouting';
-import { ComponentId } from '../dataModels';
+import { ColorSet, ComponentId } from '../dataModels';
+import { applySwitcheroo } from '../designApplication';
 
 export type DrawerState = ComponentState & {
     _type_: 'Drawer-builtin';
     anchor?: ComponentId;
     content?: ComponentId;
     side?: 'left' | 'right' | 'top' | 'bottom';
     is_modal?: boolean;
     is_open?: boolean;
     is_user_openable?: boolean;
+    color?: ColorSet;
 };
 
 export class DrawerComponent extends ComponentBase {
     state: Required<DrawerState>;
 
     private anchorContainer: HTMLElement;
     private contentOuterContainer: HTMLElement;
@@ -97,14 +99,19 @@
                 'rio-drawer-bottom'
             );
             this.element.classList.add(`rio-drawer-${deltaState.side}`);
 
             this.makeLayoutDirty();
         }
 
+        // Colorize
+        if (deltaState.color !== undefined) {
+            applySwitcheroo(this.contentOuterContainer, deltaState.color);
+        }
+
         // Open?
         //
         // Assign the changes directly to the state. This is necessary, because
         // the subsequent call to `_updateCss` uses the state to derive what the
         // CSS should be. Having values stored in the delta state rather than
         // actual state would ignore them.
         if (deltaState.is_open === true) {
```

### Comparing `rio_ui-0.8.6/frontend/code/components/dropdown.ts` & `rio_ui-0.8.7/frontend/code/components/dropdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/flowContainer.ts` & `rio_ui-0.8.7/frontend/code/components/flowContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.8.7/frontend/code/components/fundamentalRootComponent.ts`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,16 @@
     }
 
     updateNaturalWidth(ctx: LayoutContext): void {
         // Don't use `window.innerWidth`. It appears to be rounded to the
         // nearest integer, so it's inaccurate.
         //
         // `getBoundingClientRect()` doesn't account for scroll bars, but our
-        // <html> element is set to `overflow: hidden` anyway, so that's not an issue.
+        // <html> element is set to `overflow: hidden` anyway, so that's not an
+        // issue.
         let rect = document.documentElement.getBoundingClientRect();
         this.naturalWidth = this.allocatedWidth = rect.width / pixelsPerRem;
         this.naturalHeight = this.allocatedHeight = rect.height / pixelsPerRem;
     }
 
     updateAllocatedWidth(ctx: LayoutContext): void {
         // Overlays take up the full window
```

### Comparing `rio_ui-0.8.6/frontend/code/components/grid.ts` & `rio_ui-0.8.7/frontend/code/components/grid.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/headingListItem.ts` & `rio_ui-0.8.7/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/html.ts` & `rio_ui-0.8.7/frontend/code/components/separatorListItem.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import { ComponentBase, ComponentState } from './componentBase';
+import { LayoutContext } from '../layouting';
 
-export type HtmlState = ComponentState & {
-    _type_: 'Html-builtin';
-    html?: string;
+export type SeparatorListItemState = ComponentState & {
+    _type_: 'SeparatorListItem-builtin';
 };
 
-export class HtmlComponent extends ComponentBase {
-    state: Required<HtmlState>;
+export class SeparatorListItemComponent extends ComponentBase {
+    state: Required<SeparatorListItemState>;
 
     createElement(): HTMLElement {
         return document.createElement('div');
     }
 
     updateElement(
-        deltaState: HtmlState,
+        deltaState: SeparatorListItemState,
         latentComponents: Set<ComponentBase>
-    ): void {
-        if (deltaState.html !== undefined) {
-            this.element.innerHTML = deltaState.html;
-        }
+    ): void {}
+
+    updateNaturalHeight(ctx: LayoutContext): void {
+        this.naturalHeight = 1;
     }
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/icon.ts` & `rio_ui-0.8.7/frontend/code/components/icon.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/image.ts` & `rio_ui-0.8.7/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/keyEventListener.ts` & `rio_ui-0.8.7/frontend/code/components/keyEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/linearContainers.ts` & `rio_ui-0.8.7/frontend/code/components/linearContainers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/link.ts` & `rio_ui-0.8.7/frontend/code/components/link.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/listView.ts` & `rio_ui-0.8.7/frontend/code/components/listView.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/margin.ts` & `rio_ui-0.8.7/frontend/code/components/margin.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/markdown.ts` & `rio_ui-0.8.7/frontend/code/components/markdown.ts`

 * *Files 2% similar despite different names*

```diff
@@ -149,18 +149,14 @@
 
             // Any previously calculated height request is no longer valid
             this.heightRequestAssumesWidth = -1;
             this.makeLayoutDirty();
         }
     }
 
-    updateNaturalWidth(ctx: LayoutContext): void {}
-
-    updateAllocatedWidth(ctx: LayoutContext): void {}
-
     updateNaturalHeight(ctx: LayoutContext): void {
         // Is the previous height request still value?
         if (this.heightRequestAssumesWidth === this.allocatedWidth) {
             return;
         }
 
         // No, re-layout
```

### Comparing `rio_ui-0.8.6/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.8.7/frontend/code/components/mediaPlayer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.8.7/frontend/code/components/mouseEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.8.7/frontend/code/components/multiLineTextInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/nodeInput.ts` & `rio_ui-0.8.7/frontend/code/components/nodeInput.ts`

 * *Files 4% similar despite different names*

```diff
@@ -55,12 +55,8 @@
         if (deltaState.color !== undefined) {
             this.element.style.setProperty(
                 '--port-color',
                 colorToCssString(deltaState.color)
             );
         }
     }
-
-    updateNaturalWidth(ctx: LayoutContext): void {}
-
-    updateNaturalHeight(ctx: LayoutContext): void {}
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/nodeOutput.ts` & `rio_ui-0.8.7/frontend/code/components/nodeOutput.ts`

 * *Files 5% similar despite different names*

```diff
@@ -55,12 +55,8 @@
         if (deltaState.color !== undefined) {
             this.element.style.setProperty(
                 '--port-color',
                 colorToCssString(deltaState.color)
             );
         }
     }
-
-    updateNaturalWidth(ctx: LayoutContext): void {}
-
-    updateNaturalHeight(ctx: LayoutContext): void {}
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/overlay.ts` & `rio_ui-0.8.7/frontend/code/components/overlay.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/placeholder.ts` & `rio_ui-0.8.7/frontend/code/components/placeholder.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/plot.ts` & `rio_ui-0.8.7/frontend/code/components/plot.ts`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     // If plotly is currently being fetched, wait for it to finish
     if (fetchPlotlyPromise !== null) {
         fetchPlotlyPromise.then(callback);
         return;
     }
 
     // Otherwise fetch plotly and call the callback when it's done
-    console.trace('Fetching plotly.js');
+    console.debug('Fetching plotly.js');
     let script = document.createElement('script');
-    script.src = '/rio/asset/plotly.min.js';
+    script.src = '/rio/asset/special/plotly.min.js';
 
     fetchPlotlyPromise = new Promise((resolve) => {
         script.onload = () => {
             resolve(null);
         };
         document.head.appendChild(script);
     }).then(callback);
```

### Comparing `rio_ui-0.8.6/frontend/code/components/popup.ts` & `rio_ui-0.8.7/frontend/code/popupManager.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,201 +1,169 @@
-import { pixelsPerRem } from '../app';
-import { componentsById } from '../componentManagement';
-import { applySwitcheroo } from '../designApplication';
-import { LayoutContext } from '../layouting';
-import { ColorSet, ComponentId } from '../dataModels';
-import { ComponentBase, ComponentState } from './componentBase';
-
-export type PopupState = ComponentState & {
-    _type_: 'Popup-builtin';
-    anchor?: ComponentId;
-    content?: ComponentId;
-    color?: ColorSet;
-    position?: 'left' | 'top' | 'right' | 'bottom' | 'center';
-    alignment?: number;
-    gap?: number;
-    is_open?: boolean;
-};
-
-export class PopupComponent extends ComponentBase {
-    state: Required<PopupState>;
-
-    private anchorContainer: HTMLElement;
-    private contentContainer: HTMLElement;
-
-    createElement(): HTMLElement {
-        let element = document.createElement('div');
-        element.classList.add('rio-popup');
-
-        this.anchorContainer = document.createElement('div');
-        this.anchorContainer.classList.add('rio-popup-anchor');
-        element.appendChild(this.anchorContainer);
-
-        this.contentContainer = document.createElement('div');
-        this.contentContainer.classList.add('rio-popup-content');
-        element.appendChild(this.contentContainer);
+/// Helper class for creating pop-up elements.
+///
+/// Many components need to only display an element on occasion, and have it
+/// hover over the rest of the page. This is surprisingly difficult to do,
+/// because adding elements right in the HTML tree can cause them to be cut off
+/// by `overflow: hidden`, or other elements with a higher index. A simple
+/// `z-index` doesn't fix this either.
+///
+/// This class instead functions by adding the content close to the HTML root,
+/// and programmatically moves them to the right place. This way, the pop-up
+///
+/// While open, the content is assigned the CSS class `rio-popup-manager-open`.
+
+import { pixelsPerRem } from './app';
+
+/// will always be on top of everything else.
+export class PopupManager {
+    private anchor: HTMLElement;
+    private content: HTMLElement;
+
+    /// Where the pop-up should be positioned relative to the anchor.
+    ///
+    /// This is taken as a hint, but can be ignored if there isn't enough space
+    /// to fit the pop-up at that location.
+    public position: 'left' | 'top' | 'right' | 'bottom' | 'center';
+
+    /// The alignment of the popup within the anchor. If the popup opens to the
+    /// left or right, this is the vertical alignment, with `0` being the top
+    /// and `1` being the bottom. If the popup opens to the top or bottom, this
+    /// is the horizontal alignment, with `0` being the left and `1` being the
+    /// right. Has no effect if the popup opens centered.
+    public alignment: number;
+
+    /// The gap between the anchor and the popup, in `rem`.
+    public gap: number;
+
+    constructor(
+        anchor: HTMLElement,
+        content: HTMLElement,
+        position: 'left' | 'top' | 'right' | 'bottom' | 'center',
+        alignment: number,
+        gap: number
+    ) {
+        this.anchor = anchor;
+        this.content = content;
+        this.position = position;
+        this.alignment = alignment;
+        this.gap = gap;
 
-        return element;
+        // Prepare the content
+        //
+        // Note that the content is always present, even if not visible. This is
+        // so it can play CSS animations when it appears/disappears.
+        this.content.classList.add('rio-popup-manager-content'); // `rio-popup` is taken by the `Popup` component
+        document.body.appendChild(this.content);
     }
 
-    updateElement(
-        deltaState: PopupState,
-        latentComponents: Set<ComponentBase>
-    ): void {
-        // Update the children
-        this.replaceOnlyChild(
-            latentComponents,
-            deltaState.anchor,
-            this.anchorContainer
-        );
-        this.replaceOnlyChild(
-            latentComponents,
-            deltaState.content,
-            this.contentContainer
-        );
-
-        // Open / Close
-        if (deltaState.is_open === true) {
-            this.open();
-        } else {
-            this.element.classList.remove('rio-popup-open');
+    setOpen(open: boolean) {
+        // Easy case: Hide the content
+        if (!open) {
+            this.content.classList.remove('rio-popup-manager-open');
+            return;
         }
 
-        // Colorize
-        if (deltaState.color !== undefined) {
-            applySwitcheroo(this.element, deltaState.color);
-        }
-    }
-
-    open() {
-        // Add the open class. This will trigger the CSS animation
-        let element = this.element;
-        element.classList.add('rio-popup-open');
+        // Show the content
+        this.content.classList.add('rio-popup-manager-open');
 
         // The popup location is defined in developer-friendly terms. Convert
         // this to floats instead:
         //
         // - Anchor point X & Y (relative)
         // - Popup point X & Y (relative)
         // - Offset X & Y (absolute)
         //
         // The popup will appear, uch that the popup point is at the anchor
         // point. (But never off the screen.)
         let anchorRelativeX: number, anchorRelativeY: number;
         let contentRelativeX: number, contentRelativeY: number;
         let fixedOffsetXRem: number, fixedOffsetYRem: number;
 
-        if (this.state.position === 'left') {
+        if (this.position === 'left') {
             anchorRelativeX = 0;
-            anchorRelativeY = this.state.alignment;
+            anchorRelativeY = this.alignment;
             contentRelativeX = 1;
-            contentRelativeY = this.state.alignment;
-            fixedOffsetXRem = -this.state.gap;
+            contentRelativeY = this.alignment;
+            fixedOffsetXRem = -this.gap;
             fixedOffsetYRem = 0;
-        } else if (this.state.position === 'top') {
-            anchorRelativeX = this.state.alignment;
+        } else if (this.position === 'top') {
+            anchorRelativeX = this.alignment;
             anchorRelativeY = 0;
-            contentRelativeX = this.state.alignment;
+            contentRelativeX = this.alignment;
             contentRelativeY = 1;
             fixedOffsetXRem = 0;
-            fixedOffsetYRem = -this.state.gap;
-        } else if (this.state.position === 'right') {
+            fixedOffsetYRem = -this.gap;
+        } else if (this.position === 'right') {
             anchorRelativeX = 1;
-            anchorRelativeY = this.state.alignment;
+            anchorRelativeY = this.alignment;
             contentRelativeX = 0;
-            contentRelativeY = this.state.alignment;
-            fixedOffsetXRem = this.state.gap;
+            contentRelativeY = this.alignment;
+            fixedOffsetXRem = this.gap;
             fixedOffsetYRem = 0;
-        } else if (this.state.position === 'bottom') {
-            anchorRelativeX = this.state.alignment;
+        } else if (this.position === 'bottom') {
+            anchorRelativeX = this.alignment;
             anchorRelativeY = 1;
-            contentRelativeX = this.state.alignment;
+            contentRelativeX = this.alignment;
             contentRelativeY = 0;
             fixedOffsetXRem = 0;
-            fixedOffsetYRem = this.state.gap;
-        } else if (this.state.position === 'center') {
+            fixedOffsetYRem = this.gap;
+        } else if (this.position === 'center') {
             anchorRelativeX = 0.5;
             anchorRelativeY = 0.5;
             contentRelativeX = 0.5;
             contentRelativeY = 0.5;
             fixedOffsetXRem = 0;
             fixedOffsetYRem = 0;
         } else {
-            throw new Error(`Invalid Popup direction: ${this.state.position}`);
+            throw new Error(`Invalid Popup direction: ${this.position}`);
         }
 
         // Determine the size of the screen
         let screenWidth = window.innerWidth;
         let screenHeight = window.innerHeight;
 
         // Determine the size of the Popup
-        let anchorRect = this.anchorContainer.getBoundingClientRect();
+        let anchorRect = this.anchor.getBoundingClientRect();
 
         // Location of anchor
-        let popupWidth = this.contentContainer.scrollWidth;
-        let popupHeight = this.contentContainer.scrollHeight;
+        let contentWidth = this.content.scrollWidth;
+        let contentHeight = this.content.scrollHeight;
 
         // Where would the popup be positioned as requested by the user?
         let anchorPointX = anchorRect.left + anchorRect.width * anchorRelativeX;
         let anchorPointY = anchorRect.top + anchorRect.height * anchorRelativeY;
 
-        let popupPointX = popupWidth * contentRelativeX;
-        let popupPointY = popupHeight * contentRelativeY;
+        let contentPointX = contentWidth * contentRelativeX;
+        let contentPointY = contentHeight * contentRelativeY;
 
         let spawnPointX =
-            anchorPointX - popupPointX + fixedOffsetXRem * pixelsPerRem;
+            anchorPointX - contentPointX + fixedOffsetXRem * pixelsPerRem;
         let spawnPointY =
-            anchorPointY - popupPointY + fixedOffsetYRem * pixelsPerRem;
+            anchorPointY - contentPointY + fixedOffsetYRem * pixelsPerRem;
+
+        console.debug(
+            `AnchorX: ${anchorPointX}, AnchorY: ${anchorPointY}, ContentX: ${contentPointX}, ContentY: ${contentPointY}, SpawnX: ${spawnPointX}, SpawnY: ${spawnPointY}`
+        );
 
         // Establish limits, so the popup doesn't go off the screen. This is
         // relative to the popup's top left corner.
         let margin = 1 * pixelsPerRem;
 
         let minX = margin;
-        let maxX = screenWidth - popupWidth - margin;
+        let maxX = screenWidth - contentWidth - margin;
 
         let minY = margin;
-        let maxY = screenHeight - popupHeight - margin;
+        let maxY = screenHeight - contentHeight - margin;
 
         // Enforce limits
         spawnPointX = Math.min(Math.max(spawnPointX, minX), maxX);
         spawnPointY = Math.min(Math.max(spawnPointY, minY), maxY);
 
         // Set the position of the popup
-        this.contentContainer.style.left = spawnPointX + 'px';
-        this.contentContainer.style.top = spawnPointY + 'px';
-    }
-
-    updateNaturalWidth(ctx: LayoutContext): void {
-        this.naturalWidth = componentsById[this.state.anchor]!.requestedWidth;
-    }
-
-    updateAllocatedWidth(ctx: LayoutContext): void {
-        let anchorInst = componentsById[this.state.anchor]!;
-        anchorInst.allocatedWidth = this.allocatedWidth;
-
-        let contentInst = componentsById[this.state.content]!;
-        contentInst.allocatedWidth = contentInst.requestedWidth;
-    }
-
-    updateNaturalHeight(ctx: LayoutContext): void {
-        this.naturalHeight = componentsById[this.state.anchor]!.requestedHeight;
+        this.content.style.left = `${spawnPointX}px`;
+        this.content.style.top = `${spawnPointY}px`;
     }
 
-    updateAllocatedHeight(ctx: LayoutContext): void {
-        // Pass on the allocated space
-        let anchorInst = componentsById[this.state.anchor]!;
-        anchorInst.allocatedHeight = this.allocatedHeight;
-
-        let contentInst = componentsById[this.state.content]!;
-        contentInst.allocatedHeight = contentInst.requestedHeight;
-
-        // And position the children
-        let anchorElem = anchorInst.element;
-        anchorElem.style.left = '0';
-        anchorElem.style.top = '0';
-
-        let contentElem = contentInst.element;
-        contentElem.style.left = '0';
-        contentElem.style.top = '0';
+    destroy() {
+        this.content.remove();
     }
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/progressBar.ts` & `rio_ui-0.8.7/frontend/code/components/progressBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/progressCircle.ts` & `rio_ui-0.8.7/frontend/code/components/progressCircle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/rectangle.ts` & `rio_ui-0.8.7/frontend/code/components/rectangle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/revealer.ts` & `rio_ui-0.8.7/frontend/code/components/revealer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/scrollContainer.ts` & `rio_ui-0.8.7/frontend/code/components/scrollContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/scrollTarget.ts` & `rio_ui-0.8.7/frontend/code/components/scrollTarget.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/separator.ts` & `rio_ui-0.8.7/frontend/code/components/separator.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/separatorListItem.ts` & `rio_ui-0.8.7/frontend/code/components/website.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import { ComponentBase, ComponentState } from './componentBase';
-import { LayoutContext } from '../layouting';
 
-export type SeparatorListItemState = ComponentState & {
-    _type_: 'SeparatorListItem-builtin';
+export type WebsiteState = ComponentState & {
+    _type_: 'Website-builtin';
+    url?: string;
 };
 
-export class SeparatorListItemComponent extends ComponentBase {
-    state: Required<SeparatorListItemState>;
+export class WebsiteComponent extends ComponentBase {
+    state: Required<WebsiteState>;
+    element: HTMLIFrameElement;
 
     createElement(): HTMLElement {
-        return document.createElement('div');
+        return document.createElement('iframe');
     }
 
     updateElement(
-        deltaState: SeparatorListItemState,
+        deltaState: WebsiteState,
         latentComponents: Set<ComponentBase>
-    ): void {}
-
-    updateNaturalWidth(ctx: LayoutContext): void {
-        this.naturalWidth = 0;
+    ): void {
+        if (
+            deltaState.url !== undefined &&
+            deltaState.url !== this.element.src
+        ) {
+            this.element.src = deltaState.url;
+        }
     }
-
-    updateAllocatedWidth(ctx: LayoutContext): void {}
-
-    updateNaturalHeight(ctx: LayoutContext): void {
-        this.naturalHeight = 1;
-    }
-
-    updateAllocatedHeight(ctx: LayoutContext): void {}
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/singleContainer.ts` & `rio_ui-0.8.7/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/slider.ts` & `rio_ui-0.8.7/frontend/code/components/slider.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/slideshow.ts` & `rio_ui-0.8.7/frontend/code/components/slideshow.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/stack.ts` & `rio_ui-0.8.7/frontend/code/components/stack.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/switch.ts` & `rio_ui-0.8.7/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/switcher.ts` & `rio_ui-0.8.7/frontend/code/components/switcher.ts`

 * *Files 7% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             this.makeLayoutDirty();
             updateLayout();
         });
     }
 
     updateNaturalWidth(ctx: LayoutContext): void {
         // If the child's requested size has changed, start the animation
-        let childRequestedWidth, childRequestedHeight;
+        let childRequestedWidth: number, childRequestedHeight: number;
 
         if (this.activeChildInstance === null) {
             childRequestedWidth = 0;
             childRequestedHeight = 0;
         } else {
             childRequestedWidth = this.activeChildInstance.requestedWidth;
             childRequestedHeight = this.activeChildInstance.requestedHeight;
@@ -172,15 +172,17 @@
             this.animationStartedAt = -1;
         }
     }
 
     updateAllocatedWidth(ctx: LayoutContext): void {
         // Case: Trying to determine the size the child will receive once the
         // animation finishes
-        if (this.isDeterminingLayout) {
+        // OR
+        // Case: The parent component resized us
+        if (this.isDeterminingLayout || this.animationStartedAt === -1) {
             if (this.activeChildInstance !== null) {
                 this.activeChildInstance.allocatedWidth = this.allocatedWidth;
             }
             return;
         }
 
         // Case: animated layouting
@@ -230,12 +232,20 @@
 
             ctx.requestImmediateReLayout(() => {
                 this.makeLayoutDirty();
             });
             return;
         }
 
+        // Case: The parent component resized us
+        if (this.animationStartedAt === -1) {
+            if (this.activeChildInstance !== null) {
+                this.activeChildInstance.allocatedHeight = this.allocatedHeight;
+            }
+            return;
+        }
+
         // Case: animated layouting
         //
         // Nothing to do here
     }
 }
```

### Comparing `rio_ui-0.8.6/frontend/code/components/switcherBar.ts` & `rio_ui-0.8.7/frontend/code/components/switcherBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/table.ts` & `rio_ui-0.8.7/frontend/code/components/table.ts`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,14 @@
 
         this.makeLayoutDirty();
         [this.naturalWidth, this.naturalHeight] = getElementDimensions(
             this.tableElement
         );
     }
 
-    // Natural size is set in updateElement
-    updateNaturalWidth(ctx: LayoutContext): void {}
-    updateNaturalHeight(ctx: LayoutContext): void {}
-
     private displayData(): void {
         for (let element of this.dataCells) {
             element.remove();
         }
 
         this.dataCells = [];
```

### Comparing `rio_ui-0.8.6/frontend/code/components/text.ts` & `rio_ui-0.8.7/frontend/code/components/text.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/textInput.ts` & `rio_ui-0.8.7/frontend/code/components/textInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.8.7/frontend/code/components/themeContextSwitcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/code/components/tooltip.ts` & `rio_ui-0.8.7/frontend/code/components/tooltip.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import { componentsById } from '../componentManagement';
 import { LayoutContext } from '../layouting';
 import { ComponentId } from '../dataModels';
 import { ComponentBase, ComponentState } from './componentBase';
+import { PopupManager } from '../popupManager';
 
 export type TooltipState = ComponentState & {
     _type_: 'Tooltip-builtin';
     anchor?: ComponentId;
     _tip_component?: ComponentId | null;
     position?: 'left' | 'top' | 'right' | 'bottom';
+    gap?: number;
 };
 
 export class TooltipComponent extends ComponentBase {
     state: Required<TooltipState>;
 
     private anchorContainer: HTMLElement;
     private labelElement: HTMLElement;
 
+    private popupManager: PopupManager;
+
     createElement(): HTMLElement {
         // Set up the HTML
         let element = document.createElement('div');
         element.classList.add('rio-tooltip');
 
         element.innerHTML = `
             <div class="rio-tooltip-anchor"></div>
@@ -32,21 +36,31 @@
 
         this.labelElement = element.querySelector(
             '.rio-tooltip-label'
         ) as HTMLElement;
 
         // Listen for events
         this.anchorContainer.addEventListener('mouseover', () => {
-            this.labelElement.style.opacity = '1';
+            this.popupManager.setOpen(true);
         });
 
         this.anchorContainer.addEventListener('mouseout', () => {
-            this.labelElement.style.opacity = '0';
+            this.popupManager.setOpen(false);
         });
 
+        // Initialize the popup manager. Many of these values will be
+        // overwritten by the updateElement method.
+        this.popupManager = new PopupManager(
+            this.anchorContainer,
+            this.labelElement,
+            'center',
+            0.5,
+            0.0
+        );
+
         return element;
     }
 
     updateElement(
         deltaState: TooltipState,
         latentComponents: Set<ComponentBase>
     ): void {
@@ -66,52 +80,29 @@
                 deltaState._tip_component,
                 this.labelElement
             );
         }
 
         // Position
         if (deltaState.position !== undefined) {
-            let left, top, right, bottom, transform;
-
-            const theOne = 'calc(100% + 0.5rem)';
+            this.popupManager.position = deltaState.position;
+        }
 
-            if (deltaState.position === 'left') {
-                left = 'unset';
-                top = '50%';
-                right = theOne;
-                bottom = 'unset';
-                transform = 'translateY(-50%)';
-            } else if (deltaState.position === 'top') {
-                left = '50%';
-                top = 'unset';
-                right = 'unset';
-                bottom = theOne;
-                transform = 'translateX(-50%)';
-            } else if (deltaState.position === 'right') {
-                left = theOne;
-                top = '50%';
-                right = 'unset';
-                bottom = 'unset';
-                transform = 'translateY(-50%)';
-            } else {
-                left = '50%';
-                top = theOne;
-                right = 'unset';
-                bottom = 'unset';
-                transform = 'translateX(-50%)';
-            }
-
-            this.labelElement.style.left = left;
-            this.labelElement.style.top = top;
-            this.labelElement.style.right = right;
-            this.labelElement.style.bottom = bottom;
-            this.labelElement.style.transform = transform;
+        // Gap
+        if (deltaState.gap !== undefined) {
+            this.popupManager.gap = deltaState.gap;
         }
     }
 
+    onDestruction(): void {
+        super.onDestruction();
+
+        this.popupManager.destroy();
+    }
+
     updateNaturalWidth(ctx: LayoutContext): void {
         this.naturalWidth = componentsById[this.state.anchor!]!.requestedWidth;
     }
 
     updateAllocatedWidth(ctx: LayoutContext): void {
         let anchor = componentsById[this.state.anchor!]!;
         let tip = componentsById[this.state._tip_component!]!;
```

### Comparing `rio_ui-0.8.6/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.8.7/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/css/highlightjs-default-light.css` & `rio_ui-0.8.7/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/frontend/css/style.scss` & `rio_ui-0.8.7/frontend/css/style.scss`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,26 @@
     @include meta.load-css('highlightjs-default-dark.css');
 }
 
 // Not visible here:
 //
 // JavaScript sets global theming variables, of the form `--rio-global-...`.
 
-// Z-indices for components which are expected to show up on top
-$z-index-overlay: 10000;
-$z-index-dev-tools-highlighter: 10001;
-$z-index-dev-tools: 10002;
-$z-index-popup: 10003;
-$z-index-error-popup: 10004;
+// Z-indices for components which are expected to show up on top.
+//
+// - `popup` MUST be above `dev-tools` in order for dropdowns in the dev tools
+//   to work correctly.
+// - `dev-tools` must be above `dev-tools-highlighter` so they don't get greyed
+//   out by it
+$z-index-user-root: 1;
+$z-index-overlay: 2;
+$z-index-dev-tools-highlighter: 3;
+$z-index-dev-tools: 4;
+$z-index-popup: 5;
+$z-index-error-popup: 6;
 
 // "Infinite" corner radius, for creating pill shapes
 $infinite-corner-radius: 99999px;
 
 // Nonstandard transition timing function
 $transition-timing-overshoot: cubic-bezier(0.5, 0.5, 0.2, 1.14);
 
@@ -131,19 +137,24 @@
 
 // Fundamental Root Component
 .rio-fundamental-root-component {
     position: relative !important;
 
     width: 100vw;
     height: 100vh;
+
+    & > .rio-scroll-container {
+        z-index: $z-index-user-root;
+    }
 }
 
 // Dev Tools
 .rio-dev-tools {
     pointer-events: auto;
+    z-index: $z-index-dev-tools;
 }
 
 .rio-dev-tools-hidden::after {
     pointer-events: none;
 
     position: fixed;
     top: 0;
@@ -1617,15 +1628,15 @@
 
 .rio-drawer-content-outer {
     pointer-events: auto;
 
     display: flex;
 
     position: absolute;
-    background-color: var(--rio-global-neutral-bg);
+    background-color: var(--rio-local-bg);
 
     box-shadow: 0 0 1rem var(--rio-global-shadow-color);
 
     transition: transform 0.3s ease-out;
 }
 
 .rio-drawer-content-inner {
@@ -1738,26 +1749,25 @@
 .rio-popup-content {
     position: fixed;
 
     width: min-content;
     height: min-content;
 
     background-color: var(--rio-local-bg);
-    border-radius: var(--rio-global-corner-radius-medium);
     box-shadow: 0 0 1rem var(--rio-global-shadow-color);
 
     transform: scale(0);
     opacity: 0;
 
     transition:
         transform 0.2s linear,
         opacity 0.1s ease-in-out;
 }
 
-.rio-popup-open > .rio-popup-content {
+.rio-popup-content.rio-popup-manager-open {
     transform: scale(1);
     opacity: 1;
 
     transition:
         transform 0.2s $transition-timing-overshoot,
         opacity 0.1s ease-in-out;
 }
@@ -1999,15 +2009,16 @@
 
 // Traceback Popup
 .rio-traceback {
     pointer-events: auto;
 
     position: relative;
     left: 50%;
-    top: 5rem;
+    margin-top: 5rem;
+    margin-bottom: 5rem;
     width: fit-content;
     max-width: 50rem;
     padding: 2.2rem;
 
     overflow: hidden;
 
     display: flex;
@@ -2382,17 +2393,35 @@
 
     width: max-content;
     padding: 0.5rem;
     border-radius: var(--rio-global-corner-radius-small);
 
     background: var(--rio-global-hud-bg);
     box-shadow: 0 0.1rem 0.2rem var(--rio-global-shadow-color);
+
+    transform: scale(0);
     opacity: 0;
 
-    transition: opacity 0.15s ease-in-out;
+    transition:
+        transform 0.2s linear,
+        opacity 0.1s ease-in-out;
+}
+
+.rio-popup-content.rio-popup-manager-open {
+    transform: scale(1);
+    opacity: 1;
+}
+
+.rio-tooltip-label.rio-popup-manager-open {
+    transform: scale(1);
+    opacity: 1;
+
+    transition:
+        transform 0.2s $transition-timing-overshoot,
+        opacity 0.1s ease-in-out;
 }
 
 // Build failed component
 .rio-build-failed {
     pointer-events: auto;
     color: var(--rio-global-danger-fg);
 
@@ -2568,7 +2597,118 @@
     transition:
         top var(--rio-ripple-duration),
         left var(--rio-ripple-duration),
         width var(--rio-ripple-duration),
         height var(--rio-ripple-duration),
         opacity var(--rio-ripple-duration);
 }
+
+// Popup Manger (NOT the `Popup` component!)
+.rio-popup-manager-content {
+    z-index: $z-index-popup;
+}
+
+// Calendar
+.rio-calendar {
+    pointer-events: auto;
+    @include center-content;
+}
+
+.rio-calendar-inner {
+    display: flex;
+    flex-direction: column;
+    gap: 0.5rem;
+}
+
+.rio-calendar-header {
+    display: flex;
+    flex-direction: row;
+    gap: 0.2rem;
+    flex: 0;
+
+    > :nth-child(3) {
+        pointer-events: none;
+
+        display: flex;
+        justify-content: center;
+        align-items: center;
+
+        flex-grow: 1;
+    }
+}
+
+.rio-calendar-button {
+    position: relative;
+    width: 1.6rem;
+    height: 1.6rem;
+
+    cursor: pointer;
+
+    color: var(--rio-local-text-color);
+}
+
+.rio-calendar-button:hover {
+    color: var(--rio-local-level-2-bg);
+}
+
+.rio-calendar-button:hover::after {
+    content: '';
+    position: absolute;
+
+    left: 0;
+    top: 0;
+    right: 0;
+    bottom: 0;
+
+    background: var(--rio-local-level-2-bg);
+    border-radius: $infinite-corner-radius;
+    opacity: 0.1;
+}
+
+.rio-calendar-grid {
+    display: grid;
+    grid-template-columns: repeat(7, 1.8rem);
+    grid-template-rows: repeat(7, 1.8rem);
+    gap: 0.5rem;
+}
+
+.rio-calendar-day-name {
+    font-weight: bold;
+    text-align: center;
+}
+
+.rio-calendar-day {
+    position: relative;
+
+    display: flex;
+    justify-content: center;
+    align-items: center;
+
+    cursor: pointer;
+}
+
+.rio-calendar-day-other-month {
+    opacity: 0.4;
+}
+
+.rio-calendar-day:hover::after {
+    content: '';
+    position: absolute;
+
+    left: 0;
+    top: 0;
+    right: 0;
+    bottom: 0;
+
+    background: var(--rio-local-text-color);
+    border-radius: $infinite-corner-radius;
+    opacity: 0.1;
+}
+
+.rio-calendar-selected-day {
+    font-weight: bold;
+
+    color: var(--rio-local-level-2-fg);
+
+    background: var(--rio-local-level-2-bg);
+    border-radius: $infinite-corner-radius;
+}
```

### Comparing `rio_ui-0.8.6/frontend/css/switcheroos.scss` & `rio_ui-0.8.7/frontend/css/switcheroos.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.8.7/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.8.7/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.8.7/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.8.7/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/logo.svg` & `rio_ui-0.8.7/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.8.7/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.8.7/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/color/logo.svg` & `rio_ui-0.8.7/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.8.7/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.8.7/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/rio/fill/logo.svg` & `rio_ui-0.8.7/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.8.7/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.8.7/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.8.7/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.8.7/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/__init__.py` & `rio_ui-0.8.7/rio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.6"
+__version__ = "0.8.7"
 
 import logging
 
 _logger = logging.getLogger(__name__)
 
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
```

### Comparing `rio_ui-0.8.6/rio/app.py` & `rio_ui-0.8.7/rio/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,19 @@
             each time a new user visits the site. In the context of a window
             there is only one session, so this will only be called once.
 
             This function does not block the creation of the session. This
             is to make sure initialization code doesn't accidentally make
             the user wait.
 
+            Please note that the session is not fully initialized yet when this
+            function is called. In particular, the session's `active_page_url`
+            is set to whichever URL the client has requested, but before the
+            guards have had a chance to redirect the user to another page.
+
         `on_session_close`: A function that will be called each time a session
             ends. In the context of a website that would be each time a user
             closes their browser tab. In the context of a window this will
             only be called once, when the window is closed.
 
         `default_attachments`: A list of attachments that will be attached to
             every new session.
@@ -496,15 +501,15 @@
         app.run_in_window()
         ```
 
         This method requires the `window` extra. If you don't have it installed,
         you can install it with:
 
         ```sh
-        pip install rio-ui[window]
+        pip install "rio-ui[window]"
         ```
 
         This method will synchronously block until the window is closed.
 
 
         ## Parameters
 
@@ -512,15 +517,15 @@
             Error messages will be printed regardless of this setting.
         """
         try:
             import webview  # type: ignore
         except ImportError:
             raise Exception(
                 "The `window` extra is required to use `App.run_in_window`."
-                " Run `pip install rio-ui[window]` to install it."
+                """ Run `pip install "rio-ui[window]"` to install it."""
             ) from None
 
         # Unfortunately, WebView must run in the main thread, which makes this
         # tricky. We'll have to banish uvicorn to a background thread, and shut
         # it down when the window is closed.
 
         host = "localhost"
```

### Comparing `rio_ui-0.8.6/rio/app_server.py` & `rio_ui-0.8.7/rio/app_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 import contextlib
 import functools
 import html
 import inspect
 import io
 import json
 import logging
+import mimetypes
 import secrets
 import time
 import traceback
 import weakref
-from datetime import timedelta
+from dataclasses import dataclass
+from datetime import date, timedelta
+from pathlib import Path
 from typing import *  # type: ignore
 from xml.etree import ElementTree as ET
 
 import fastapi.staticfiles
 import langcodes
 import pytz
 import timer_dict
@@ -28,14 +31,15 @@
 
 from . import (
     app,
     assets,
     byte_serving,
     components,
     inspection,
+    language_info,
     routing,
     session,
     user_settings_module,
     utils,
 )
 from .errors import AssetError
 from .serialization import serialize_json
@@ -102,36 +106,74 @@
     )
 
 
 def add_cache_headers(
     func: Callable[P, Awaitable[fastapi.Response]],
 ) -> Callable[P, Coroutine[None, None, fastapi.Response]]:
     """
-    Decorator for the `_serve_asset` method. Ensures that the response has the
-    `Cache-Control` header set appropriately.
+    Decorator for routes that serve static files. Ensures that the response has
+    the `Cache-Control` header set appropriately.
     """
 
     @functools.wraps(func)
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> fastapi.Response:
         response = await func(*args, **kwargs)
         response.headers["Cache-Control"] = "max-age=31536000, immutable"
         return response
 
     return wrapper
 
 
+@dataclass
 class InitialClientMessage(uniserde.Serde):
     website_url: str
+    user_settings: dict[str, Any]
+    prefers_light_theme: bool
+
+    # List of RFC 5646 language codes. Most preferred first. May be empty!
     preferred_languages: list[str]
+
+    # The names for all months, starting with January
+    month_names_long: tuple[
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+    ]
+
+    # The names of all weekdays, starting with monday
+    day_names_long: tuple[
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+        str,
+    ]
+
+    # The format string for dates, as used by Python's `strftime`
+    date_format_string: str
+
+    # IANA timezone
     timezone: str
+
+    # Separators for number rendering
     decimal_separator: str
     thousands_separator: str
-    user_settings: dict[str, Any]
-    prefers_light_theme: bool
 
+    # Window Information
     window_width: float
     window_height: float
 
 
 async def _periodically_clean_up_expired_sessions(
     app_server_ref: weakref.ReferenceType[AppServer],
 ):
@@ -217,21 +259,32 @@
 
         # FastAPI
         self.add_api_route("/robots.txt", self._serve_robots, methods=["GET"])
         self.add_api_route("/rio/sitemap", self._serve_sitemap, methods=["GET"])
         self.add_api_route(
             "/rio/favicon.png", self._serve_favicon, methods=["GET"]
         )
-        self.mount(
-            "/rio/frontend",
-            fastapi.staticfiles.StaticFiles(directory=utils.FRONTEND_FILES_DIR),
-            name="frontend",
+        self.add_api_route(
+            "/rio/frontend/assets/{asset_id:path}",
+            self._serve_frontend_asset,
+        )
+        self.add_api_route(
+            "/rio/asset/special/{asset_id:path}",
+            self._serve_special_asset,
+            methods=["GET"],
         )
         self.add_api_route(
-            "/rio/asset/{asset_id:path}", self._serve_asset, methods=["GET"]
+            "/rio/asset/hosted/{asset_id:path}",
+            self._serve_hosted_asset,
+            methods=["GET"],
+        )
+        self.add_api_route(
+            "/rio/asset/temp/{asset_id:path}",
+            self._serve_temp_asset,
+            methods=["GET"],
         )
         self.add_api_route(
             "/rio/icon/{icon_name:path}", self._serve_icon, methods=["GET"]
         )
         self.add_api_route(
             "/rio/upload/{upload_token}",
             self._serve_file_upload,
@@ -519,68 +572,73 @@
 
         # There is an icon, respond
         return fastapi.responses.Response(
             content=self._icon_as_png_blob,
             media_type="image/png",
         )
 
-    @add_cache_headers
-    async def _serve_asset(
+    async def _serve_frontend_asset(
         self,
         request: fastapi.Request,
         asset_id: str,
     ) -> fastapi.responses.Response:
-        """
-        Handler for serving assets via fastapi.
-
-        Some common assets are hosted under permanent, well known URLs under the
-        `/rio/asset/{some-name}` path.
+        response = await self._serve_file_from_directory(
+            request,
+            utils.FRONTEND_ASSETS_DIR,
+            asset_id + ".gz",
+        )
+        response.headers["content-encoding"] = "gzip"
+
+        media_type = mimetypes.guess_type(asset_id, strict=False)[0]
+        if media_type:
+            response.headers["content-type"] = media_type
 
-        In addition, `HostedAsset` instances are hosted under their secret id
-        under the `/rio/asset/temp-{asset_id}` path. These assets are held
-        weakly by the session, meaning they will be served for as long as the
-        corresponding Python object is alive.
-        """
+        return response
 
-        # Special case: plotly
-        #
+    @add_cache_headers
+    async def _serve_special_asset(
+        self,
+        request: fastapi.Request,
+        asset_id: str,
+    ) -> fastapi.responses.Response:
         # The python plotly library already includes a minified version of
         # plotly.js. Rather than shipping another one, just serve the one
         # included in the library.
-        if asset_id == "plotly.min.js" and plotly is not None:
+        if asset_id == "plotly.min.js":
+            if plotly is None:
+                return fastapi.responses.Response(status_code=404)
+
             return fastapi.responses.Response(
                 content=plotly.offline.get_plotlyjs(),
                 media_type="text/javascript",
             )
 
-        # Well known asset?
-        if not asset_id.startswith("temp-"):
-            # Construct the path to the target file
-            asset_file_path = utils.HOSTED_ASSETS_DIR / asset_id
-
-            # Make sure the path is inside the hosted assets directory
-            #
-            # TODO: Is this safe? Would this allow the client to break out from
-            # the directory using tricks such as "../", links, etc?
-            asset_file_path = asset_file_path.absolute()
-            if utils.HOSTED_ASSETS_DIR not in asset_file_path.parents:
-                logging.warning(
-                    f'Client requested asset "{asset_id}" which is not located inside the hosted assets directory. Somebody might be trying to break out of the assets directory!'
-                )
-                return fastapi.responses.Response(status_code=404)
+        return fastapi.responses.Response(status_code=404)
 
-            return byte_serving.range_requests_response(
-                request,
-                file_path=asset_file_path,
-            )
+    async def _serve_hosted_asset(
+        self,
+        request: fastapi.Request,
+        asset_id: str,
+    ) -> fastapi.responses.Response:
+        return await self._serve_file_from_directory(
+            request,
+            utils.HOSTED_ASSETS_DIR,
+            asset_id,
+        )
 
+    @add_cache_headers
+    async def _serve_temp_asset(
+        self,
+        request: fastapi.Request,
+        asset_id: str,
+    ) -> fastapi.responses.Response:
         # Get the asset's Python instance. The asset's id acts as a secret, so
         # no further authentication is required.
         try:
-            asset = self._assets[asset_id.removeprefix("temp-")]
+            asset = self._assets[asset_id]
         except KeyError:
             return fastapi.responses.Response(status_code=404)
 
         # Fetch the asset's content and respond
         if isinstance(asset, assets.BytesAsset):
             return fastapi.responses.Response(
                 content=asset.data,
@@ -591,14 +649,39 @@
                 request,
                 file_path=asset.path,
                 media_type=asset.media_type,
             )
         else:
             assert False, f"Unable to serve asset of unknown type: {asset}"
 
+    @add_cache_headers
+    async def _serve_file_from_directory(
+        self,
+        request: fastapi.Request,
+        directory: Path,
+        asset_id: str,
+    ) -> fastapi.responses.Response:
+        # Construct the path to the target file
+        asset_file_path = directory / asset_id
+
+        # Make sure the path is inside the hosted assets directory
+        asset_file_path = asset_file_path.absolute()
+        if not asset_file_path.is_relative_to(directory):
+            logging.warning(
+                f'Client requested asset "{asset_id}" which is not located'
+                f" inside the assets directory. Somebody might be trying to"
+                f" break out of the assets directory!"
+            )
+            return fastapi.responses.Response(status_code=404)
+
+        return byte_serving.range_requests_response(
+            request,
+            file_path=asset_file_path,
+        )
+
     async def _serve_icon(self, icon_name: str) -> fastapi.responses.Response:
         """
         Allows the client to request an icon by name. This is not actually the
         mechanism used by the `Icon` component, but allows JavaScript to request
         icons.
         """
         # Get the icon's SVG
@@ -816,27 +899,52 @@
                 language = langcodes.standardize_tag(language)
             except ValueError:
                 continue
 
             if language not in preferred_languages:
                 preferred_languages.append(language)
 
+        if len(preferred_languages) == 0:
+            preferred_languages.append("en-US")
+
         # Get locale information
         if len(initial_message.decimal_separator) != 1:
             logging.warning(
                 f'Client sent invalid decimal separator "{initial_message.decimal_separator}". Using "." instead.'
             )
             initial_message.decimal_separator = "."
 
         if len(initial_message.thousands_separator) > 1:
             logging.warning(
                 f'Client sent invalid thousands separator "{initial_message.thousands_separator}". Using "" instead.'
             )
             initial_message.thousands_separator = ""
 
+        # There does not seem to be any good way to determine the first day of
+        # the week in JavaScript. Look up the first day of the week based on
+        # the preferred language.
+        first_day_of_week = language_info.get_week_start_day(
+            preferred_languages[0]
+        )
+
+        # Make sure the date format string is valid
+        formatted_date = date(3333, 11, 22).strftime(
+            initial_message.date_format_string
+        )
+
+        if (
+            "33" not in formatted_date
+            or "11" not in formatted_date
+            or "22" not in formatted_date
+        ):
+            logging.warning(
+                f'Client sent invalid date format string "{initial_message.date_format_string}". Using "%Y-%m-%d" instead.'
+            )
+            initial_message.date_format_string = "%Y-%m-%d"
+
         # Parse the timezone
         try:
             timezone = pytz.timezone(initial_message.timezone)
         except pytz.UnknownTimeZoneError:
             logging.warning(
                 f'Client sent unknown timezone "{initial_message.timezone}". Using UTC instead.'
             )
@@ -853,26 +961,37 @@
         theme = self.app._theme
         if isinstance(theme, tuple):
             if initial_message.prefers_light_theme:
                 theme = theme[0]
             else:
                 theme = theme[1]
 
+        # Prepare the initial URL. This will be exposed to the session as the
+        # `active_page_url`, but overridden later once the page guards have been
+        # run.
+        initial_page_url = rio.URL(initial_message.website_url.lower())
+
+        # Create the session
         sess = session.Session(
             app_server_=self,
             session_token=session_token,
             send_message=send_message,
             receive_message=receive_message,
             websocket=websocket,
             client_ip=request.client.host,
             client_port=request.client.port,
             http_headers=request.headers,
             base_url=base_url,
+            active_page_url=initial_page_url,
             timezone=timezone,
             preferred_languages=preferred_languages,
+            month_names_long=initial_message.month_names_long,
+            day_names_long=initial_message.day_names_long,
+            date_format_string=initial_message.date_format_string,
+            first_day_of_week=first_day_of_week,
             decimal_separator=initial_message.decimal_separator,
             thousands_separator=initial_message.thousands_separator,
             window_width=initial_message.window_width,
             window_height=initial_message.window_height,
             theme_=theme,
         )
 
@@ -901,22 +1020,20 @@
         )
 
         # Run any page guards for the initial page
         try:
             (
                 active_page_instances,
                 active_page_url_absolute,
-            ) = routing.check_page_guards(
-                sess, rio.URL(initial_message.website_url.lower())
-            )
+            ) = routing.check_page_guards(sess, initial_page_url)
         except routing.NavigationFailed:
             # TODO: Notify the client? Show an error?
             raise fastapi.HTTPException(
                 status_code=fastapi.status.HTTP_500_INTERNAL_SERVER_ERROR,
-                detail=f"Navigation to initial page `{sess._active_page_url}` has failed.",
+                detail=f"Navigation to initial page `{initial_page_url}` has failed.",
             ) from None
 
         # Is this a page, or a full URL to another site?
         try:
             utils.make_url_relative(
                 sess._base_url,
                 active_page_url_absolute,
@@ -936,21 +1053,21 @@
 
             # TODO: End the session? Abort initialization?
 
         # Set the initial page URL. When connecting to the server, all relevant
         # page guards execute. These may change the URL of the page, so the
         # client needs to take care to update the browser's URL to match the
         # server's.
-        if str(active_page_url_absolute) != initial_message.website_url:
+        if str(active_page_url_absolute) != initial_page_url:
 
             async def update_url_worker():
                 js_page_url = json.dumps(str(active_page_url_absolute))
                 await sess._evaluate_javascript(
                     f"""
-                    console.trace("Updating browser URL to match the one modified by guards:", {js_page_url});
+                    console.debug("Updating browser URL to match the one modified by guards:", {js_page_url});
                     window.history.replaceState(null, "", {js_page_url});
                     """
                 )
 
             sess.create_task(
                 update_url_worker(),
                 name="Update browser URL to match the one modified by guards",
```

### Comparing `rio_ui-0.8.6/rio/assets.py` & `rio_ui-0.8.7/rio/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,19 +191,19 @@
 
     @abc.abstractmethod
     def _get_secret_id(self) -> str:
         raise NotImplementedError
 
     @property
     def url(self) -> URL:
-        return URL(f"/rio/asset/temp-{self.secret_id}")
+        return URL(f"/rio/asset/temp/{self.secret_id}")
 
     def _serialize(self, sess: rio.Session) -> str:
         sess._app_server.weakly_host_asset(self)
-        return f"/rio/asset/temp-{self.secret_id}"
+        return f"/rio/asset/temp/{self.secret_id}"
 
 
 class BytesAsset(HostedAsset):
     def __init__(
         self,
         data: bytes | bytearray,
         media_type: str | None = None,
```

### Comparing `rio_ui-0.8.6/rio/byte_serving.py` & `rio_ui-0.8.7/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/color.py` & `rio_ui-0.8.7/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/dataclass.py` & `rio_ui-0.8.7/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/deprecations.py` & `rio_ui-0.8.7/rio/deprecations.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/errors.py` & `rio_ui-0.8.7/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/fills.py` & `rio_ui-0.8.7/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/global_state.py` & `rio_ui-0.8.7/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/icon_registry.py` & `rio_ui-0.8.7/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/inspection.py` & `rio_ui-0.8.7/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/maybes.py` & `rio_ui-0.8.7/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/routing.py` & `rio_ui-0.8.7/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/serialization.py` & `rio_ui-0.8.7/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/session.py` & `rio_ui-0.8.7/rio/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,34 +140,47 @@
         receive_message: Callable[[], Awaitable[Jsonable]],
         websocket: fastapi.WebSocket,
         client_ip: str,
         client_port: int,
         http_headers: starlette.datastructures.Headers,
         timezone: tzinfo,
         preferred_languages: Iterable[str],
+        month_names_long: tuple[
+            str, str, str, str, str, str, str, str, str, str, str, str
+        ],
+        day_names_long: tuple[str, str, str, str, str, str, str],
+        date_format_string: str,
+        first_day_of_week: int,
         decimal_separator: str,  # == 1 character
         thousands_separator: str,  # <= 1 character
         window_width: float,
         window_height: float,
         base_url: rio.URL,
+        active_page_url: rio.URL,
         theme_: theme.Theme,
     ) -> None:
         super().__init__(
             send_message=send_message,
             receive_message=receive_message,
         )
 
         self._app_server = app_server_
         self._session_token = session_token
         self.timezone = timezone
 
-        # Make sure there is at least one preferred language
         self.preferred_languages = tuple(preferred_languages)
-        self.preferred_languages = self.preferred_languages or ("en-US",)
+        assert self.preferred_languages, "Preferred languages must not be empty"
 
+        # General local information
+        self._month_names_long = month_names_long
+        self._day_names_long = day_names_long
+        self._date_format_string = date_format_string
+        self._first_day_of_week = first_day_of_week
+
+        # Separators for number rendering
         self._decimal_separator = decimal_separator
         self._thousands_separator = thousands_separator
 
         self.window_width = window_width
         self.window_height = window_height
 
         self._base_url = base_url
@@ -176,15 +189,15 @@
         # This attribute is initialized after the Session has been instantiated,
         # because the Session must already exist when the Component is created
         self._root_component: root_components.HighLevelRootComponent
 
         # These are initialized with dummy values. Once the Session has been
         # instantiated, the page guards will run and then these will be set to
         # the correct values.
-        self._active_page_url = base_url
+        self._active_page_url = active_page_url
         self._active_page_instances: tuple[rio.Page, ...] = tuple()
 
         # Components need unique ids, but we don't want them to be globally unique
         # because then people could guesstimate the approximate number of
         # visitors on a server based on how quickly the component ids go up. So
         # each session will assign its components ids starting from 0.
         self._next_free_component_id: int = 0
@@ -555,14 +568,34 @@
         for task in self._running_tasks:
             task.cancel()
 
         # Close the websocket connection
         if self._websocket is not None:
             await self._websocket.close()
 
+    def _get_user_root_component(self) -> rio.Component:
+        high_level_root = self._root_component
+        assert isinstance(
+            high_level_root, root_components.HighLevelRootComponent
+        ), high_level_root
+
+        low_level_root = self._weak_component_data_by_component[
+            high_level_root
+        ].build_result
+        assert isinstance(
+            low_level_root, root_components.FundamentalRootComponent
+        ), low_level_root
+
+        scroll_container = low_level_root.content
+        assert isinstance(
+            scroll_container, rio.ScrollContainer
+        ), scroll_container
+
+        return scroll_container.content
+
     async def _get_webview_window(self):
         import webview  # type: ignore
 
         assert (
             self.running_in_window
         ), f"Can't get the window when not running inside one"
```

### Comparing `rio_ui-0.8.6/rio/session_attachments.py` & `rio_ui-0.8.7/rio/session_attachments.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/state_properties.py` & `rio_ui-0.8.7/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/testing.py` & `rio_ui-0.8.7/rio/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping
 
 import ordered_set
 from typing_extensions import Any, Self, TypeVar, overload
 from uniserde import Jsonable, JsonDoc
 
 import rio
+import rio.app_server
 from rio.app_server import AppServer
-from rio.components.root_components import (
-    FundamentalRootComponent,
-    HighLevelRootComponent,
-)
 
 __all__ = ["TestClient"]
 
 
 T = TypeVar("T")
 C = TypeVar("C", bound=rio.Component)
 
@@ -85,25 +82,49 @@
         self._use_ordered_dirty_set = use_ordered_dirty_set
 
         self._session: rio.Session | None = None
         self._server_task: asyncio.Task | None = None
         self._outgoing_messages = list[JsonDoc]()
         self._responses = asyncio.Queue[JsonDoc]()
         self._responses.put_nowait(
-            {
-                "websiteUrl": "https://unit.test" + active_url,
-                "preferredLanguages": [],
-                "userSettings": user_settings,
-                "windowWidth": 1920,
-                "windowHeight": 1080,
-                "timezone": "America/New_York",
-                "decimalSeparator": ".",
-                "thousandsSeparator": ",",
-                "prefersLightTheme": True,
-            }
+            rio.app_server.InitialClientMessage(
+                website_url="https://unit.test" + active_url,
+                user_settings=user_settings,
+                prefers_light_theme=True,
+                preferred_languages=[],
+                month_names_long=(
+                    "January",
+                    "February",
+                    "March",
+                    "April",
+                    "May",
+                    "June",
+                    "July",
+                    "August",
+                    "September",
+                    "October",
+                    "November",
+                    "December",
+                ),
+                day_names_long=(
+                    "Monday",
+                    "Tuesday",
+                    "Wednesday",
+                    "Thursday",
+                    "Friday",
+                    "Saturday",
+                    "Sunday",
+                ),
+                date_format_string="%Y-%m-%d",
+                timezone="America/New_York",
+                decimal_separator=".",
+                thousands_separator=",",
+                window_width=1920,
+                window_height=1080,
+            ).as_json()
         )
         self._first_refresh_completed = asyncio.Event()
 
     async def _send_message(self, message_text: str) -> None:
         message = json.loads(message_text)
 
         self._outgoing_messages.append(message)
@@ -232,32 +253,15 @@
 
     @property
     def crashed_build_functions(self) -> Mapping[Callable, str]:
         return self.session._crashed_build_functions
 
     @property
     def root_component(self) -> rio.Component:
-        high_level_root = self.session._root_component
-        assert isinstance(
-            high_level_root, HighLevelRootComponent
-        ), high_level_root
-
-        low_level_root = self.session._weak_component_data_by_component[
-            high_level_root
-        ].build_result
-        assert isinstance(
-            low_level_root, FundamentalRootComponent
-        ), low_level_root
-
-        scroll_container = low_level_root.content
-        assert isinstance(
-            scroll_container, rio.ScrollContainer
-        ), scroll_container
-
-        return scroll_container.content
+        return self.session._get_user_root_component()
 
     def get_components(self, component_type: type[C]) -> Iterator[C]:
         root_component = self.root_component
 
         for component in root_component._iter_component_tree():
             if type(component) is component_type:
                 yield component  # type: ignore
```

### Comparing `rio_ui-0.8.6/rio/text_style.py` & `rio_ui-0.8.7/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/theme.py` & `rio_ui-0.8.7/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/user_settings_module.py` & `rio_ui-0.8.7/rio/user_settings_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     ## Attributes
 
     `section_name`: If provided, the settings file will contain a section with
         this name. This allows you to keep the configuration file organized.
         If `None`, the settings will be stored outside of any section.
     """
 
+    # TODO: Document which datatypes are supported
+
     # Any values from this class will be stored in the configuration file under
     # this section. This has to be set to a string. If empty, the values will be
     # set outside of any sections.
     section_name: ClassVar[str] = ""
 
     _rio_session_: session.Session | None = field(
         default=None, init=False, repr=False, compare=False
```

### Comparing `rio_ui-0.8.6/rio/utils.py` & `rio_ui-0.8.7/rio/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,22 @@
     "escape_markdown_code",
 ]
 
 
 _SECURE_HASH_SEED: bytes = secrets.token_bytes(32)
 
 # Expose common paths on the filesystem
-PACKAGE_ROOT_DIR = Path(__file__).resolve().parent
+PACKAGE_ROOT_DIR = Path(__file__).absolute().parent
 PROJECT_ROOT_DIR = PACKAGE_ROOT_DIR.parent
 
 RIO_ASSETS_DIR = PACKAGE_ROOT_DIR / "assets"
 HOSTED_ASSETS_DIR = RIO_ASSETS_DIR / "hosted"
 
 FRONTEND_FILES_DIR = PACKAGE_ROOT_DIR / "frontend files"
+FRONTEND_ASSETS_DIR = FRONTEND_FILES_DIR / "assets"
 
 RIO_LOGO_ASSET_PATH = HOSTED_ASSETS_DIR / "rio-logos/rio-logo-square.png"
 
 SNIPPETS_DIR = PACKAGE_ROOT_DIR / "snippets" / "snippet-files"
 
 if os.name == "nt":
     USER_CACHE_DIR = Path.home() / "AppData" / "Local" / "Cache"
```

### Comparing `rio_ui-0.8.6/rio/world_units.py` & `rio_ui-0.8.7/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto/LICENSE.txt` & `rio_ui-0.8.7/rio/assets/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.8.7/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.8.7/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.8.7/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.8.7/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.8.7/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.8.7/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/__init__.py` & `rio_ui-0.8.7/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/cli_instance.py` & `rio_ui-0.8.7/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/nice_traceback.py` & `rio_ui-0.8.7/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/project.py` & `rio_ui-0.8.7/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/project_setup.py` & `rio_ui-0.8.7/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/rio_api.py` & `rio_ui-0.8.7/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/rioignore.py` & `rio_ui-0.8.7/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/tomlconfig.py` & `rio_ui-0.8.7/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/run_project/app_loading.py` & `rio_ui-0.8.7/rio/cli/run_project/app_loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,32 +43,30 @@
         traceback_html = nice_traceback.format_exception_html(
             err,
             relpath=project_directory,
             frame_filter=traceback_frame_filter,
         )
 
     return f"""
-<div>
-    <div class="rio-traceback rio-dev-tools-background rio-switcheroo-neutral">
-        <div class="rio-traceback-header">
-            {error_icon_svg}
-            <div>Couldn't load the app</div>
-        </div>
-        <div class="rio-traceback-message">
-            Fix the issue below. The app will automatically reload once you save the
-            file.
-        </div>
-        <div class="rio-traceback-traceback">{traceback_html}</div>
-        <div class="rio-traceback-footer">
-            Need help?
-            <div class="rio-traceback-footer-links">
-                <a class="rio-text-link" target="_blank" href="https://discord.gg/7ejXaPwhyH">Ask on Rio's Discord</a>
-                <a class="rio-text-link" target="_blank" href="https://chatgpt.com">Ask ChatGPT</a>
-                <a class="rio-text-link" target="_blank" href="https://rio.dev/docs">Read the docs</a>
-            </div>
+<div class="rio-traceback rio-dev-tools-background rio-switcheroo-neutral">
+    <div class="rio-traceback-header">
+        {error_icon_svg}
+        <div>Couldn't load the app</div>
+    </div>
+    <div class="rio-traceback-message">
+        Fix the issue below. The app will automatically reload once you save the
+        file.
+    </div>
+    <div class="rio-traceback-traceback">{traceback_html}</div>
+    <div class="rio-traceback-footer">
+        Need help?
+        <div class="rio-traceback-footer-links">
+            <a class="rio-text-link" target="_blank" href="https://discord.gg/7ejXaPwhyH">Ask on Rio's Discord</a>
+            <a class="rio-text-link" target="_blank" href="https://chatgpt.com">Ask ChatGPT</a>
+            <a class="rio-text-link" target="_blank" href="https://rio.dev/docs">Read the docs</a>
         </div>
     </div>
 </div>
 """
 
 
 def make_error_message_component(
```

### Comparing `rio_ui-0.8.6/rio/cli/run_project/arbiter.py` & `rio_ui-0.8.7/rio/cli/run_project/arbiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
         # Publish the task, so it can be cancelled
         self._arbiter_task = asyncio.current_task()
 
         # Make sure the webview module is available
         if self.run_in_window and webview is None:
             revel.fatal(
                 "The `window` extra is required to run apps inside of a window."
-                " Run `pip install rio-ui[[window]` to install it."
+                """ Run `pip install "rio-ui[window]"` to install it."""
             )
 
         # Make sure the app is cleanly shut down, even if the arbiter crashes
         # for whichever reason.
         #
         # This loop has a bad case of hiding important exceptions. It would
         # really be nice to only shut down on intentional errors and at least
```

### Comparing `rio_ui-0.8.6/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.8.7/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.8.7/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/cli/run_project/webview_worker.py` & `rio_ui-0.8.7/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/__init__.py` & `rio_ui-0.8.7/rio/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from .auto_form import *
 from .banner import *
 from .button import *
+from .calendar import *
 from .card import *
 from .code_block import *
 from .code_explorer import *
 from .color_picker import *
 from .component import *
 from .container import *
+from .date_input import *
 from .devel_component import *
 from .drawer import *
 from .dropdown import *
 from .flow_container import *
 from .grid import *
 from .html import *
 from .icon import *
```

### Comparing `rio_ui-0.8.6/rio/components/app_root.py` & `rio_ui-0.8.7/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/auto_form.py` & `rio_ui-0.8.7/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/banner.py` & `rio_ui-0.8.7/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/build_failed.py` & `rio_ui-0.8.7/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/button.py` & `rio_ui-0.8.7/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/card.py` & `rio_ui-0.8.7/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/class_container.py` & `rio_ui-0.8.7/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/code_block.py` & `rio_ui-0.8.7/rio/components/code_block.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/color_picker.py` & `rio_ui-0.8.7/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/component.py` & `rio_ui-0.8.7/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/component_tree.py` & `rio_ui-0.8.7/rio/components/component_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .fundamental_component import FundamentalComponent
 
 __all__ = ["ComponentTree"]
 
 
 class ComponentTree(FundamentalComponent):
     """
-    Note: This component makes not attempt to request the correct amount of
+    Note: This component makes no attempt to request the correct amount of
     space. Specify a width/height manually, or make sure it's in a properly
     sized parent.
 
     ## Metadata
 
     public: False
     """
@@ -29,14 +29,16 @@
 
     async def _on_message(self, msg: Any) -> None:
         # Parse the message
         assert isinstance(msg, dict), msg
         selected_component_id = msg["selectedComponentId"]
 
         # Trigger the press event
-        await self.call_event_handler(self.on_select_component, selected_component_id)
+        await self.call_event_handler(
+            self.on_select_component, selected_component_id
+        )
 
         # Refresh the session
         await self.session._refresh()
 
 
 ComponentTree._unique_id = "ComponentTree-builtin"
```

### Comparing `rio_ui-0.8.6/rio/components/container.py` & `rio_ui-0.8.7/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/devel_component.py` & `rio_ui-0.8.7/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/drawer.py` & `rio_ui-0.8.7/rio/components/drawer.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 
     `is_open`: Whether the drawer is currently open.
 
     `is_user_openable`: Whether the user can open or close the drawer. If this
         is `False`, the drawer can only be opened or closed
         programmatically.
 
+    `color`: The color scheme to use for the drawer content. The drawer itself
+        will use the specified color, while content will automatically use one
+        that is legible on top of it. This has no effect on the anchor.
+
 
     ## Examples
 
     A simple drawer with a button as the anchor and some text as content:
 
     ```python
     rio.Drawer(
@@ -110,27 +114,30 @@
     content: rio.Component
     _: KW_ONLY
     on_open_or_close: rio.EventHandler[DrawerOpenOrCloseEvent] = None
     side: Literal["left", "right", "top", "bottom"] = "left"
     is_modal: bool = True
     is_open: bool = False
     is_user_openable: bool = True
+    color: rio.ColorSet = "neutral"
 
     def _validate_delta_state_from_frontend(self, delta_state: JsonDoc) -> None:
         if not set(delta_state) <= {"is_open"}:
             raise AssertionError(
                 f"Frontend tried to change `{type(self).__name__}` state: {delta_state}"
             )
 
         if "is_open" in delta_state and not self.is_user_openable:
             raise AssertionError(
                 "Frontend tried to change value of `Drawer.is_open` even though `is_user_openable` is `False`"
             )
 
-    async def _call_event_handlers_for_delta_state(self, delta_state: JsonDoc) -> None:
+    async def _call_event_handlers_for_delta_state(
+        self, delta_state: JsonDoc
+    ) -> None:
         # Trigger on_open_or_close event
         try:
             is_open = delta_state["is_open"]
         except KeyError:
             pass
         else:
             assert isinstance(is_open, bool), (is_open, type(is_open))
```

### Comparing `rio_ui-0.8.6/rio/components/dropdown.py` & `rio_ui-0.8.7/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/flow_container.py` & `rio_ui-0.8.7/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/fundamental_component.py` & `rio_ui-0.8.7/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/grid.py` & `rio_ui-0.8.7/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/html.py` & `rio_ui-0.8.7/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/icon.py` & `rio_ui-0.8.7/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/image.py` & `rio_ui-0.8.7/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/key_event_listener.py` & `rio_ui-0.8.7/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/labeled_column.py` & `rio_ui-0.8.7/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/linear_containers.py` & `rio_ui-0.8.7/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/link.py` & `rio_ui-0.8.7/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/list_items.py` & `rio_ui-0.8.7/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/list_view.py` & `rio_ui-0.8.7/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/markdown.py` & `rio_ui-0.8.7/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/media_player.py` & `rio_ui-0.8.7/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/mouse_event_listener.py` & `rio_ui-0.8.7/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/multi_line_text_input.py` & `rio_ui-0.8.7/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/node_input.py` & `rio_ui-0.8.7/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/node_output.py` & `rio_ui-0.8.7/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/number_input.py` & `rio_ui-0.8.7/rio/components/number_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,20 +78,20 @@
     respectively.
 
 
     ## Attributes
 
     `value`: The number currently entered by the user.
 
-    `label`: A short text to display next to the text input.
+    `label`: A short text to display next to the number input.
 
-    `prefix_text`: A short text to display before the text input. Useful for
+    `prefix_text`: A short text to display before the number input. Useful for
         displaying currency symbols or other prefixed units.
 
-    `suffix_text`: A short text to display after the text input. Useful for
+    `suffix_text`: A short text to display after the number input. Useful for
         displaying currency names or units.
 
     `minimum`: The minimum value the number can be set to.
 
     `maximum`: The maximum value the number can be set to.
 
     `decimals`: The number of decimals to accept. If the user enters more
```

### Comparing `rio_ui-0.8.6/rio/components/overlay.py` & `rio_ui-0.8.7/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/page_view.py` & `rio_ui-0.8.7/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/plot.py` & `rio_ui-0.8.7/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/popup.py` & `rio_ui-0.8.7/rio/components/popup.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,36 +52,45 @@
 
     ## Attributes
 
     `anchor`: A component which is always visible and positions the popup.
 
     `content`: A component which is only visible when the popup is open.
 
+    `color`: The color scheme to use for the popup's content. The popup will use the
+        specified color as background, while content will automatically use one
+        that is legible on top of it.
+
+    `corner_radius`: The radius of the card's corners. If set to `None`, it
+        is picked from the active theme.
+
     `position`: The location at which the popup opens, relative to the anchor.
 
     `alignment`: The alignment of the popup within the anchor. If the popup
         opens to the left or right, this is the vertical alignment, with `0`
         being the top and `1` being the bottom. If the popup opens to the top or
         bottom, this is the horizontal alignment, with `0` being the left and
         `1` being the right. Has no effect if the popup opens centered.
 
     `gap`: How much space to leave between the popup and the anchor. Has no
-        effect popup opens centered.
+        effect popup opens centered. As all units in Rio, this is measured in
+        font-heights.
 
     `is_open`: Whether the popup is currently open.
 
     `on_open_or_close`: Triggered when the popup is opened or closed.
     """
 
     # TODO: Add example to docstring
 
     anchor: rio.Component
     content: rio.Component
     _: KW_ONLY
     color: rio.ColorSet = "hud"
+    corner_radius: float | tuple[float, float, float, float] | None = None
     position: Literal["left", "top", "right", "bottom", "center"] = "center"
     alignment: float = 0.5
     gap: float = 0.8
     is_open: bool = False
     on_open_or_close: rio.EventHandler[PopupOpenOrCloseEvent] = None
 
     def _validate_delta_state_from_frontend(self, delta_state: JsonDoc) -> None:
@@ -104,11 +113,16 @@
                 self.on_open_or_close,
                 PopupOpenOrCloseEvent(is_open),
             )
 
     def _custom_serialize(self) -> JsonDoc:
         return {
             "color": self.session.theme._serialize_colorset(self.color),
+            "corner_radius": (
+                self.session.theme.corner_radius_medium
+                if self.corner_radius is None
+                else self.corner_radius
+            ),
         }
 
 
 Popup._unique_id = "Popup-builtin"
```

### Comparing `rio_ui-0.8.6/rio/components/progress_bar.py` & `rio_ui-0.8.7/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/progress_circle.py` & `rio_ui-0.8.7/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/rectangle.py` & `rio_ui-0.8.7/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/revealer.py` & `rio_ui-0.8.7/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/root_components.py` & `rio_ui-0.8.7/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/scroll_container.py` & `rio_ui-0.8.7/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/scroll_target.py` & `rio_ui-0.8.7/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/separator.py` & `rio_ui-0.8.7/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/slider.py` & `rio_ui-0.8.7/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/slideshow.py` & `rio_ui-0.8.7/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/spacer.py` & `rio_ui-0.8.7/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/stack.py` & `rio_ui-0.8.7/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/switch.py` & `rio_ui-0.8.7/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/switcher_bar.py` & `rio_ui-0.8.7/rio/components/switcher_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,17 @@
                     rio.Spacer(),
                     rio.SwitcherBar(
                         # For the values, we'll use the URL segments of the
                         # pages in the app. This makes it easy to navigate
                         # to them.
                         values=["/", "first-page", "second-page"],
                         names=["Home", "First Page", "Second Page"],
-                        selected_value=self.session.active_page_instances[0].page_url,
+                        selected_value=self.session.active_page_instances[
+                            0
+                        ].page_url,
                         align_y=0.5,
                         color="primary",
                         on_change=self.on_change,
                     ),
                     margin=1,
                     width="grow",
                 ),
```

### Comparing `rio_ui-0.8.6/rio/components/table.py` & `rio_ui-0.8.7/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/text.py` & `rio_ui-0.8.7/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/text_input.py` & `rio_ui-0.8.7/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/theme_context_switcher.py` & `rio_ui-0.8.7/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/components/tooltip.py` & `rio_ui-0.8.7/rio/components/tooltip.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,28 @@
 
     `experimental`: True
     """
 
     anchor: rio.Component
     tip: str | rio.Component
     position: Literal["left", "top", "right", "bottom"]
+    gap: float
 
     # Hide internal attributes from the IDE
     if not TYPE_CHECKING:
         _tip_component: rio.Component | None
 
     # Impute a Text instance if a string is passed in as the tip
     def __init__(
         self,
         anchor: rio.Component,
         tip: str | rio.Component,
         position: Literal["left", "top", "right", "bottom"],
         *,
+        gap: float = 0.5,
         key: str | None = None,
         margin: float | None = None,
         margin_x: float | None = None,
         margin_y: float | None = None,
         margin_left: float | None = None,
         margin_top: float | None = None,
         margin_right: float | None = None,
@@ -98,14 +100,15 @@
             self._tip_text = tip
             self._tip_component = None
         else:
             self._tip_text = None
             self._tip_component = tip
 
         self.position = position
+        self.gap = gap
 
         self._properties_set_by_creator_.add("_tip_component")
 
     def __post_init__(self):
         # FIXME: This breaks attribute bindings
         if isinstance(self._tip_text, str):
             self._tip_component = rio.Text(self._tip_text)
```

### Comparing `rio_ui-0.8.6/rio/components/website.py` & `rio_ui-0.8.7/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/monkeypatches.py` & `rio_ui-0.8.7/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/typing_utils.py` & `rio_ui-0.8.7/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/validator.py` & `rio_ui-0.8.7/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/component_details.py` & `rio_ui-0.8.7/rio/debug/dev_tools/component_details.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 from typing import *  # type: ignore
 
 import rio
 import rio.docs
 
 from ... import utils
 
+try:
+    RIO_PATH = Path(rio.__file__).parent
+except Exception:
+    # Use a dummy path. It doesn't really matter, as long as it doesn't crash
+    # `Path.is_relative_to`
+    RIO_PATH = Path.cwd() / "rio"
+
 
 class ComponentDetails(rio.Component):
     component_id: int
 
     component_natural_width: float = 0
     component_natural_height: float = 0
 
@@ -90,121 +97,154 @@
 
         # In rare cases components can't be found, because they're created
         # client-side (e.g. injected margins). In this case, just don't display
         # anything.
         except KeyError:
             return rio.Spacer(height=0)
 
-        # Create a grid with all the details
-        result = rio.Grid(row_spacing=0.5, column_spacing=0.5)
-        row_index = 0
+        debug_details = target._get_debug_details()
 
-        def add_cell(
-            text: str,
-            column_index: int,
-            is_label: bool,
-            *,
-            width: int = 1,
-        ) -> None:
-            result.add(
-                rio.Text(
-                    text,
-                    style="dim" if is_label else "text",
-                    justify="right" if is_label else "left",
-                ),
-                row_index,
-                column_index,
-                width=width,
-            )
+        return rio.Column(
+            self._create_header(target),
+            *self._create_instantiation_info(target),
+            self._create_layout_details(target, debug_details),
+            *self._create_extra_details(debug_details),
+            spacing=0.2,
+        )
 
+    def _create_header(self, target: rio.Component) -> rio.Component:
         # Any values which should be displayed right in the title
         header_accessories = []
 
         if target.key is not None:
             header_accessories = [
                 rio.Icon("material/key", fill="dim"),
                 rio.Text(
                     target.key,
                     style="dim",
                     justify="left",
                 ),
             ]
 
-        # Title
-        result.add(
-            rio.Row(
-                rio.Text(
-                    type(target).__qualname__,
-                    style="heading3",
+        # Link to docs
+        if type(target)._rio_builtin_:
+            docs_url = rio.docs.build_documentation_url(type(target).__name__)
+            link_color = self.session.theme.secondary_color
+
+            docs_link = [
+                rio.Link(
+                    rio.Row(
+                        rio.Icon("material/library-books", fill=link_color),
+                        rio.Text("Docs", style=rio.TextStyle(fill=link_color)),
+                        spacing=0.5,
+                        align_x=0,
+                    ),
+                    docs_url,
+                    # TODO: Support icons in links
+                    open_in_new_tab=True,
+                    margin_left=0.5,
                 ),
-                rio.Spacer(),
-                *header_accessories,
-                margin_bottom=0.2,
-                spacing=0.5,
+            ]
+        else:
+            docs_link = []
+
+        return rio.Row(
+            rio.Text(
+                type(target).__qualname__,
+                style="heading3",
             ),
-            row_index,
-            0,
-            width=5,
+            rio.Spacer(),
+            *header_accessories,
+            *docs_link,
+            spacing=0.5,
         )
-        row_index += 1
 
+    def _create_instantiation_info(
+        self, target: rio.Component
+    ) -> Iterable[rio.Component]:
         # Which file/line was this component instantiated from?
         file, line = target._creator_stackframe_
 
+        # If it was instantiated somewhere in the rio internals, don't show it
+        if file.is_relative_to(RIO_PATH):
+            return
+
         try:
             file = file.relative_to(Path.cwd())
         except ValueError:
             pass
 
-        result.add(
-            rio.Text(
-                f"{file} line {line}",
-                style="dim",
-                justify="left",
-            ),
-            row_index,
-            0,
-            width=5,
+        yield rio.Text(
+            f"{file} line {line}",
+            style="dim",
+            justify="left",
         )
 
-        row_index_before_properties = row_index
-        row_index += 1
+    def _create_layout_details(
+        self, target: rio.Component, debug_details: dict[str, Any]
+    ) -> rio.Component:
+        # Create a grid with all the details
+        grid = DetailsGrid()
 
-        # Custom properties
-        #
-        # Make sure to skip any which already have custom tailored cells
-        debug_details = target._get_debug_details()
-        for prop_name, prop_value in debug_details.items():
-            # Some values have special handling below
-            if prop_name in (
-                "key",
-                "width",
-                "height",
-                "margin",
-                "margin_x",
-                "margin_y",
-                "margin_left",
-                "margin_right",
-                "margin_top",
-                "margin_bottom",
-                "align_x",
-                "align_y",
-            ):
-                continue
+        # Add some extra spacing
+        grid.row += 1
 
-            # Display this property
-            value_limit = 30
-            prop_str = repr(prop_value)
+        # Margins
+        (
+            margin_left,
+            margin_top,
+            margin_right,
+            margin_bottom,
+        ) = self._get_effective_margins(target)
+
+        single_x_margin = margin_left == margin_right
+        single_y_margin = margin_top == margin_bottom
+
+        if single_x_margin and single_y_margin:
+            grid.add_label("margin", column=0)
+            grid.add_value(str(margin_left), column=1)
 
-            if len(prop_str) > value_limit:
-                prop_str = prop_str[: value_limit - 1] + "…"
+            grid.row += 1
 
-            add_cell(prop_name, 0, True)
-            add_cell(prop_str, 1, False, width=4)
-            row_index += 1
+        else:
+            if single_x_margin:
+                grid.add_label("margin_x", column=0)
+                grid.add_value(str(margin_left), column=1)
+
+            else:
+                grid.add_label("margin_left", column=0)
+                grid.add_value(str(margin_left), column=1)
+
+                grid.add_label("margin_right", column=2)
+                grid.add_value(str(margin_right), column=3)
+
+            grid.row += 1
+
+            if single_y_margin:
+                grid.add_label("margin_y", column=0)
+                grid.add_value(str(margin_top), column=1)
+
+            else:
+                grid.add_label("margin_top", column=0)
+                grid.add_value(str(margin_top), column=1)
+
+                grid.add_label("margin_bottom", column=2)
+                grid.add_value(str(margin_bottom), column=3)
+
+            grid.row += 1
+
+        # Alignment
+        if "align_x" in debug_details or "align_y" in debug_details:
+            grid.add_label("align_x", column=0)
+            grid.add_value(str(debug_details.get("align_x", "-")), column=1)
+
+            grid.add_label("align_y", column=2)
+            grid.add_value(str(debug_details.get("align_y", "-")), column=3)
+
+            grid.row += 1
 
         # Size
         if "width" in debug_details or "height" in debug_details:
             try:
                 py_width_str = debug_details["width"]
             except KeyError:
                 py_width_str = "-"
@@ -220,133 +260,161 @@
                 py_height_str = "-"
             else:
                 if isinstance(py_height_str, (int, float)):
                     py_height_str = round(py_height_str, 2)
 
                 py_height_str = repr(py_height_str)
 
-            # Spacing to separate the table from the rest
-            row_index += 1
+            # Add some extra spacing
+            grid.row += 1
 
             # Header
-            result.add(
-                rio.Text("width", style="dim", justify="left"), row_index, 1
-            )
-            result.add(
-                rio.Text("height", style="dim", justify="left"), row_index, 2
-            )
-            row_index += 1
+            grid.add_label("width", column=1)
+            grid.add_label("height", column=2)
+            grid.row += 1
 
             # The size as specified in Python
-            add_cell("python", 0, True)
-            add_cell(py_width_str, 1, False)
-            add_cell(py_height_str, 2, False)
-            row_index += 1
+            grid.add_label("python", column=0)
+            grid.add_value(py_width_str, column=1)
+            grid.add_value(py_height_str, column=2)
+            grid.row += 1
 
             # The component's natural size
-            add_cell("natural", 0, True)
-            add_cell(str(round(self.component_natural_width, 2)), 1, False)
-            add_cell(str(round(self.component_natural_height, 2)), 2, False)
-            row_index += 1
+            grid.add_label("natural", column=0)
+            grid.add_value(
+                str(round(self.component_natural_width, 2)), column=1
+            )
+            grid.add_value(
+                str(round(self.component_natural_height, 2)), column=2
+            )
+            grid.row += 1
 
             # The component's allocated size
-            add_cell("allocated", 0, True)
-            add_cell(str(round(self.component_allocated_width, 2)), 1, False)
-            add_cell(str(round(self.component_allocated_height, 2)), 2, False)
-            row_index += 1
-
-            # More spacing
-            row_index += 1
-
-        # Margins
-        (
-            margin_left,
-            margin_top,
-            margin_right,
-            margin_bottom,
-        ) = self._get_effective_margins(target)
-
-        single_x_margin = margin_left == margin_right
-        single_y_margin = margin_top == margin_bottom
-
-        if single_x_margin and single_y_margin:
-            add_cell("margin", 0, True)
-            add_cell(str(margin_left), 1, False)
-            row_index += 1
+            grid.add_label("allocated", column=0)
+            grid.add_value(
+                str(round(self.component_allocated_width, 2)), column=1
+            )
+            grid.add_value(
+                str(round(self.component_allocated_height, 2)), column=2
+            )
+            grid.row += 1
 
-        else:
-            if single_x_margin:
-                add_cell("margin_x", 0, True)
-                add_cell(str(margin_left), 1, False)
+        # result.add(
+        #     layout_preview.LayoutPreview(component=target),
+        #     row_index_before_properties + 1,
+        #     4,
+        #     height=row_index - row_index_before_properties,
+        # )
 
-            else:
-                add_cell("margin_left", 0, True)
-                add_cell(str(margin_left), 1, False)
+        # Push all of the content to the left. This could be done by aligning
+        # the entire Grid, but that would ellipsize some long texts. Instead,
+        # add a Spacer into a fifth column, which will take up any unused space.
+        grid.add(
+            rio.Spacer(height=0),
+            column=5,
+        )
 
-                add_cell("margin_right", 2, True)
-                add_cell(str(margin_right), 3, False)
+        # Done
+        return grid.as_rio_component()
 
-            row_index += 1
+    def _create_extra_details(
+        self, debug_details: dict[str, Any]
+    ) -> Iterable[rio.Component]:
+        grid = DetailsGrid()
 
-            if single_y_margin:
-                add_cell("margin_y", 0, True)
-                add_cell(str(margin_top), 1, False)
+        # Custom properties
+        #
+        # Make sure to skip any which already have custom tailored cells
+        for prop_name, prop_value in debug_details.items():
+            # Some values have special handling below
+            if prop_name in (
+                "key",
+                "width",
+                "height",
+                "margin",
+                "margin_x",
+                "margin_y",
+                "margin_left",
+                "margin_right",
+                "margin_top",
+                "margin_bottom",
+                "align_x",
+                "align_y",
+            ):
+                continue
 
-            else:
-                add_cell("margin_top", 0, True)
-                add_cell(str(margin_top), 1, False)
+            # Display this property
+            grid.add_row(prop_name, repr(prop_value))
 
-                add_cell("margin_bottom", 2, True)
-                add_cell(str(margin_bottom), 3, False)
+        if grid.row > 0:
+            yield rio.Revealer("More details", grid.as_rio_component())
 
-            row_index += 1
 
-        # Alignment
-        if "align_x" in debug_details or "align_y" in debug_details:
-            add_cell("align_x", 0, True)
-            add_cell(str(debug_details.get("align_x", "-")), 1, False)
+class DetailsGrid:
+    def __init__(self):
+        self.grid = rio.Grid(row_spacing=0.5, column_spacing=0.5)
+        self.row = 0
+        self.max_column = 0
+
+    def add_row(self, label: str, value: str) -> None:
+        self.add_label(label, column=0)
+        self.add_value(value, column=1, ellipsize=True)
+        self.row += 1
+
+    def add_label(
+        self,
+        text: str,
+        *,
+        row: int | None = None,
+        column: int,
+        width: int = 1,
+    ) -> None:
+        self.add(
+            rio.Text(
+                text,
+                style="dim",
+                justify="right",
+            ),
+            row=row,
+            column=column,
+            width=width,
+        )
 
-            add_cell("align_y", 2, True)
-            add_cell(str(debug_details.get("align_y", "-")), 3, False)
-            row_index += 1
+    def add_value(
+        self,
+        value: str,
+        *,
+        row: int | None = None,
+        column: int,
+        width: int = 1,
+        ellipsize: bool = False,
+    ) -> None:
+        self.add(
+            rio.Text(
+                value,
+                justify="left",
+                width="grow" if ellipsize else "natural",
+                wrap="ellipsize" if ellipsize else False,
+            ),
+            row=row,
+            column=column,
+            width=width,
+        )
 
-        # Link to docs
-        if type(target)._rio_builtin_:
-            docs_url = rio.docs.build_documentation_url(type(target).__name__)
-            link_color = self.session.theme.secondary_color
+    def add(
+        self,
+        child: rio.Component,
+        *,
+        row: int | None = None,
+        column: int,
+        width: int = 1,
+        height: int = 1,
+    ) -> None:
+        if row is None:
+            row = self.row
 
-            result.add(
-                rio.Link(
-                    rio.Row(
-                        rio.Icon("material/library-books", fill=link_color),
-                        rio.Text("Docs", style=rio.TextStyle(fill=link_color)),
-                        spacing=0.5,
-                        align_x=0,
-                    ),
-                    docs_url,
-                    # TODO: Support icons in links
-                    open_in_new_tab=True,
-                    margin_top=0.2,
-                ),
-                row_index,
-                0,
-                width=2,
-            )
-            row_index += 1
+        self.grid.add(child, row, column, width=width, height=height)
 
-        # Push all of the content to the left. This could be done by aligning
-        # the entire Grid, but that would ellipsize some long texts. Instead,
-        # add a Spacer into a fifth column, which will take up any unused space.
-        result.add(
-            rio.Spacer(height=0),
-            row_index - 1,
-            4,
-        )
-        # result.add(
-        #     layout_preview.LayoutPreview(component=target),
-        #     row_index_before_properties + 1,
-        #     4,
-        #     height=row_index - row_index_before_properties,
-        # )
+        self.max_column = max(self.max_column, column)
 
-        # Done
-        return result
+    def as_rio_component(self) -> rio.Component:
+        return self.grid
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/deploy_page.py` & `rio_ui-0.8.7/rio/debug/dev_tools/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/dev_tools_sidebar.py` & `rio_ui-0.8.7/rio/debug/dev_tools/dev_tools_sidebar.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,56 +72,64 @@
         return rio.Text(
             f"TODO: {self.selected_page}",
             margin=2,
             width=REGULAR_PAGE_WIDTH,
         )
 
     def build(self) -> rio.Component:
-        return rio.Row(
-            # Big fat line to separate the dev tools from the rest of the page
-            rio.Rectangle(
-                width=0.3,
-                fill=self.session.theme.primary_palette.background,
-            ),
-            # Currently active page
-            rio.components.class_container.ClassContainer(
-                rio.Switcher(self.get_selected_page()),
-                classes=["rio-switcheroo-neutral", "rio-dev-tools-background"],
-            ),
-            # Navigation
-            rio.Column(
-                rio.SwitcherBar(
-                    names=[
-                        # "Project",
-                        "Tree",
-                        "Icons",
-                        "Theme",
-                        # "Docs",
-                        "Deploy",
-                    ],
-                    icons=[
-                        # "rio/logo",
-                        "material/view-quilt",
-                        "material/emoji-people",
-                        "material/palette",
-                        # "material/library-books",
-                        "material/rocket-launch",
-                    ],
-                    values=[
-                        # "project",
-                        "tree",
-                        "icons",
-                        "theme",
-                        # "docs",
-                        "deploy",
+        return rio.Rectangle(
+            # Make sure everything has a background, otherwise the component
+            # highlighter will be visible behind this component
+            fill=self.session.theme.background_color,
+            content=rio.Row(
+                # Big fat line to separate the dev tools from the rest of the page
+                rio.Rectangle(
+                    width=0.3,
+                    fill=self.session.theme.primary_palette.background,
+                ),
+                # Currently active page
+                rio.components.class_container.ClassContainer(
+                    rio.Switcher(self.get_selected_page()),
+                    classes=[
+                        "rio-switcheroo-neutral",
+                        "rio-dev-tools-background",
                     ],
-                    allow_none=True,
-                    orientation="vertical",
-                    spacing=2,
-                    color="primary",
-                    selected_value=self.bind().selected_page,
-                    margin=0.2,
                 ),
-                rio.Spacer(),
-                rio.components.dev_tools_connector.DevToolsConnector(),
+                # Navigation
+                rio.Column(
+                    rio.SwitcherBar(
+                        names=[
+                            # "Project",
+                            "Tree",
+                            "Icons",
+                            "Theme",
+                            # "Docs",
+                            "Deploy",
+                        ],
+                        icons=[
+                            # "rio/logo",
+                            "material/view-quilt",
+                            "material/emoji-people",
+                            "material/palette",
+                            # "material/library-books",
+                            "material/rocket-launch",
+                        ],
+                        values=[
+                            # "project",
+                            "tree",
+                            "icons",
+                            "theme",
+                            # "docs",
+                            "deploy",
+                        ],
+                        allow_none=True,
+                        orientation="vertical",
+                        spacing=2,
+                        color="primary",
+                        selected_value=self.bind().selected_page,
+                        margin=0.2,
+                    ),
+                    rio.Spacer(),
+                    rio.components.dev_tools_connector.DevToolsConnector(),
+                ),
             ),
         )
```

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/docs_page.py` & `rio_ui-0.8.7/rio/debug/dev_tools/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/icons_page.py` & `rio_ui-0.8.7/rio/debug/dev_tools/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/layout_preview.py` & `rio_ui-0.8.7/rio/debug/dev_tools/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/project_page.py` & `rio_ui-0.8.7/rio/debug/dev_tools/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/sample_icons_grid.py` & `rio_ui-0.8.7/rio/debug/dev_tools/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/theme_picker_page.py` & `rio_ui-0.8.7/rio/debug/dev_tools/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/debug/dev_tools/tree_page.py` & `rio_ui-0.8.7/rio/debug/dev_tools/tree_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 
     def _on_select_component(self, component_id: int) -> None:
         self._selected_component_id = component_id
 
     def build(self) -> rio.Component:
         margin = 1
 
-        children = [
+        column = rio.Column(
             rio.Text(
                 "Component Tree",
                 style="heading2",
                 margin=margin,
                 justify="left",
             ),
-            rio.components.component_tree.ComponentTree(
-                width=10,
+            rio.Container(
+                rio.components.component_tree.ComponentTree(
+                    width=10,
+                    height=10,
+                    margin_left=margin,
+                    on_select_component=self._on_select_component,
+                ),
                 height="grow",
-                margin_left=margin,
-                on_select_component=self._on_select_component,
             ),
-        ]
+            height="grow",
+        )
 
         if self._selected_component_id is not None:
-            children.append(
+            column.add(
                 component_details.ComponentDetails(
                     component_id=self._selected_component_id,
                     margin=margin,
                 )
             )
 
-        return rio.Column(*children)
+        return column
```

### Comparing `rio_ui-0.8.6/rio/docs/__init__.py` & `rio_ui-0.8.7/rio/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/frontend files/index.html` & `rio_ui-0.8.7/rio/frontend files/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,13 @@
             globalThis.RUNNING_IN_WINDOW = '{running_in_window}';
             globalThis.CHILD_ATTRIBUTE_NAMES = '{child_attribute_names}';
 
             // Create a Promise that resolves when the CSS is done loading
             let { cssLoaded, resolveCssLoaded, rejectCssLoaded } =
                 Promise.withResolvers();
         </script>
-        
-        
-      <script type="module" crossorigin src="/rio/frontend/assets/index-8ca8e5f1.js"></script>
-      <link rel="stylesheet" href="/rio/frontend/assets/index-9eba151c.css">
+      <script type="module" crossorigin src="/rio/frontend/assets/index-BqnRx0kk.js"></script>
+      <link rel="stylesheet" crossorigin href="/rio/frontend/assets/index-CVJ3BDCx.css">
     </head>
 
     <body class="rio-switcheroo-background"></body>
 </html>
```

### Comparing `rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.8.7/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/README.md` & `rio_ui-0.8.7/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/__init__.py` & `rio_ui-0.8.7/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/core-classes.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/core-classes.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/debugging-setup.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/debugging-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/deployment.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/deployment.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-custom-events.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-custom-events.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-install.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-install.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # How do I install Rio?
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
-pip install rio
+pip install rio-ui
 ```
 
 On some platforms, `pip` isn't available directly in the command line. If you're
 running into trouble with the command above, try one of theses alternatives:
 
 ```bash
-python -m pip install rio
+python -m pip install rio-ui
 ```
 
 ```bash
-python3 -m pip install rio
+python3 -m pip install rio-ui
 ```
 
 ```bash
-py -m pip install rio
+py -m pip install rio-ui
 ```
 
 After this, a `rio` command will be available in your terminal. You can use this
 to create new projects, add components to existing ones, and much more. Once
 again, if the command for some reason isn't available, you can try running `rio`
 through `python`:
```

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/persistent-settings.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/persistent-settings.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/project-setup.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/project-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/run-project.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/run-project.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/howtos/theming.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/howtos/theming.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/README.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/README.md` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.8.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/scripts/benchmark.py` & `rio_ui-0.8.7/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/scripts/build_frontend.py` & `rio_ui-0.8.7/scripts/build_frontend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import subprocess
 import sys
 from pathlib import Path
 
 import rio.utils
 
-PROJECT_ROOT_DIR = rio.utils.PROJECT_ROOT_DIR.relative_to(Path.cwd())
+PROJECT_ROOT_DIR = rio.utils.PROJECT_ROOT_DIR
 INPUT_DIR = PROJECT_ROOT_DIR / "frontend"
-OUTPUT_DIR = Path("..") / "rio" / "frontend files"
-
-OUTPUT_DIR.mkdir(exist_ok=True)
+OUTPUT_DIR = PROJECT_ROOT_DIR / "rio" / "frontend files"
+ASSETS_DIR = OUTPUT_DIR / "assets"
 
 
 def build(*extra_args: str):
     npx(
         "vite",
         "build",
         INPUT_DIR,
         "--outDir",
         OUTPUT_DIR,
         "--config",
-        PROJECT_ROOT_DIR / "vite.config.js",
+        PROJECT_ROOT_DIR / "vite.config.mjs",
         "--base",
         "/rio/frontend",
         "--emptyOutDir",
         *extra_args,
     )
```

### Comparing `rio_ui-0.8.6/scripts/build_material_icon_set.py` & `rio_ui-0.8.7/scripts/build_material_icon_set.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/scripts/code_coverage.py` & `rio_ui-0.8.7/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/scripts/publish_new_release.py` & `rio_ui-0.8.7/scripts/publish_new_release.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_attribute_bindings.py` & `rio_ui-0.8.7/tests/test_attribute_bindings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_custom_components.py` & `rio_ui-0.8.7/tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_docstring_code_blocks.py` & `rio_ui-0.8.7/tests/test_docstring_code_blocks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+import json
 import re
 import subprocess
-import sys
 import tempfile
 import textwrap
 from typing import *  # type: ignore
 
-import black
-import pyright
 import pytest
 
 import rio.docs
 
 CODE_BLOCK_PATTERN = re.compile(r"```(.*?)```", re.DOTALL)
 
 
@@ -45,88 +43,114 @@
         assert language, "The code block has no language specified"
 
         result.append(block)
 
     return result
 
 
-@pytest.mark.parametrize("obj", all_documented_objects)
-def test_eval_code_block(obj: type | Callable) -> None:
-    # Eval all code blocks and make sure they don't crash
-    for source in get_code_blocks(obj):
-        compile(source, "<string>", "exec")
-
-
-@pytest.mark.parametrize("obj", all_documented_objects)
-def test_code_block_is_formatted(obj: type | Callable) -> None:
-    # Make sure all code blocks are formatted according to black
-    for source in get_code_blocks(obj):
-        formatted_source = black.format_str(source, mode=black.FileMode())
-
-        # Black often inserts 2 empty lines between stuff, but that's really not
-        # necessary in docstrings. So we'll collapse those into a single empty
-        # line.
-        source = source.replace("\n\n\n", "\n\n")
-        formatted_source = formatted_source.replace("\n\n\n", "\n\n")
-
-        assert source == formatted_source
-
+def ruff_format(source_code: str) -> str:
+    # Write the source code to a temporary file
+    with tempfile.NamedTemporaryFile(suffix=".py", mode="w") as temp_file:
+        temp_file.write(source_code)
+        temp_file.flush()
+
+        # Run ruff to format the source code in the temporary file
+        subprocess.run(
+            [
+                "python",
+                "-m",
+                "ruff",
+                "format",
+                temp_file.name,
+            ],
+            check=True,
+        )
 
-PYRIGHT_ERROR_OR_WARNING_REGEX = re.compile(
-    r".*\.py:\d+:\d+ - (?:error|warning): (.*)"
-)
+        # Read the formatted source code
+        with open(temp_file.name, "r") as temp_file:
+            return temp_file.read()
 
 
-def _find_static_typing_errors(source: str) -> str:
+def ruff_check(source_code: str) -> list[str]:
     """
-    Run pyright on the given source and return the number of errors and
-    warnings.
+    Checks the given source code using `ruff`. Returns any encountered problems.
     """
-    with tempfile.NamedTemporaryFile(suffix=".py") as f:
-        # Dump the source to a file, and implicitly define/import some stuff
-        f.write(
-            """
-import pathlib, rio
+    # Dump the source to a file, and implicitly define/import some stuff
+    with tempfile.NamedTemporaryFile(
+        suffix=".py", mode="w", encoding="utf-8"
+    ) as temp_file:
+        temp_file.write(
+            f"""
+import pathlib
+import rio
 
+# Importing `Path` directly causes ruff to complain about a redefinition
 Path = pathlib.Path
 self = rio.Spacer()
-""".encode("utf-8")
+
+{source_code}
+"""
         )
-        f.write(source.encode("utf-8"))
-        f.flush()
+        temp_file.flush()
 
-        # Run pyright
-        proc = pyright.run(
-            "--pythonpath",
-            sys.executable,
-            f.name,
+        # Run ruff to format the source code in the temporary file
+        proc = subprocess.run(
+            [
+                "python",
+                "-m",
+                "ruff",
+                "check",
+                temp_file.name,
+                "--ignore=E402",  # Caused by the injected imports
+                "--output-format=json",
+            ],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
+            text=True,
         )
-        result_out = proc.stdout
-        assert isinstance(result_out, bytes), type(result_out)
-        result_out = result_out.decode()
 
-        # Find the number of errors and warnings
-        lines = list[str]()
+        output = json.loads(proc.stdout)
+        assert isinstance(output, list), output
 
-        for line in result_out.splitlines():
-            match = PYRIGHT_ERROR_OR_WARNING_REGEX.match(line)
+    # Parse the output
+    result: list[str] = []
 
-            if match:
-                lines.append(match.group(1))
+    for entry in output:
+        result.append(entry["message"])
+
+    return result
+
+
+@pytest.mark.parametrize("obj", all_documented_objects)
+def test_eval_code_block(obj: type | Callable) -> None:
+    # Eval all code blocks and make sure they don't crash
+    for source in get_code_blocks(obj):
+        compile(source, "<string>", "exec")
+
+
+@pytest.mark.parametrize("obj", all_documented_objects)
+def test_code_block_is_formatted(obj: type | Callable) -> None:
+    # Make sure all code blocks are formatted according to ruff
+    for source in get_code_blocks(obj):
+        formatted_source = ruff_format(source)
+
+        # Ruff often inserts 2 empty lines between definitions, but that's
+        # really not necessary in docstrings. Collapse them to a single empty
+        # line.
+        source = source.replace("\n\n\n", "\n\n")
+        formatted_source = formatted_source.replace("\n\n\n", "\n\n")
 
-        return "\n".join(lines)
+        assert formatted_source == source
 
 
 @pytest.mark.parametrize("obj", all_documented_objects)
 def test_analyze_code_block(obj: type | Callable) -> None:
-    # A lot of snippets are missing context, so it's only natural that pyright
-    # will find issues with the code. There isn't really anything we can do
-    # about it, so we'll just skip those object.
+    # A lot of snippets are missing context, so it's only natural that ruff will
+    # find issues with the code. There isn't really anything we can do about it,
+    # so we'll just skip those object.
     if obj in (rio.App, rio.Color, rio.UserSettings):
         pytest.xfail()
 
-    # Make sure pyright is happy with all code blocks
+    # Make sure ruff is happy with all code blocks
     for source in get_code_blocks(obj):
-        errors = _find_static_typing_errors(source)
+        errors = ruff_check(source)
         assert not errors, errors
```

### Comparing `rio_ui-0.8.6/tests/test_documentation.py` & `rio_ui-0.8.7/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_events.py` & `rio_ui-0.8.7/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_project_templates.py` & `rio_ui-0.8.7/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_reconciliation.py` & `rio_ui-0.8.7/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_refresh.py` & `rio_ui-0.8.7/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_session.py` & `rio_ui-0.8.7/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_testing_tools.py` & `rio_ui-0.8.7/tests/test_testing_tools.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_user_settings.py` & `rio_ui-0.8.7/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/test_zzz_guardrails.py` & `rio_ui-0.8.7/tests/test_zzz_guardrails.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/tests/utils.py` & `rio_ui-0.8.7/tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,28 +38,54 @@
             debug_mode=False,
             running_in_window=False,
             internal_on_app_start=None,
         )
         websocket: fastapi.WebSocket = None  # type: ignore
         session = rio.Session(
             app_server_=app_server,
-            session_token="<a fake session token>",
+            session_token="<very-fake-session-token>",
             send_message=_fake_send_message,
             receive_message=_fake_receive_message,
             websocket=websocket,
             client_ip="localhost",
             client_port=12345,
             http_headers=starlette.datastructures.Headers(),
             timezone=pytz.UTC,
             preferred_languages=["en-US"],
+            month_names_long=(
+                "January",
+                "February",
+                "March",
+                "April",
+                "May",
+                "June",
+                "July",
+                "August",
+                "September",
+                "October",
+                "November",
+                "December",
+            ),
+            day_names_long=(
+                "Monday",
+                "Tuesday",
+                "Wednesday",
+                "Thursday",
+                "Friday",
+                "Saturday",
+                "Sunday",
+            ),
+            date_format_string="%Y-%m-%d",
+            first_day_of_week=0,
             decimal_separator=".",
             thousands_separator=",",
             window_width=1920,
             window_height=1080,
             base_url=rio.URL("https://unit.test"),
+            active_page_url=rio.URL("https://unit.test"),
             theme_=rio.Theme.from_colors(),
         )
 
         rio.global_state.currently_building_session = session
         session._root_component = HighLevelRootComponent(
             build, lambda: rio.Text("")
         )
```

### Comparing `rio_ui-0.8.6/LICENSE.txt` & `rio_ui-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/README.md` & `rio_ui-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.8.6/pyproject.toml` & `rio_ui-0.8.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 [project.optional-dependencies]
 window = [
     "aiofiles~=23.2",
     "platformdirs~=3.11",
     "pywebview~=4.2",
     "cefpython3~=66.1 ; sys_platform == 'win32'",
-    "pygobject~=3.44 ; sys_platform == 'linux'",
+    "pywebview[qt] ; sys_platform == 'linux'",
 ]
 
 [project.urls]
 homepage = "https://rio.dev"
 repository = "https://github.com/rio-labs/rio"
 documentation = "https://rio.dev/docs"
 
@@ -87,24 +87,22 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 dev-dependencies = [
     "aiofiles>=23.2.1",
     "alt-pytest-asyncio~=0.7.2",
-    "black~=24.4",
     "coverage~=7.2",
     "pandas>=2.2",
     "plotly>=5.22",
     "polars>=0.20",
     "pre-commit~=3.1",
-    "pyright~=1.1.350",
     "pytest~=7.3",
     "requests~=2.31",
-    "ruff~=0.4",
+    "ruff>=0.4.7",
     "hatch>=1.11.1",
 ]
 managed = true
 
 [tool.rye.scripts]
 build = { call = "scripts.build_frontend:build" }
 dev-build = { call = "scripts.build_frontend:dev_build" }
```

### Comparing `rio_ui-0.8.6/PKG-INFO` & `rio_ui-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.8.6
+Version: 0.8.7
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: repository, https://github.com/rio-labs/rio
 Project-URL: documentation, https://rio.dev/docs
 Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
@@ -245,15 +245,15 @@
 Requires-Dist: uvicorn[standard]~=0.29.0
 Requires-Dist: watchfiles~=0.21
 Requires-Dist: yarl>=1.9
 Provides-Extra: window
 Requires-Dist: aiofiles~=23.2; extra == 'window'
 Requires-Dist: cefpython3~=66.1; (sys_platform == 'win32') and extra == 'window'
 Requires-Dist: platformdirs~=3.11; extra == 'window'
-Requires-Dist: pygobject~=3.44; (sys_platform == 'linux') and extra == 'window'
+Requires-Dist: pywebview[qt]; (sys_platform == 'linux') and extra == 'window'
 Requires-Dist: pywebview~=4.2; extra == 'window'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem; height: 8.8rem"/>
 </p>
```

