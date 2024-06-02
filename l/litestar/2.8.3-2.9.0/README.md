# Comparing `tmp/litestar-2.8.3.tar.gz` & `tmp/litestar-2.9.0.tar.gz`

## Comparing `litestar-2.8.3.tar` & `litestar-2.9.0.tar`

### file list

```diff
@@ -1,730 +1,763 @@
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 litestar-2.8.3/Makefile
--rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 litestar-2.8.3/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/__main__.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_multipart.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_parsers.py
--rw-r--r--   0        0        0    39586 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/app.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/background_tasks.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/concurrency.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/constants.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/controller.py
--rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/data_extractors.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/di.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/enums.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/file_system.py
--rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/pagination.py
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/py.typed
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/router.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/status_codes.py
--rw-r--r--   0        0        0    25806 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/typing.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/utils.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_layers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/datastructures.py
--rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/plugin.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/responses.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    25613 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/dataclass.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/pagination.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/struct.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/typed_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/__init__.py
--rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/model.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/types.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/utils.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/__init__.py
--rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/asyncpg.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/psycopg.py
--rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/__init__.py
--rw-r--r--   0        0        0    20230 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/_utils.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/app.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/compression.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/csrf.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/__init__.py
--rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/base.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/request.py
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/__init__.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jinja.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/mako.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/minijinja.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/minijnja.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/piccolo.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/attrs/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/attrs/attrs_schema_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/config.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_di_plugin.py
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_dto_factory.py
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_init_plugin.py
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_schema_plugin.py
--rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/utils.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/testing.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/state.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/url.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/__init__.py
--rw-r--r--   0        0        0    33807 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/_backend.py
--rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/_codegen_backend.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/_types.py
--rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/base_dto.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/config.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/data_structures.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/dataclass_dto.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/field.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/msgspec_dto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/types.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/events/__init__.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/events/emitter.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/events/listener.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/dto_exceptions.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/_utils.py
--rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/picologging.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/base.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/csrf.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/response_cache.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/brotli_facade.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/facade.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/gzip_facade.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/middleware.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/__init__.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/config.py
--rw-r--r--   0        0        0    23353 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/controller.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/plugins.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/__init__.py
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/base.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/core.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/flash.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/sqlalchemy.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/structlog.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/_exceptions.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/_filters.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/exceptions.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/filters.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/handlers.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/abc/__init__.py
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/abc/_async.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/abc/_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/testing/__init__.py
--rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/__init__.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/base.py
--rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/file.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/redirect.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/sse.py
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/streaming.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/template.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/asgi.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/base.py
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/http.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/__init__.py
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/base.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/__init__.py
--rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/auth.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/middleware.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/token.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/serialization/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/serialization/msgspec_hooks.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/static_files/base.py
--rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/static_files/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/base.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/file.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/memory.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/redis.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/template/__init__.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/template/base.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/template/config.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/__init__.py
--rw-r--r--   0        0        0    31457 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/transport.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/__init__.py
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/composite_types.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/empty.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/file_types.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/protocols.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/serialization.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/compat.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/deprecation.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/empty.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/helpers.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/module_loader.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/path.py
--rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/predicates.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/sequence.py
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/signature.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/sync.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/typing.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/warnings.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/scope/__init__.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/scope/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/__init__.py
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/conftest.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/docker-compose.yml
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/docker_service_fixtures.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/helpers.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/__init__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_advanced_alchemy.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_exception_handlers.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_option_requests.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_pydantic.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_regular_handler_under_asgi_mount_path.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_response_caching.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_router_registration.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_starlette_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_dependency_validation.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_classes.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_inter_dependencies.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_request_local_caching.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/__init__.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_request.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_response.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_before_request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_logging/__init__.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_logging/test_structlog_to_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_middleware/__init__.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_middleware/test_middleware_send_wrapper_called_on_error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_openapi/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_openapi/test_spec_headers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/conftest.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_asset_url_path.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_path_mounting.py
--rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_path_resolution.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_route_indexing.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_route_reverse.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/__init__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/conftest.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_cache_control_headers.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_exceptions.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_hello_world.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_lifecycle_hooks.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_request_data.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_routing.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_signature_namespace.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_startup_and_shutdown.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_static_files.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_stores.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_todo_app.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_using_session_auth.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_application_after_exception_hook.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_application_before_send.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_lifespan_manager.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_on_app_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_passing_initial_state.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_using_application_state.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_using_custom_state.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_using_immutable_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/__init__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_piccolo_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/conftest.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_defining_dtos_on_layers.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_overriding_implicit_return_dto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_problem_statement.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_usage.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private_override.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_type_checking.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_validation_error.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dto/__init__.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dto/test_example_apps.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dto/test_tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/__init__.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_abstract_middleware.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_call_order.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_session_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_openapi/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_openapi/test_openapi.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_openapi/test_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/test_using_classic_pagination.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/test_using_cursor_pagination.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/test_using_offset_pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_header_and_cookies_parameters.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_layered_parameters.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_path_parameters.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_query_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/test_di_plugin.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/test_example_apps.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_background_tasks.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_custom_responses.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_json_suffix_responses.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_response_cookies.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_response_headers.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_returning_responses.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_sse_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/test_engine_instance.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/test_returning_templates.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/test_template_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/conftest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/piccolo_conf.py
--rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_app.py
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_asgi_router.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_background_tasks.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_concurrency.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_controller.py
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_data_extractors.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_deprecations.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_di.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_events.py
--rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_file_system.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_guards.py
--rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_pagination.py
--rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_params.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_parsers.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_request_class_resolution.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response_class_resolution.py
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_stores.py
--rw-r--r--   0        0        0    17777 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_typing.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_websocket_class_resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/__init__.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/conftest.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/test_backends.py
--rw-r--r--   0        0        0    16494 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/test_plugin.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/test_subscriber.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/util.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/conftest.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_cli.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_cli_plugin.py
--rw-r--r--   0        0        0    23082 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_core_commands.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_env_resolution.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_schema_commands.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_session_commands.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_ssl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_base.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_connection_caching.py
--rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_request.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/conftest.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_minijinja.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_msgspec.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_opentelemetry.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_prometheus.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_repository.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_htmx/__init__.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_request.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_response.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/tables.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/conftest.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/models.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_dto.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
--rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_integration.py
--rw-r--r--   0        0        0    29635 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_openapi.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/__init_.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_cookie.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_headers.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_multi_dicts.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_response_header.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_state.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_upload_file.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_url.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/__init__.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/conftest.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_config.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_integration.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_interface.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/__init__.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_base_dto.py
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_dataclass_dto.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_field.py
--rw-r--r--   0        0        0    33747 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_integration.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/conftest.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_backends.py
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/__init__.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_opt.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_resolution.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_defaults.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_delete.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_head.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_media_type.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_sync.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/__init__.py
--rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/flower.jpeg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_cleanup_group.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_cookie_params.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_defaults.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_dependency_batches.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_generator_dependencies.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_header_params.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_json_data.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_layered_params.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_msgpack_data.py
--rw-r--r--   0        0        0    22582 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_multipart_data.py
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_path_params.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_query_params.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_url_encoded_data.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_logging/__init__.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_logging/test_logging_config.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_logging/test_structlog_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/__init__.py
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_allowed_hosts_middleware.py
--rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_base_authentication_middleware.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_base_middleware.py
--rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_compression_middleware.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_cors_middleware.py
--rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_csrf_middleware.py
--rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_exception_handler_middleware.py
--rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_middleware_handling.py
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/conftest.py
--rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_client_side_backend.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_integration.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_middleware.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_server_side_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/__init__.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/conftest.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_constrained_fields.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_datastructures.py
--rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_endpoints.py
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_integration.py
--rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_parameters.py
--rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_path_item.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_render_plugins.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_request_body.py
--rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_responses.py
--rw-r--r--   0        0        0    22895 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_schema.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_security_schemes.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_spec_generation.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_tags.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/__init__.py
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_converter.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/__init__.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/test_base.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/test_flash.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/models_bigint.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/models_uuid.py
--rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/test_generic_mock_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/__init__.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_base_response.py
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_file_response.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_redirect_response.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_response_cookies.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_response_headers.py
--rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_response_to_asgi_response.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_serialization.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_sse.py
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_streaming_response.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_type_decoders.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_type_encoders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/__init__.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_security.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_session_auth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/test_auth.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/test_integration.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_signature/__init__.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_signature/test_parsing.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_signature/test_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/conftest.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_create_static_router.py
--rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_file_serving_resolution.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_html_mode.py
--rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_static_files_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/__init__.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_built_in.py
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_builtin_functions.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_config.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_context.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_csrf_token.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/test_lifespan_handler.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/test_request_factory.py
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_types/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_types/test_protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_compat.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_dataclass.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_deprecation.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_helpers.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_module_loader.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_path.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_predicates.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_scope.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_sequence.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_signature.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_sync.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_typing.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_version.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 litestar-2.8.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.8.3/LICENSE
--rw-r--r--   0        0        0    93354 2020-02-02 00:00:00.000000 litestar-2.8.3/README.md
--rw-r--r--   0        0        0    12992 2020-02-02 00:00:00.000000 litestar-2.8.3/pyproject.toml
--rw-r--r--   0        0        0    99274 2020-02-02 00:00:00.000000 litestar-2.8.3/PKG-INFO
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 litestar-2.9.0/Makefile
+-rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 litestar-2.9.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/__main__.py
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_multipart.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_parsers.py
+-rw-r--r--   0        0        0    39463 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/app.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/background_tasks.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/concurrency.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/constants.py
+-rw-r--r--   0        0        0    12322 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/controller.py
+-rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/data_extractors.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/di.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/enums.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/file_system.py
+-rw-r--r--   0        0        0    11381 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/pagination.py
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/py.typed
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/router.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/status_codes.py
+-rw-r--r--   0        0        0    25806 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/typing.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_layers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/datastructures.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/plugin.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    25741 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/plugins/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/plugins/dataclass.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/plugins/pagination.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/plugins/struct.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/schema_generation/plugins/typed_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    11963 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_signature/model.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_signature/types.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/_signature/utils.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/__init__.py
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/asyncpg.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/psycopg.py
+-rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    20276 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/_utils.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/app.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/connection/base.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/connection/request.py
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/connection/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/mako.py
+-rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/minijinja.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/minijnja.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/config.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/pydantic_di_plugin.py
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0    13057 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/pydantic/utils.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/repository/testing.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/secret_values.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/datastructures/url.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    34446 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/_backend.py
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/_codegen_backend.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/_types.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/base_dto.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/config.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/dataclass_dto.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/field.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/msgspec_dto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/dto/types.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/events/emitter.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/responses/__init__.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/responses/_debug_response.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/responses/templates/body.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/responses/templates/frame.html
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/responses/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/exceptions/responses/templates/styles.css
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    66152 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    18726 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/logging/picologging.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/base.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/response_cache.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/_internal/__init__.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/_internal/cors.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/_internal/exceptions/__init__.py
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/_internal/exceptions/middleware.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/compression/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/compression/brotli_facade.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/compression/facade.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/compression/gzip_facade.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/compression/middleware.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/config.py
+-rw-r--r--   0        0        0    23353 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/plugins.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/plugins/__init__.py
+-rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/plugins/base.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/plugins/core.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/plugins/flash.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/plugins/sqlalchemy.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/plugins/structlog.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/_exceptions.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/_filters.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/exceptions.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/filters.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/handlers.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/abc/__init__.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/abc/_async.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/abc/_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/testing/__init__.py
+-rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/__init__.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/base.py
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/file.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/sse.py
+-rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/streaming.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/response/template.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/routes/base.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/routes/http.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/base.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/jwt/__init__.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/jwt/auth.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/jwt/middleware.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/jwt/token.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/static_files/base.py
+-rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/static_files/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/stores/base.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/stores/file.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/stores/memory.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/template/__init__.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/template/base.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/__init__.py
+-rw-r--r--   0        0        0    31409 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    23057 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    20203 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/empty.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/file_types.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/types/serialization.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/empty.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/helpers.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/module_loader.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/path.py
+-rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/predicates.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/signature.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/sync.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/warnings.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/scope/__init__.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 litestar-2.9.0/litestar/utils/scope/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/docker_service_fixtures.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/helpers.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/__init__.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_advanced_alchemy.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_option_requests.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_pydantic.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_regular_handler_under_asgi_mount_path.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_response_caching.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_router_registration.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_starlette_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/__init__.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_allowed_headers.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_allowed_methods.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_credentials.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_for_middleware_exception.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_for_mount.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_for_routing_exception.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_cors_origins.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_custom_options_handlers.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_cors/test_non_cors_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_dependency_validation.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_injection_of_classes.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_inter_dependencies.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_request_local_caching.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_exception_handlers/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_exception_handlers/test_exception_handler_registered_on_handler.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_exception_handlers/test_exception_handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_life_cycle_hooks/__init__.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_life_cycle_hooks/test_after_request.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_life_cycle_hooks/test_after_response.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_life_cycle_hooks/test_before_request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_logging/__init__.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_logging/test_structlog_to_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_middleware/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_middleware/test_exception_handler_applied_to_middleware_exception.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_middleware/test_exception_handler_called_from_mounted_app.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_middleware/test_exception_handler_called_if_no_middleware.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_middleware/test_logging_middleware_with_multi_body_response.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_middleware/test_middleware_send_wrapper_called_on_error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_openapi/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_openapi/test_spec_headers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/conftest.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/test_asset_url_path.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/test_path_mounting.py
+-rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/test_path_resolution.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/test_route_indexing.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/test_route_reverse.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/e2e/test_routing/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/__init__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/conftest.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_cache_control_headers.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_exceptions.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_hello_world.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_lifecycle_hooks.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_request_data.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_routing.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_signature_namespace.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_startup_and_shutdown.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_static_files.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_stores.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_todo_app.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_using_session_auth.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_hooks/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_hooks/test_application_after_exception_hook.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_hooks/test_application_before_send.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_hooks/test_lifespan_manager.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_hooks/test_on_app_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_state/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_state/test_passing_initial_state.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_state/test_using_application_state.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_state/test_using_custom_state.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_application_state/test_using_immutable_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/test_piccolo_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/test_sqlalchemy_examples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/conftest.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_defining_dtos_on_layers.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_overriding_implicit_return_dto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_problem_statement.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_usage.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private_override.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_type_checking.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_datastructures/__init__.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_datastructures/test_secrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dependency_injection/test_dependency_validation_error.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dto/__init__.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dto/test_example_apps.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_dto/test_tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_middleware/__init__.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_middleware/test_abstract_middleware.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_middleware/test_call_order.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_middleware/test_session_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_openapi/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_openapi/test_openapi.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_openapi/test_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_pagination/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_pagination/test_using_classic_pagination.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_pagination/test_using_cursor_pagination.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_pagination/test_using_offset_pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_parameters/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_parameters/test_header_and_cookies_parameters.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_parameters/test_layered_parameters.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_parameters/test_path_parameters.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_parameters/test_query_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_plugins/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_plugins/test_di_plugin.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_plugins/test_example_apps.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_background_tasks.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_custom_responses.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_json_suffix_responses.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_response_cookies.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_response_headers.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_returning_responses.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_responses/test_sse_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_security/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_templating/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_templating/test_engine_instance.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_templating/test_returning_templates.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/examples/test_templating/test_template_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/piccolo_conf.py
+-rw-r--r--   0        0        0    15370 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_app.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_background_tasks.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_concurrency.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_controller.py
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_data_extractors.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_deprecations.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_di.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_events.py
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_file_system.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_guards.py
+-rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_pagination.py
+-rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_params.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_parsers.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_request_class_resolution.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response_class_resolution.py
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_stores.py
+-rw-r--r--   0        0        0    17777 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_typing.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_websocket_class_resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_asgi/__init__.py
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_asgi/test_asgi_router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_asgi/test_routing_trie/__init__.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_asgi/test_routing_trie/test_mapping.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_asgi/test_routing_trie/test_traversal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_channels/__init__.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_channels/conftest.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_channels/test_backends.py
+-rw-r--r--   0        0        0    16494 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_channels/test_plugin.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_channels/test_subscriber.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_channels/util.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/conftest.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_cli.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_cli_plugin.py
+-rw-r--r--   0        0        0    23082 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_core_commands.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_env_resolution.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_schema_commands.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_session_commands.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_cli/test_ssl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_connection/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_connection/test_base.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_connection/test_connection_caching.py
+-rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_connection/test_request.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_connection/test_websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/conftest.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_minijinja.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_msgspec.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_opentelemetry.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_prometheus.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_repository.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_attrs/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_htmx/__init__.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_htmx/test_htmx_request.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_htmx/test_htmx_response.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/tables.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/conftest.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/models.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_dto.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
+-rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_integration.py
+-rw-r--r--   0        0        0    29635 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_openapi.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/__init_.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_cookie.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_headers.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_multi_dicts.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_response_header.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_secret_values.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_state.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_upload_file.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_datastructures/test_url.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/__init__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/conftest.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_config.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_integration.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_interface.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/__init__.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_base_dto.py
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_dataclass_dto.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_field.py
+-rw-r--r--   0        0        0    35049 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_integration.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/conftest.py
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/test_backends.py
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/__init__.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/test_opt.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/test_resolution.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_defaults.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_delete.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_deprecation.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_head.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_media_type.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_sync.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/__init__.py
+-rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/flower.jpeg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_cleanup_group.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_cookie_params.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_defaults.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_dependency_batches.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_generator_dependencies.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_header_params.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_json_data.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_layered_params.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_msgpack_data.py
+-rw-r--r--   0        0        0    22582 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_multipart_data.py
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_path_params.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_query_params.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_url_encoded_data.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_kwargs/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_logging/__init__.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_logging/test_logging_config.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_logging/test_structlog_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/__init__.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_allowed_hosts_middleware.py
+-rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_base_authentication_middleware.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_base_middleware.py
+-rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_compression_middleware.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_cors_middleware.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_csrf_middleware.py
+-rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_exception_handler_middleware.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_middleware_handling.py
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_session/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_session/conftest.py
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_session/test_client_side_backend.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_session/test_integration.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_session/test_middleware.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_middleware/test_session/test_server_side_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/__init__.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/conftest.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_constrained_fields.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_datastructures.py
+-rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_endpoints.py
+-rw-r--r--   0        0        0    21215 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_integration.py
+-rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_parameters.py
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_path_item.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_render_plugins.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_request_body.py
+-rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_responses.py
+-rw-r--r--   0        0        0    22895 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_schema.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_security_schemes.py
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_spec_generation.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_tags.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/__init__.py
+-rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/test_converter.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_plugins/__init__.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_plugins/test_base.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_plugins/test_flash.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_plugins/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_repository/__init__.py
+-rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_repository/models_bigint.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_repository/models_uuid.py
+-rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_repository/test_generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/__init__.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_base_response.py
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_file_response.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_redirect_response.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_response_cookies.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_response_headers.py
+-rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_response_to_asgi_response.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_serialization.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_sse.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_streaming_response.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_type_decoders.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_response/test_type_encoders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/__init__.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/test_security.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/test_session_auth.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/test_jwt/test_auth.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/test_jwt/test_integration.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_security/test_jwt/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_signature/__init__.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_signature/test_parsing.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_signature/test_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_static_files/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_static_files/conftest.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_static_files/test_create_static_router.py
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_static_files/test_file_serving_resolution.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_static_files/test_html_mode.py
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_static_files/test_static_files_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/__init__.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/test_built_in.py
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/test_builtin_functions.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/test_config.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/test_context.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/test_csrf_token.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_template/test_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_testing/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_testing/test_lifespan_handler.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_testing/test_request_factory.py
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_testing/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_types/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_types/test_protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_compat.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_dataclass.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_deprecation.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_empty.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_helpers.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_module_loader.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_path.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_predicates.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_scope.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_sequence.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_signature.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_sync.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_typing.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.9.0/tests/unit/test_utils/test_version.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 litestar-2.9.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.9.0/LICENSE
+-rw-r--r--   0        0        0    94686 2020-02-02 00:00:00.000000 litestar-2.9.0/README.md
+-rw-r--r--   0        0        0    13182 2020-02-02 00:00:00.000000 litestar-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0   100577 2020-02-02 00:00:00.000000 litestar-2.9.0/PKG-INFO
```

### Comparing `litestar-2.8.3/Makefile` & `litestar-2.9.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 docs-clean: 										## Dump the existing built docs
 	@echo "=> Cleaning documentation build assets"
 	@rm -rf docs/_build
 	@echo "=> Removed existing documentation build assets"
 
 docs-serve: docs-clean 								## Serve the docs locally
 	@echo "=> Serving documentation"
-	$(PDM) run sphinx-autobuild docs docs/_build/ -j auto --watch polyfactory --watch docs --watch tests --watch CONTRIBUTING.rst --port 8002
+	$(PDM) run sphinx-autobuild docs docs/_build/ -j auto --watch litestar --watch docs --watch tests --watch CONTRIBUTING.rst --port 8002
 
 docs: docs-clean 									## Dump the existing built docs and rebuild them
 	@echo "=> Building documentation"
 	@$(PDM) run sphinx-build -M html docs docs/_build/ -E -a -j auto -W --keep-going
 
 .PHONY: docs-linkcheck
 docs-linkcheck: 									## Run the link check on the docs
```

### Comparing `litestar-2.8.3/docs/PYPI_README.md` & `litestar-2.9.0/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/__init__.py` & `litestar-2.9.0/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_multipart.py` & `litestar-2.9.0/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_parsers.py` & `litestar-2.9.0/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/app.py` & `litestar-2.9.0/litestar/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from litestar.events.emitter import BaseEventEmitterBackend, SimpleEventEmitter
 from litestar.exceptions import (
     LitestarWarning,
     MissingDependencyException,
     NoRouteMatchFoundException,
 )
 from litestar.logging.config import LoggingConfig, get_logger_placeholder
-from litestar.middleware.cors import CORSMiddleware
+from litestar.middleware._internal.cors import CORSMiddleware
 from litestar.openapi.config import OpenAPIConfig
 from litestar.plugins import (
     CLIPluginProtocol,
     InitPluginProtocol,
     OpenAPISchemaPluginProtocol,
     PluginProtocol,
     PluginRegistry,
@@ -241,15 +241,15 @@
             before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
                 when the ASGI send function is called.
             cache_control: A ``cache-control`` header of type
                 :class:`CacheControlHeader <litestar.datastructures.CacheControlHeader>` to add to route handlers of
                 this app. Can be overridden by route handlers.
             compression_config: Configures compression behaviour of the application, this enabled a builtin or user
                 defined Compression middleware.
-            cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
+            cors_config: If set, configures CORS handling for the application.
             csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
             debug: If ``True``, app errors rendered as HTML with a stack trace.
             dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
             dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
                 validation of request data.
             etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
                 Can be overridden by route handlers.
@@ -408,15 +408,14 @@
                 category=LitestarWarning,
                 stacklevel=2,
             )
 
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
-        self.asgi_router = ASGIRouter(app=self)
 
         self.after_exception = [ensure_async_callable(h) for h in config.after_exception]
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
         self.before_send = [ensure_async_callable(h) for h in config.before_send]
         self.compression_config = config.compression_config
         self.cors_config = config.cors_config
         self.csrf_config = config.csrf_config
@@ -438,15 +437,15 @@
 
         if self.pdb_on_exception:
             warn_pdb_on_exception()
 
         try:
             from starlette.exceptions import HTTPException as StarletteHTTPException
 
-            from litestar.middleware.exceptions.middleware import _starlette_exception_handler
+            from litestar.middleware._internal.exceptions.middleware import _starlette_exception_handler
 
             config.exception_handlers.setdefault(StarletteHTTPException, _starlette_exception_handler)
         except ImportError:
             pass
 
         super().__init__(
             after_request=config.after_request,
@@ -475,14 +474,16 @@
             tags=config.tags,
             type_encoders=config.type_encoders,
             type_decoders=config.type_decoders,
             include_in_schema=config.include_in_schema,
             websocket_class=self.websocket_class,
         )
 
+        self.asgi_router = ASGIRouter(app=self)
+
         for route_handler in config.route_handlers:
             self.register(route_handler)
 
         if self.logging_config:
             self.get_logger = self.logging_config.configure()
             self.logger = self.get_logger("litestar")
 
@@ -835,22 +836,20 @@
         return route_map
 
     def _create_asgi_handler(self) -> ASGIApp:
         """Create an ASGIApp that wraps the ASGI router inside an exception handler.
 
         If CORS or TrustedHost configs are provided to the constructor, they will wrap the router as well.
         """
-        asgi_handler: ASGIApp = self.asgi_router
+        asgi_handler = wrap_in_exception_handler(app=self.asgi_router)
+
         if self.cors_config:
-            asgi_handler = CORSMiddleware(app=asgi_handler, config=self.cors_config)
+            return CORSMiddleware(app=asgi_handler, config=self.cors_config)
 
-        return wrap_in_exception_handler(
-            app=asgi_handler,
-            exception_handlers=self.exception_handlers or {},  # pyright: ignore
-        )
+        return asgi_handler
 
     def _wrap_send(self, send: Send, scope: Scope) -> Send:
         """Wrap the ASGI send and handles any 'before send' hooks.
 
         Args:
             send: The ASGI send function.
             scope: The ASGI scope.
```

### Comparing `litestar-2.8.3/litestar/background_tasks.py` & `litestar-2.9.0/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/concurrency.py` & `litestar-2.9.0/litestar/concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/constants.py` & `litestar-2.9.0/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/controller.py` & `litestar-2.9.0/litestar/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.base import BaseRouteHandler
 from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.handlers.websocket_handlers import WebsocketRouteHandler
 from litestar.types.empty import Empty
-from litestar.utils import ensure_async_callable, normalize_path
+from litestar.utils import normalize_path
 from litestar.utils.signature import add_types_to_signature_namespace
 
 __all__ = ("Controller",)
 
 
 if TYPE_CHECKING:
     from litestar.connection import Request, WebSocket
@@ -47,14 +47,15 @@
     Subclass this class to create 'view' like components and utilize OOP.
     """
 
     __slots__ = (
         "after_request",
         "after_response",
         "before_request",
+        "cache_control",
         "dependencies",
         "dto",
         "etag",
         "exception_handlers",
         "guards",
         "include_in_schema",
         "middleware",
@@ -65,14 +66,15 @@
         "request_class",
         "response_class",
         "response_cookies",
         "response_headers",
         "return_dto",
         "security",
         "signature_namespace",
+        "signature_types",
         "tags",
         "type_encoders",
         "type_decoders",
         "websocket_class",
     )
 
     after_request: AfterRequestHookHandler | None
@@ -170,20 +172,19 @@
         """Initialize a controller.
 
         Should only be called by routers as part of controller registration.
 
         Args:
             owner: An instance of :class:`Router <.router.Router>`
         """
-        # Since functions set on classes are bound, we need replace the bound instance with the class version and wrap
-        # it to ensure it does not get bound.
+        # Since functions set on classes are bound, we need replace the bound instance with the class version
         for key in ("after_request", "after_response", "before_request"):
             cls_value = getattr(type(self), key, None)
             if callable(cls_value):
-                setattr(self, key, ensure_async_callable(cls_value))
+                setattr(self, key, cls_value)
 
         if not hasattr(self, "dto"):
             self.dto = Empty
 
         if not hasattr(self, "return_dto"):
             self.return_dto = Empty
 
@@ -199,14 +200,49 @@
                 setattr(self, key, None)
 
         self.response_cookies = narrow_response_cookies(self.response_cookies)
         self.response_headers = narrow_response_headers(self.response_headers)
         self.path = normalize_path(self.path or "/")
         self.owner = owner
 
+    def as_router(self) -> Router:
+        from litestar.router import Router
+
+        router = Router(
+            path=self.path,
+            route_handlers=self.get_route_handlers(),
+            after_request=self.after_request,
+            after_response=self.after_response,
+            before_request=self.before_request,
+            cache_control=self.cache_control,
+            dependencies=self.dependencies,
+            dto=self.dto,
+            etag=self.etag,
+            exception_handlers=self.exception_handlers,
+            guards=self.guards,
+            include_in_schema=self.include_in_schema,
+            middleware=self.middleware,
+            opt=self.opt,
+            parameters=self.parameters,
+            request_class=self.request_class,
+            response_class=self.response_class,
+            response_cookies=self.response_cookies,
+            response_headers=self.response_headers,
+            return_dto=self.return_dto,
+            security=self.security,
+            signature_types=self.signature_types,
+            signature_namespace=self.signature_namespace,
+            tags=self.tags,
+            type_encoders=self.type_encoders,
+            type_decoders=self.type_decoders,
+            websocket_class=self.websocket_class,
+        )
+        router.owner = self.owner
+        return router
+
     def get_route_handlers(self) -> list[BaseRouteHandler]:
         """Get a controller's route handlers and set the controller as the handlers' owner.
 
         Returns:
             A list containing a copy of the route handlers defined on the controller
         """
```

### Comparing `litestar-2.8.3/litestar/data_extractors.py` & `litestar-2.9.0/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/di.py` & `litestar-2.9.0/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/enums.py` & `litestar-2.9.0/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/file_system.py` & `litestar-2.9.0/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/pagination.py` & `litestar-2.9.0/litestar/pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,31 +35,39 @@
     """Number of items per page."""
     current_page: int
     """Current page number."""
     total_pages: int
     """Total number of pages."""
 
 
-@dataclass
-class OffsetPagination(Generic[T]):
-    """Container for data returned using limit/offset pagination."""
-
-    __slots__ = ("items", "limit", "offset", "total")
-
-    items: List[T]
-    """List of data being sent as part of the response."""
-    limit: int
-    """Maximal number of items to send."""
-    offset: int
-    """Offset from the beginning of the query.
-
-    Identical to an index.
-    """
-    total: int
-    """Total number of items."""
+# AA requires it's own `OffsetPagination` class in versions greater that 0.9.0
+# If we find it, use it.
+try:
+    from advanced_alchemy.service import (
+        OffsetPagination,  # pyright: ignore[reportMissingImports,reportGeneralTypeIssues]
+    )
+except ImportError:
+
+    @dataclass
+    class OffsetPagination(Generic[T]):  # type: ignore[no-redef]
+        """Container for data returned using limit/offset pagination."""
+
+        __slots__ = ("items", "limit", "offset", "total")
+
+        items: List[T]
+        """List of data being sent as part of the response."""
+        limit: int
+        """Maximal number of items to send."""
+        offset: int
+        """Offset from the beginning of the query.
+
+        Identical to an index.
+        """
+        total: int
+        """Total number of items."""
 
 
 @dataclass
 class CursorPagination(Generic[C, T]):
     """Container for data returned using cursor pagination."""
 
     __slots__ = ("items", "results_per_page", "cursor", "next_cursor")
```

### Comparing `litestar-2.8.3/litestar/params.py` & `litestar-2.9.0/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/router.py` & `litestar-2.9.0/litestar/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -276,48 +276,33 @@
                 )
 
         return route_map
 
     @classmethod
     def get_route_handler_map(
         cls,
-        value: Controller | RouteHandlerType | Router,
+        value: RouteHandlerType | Router,
     ) -> dict[str, RouteHandlerMapItem]:
         """Map route handlers to HTTP methods."""
         if isinstance(value, Router):
             return value.route_handler_method_map
 
-        if isinstance(value, (HTTPRouteHandler, ASGIRouteHandler, WebsocketRouteHandler)):
-            copied_value = copy(value)
-            if isinstance(value, HTTPRouteHandler):
-                return {path: {http_method: copied_value for http_method in value.http_methods} for path in value.paths}
-
-            return {
-                path: {"websocket" if isinstance(value, WebsocketRouteHandler) else "asgi": copied_value}
-                for path in value.paths
-            }
-
-        handlers_map: defaultdict[str, RouteHandlerMapItem] = defaultdict(dict)
-        for route_handler in value.get_route_handlers():
-            for handler_path in route_handler.paths:
-                path = join_paths([value.path, handler_path]) if handler_path else value.path
-                if isinstance(route_handler, HTTPRouteHandler):
-                    for http_method in route_handler.http_methods:
-                        handlers_map[path][http_method] = route_handler
-                else:
-                    handlers_map[path]["websocket" if isinstance(route_handler, WebsocketRouteHandler) else "asgi"] = (
-                        cast("WebsocketRouteHandler | ASGIRouteHandler", route_handler)
-                    )
+        copied_value = copy(value)
+        if isinstance(value, HTTPRouteHandler):
+            return {path: {http_method: copied_value for http_method in value.http_methods} for path in value.paths}
+
+        return {
+            path: {"websocket" if isinstance(value, WebsocketRouteHandler) else "asgi": copied_value}
+            for path in value.paths
+        }
 
-        return handlers_map
-
-    def _validate_registration_value(self, value: ControllerRouterHandler) -> Controller | RouteHandlerType | Router:
+    def _validate_registration_value(self, value: ControllerRouterHandler) -> RouteHandlerType | Router:
         """Ensure values passed to the register method are supported."""
         if is_class_and_subclass(value, Controller):
-            return value(owner=self)
+            return value(owner=self).as_router()
 
         # this narrows down to an ABC, but we assume a non-abstract subclass of the ABC superclass
         if is_class_and_subclass(value, WebsocketListener):
             return value(owner=self).to_handler()  # pyright: ignore
 
         if isinstance(value, Router):
             if value is self:
```

### Comparing `litestar-2.8.3/litestar/status_codes.py` & `litestar-2.9.0/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/typing.py` & `litestar-2.9.0/litestar/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_asgi/asgi_router.py` & `litestar-2.9.0/litestar/_asgi/asgi_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,46 +9,48 @@
 from litestar._asgi.routing_trie import validate_node
 from litestar._asgi.routing_trie.mapping import add_route_to_trie
 from litestar._asgi.routing_trie.traversal import parse_path_to_route
 from litestar._asgi.routing_trie.types import create_node
 from litestar._asgi.utils import get_route_handlers
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.utils import normalize_path
-
-__all__ = ("ASGIRouter",)
-
+from litestar.utils.scope.state import ScopeState
 
 if TYPE_CHECKING:
     from litestar._asgi.routing_trie.types import RouteTrieNode
     from litestar.app import Litestar
     from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
     from litestar.routes.base import BaseRoute
     from litestar.types import (
         ASGIApp,
+        ExceptionHandlersMap,
         LifeSpanReceive,
         LifeSpanSend,
         LifeSpanShutdownCompleteEvent,
         LifeSpanShutdownFailedEvent,
         LifeSpanStartupCompleteEvent,
         LifeSpanStartupFailedEvent,
         Method,
         Receive,
         RouteHandlerType,
         Scope,
         Send,
     )
 
+__all__ = ("ASGIRouter",)
+
 
 class ASGIRouter:
     """Litestar ASGI router.
 
     Handling both the ASGI lifespan events and routing of connection requests.
     """
 
     __slots__ = (
+        "_app_exception_handlers",
         "_mount_paths_regex",
         "_mount_routes",
         "_plain_routes",
         "_registered_routes",
         "_static_routes",
         "app",
         "root_route_map_node",
@@ -58,14 +60,15 @@
 
     def __init__(self, app: Litestar) -> None:
         """Initialize ``ASGIRouter``.
 
         Args:
             app: The Litestar app instance
         """
+        self._app_exception_handlers: ExceptionHandlersMap = app.exception_handlers
         self._mount_paths_regex: Pattern | None = None
         self._mount_routes: dict[str, RouteTrieNode] = {}
         self._plain_routes: set[str] = set()
         self._registered_routes: set[HTTPRoute | WebSocketRoute | ASGIRoute] = set()
         self.app = app
         self.root_route_map_node: RouteTrieNode = create_node()
         self.route_handler_index: dict[str, RouteHandlerType] = {}
@@ -79,17 +82,24 @@
         scope.setdefault("path_params", {})
 
         path = scope["path"]
         if root_path := scope.get("root_path", ""):
             path = path.split(root_path, maxsplit=1)[-1]
         normalized_path = normalize_path(path)
 
-        asgi_app, scope["route_handler"], scope["path"], scope["path_params"] = self.handle_routing(
-            path=normalized_path, method=scope.get("method")
-        )
+        try:
+            asgi_app, route_handler, scope["path"], scope["path_params"] = self.handle_routing(
+                path=normalized_path, method=scope.get("method")
+            )
+        except Exception:
+            ScopeState.from_scope(scope).exception_handlers = self._app_exception_handlers
+            raise
+        else:
+            ScopeState.from_scope(scope).exception_handlers = route_handler.resolve_exception_handlers()
+            scope["route_handler"] = route_handler
         await asgi_app(scope, receive, send)
 
     @lru_cache(1024)  # noqa: B019
     def handle_routing(self, path: str, method: Method | None) -> tuple[ASGIApp, RouteHandlerType, str, dict[str, Any]]:
         """Handle routing for a given path / method combo. This method is meant to allow easy caching.
 
         Args:
```

### Comparing `litestar-2.8.3/litestar/_asgi/utils.py` & `litestar-2.9.0/litestar/_asgi/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
-__all__ = ("get_route_handlers", "wrap_in_exception_handler")
-
-
 if TYPE_CHECKING:
     from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
     from litestar.routes.base import BaseRoute
-    from litestar.types import ASGIApp, ExceptionHandlersMap, RouteHandlerType
+    from litestar.types import ASGIApp, RouteHandlerType
+
+__all__ = ("get_route_handlers", "wrap_in_exception_handler")
 
 
-def wrap_in_exception_handler(app: ASGIApp, exception_handlers: ExceptionHandlersMap) -> ASGIApp:
+def wrap_in_exception_handler(app: ASGIApp) -> ASGIApp:
     """Wrap the given ASGIApp in an instance of ExceptionHandlerMiddleware.
 
     Args:
         app: The ASGI app that is being wrapped.
-        exception_handlers: A mapping of exceptions to handler functions.
 
     Returns:
         A wrapped ASGIApp.
     """
-    from litestar.middleware.exceptions import ExceptionHandlerMiddleware
+    from litestar.middleware._internal.exceptions import ExceptionHandlerMiddleware
 
-    return ExceptionHandlerMiddleware(app=app, exception_handlers=exception_handlers, debug=None)
+    return ExceptionHandlerMiddleware(app=app, debug=None)
 
 
 def get_route_handlers(route: BaseRoute) -> list[RouteHandlerType]:
     """Retrieve handler(s) as a list for given route.
 
     Args:
         route: The route from which the route handlers are extracted.
```

### Comparing `litestar-2.8.3/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.9.0/litestar/_asgi/routing_trie/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -185,37 +185,40 @@
     """
     from litestar.middleware.allowed_hosts import AllowedHostsMiddleware
     from litestar.middleware.compression import CompressionMiddleware
     from litestar.middleware.csrf import CSRFMiddleware
     from litestar.middleware.response_cache import ResponseCacheMiddleware
     from litestar.routes import HTTPRoute
 
-    # we wrap the route.handle method in the ExceptionHandlerMiddleware
-    asgi_handler = wrap_in_exception_handler(
-        app=route.handle,  # type: ignore[arg-type]
-        exception_handlers=route_handler.resolve_exception_handlers(),
+    asgi_handler: ASGIApp = route.handle  # type: ignore[assignment]
+    handler_middleware = route_handler.resolve_middleware()
+    has_cached_route = isinstance(route, HTTPRoute) and any(r.cache for r in route.route_handlers)
+    has_middleware = (
+        app.csrf_config or app.compression_config or has_cached_route or app.allowed_hosts or handler_middleware
     )
 
-    if app.csrf_config:
-        asgi_handler = CSRFMiddleware(app=asgi_handler, config=app.csrf_config)
-
-    if app.compression_config:
-        asgi_handler = CompressionMiddleware(app=asgi_handler, config=app.compression_config)
-
-    if isinstance(route, HTTPRoute) and any(r.cache for r in route.route_handlers):
-        asgi_handler = ResponseCacheMiddleware(app=asgi_handler, config=app.response_cache_config)
-
-    if app.allowed_hosts:
-        asgi_handler = AllowedHostsMiddleware(app=asgi_handler, config=app.allowed_hosts)
-
-    for middleware in route_handler.resolve_middleware():
-        if hasattr(middleware, "__iter__"):
-            handler, kwargs = cast("tuple[Any, dict[str, Any]]", middleware)
-            asgi_handler = handler(app=asgi_handler, **kwargs)
-        else:
-            asgi_handler = middleware(app=asgi_handler)  # type: ignore[call-arg]
-
-    # we wrap the entire stack again in ExceptionHandlerMiddleware
-    return wrap_in_exception_handler(
-        app=cast("ASGIApp", asgi_handler),
-        exception_handlers=route_handler.resolve_exception_handlers(),
-    )  # pyright: ignore
+    if has_middleware:
+        # If there is an exception raised from the handler, the first ExceptionHandlerMiddleware that catches the
+        # exception will create the response and call send(). As middleware may wrap the send() callable, we need there
+        # to be an instance of ExceptionHandlerMiddleware in between the handler and the middleware so that any send
+        # wrappers instated by middleware are called. If there is no middleware, we can skip this step.
+        asgi_handler = wrap_in_exception_handler(app=asgi_handler)
+
+        if app.csrf_config:
+            asgi_handler = CSRFMiddleware(app=asgi_handler, config=app.csrf_config)
+
+        if app.compression_config:
+            asgi_handler = CompressionMiddleware(app=asgi_handler, config=app.compression_config)
+
+        if has_cached_route:
+            asgi_handler = ResponseCacheMiddleware(app=asgi_handler, config=app.response_cache_config)
+
+        if app.allowed_hosts:
+            asgi_handler = AllowedHostsMiddleware(app=asgi_handler, config=app.allowed_hosts)
+
+        for middleware in handler_middleware:
+            if hasattr(middleware, "__iter__"):
+                handler, kwargs = cast("tuple[Any, dict[str, Any]]", middleware)
+                asgi_handler = handler(app=asgi_handler, **kwargs)
+            else:
+                asgi_handler = middleware(app=asgi_handler)  # type: ignore[call-arg]
+    return asgi_handler
```

### Comparing `litestar-2.8.3/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.9.0/litestar/_asgi/routing_trie/traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,16 @@
     """
 
     try:
         if path in plain_routes:
             asgi_app, handler = parse_node_handlers(node=root_node.children[path], method=method)
             return asgi_app, handler, path, {}
 
-        if mount_paths_regex and (match := mount_paths_regex.search(path)):
-            mount_path = path[match.start() : match.end()]
+        if mount_paths_regex and (match := mount_paths_regex.match(path)):
+            mount_path = path[: match.end()]
             mount_node = mount_routes[mount_path]
             remaining_path = path[match.end() :]
             # since we allow regular handlers under static paths, we must validate that the request does not match
             # any such handler.
             children = (
                 normalize_path(sub_route)
                 for sub_route in mount_node.children or []
```

### Comparing `litestar-2.8.3/litestar/_asgi/routing_trie/types.py` & `litestar-2.9.0/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_asgi/routing_trie/validate.py` & `litestar-2.9.0/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_kwargs/cleanup.py` & `litestar-2.9.0/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_kwargs/dependencies.py` & `litestar-2.9.0/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_kwargs/extractors.py` & `litestar-2.9.0/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_kwargs/kwargs_model.py` & `litestar-2.9.0/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_kwargs/parameter_definition.py` & `litestar-2.9.0/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_layers/utils.py` & `litestar-2.9.0/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/datastructures.py` & `litestar-2.9.0/litestar/_openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/parameters.py` & `litestar-2.9.0/litestar/_openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/path_item.py` & `litestar-2.9.0/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/plugin.py` & `litestar-2.9.0/litestar/_openapi/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/request_body.py` & `litestar-2.9.0/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/responses.py` & `litestar-2.9.0/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/utils.py` & `litestar-2.9.0/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/examples.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/schema.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from litestar._openapi.schema_generation.utils import (
     _get_normalized_schema_key,
     _should_create_enum_schema,
     _should_create_literal_schema,
     _type_or_first_not_none_inner_type,
     get_json_schema_formatted_examples,
 )
-from litestar.datastructures import UploadFile
+from litestar.datastructures import SecretBytes, SecretString, UploadFile
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema, SchemaDataContainer
 from litestar.params import BodyKwarg, KwargDefinition, ParameterKwarg
 from litestar.plugins import OpenAPISchemaPlugin
 from litestar.types import Empty
 from litestar.types.builtin_types import NoneType
@@ -110,14 +110,16 @@
     MutableMapping: Schema(type=OpenAPIType.OBJECT),
     MutableSequence: Schema(type=OpenAPIType.ARRAY),
     None: Schema(type=OpenAPIType.NULL),
     NoneType: Schema(type=OpenAPIType.NULL),
     OrderedDict: Schema(type=OpenAPIType.OBJECT),
     Path: Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.URI),
     Pattern: Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.REGEX),
+    SecretBytes: Schema(type=OpenAPIType.STRING),
+    SecretString: Schema(type=OpenAPIType.STRING),
     Sequence: Schema(type=OpenAPIType.ARRAY),
     Set: Schema(type=OpenAPIType.ARRAY),
     Tuple: Schema(type=OpenAPIType.ARRAY),
     UUID: Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.UUID),
     bool: Schema(type=OpenAPIType.BOOLEAN),
     bytearray: Schema(type=OpenAPIType.STRING),
     bytes: Schema(type=OpenAPIType.STRING),
```

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/utils.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/__init__.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/dataclass.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/plugins/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/pagination.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/plugins/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/struct.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/plugins/struct.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/typed_dict.py` & `litestar-2.9.0/litestar/_openapi/schema_generation/plugins/typed_dict.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.9.0/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.9.0/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_openapi/typescript_converter/types.py` & `litestar-2.9.0/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/_signature/model.py` & `litestar-2.9.0/litestar/_signature/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from litestar.datastructures.state import ImmutableState
 from litestar.datastructures.url import URL
 from litestar.dto import AbstractDTO, DTOData
 from litestar.enums import ParamType, ScopeType
 from litestar.exceptions import InternalServerException, ValidationException
 from litestar.params import KwargDefinition, ParameterKwarg
 from litestar.typing import FieldDefinition  # noqa
-from litestar.utils import is_class_and_subclass
+from litestar.utils import get_origin_or_inner_type, is_class_and_subclass
 from litestar.utils.dataclass import simple_asdict
 
 if TYPE_CHECKING:
     from typing_extensions import NotRequired
 
     from litestar.connection import ASGIConnection
     from litestar.types import AnyCallable, TypeDecodersSequence
@@ -81,16 +81,23 @@
 ]
 
 
 def _deserializer(target_type: Any, value: Any, default_deserializer: Callable[[Any, Any], Any]) -> Any:
     if isinstance(value, DTOData):
         return value
 
-    if isinstance(value, target_type):
-        return value
+    try:
+        if isinstance(value, target_type):
+            return value
+    except TypeError as exc:
+        if (origin := get_origin_or_inner_type(target_type)) is not None:
+            if isinstance(value, origin):
+                return value
+        else:
+            raise exc
 
     if decoder := getattr(target_type, "_decoder", None):
         return decoder(target_type, value)
 
     return default_deserializer(target_type, value)
```

### Comparing `litestar-2.8.3/litestar/_signature/utils.py` & `litestar-2.9.0/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/plugin.py` & `litestar-2.9.0/litestar/channels/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/subscriber.py` & `litestar-2.9.0/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/backends/asyncpg.py` & `litestar-2.9.0/litestar/channels/backends/asyncpg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/backends/base.py` & `litestar-2.9.0/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/backends/memory.py` & `litestar-2.9.0/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/backends/psycopg.py` & `litestar-2.9.0/litestar/channels/backends/psycopg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/channels/backends/redis.py` & `litestar-2.9.0/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/cli/__init__.py` & `litestar-2.9.0/litestar/cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from __future__ import annotations
 
 from importlib.util import find_spec
 
 # Ensure `rich_click` patching occurs before we do any imports from `click`.
 if find_spec("rich_click") is not None:  # pragma: no cover
     import rich_click as click
-    from rich_click.cli import patch as rich_click_patch
+
+    try:
+        from rich_click.patch import patch as rich_click_patch
+    except ImportError:
+        from rich_click.cli import patch as rich_click_patch
 
     rich_click_patch()
     click.rich_click.USE_RICH_MARKUP = True
     click.rich_click.USE_MARKDOWN = False
     click.rich_click.SHOW_ARGUMENTS = True
     click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
     click.rich_click.STYLE_ERRORS_SUGGESTION = "magenta italic"
```

### Comparing `litestar-2.8.3/litestar/cli/_utils.py` & `litestar-2.9.0/litestar/cli/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,16 +248,16 @@
         return func(*args, **kwargs)
 
     return pass_context(wrapped)
 
 
 def _wrap_commands(commands: Iterable[Command]) -> None:
     for command in commands:
-        if isinstance(command, Group):
-            _wrap_commands(command.commands.values())
+        if hasattr(command, "commands"):
+            _wrap_commands(command.commands.values())  # pyright: ignore[reportGeneralTypeIssues]
         elif command.callback:
             command.callback = _inject_args(command.callback)
 
 
 def _bool_from_env(key: str, default: bool = False) -> bool:
     value = getenv(key)
     if not value:
```

### Comparing `litestar-2.8.3/litestar/cli/main.py` & `litestar-2.9.0/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/cli/commands/core.py` & `litestar-2.9.0/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/cli/commands/schema.py` & `litestar-2.9.0/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/cli/commands/sessions.py` & `litestar-2.9.0/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/config/allowed_hosts.py` & `litestar-2.9.0/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/config/app.py` & `litestar-2.9.0/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/config/compression.py` & `litestar-2.9.0/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/config/cors.py` & `litestar-2.9.0/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/config/csrf.py` & `litestar-2.9.0/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/config/response_cache.py` & `litestar-2.9.0/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/connection/__init__.py` & `litestar-2.9.0/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/connection/base.py` & `litestar-2.9.0/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/connection/request.py` & `litestar-2.9.0/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/connection/websocket.py` & `litestar-2.9.0/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/jinja.py` & `litestar-2.9.0/litestar/contrib/jinja.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         """Jinja-based TemplateEngine.
 
         Args:
             directory: Direct path or list of directory paths from which to serve templates.
             engine_instance: A jinja Environment instance.
         """
 
-        super().__init__(directory, engine_instance)
         if directory and engine_instance:
             raise ImproperlyConfiguredException("You must provide either a directory or a jinja2 Environment instance.")
         if directory:
             loader = FileSystemLoader(searchpath=directory)
             self.engine = Environment(loader=loader, autoescape=True)
         elif engine_instance:
             self.engine = engine_instance
```

### Comparing `litestar-2.8.3/litestar/contrib/mako.py` & `litestar-2.9.0/litestar/contrib/mako.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     def __init__(self, directory: Path | list[Path] | None = None, engine_instance: Any | None = None) -> None:
         """Initialize template engine.
 
         Args:
             directory: Direct path or list of directory paths from which to serve templates.
             engine_instance: A mako TemplateLookup instance.
         """
-        super().__init__(directory, engine_instance)
         if directory and engine_instance:
             raise ImproperlyConfiguredException("You must provide either a directory or a mako TemplateLookup.")
         if directory:
             self.engine = TemplateLookup(
                 directories=directory if isinstance(directory, (list, tuple)) else [directory], default_filters=["h"]
             )
         elif engine_instance:
```

### Comparing `litestar-2.8.3/litestar/contrib/minijinja.py` & `litestar-2.9.0/litestar/contrib/minijinja.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
     def __init__(self, directory: Path | list[Path] | None = None, engine_instance: Environment | None = None) -> None:
         """Minijinja based TemplateEngine.
 
         Args:
             directory: Direct path or list of directory paths from which to serve templates.
             engine_instance: A Minijinja Environment instance.
         """
-        super().__init__(directory, engine_instance)
         if directory and engine_instance:
             raise ImproperlyConfiguredException(
                 "You must provide either a directory or a minijinja Environment instance."
             )
         if directory:
 
             def _loader(name: str) -> str:
```

### Comparing `litestar-2.8.3/litestar/contrib/piccolo.py` & `litestar-2.9.0/litestar/contrib/piccolo.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/attrs/attrs_schema_plugin.py` & `litestar-2.9.0/litestar/contrib/attrs/attrs_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/htmx/_utils.py` & `litestar-2.9.0/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/htmx/request.py` & `litestar-2.9.0/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/htmx/response.py` & `litestar-2.9.0/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/htmx/types.py` & `litestar-2.9.0/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/jwt/__init__.py` & `litestar-2.9.0/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.9.0/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/opentelemetry/config.py` & `litestar-2.9.0/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.9.0/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/prometheus/config.py` & `litestar-2.9.0/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/prometheus/controller.py` & `litestar-2.9.0/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/prometheus/middleware.py` & `litestar-2.9.0/litestar/contrib/prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/pydantic/__init__.py` & `litestar-2.9.0/litestar/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/pydantic/pydantic_di_plugin.py` & `litestar-2.9.0/litestar/contrib/pydantic/pydantic_di_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/pydantic/pydantic_dto_factory.py` & `litestar-2.9.0/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/pydantic/pydantic_init_plugin.py` & `litestar-2.9.0/litestar/contrib/pydantic/pydantic_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/pydantic/pydantic_schema_plugin.py` & `litestar-2.9.0/litestar/contrib/pydantic/pydantic_schema_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,16 @@
             # extract the annotations from the FieldInfo. This allows us to skip fields
             # which have been marked as private
             model_annotations = {k: field_info.annotation for k, field_info in model_fields.items()}  # type: ignore[union-attr]
 
         else:
             # pydantic v1 requires some workarounds here
             model_annotations = {
-                k: f.outer_type_ if f.required else Optional[f.outer_type_] for k, f in model.__fields__.items()
+                k: f.outer_type_ if f.required or f.default else Optional[f.outer_type_]
+                for k, f in model.__fields__.items()
             }
 
         if is_generic_model:
             # if the model is generic, resolve the type variables. We pass in the
             # already extracted annotations, to keep the logic of respecting private
             # fields consistent with the above
             model_annotations = pydantic_get_type_hints_with_generics_resolved(
```

### Comparing `litestar-2.8.3/litestar/contrib/pydantic/utils.py` & `litestar-2.9.0/litestar/contrib/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/repository/__init__.py` & `litestar-2.9.0/litestar/contrib/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/repository/exceptions.py` & `litestar-2.9.0/litestar/contrib/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/repository/filters.py` & `litestar-2.9.0/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/repository/handlers.py` & `litestar-2.9.0/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/repository/testing.py` & `litestar-2.9.0/litestar/contrib/repository/testing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/repository/abc/__init__.py` & `litestar-2.9.0/litestar/contrib/repository/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/sqlalchemy/base.py` & `litestar-2.9.0/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/compat.py` & `litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.9.0/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/datastructures/__init__.py` & `litestar-2.9.0/litestar/datastructures/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from litestar.datastructures.multi_dicts import (
     FormMultiDict,
     ImmutableMultiDict,
     MultiDict,
     MultiMixin,
 )
 from litestar.datastructures.response_header import ResponseHeader
+from litestar.datastructures.secret_values import SecretBytes, SecretString
 from litestar.datastructures.state import ImmutableState, State
 from litestar.datastructures.upload_file import UploadFile
 from litestar.datastructures.url import URL, Address
 
 __all__ = (
     "Accept",
     "Address",
@@ -29,11 +30,13 @@
     "Headers",
     "ImmutableMultiDict",
     "ImmutableState",
     "MultiDict",
     "MultiMixin",
     "MutableScopeHeaders",
     "ResponseHeader",
+    "SecretBytes",
+    "SecretString",
     "State",
     "UploadFile",
     "URL",
 )
```

### Comparing `litestar-2.8.3/litestar/datastructures/cookie.py` & `litestar-2.9.0/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/datastructures/headers.py` & `litestar-2.9.0/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/datastructures/multi_dicts.py` & `litestar-2.9.0/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/datastructures/response_header.py` & `litestar-2.9.0/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/datastructures/state.py` & `litestar-2.9.0/litestar/datastructures/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
-from copy import copy, deepcopy
+from copy import deepcopy
 from threading import RLock
 from typing import TYPE_CHECKING, Any, Callable, Generator, Iterable, Iterator, Mapping, MutableMapping
 
+from litestar.utils.scope.state import CONNECTION_STATE_KEY
+
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 __all__ = ("ImmutableState", "State")
 
 
 class ImmutableState(Mapping[str, Any]):
@@ -139,15 +141,15 @@
 
     def dict(self) -> dict[str, Any]:
         """Return a shallow copy of the wrapped dict.
 
         Returns:
             A dict
         """
-        return copy(self._state)
+        return {k: v for k, v in self._state.items() if k != CONNECTION_STATE_KEY}
 
     @classmethod
     def __get_validators__(
         cls,
     ) -> Generator[Callable[[ImmutableState | dict[str, Any] | Iterable[tuple[str, Any]]], ImmutableState], None, None]:  # type: ignore[valid-type]
         """Pydantic compatible method to allow custom parsing of state instances in a SignatureModel."""
         yield cls.validate
```

### Comparing `litestar-2.8.3/litestar/datastructures/upload_file.py` & `litestar-2.9.0/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/datastructures/url.py` & `litestar-2.9.0/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/dto/_backend.py` & `litestar-2.9.0/litestar/dto/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -697,14 +697,32 @@
                     nested_as_dict=False,
                     is_data_field=is_data_field,
                 )
                 for item in source_value
             )
 
         return transfer_type.field_definition.instantiable_origin(source_value)
+
+    if isinstance(transfer_type, MappingType):
+        if transfer_type.has_nested:
+            return transfer_type.field_definition.instantiable_origin(
+                (
+                    key,
+                    _transfer_type_data(
+                        source_value=value,
+                        transfer_type=transfer_type.value_type,
+                        nested_as_dict=False,
+                        is_data_field=is_data_field,
+                    ),
+                )
+                for key, value in source_value.items()
+            )
+
+        return transfer_type.field_definition.instantiable_origin(source_value)
+
     return source_value
 
 
 def _transfer_nested_union_type_data(
     transfer_type: UnionType,
     source_value: Any,
     is_data_field: bool,
```

### Comparing `litestar-2.8.3/litestar/dto/_codegen_backend.py` & `litestar-2.9.0/litestar/dto/_codegen_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from msgspec import UNSET
 
 from litestar.dto._backend import DTOBackend
 from litestar.dto._types import (
     CollectionType,
     CompositeType,
+    MappingType,
     SimpleType,
     TransferDTOFieldDefinition,
     TransferType,
     UnionType,
 )
 from litestar.utils.helpers import unique_name_for_scope
 
@@ -502,14 +503,29 @@
                     f"{assignment_target} = {origin_name}({transfer_type_data_name}(item) for item in {source_value_name})"
                 )
                 return
 
             self._add_stmt(f"{assignment_target} = {origin_name}({source_value_name})")
             return
 
+        if isinstance(transfer_type, MappingType):
+            origin_name = self._add_to_fn_globals("origin", transfer_type.field_definition.instantiable_origin)
+            if transfer_type.has_nested:
+                transfer_type_data_fn = TransferFunctionFactory.create_transfer_type_data(
+                    is_data_field=self.is_data_field, transfer_type=transfer_type.value_type
+                )
+                transfer_type_data_name = self._add_to_fn_globals("transfer_type_data", transfer_type_data_fn)
+                self._add_stmt(
+                    f"{assignment_target} = {origin_name}((key, {transfer_type_data_name}(item)) for key, item in {source_value_name}.items())"
+                )
+                return
+
+            self._add_stmt(f"{assignment_target} = {origin_name}({source_value_name})")
+            return
+
         self._add_stmt(f"{assignment_target} = {source_value_name}")
 
     def _create_transfer_nested_union_type_data(
         self,
         transfer_type: UnionType,
         source_value_name: str,
         assignment_target: str,
```

### Comparing `litestar-2.8.3/litestar/dto/_types.py` & `litestar-2.9.0/litestar/dto/_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/dto/base_dto.py` & `litestar-2.9.0/litestar/dto/base_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,18 +213,21 @@
             # The backend doesn't receive the full annotation, only the type of the attribute on the outer type that
             # holds the DTO supported type.
             #
             # This special casing rebuilds the outer generic type annotation with the original model replaced by the DTO
             # generated transfer model type in the type arguments.
             transfer_model = backend.transfer_model_type
             generic_args = tuple(transfer_model if a is cls.model_type else a for a in field_definition.args)
-            return schema_creator.for_field_definition(
-                FieldDefinition.from_annotation(field_definition.origin[generic_args])
-            )
-        return schema_creator.for_field_definition(FieldDefinition.from_annotation(backend.annotation))
+            annotation = field_definition.safe_generic_origin[generic_args]
+        else:
+            annotation = backend.annotation
+
+        return schema_creator.for_field_definition(
+            FieldDefinition.from_annotation(annotation, kwarg_definition=field_definition.kwarg_definition)
+        )
 
     @classmethod
     def resolve_generic_wrapper_type(
         cls, field_definition: FieldDefinition
     ) -> tuple[FieldDefinition, FieldDefinition, str] | None:
         """Handle where DTO supported data is wrapped in a generic container type.
```

### Comparing `litestar-2.8.3/litestar/dto/config.py` & `litestar-2.9.0/litestar/dto/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/dto/data_structures.py` & `litestar-2.9.0/litestar/dto/data_structures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/dto/dataclass_dto.py` & `litestar-2.9.0/litestar/dto/dataclass_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/dto/field.py` & `litestar-2.9.0/litestar/dto/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/dto/msgspec_dto.py` & `litestar-2.9.0/litestar/dto/msgspec_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/events/emitter.py` & `litestar-2.9.0/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/events/listener.py` & `litestar-2.9.0/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/exceptions/__init__.py` & `litestar-2.9.0/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/exceptions/base_exceptions.py` & `litestar-2.9.0/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/exceptions/http_exceptions.py` & `litestar-2.9.0/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/exceptions/websocket_exceptions.py` & `litestar-2.9.0/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/__init__.py` & `litestar-2.9.0/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/asgi_handlers.py` & `litestar-2.9.0/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/base.py` & `litestar-2.9.0/litestar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/http_handlers/_utils.py` & `litestar-2.9.0/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/http_handlers/base.py` & `litestar-2.9.0/litestar/handlers/http_handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/http_handlers/decorators.py` & `litestar-2.9.0/litestar/handlers/http_handlers/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from typing import TYPE_CHECKING
 
 from litestar.enums import HttpMethod, MediaType
 from litestar.exceptions import HTTPException, ImproperlyConfiguredException
 from litestar.openapi.spec import Operation
 from litestar.response.file import ASGIFileResponse, File
 from litestar.types import Empty, TypeDecodersSequence
@@ -41,15 +42,25 @@
 
 
 __all__ = ("get", "head", "post", "put", "patch", "delete")
 
 MSG_SEMANTIC_ROUTE_HANDLER_WITH_HTTP = "semantic route handlers cannot define http_method"
 
 
-class delete(HTTPRouteHandler):
+class _SubclassWarningMixin:
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        warnings.warn(
+            "Semantic HTTP route handler classes are deprecated and will be replaced by"
+            "functional decorators in Litestar 3.0.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+
+
+class delete(HTTPRouteHandler, _SubclassWarningMixin):
     """DELETE Route Decorator.
 
     Use this decorator to decorate an HTTP handler for DELETE requests.
     """
 
     def __init__(
         self,
@@ -213,15 +224,15 @@
             tags=tags,
             type_decoders=type_decoders,
             type_encoders=type_encoders,
             **kwargs,
         )
 
 
-class get(HTTPRouteHandler):
+class get(HTTPRouteHandler, _SubclassWarningMixin):
     """GET Route Decorator.
 
     Use this decorator to decorate an HTTP handler for GET requests.
     """
 
     def __init__(
         self,
@@ -386,15 +397,15 @@
             tags=tags,
             type_decoders=type_decoders,
             type_encoders=type_encoders,
             **kwargs,
         )
 
 
-class head(HTTPRouteHandler):
+class head(HTTPRouteHandler, _SubclassWarningMixin):
     """HEAD Route Decorator.
 
     Use this decorator to decorate an HTTP handler for HEAD requests.
     """
 
     def __init__(
         self,
@@ -576,15 +587,15 @@
             return_annotation in {NoneType, None}
             or is_class_and_subclass(return_annotation, File)
             or is_class_and_subclass(return_annotation, ASGIFileResponse)
         ):
             raise ImproperlyConfiguredException("A response to a head request should not have a body")
 
 
-class patch(HTTPRouteHandler):
+class patch(HTTPRouteHandler, _SubclassWarningMixin):
     """PATCH Route Decorator.
 
     Use this decorator to decorate an HTTP handler for PATCH requests.
     """
 
     def __init__(
         self,
@@ -748,15 +759,15 @@
             tags=tags,
             type_decoders=type_decoders,
             type_encoders=type_encoders,
             **kwargs,
         )
 
 
-class post(HTTPRouteHandler):
+class post(HTTPRouteHandler, _SubclassWarningMixin):
     """POST Route Decorator.
 
     Use this decorator to decorate an HTTP handler for POST requests.
     """
 
     def __init__(
         self,
@@ -920,15 +931,15 @@
             tags=tags,
             type_decoders=type_decoders,
             type_encoders=type_encoders,
             **kwargs,
         )
 
 
-class put(HTTPRouteHandler):
+class put(HTTPRouteHandler, _SubclassWarningMixin):
     """PUT Route Decorator.
 
     Use this decorator to decorate an HTTP handler for PUT requests.
     """
 
     def __init__(
         self,
```

### Comparing `litestar-2.8.3/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.9.0/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.9.0/litestar/handlers/websocket_handlers/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.9.0/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/logging/_utils.py` & `litestar-2.9.0/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/logging/config.py` & `litestar-2.9.0/litestar/logging/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from importlib.util import find_spec
 from logging import INFO
 from typing import TYPE_CHECKING, Any, Callable, Literal, cast
 
 from litestar.exceptions import ImproperlyConfiguredException, MissingDependencyException
 from litestar.serialization.msgspec_hooks import _msgspec_json_encoder
 from litestar.utils.dataclass import simple_asdict
-from litestar.utils.deprecation import deprecated
+from litestar.utils.deprecation import deprecated, warn_deprecation
 
 __all__ = ("BaseLoggingConfig", "LoggingConfig", "StructLoggingConfig")
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
     from typing import NoReturn
@@ -86,56 +86,71 @@
     """
     if find_spec("picologging"):
         return default_picologging_handlers
     return default_handlers
 
 
 def _default_exception_logging_handler_factory(
-    is_struct_logger: bool, traceback_line_limit: int
+    is_struct_logger: bool,
+    traceback_line_limit: int,
 ) -> ExceptionLoggingHandler:
     """Create an exception logging handler function.
 
     Args:
         is_struct_logger: Whether the logger is a structlog instance.
         traceback_line_limit: Maximal number of lines to log from the
-            traceback.
+            traceback. This parameter is deprecated and ignored.
 
     Returns:
         An exception logging handler.
     """
 
-    def _default_exception_logging_handler(logger: Logger, scope: Scope, tb: list[str]) -> None:
-        # we limit the length of the stack trace to 20 lines.
-        first_line = tb.pop(0)
+    if traceback_line_limit != -1:
+        warn_deprecation(
+            version="2.9.0",
+            deprecated_name="traceback_line_limit",
+            kind="parameter",
+            info="The value is ignored. Use a custom 'exception_logging_handler' instead.",
+            removal_in="3.0",
+        )
+
+    if is_struct_logger:
 
-        if is_struct_logger:
+        def _default_exception_logging_handler(logger: Logger, scope: Scope, tb: list[str]) -> None:
             logger.exception(
-                "Uncaught Exception",
+                "Uncaught exception",
                 connection_type=scope["type"],
                 path=scope["path"],
-                traceback="".join(tb[-traceback_line_limit:]),
             )
-        else:
-            stack_trace = first_line + "".join(tb[-traceback_line_limit:])
+
+    else:
+
+        def _default_exception_logging_handler(logger: Logger, scope: Scope, tb: list[str]) -> None:
             logger.exception(
-                "exception raised on %s connection to route %s\n\n%s", scope["type"], scope["path"], stack_trace
+                "Uncaught exception (connection_type=%s, path=%s):",
+                scope["type"],
+                scope["path"],
             )
 
     return _default_exception_logging_handler
 
 
 class BaseLoggingConfig(ABC):
     """Abstract class that should be extended by logging configs."""
 
     __slots__ = ("log_exceptions", "traceback_line_limit", "exception_logging_handler")
 
     log_exceptions: Literal["always", "debug", "never"]
     """Should exceptions be logged, defaults to log exceptions when ``app.debug == True``'"""
     traceback_line_limit: int
-    """Max number of lines to print for exception traceback"""
+    """Max number of lines to print for exception traceback.
+
+    .. deprecated:: 2.9.0
+        This parameter is deprecated and ignored. It will be removed in a future release.
+    """
     exception_logging_handler: ExceptionLoggingHandler | None
     """Handler function for logging exceptions."""
 
     @abstractmethod
     def configure(self) -> GetLogger:
         """Return logger with the given configuration.
 
@@ -201,16 +216,20 @@
 
     Processing of the configuration will be as for any logger, except that the propagate setting will not be applicable.
     """
     configure_root_logger: bool = field(default=True)
     """Should the root logger be configured, defaults to True for ease of configuration."""
     log_exceptions: Literal["always", "debug", "never"] = field(default="debug")
     """Should exceptions be logged, defaults to log exceptions when 'app.debug == True'"""
-    traceback_line_limit: int = field(default=20)
-    """Max number of lines to print for exception traceback"""
+    traceback_line_limit: int = field(default=-1)
+    """Max number of lines to print for exception traceback.
+
+    .. deprecated:: 2.9.0
+        This parameter is deprecated and ignored. It will be removed in a future release.
+    """
     exception_logging_handler: ExceptionLoggingHandler | None = field(default=None)
     """Handler function for logging exceptions."""
 
     def __post_init__(self) -> None:
         if "queue_listener" not in self.handlers:
             self.handlers["queue_listener"] = _get_default_handlers()["queue_listener"]
 
@@ -417,47 +436,52 @@
     """Context class (a 'contextvar' context) for the logger."""
     logger_factory: Callable[..., WrappedLogger] | None = field(default=None)  # pyright: ignore
     """Logger factory to use."""
     cache_logger_on_first_use: bool = field(default=True)
     """Whether to cache the logger configuration and reuse."""
     log_exceptions: Literal["always", "debug", "never"] = field(default="debug")
     """Should exceptions be logged, defaults to log exceptions when 'app.debug == True'"""
-    traceback_line_limit: int = field(default=20)
-    """Max number of lines to print for exception traceback"""
+    traceback_line_limit: int = field(default=-1)
+    """Max number of lines to print for exception traceback.
+
+    .. deprecated:: 2.9.0
+        This parameter is deprecated and ignored. It will be removed in a future release.
+    """
     exception_logging_handler: ExceptionLoggingHandler | None = field(default=None)
     """Handler function for logging exceptions."""
     pretty_print_tty: bool = field(default=True)
     """Pretty print log output when run from an interactive terminal."""
 
     def __post_init__(self) -> None:
         if self.processors is None:
-            self.processors = default_structlog_processors(not sys.stderr.isatty() and self.pretty_print_tty)
+            self.processors = default_structlog_processors(as_json=self.as_json())
         if self.logger_factory is None:
-            self.logger_factory = default_logger_factory(not sys.stderr.isatty() and self.pretty_print_tty)
+            self.logger_factory = default_logger_factory(as_json=self.as_json())
         if self.log_exceptions != "never" and self.exception_logging_handler is None:
             self.exception_logging_handler = _default_exception_logging_handler_factory(
                 is_struct_logger=True, traceback_line_limit=self.traceback_line_limit
             )
         try:
             import structlog
 
             if self.standard_lib_logging_config is None:
                 self.standard_lib_logging_config = LoggingConfig(
                     formatters={
                         "standard": {
                             "()": structlog.stdlib.ProcessorFormatter,
-                            "processors": default_structlog_standard_lib_processors(
-                                as_json=not sys.stderr.isatty() and self.pretty_print_tty
-                            ),
+                            "processors": default_structlog_standard_lib_processors(as_json=self.as_json()),
                         }
                     }
                 )
         except ImportError:
             self.standard_lib_logging_config = LoggingConfig()
 
+    def as_json(self) -> bool:
+        return not (sys.stderr.isatty() and self.pretty_print_tty)
+
     def configure(self) -> GetLogger:
         """Return logger with the given configuration.
 
         Returns:
             A 'logging.getLogger' like function.
         """
         try:
```

### Comparing `litestar-2.8.3/litestar/logging/picologging.py` & `litestar-2.9.0/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/logging/standard.py` & `litestar-2.9.0/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/_utils.py` & `litestar-2.9.0/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/allowed_hosts.py` & `litestar-2.9.0/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/authentication.py` & `litestar-2.9.0/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/base.py` & `litestar-2.9.0/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/csrf.py` & `litestar-2.9.0/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/logging.py` & `litestar-2.9.0/litestar/middleware/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,17 @@
             An dict.
         """
         data: dict[str, Any] = {"message": self.config.response_log_message}
         serializer = get_serializer_from_scope(scope)
         connection_state = ScopeState.from_scope(scope)
         extracted_data = self.response_extractor(
             messages=(
-                connection_state.log_context.pop(HTTP_RESPONSE_START),
+                # NOTE: we don't pop the start message from the logging context in case
+                #   there are multiple body messages to be logged
+                connection_state.log_context[HTTP_RESPONSE_START],
                 connection_state.log_context.pop(HTTP_RESPONSE_BODY),
             ),
         )
         response_body_compressed = value_or_default(connection_state.response_compressed, False)
         for key in self.config.response_log_fields:
             value: Any
             value = extracted_data.get(key)
@@ -220,14 +222,18 @@
 
         async def send_wrapper(message: Message) -> None:
             if message["type"] == HTTP_RESPONSE_START:
                 connection_state.log_context[HTTP_RESPONSE_START] = message
             elif message["type"] == HTTP_RESPONSE_BODY:
                 connection_state.log_context[HTTP_RESPONSE_BODY] = message
                 self.log_response(scope=scope)
+
+                if not message["more_body"]:
+                    connection_state.log_context.clear()
+
             await send(message)
 
         return send_wrapper
 
 
 @dataclass
 class LoggingMiddlewareConfig:
```

### Comparing `litestar-2.8.3/litestar/middleware/rate_limit.py` & `litestar-2.9.0/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/response_cache.py` & `litestar-2.9.0/litestar/middleware/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/compression/brotli_facade.py` & `litestar-2.9.0/litestar/middleware/compression/brotli_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/compression/facade.py` & `litestar-2.9.0/litestar/middleware/compression/facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/compression/gzip_facade.py` & `litestar-2.9.0/litestar/middleware/compression/gzip_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/compression/middleware.py` & `litestar-2.9.0/litestar/middleware/compression/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.9.0/litestar/exceptions/responses/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/exceptions/middleware.py` & `litestar-2.9.0/litestar/middleware/_internal/exceptions/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from __future__ import annotations
 
 import pdb  # noqa: T100
-from dataclasses import asdict, dataclass, field
 from inspect import getmro
 from sys import exc_info
 from traceback import format_exception
 from typing import TYPE_CHECKING, Any, Type, cast
 
-from litestar.datastructures import Headers
-from litestar.enums import MediaType, ScopeType
+from litestar.enums import ScopeType
 from litestar.exceptions import HTTPException, LitestarException, WebSocketException
-from litestar.middleware.cors import CORSMiddleware
-from litestar.middleware.exceptions._debug_response import _get_type_encoders_for_request, create_debug_response
-from litestar.serialization import encode_json, get_serializer
+from litestar.exceptions.responses import create_exception_response
+from litestar.exceptions.responses._debug_response import (
+    create_debug_response,
+)
 from litestar.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.utils.deprecation import warn_deprecation
-
-__all__ = ("ExceptionHandlerMiddleware", "ExceptionResponseContent", "create_exception_response")
-
+from litestar.utils.empty import value_or_raise
+from litestar.utils.scope.state import ScopeState
 
 if TYPE_CHECKING:
     from starlette.exceptions import HTTPException as StarletteHTTPException
 
     from litestar import Response
     from litestar.app import Litestar
     from litestar.connection import Request
     from litestar.logging import BaseLoggingConfig
     from litestar.types import (
         ASGIApp,
         ExceptionHandler,
         ExceptionHandlersMap,
         Logger,
+        Message,
         Receive,
         Scope,
         Send,
     )
     from litestar.types.asgi_types import WebSocketCloseEvent
 
+__all__ = ("ExceptionHandlerMiddleware",)
+
 
 def get_exception_handler(exception_handlers: ExceptionHandlersMap, exc: Exception) -> ExceptionHandler | None:
     """Given a dictionary that maps exceptions and status codes to handler functions, and an exception, returns the
     appropriate handler if existing.
 
     Status codes are given preference over exception type.
 
@@ -69,137 +70,68 @@
 
     return next(
         (exception_handlers[cast("Type[Exception]", cls)] for cls in getmro(type(exc)) if cls in exception_handlers),
         default_handler,
     )
 
 
-@dataclass
-class ExceptionResponseContent:
-    """Represent the contents of an exception-response."""
-
-    status_code: int
-    """Exception status code."""
-    detail: str
-    """Exception details or message."""
-    media_type: MediaType | str
-    """Media type of the response."""
-    headers: dict[str, str] | None = field(default=None)
-    """Headers to attach to the response."""
-    extra: dict[str, Any] | list[Any] | None = field(default=None)
-    """An extra mapping to attach to the exception."""
-
-    def to_response(self, request: Request | None = None) -> Response:
-        """Create a response from the model attributes.
-
-        Returns:
-            A response instance.
-        """
-        from litestar.response import Response
-
-        content: Any = {k: v for k, v in asdict(self).items() if k not in ("headers", "media_type") and v is not None}
-        type_encoders = _get_type_encoders_for_request(request) if request is not None else None
-
-        if self.media_type != MediaType.JSON:
-            content = encode_json(content, get_serializer(type_encoders))
-
-        return Response(
-            content=content,
-            headers=self.headers,
-            status_code=self.status_code,
-            media_type=self.media_type,
-            type_encoders=type_encoders,
-        )
-
-
 def _starlette_exception_handler(request: Request[Any, Any, Any], exc: StarletteHTTPException) -> Response:
     return create_exception_response(
         request=request,
         exc=HTTPException(
             detail=exc.detail,
             status_code=exc.status_code,
             headers=exc.headers,
         ),
     )
 
 
-def create_exception_response(request: Request[Any, Any, Any], exc: Exception) -> Response:
-    """Construct a response from an exception.
-
-    Notes:
-        - For instances of :class:`HTTPException <litestar.exceptions.HTTPException>` or other exception classes that have a
-          ``status_code`` attribute (e.g. Starlette exceptions), the status code is drawn from the exception, otherwise
-          response status is ``HTTP_500_INTERNAL_SERVER_ERROR``.
-
-    Args:
-        request: The request that triggered the exception.
-        exc: An exception.
-
-    Returns:
-        Response: HTTP response constructed from exception details.
-    """
-    headers: dict[str, Any] | None
-    extra: dict[str, Any] | list | None
-
-    if isinstance(exc, HTTPException):
-        status_code = exc.status_code
-        headers = exc.headers
-        extra = exc.extra
-    else:
-        status_code = HTTP_500_INTERNAL_SERVER_ERROR
-        headers = None
-        extra = None
-
-    detail = (
-        exc.detail
-        if isinstance(exc, LitestarException) and status_code != HTTP_500_INTERNAL_SERVER_ERROR
-        else "Internal Server Error"
-    )
-
-    try:
-        media_type = request.route_handler.media_type
-    except (KeyError, AttributeError):
-        media_type = MediaType.JSON
-
-    content = ExceptionResponseContent(
-        status_code=status_code,
-        detail=detail,
-        headers=headers,
-        extra=extra,
-        media_type=media_type,
-    )
-    return content.to_response(request=request)
-
-
 class ExceptionHandlerMiddleware:
     """Middleware used to wrap an ASGIApp inside a try catch block and handle any exceptions raised.
 
     This used in multiple layers of Litestar.
     """
 
-    def __init__(self, app: ASGIApp, debug: bool | None, exception_handlers: ExceptionHandlersMap) -> None:
+    def __init__(
+        self, app: ASGIApp, debug: bool | None, exception_handlers: ExceptionHandlersMap | None = None
+    ) -> None:
         """Initialize ``ExceptionHandlerMiddleware``.
 
         Args:
             app: The ``next`` ASGI app to call.
             debug: Whether ``debug`` mode is enabled. Deprecated. Debug mode will be inferred from the request scope
             exception_handlers: A dictionary mapping status codes and/or exception types to handler functions.
 
         .. deprecated:: 2.0.0
             The ``debug`` parameter is deprecated. It will be inferred from the request scope
+
+        .. deprecated:: 2.9.0
+            The ``exception_handlers`` parameter is deprecated. It will be inferred from the application or the
+            route handler.
         """
         self.app = app
         self.exception_handlers = exception_handlers
         self.debug = debug
+
         if debug is not None:
             warn_deprecation(
                 "2.0.0",
                 deprecated_name="debug",
                 kind="parameter",
                 info="Debug mode will be inferred from the request scope",
+                removal_in="3.0.0",
+            )
+
+        if exception_handlers is not None:
+            warn_deprecation(
+                "2.9.0",
+                deprecated_name="exception_handlers",
+                kind="parameter",
+                info="It will be inferred from the application or the route handler",
+                removal_in="3.0.0",
             )
 
         self._get_debug = self._get_debug_scope if debug is None else lambda *a: debug
 
     @staticmethod
     def _get_debug_scope(scope: Scope) -> bool:
         return scope["app"].debug
@@ -211,17 +143,27 @@
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
             None
         """
+        scope_state = ScopeState.from_scope(scope)
+
+        async def capture_response_started(event: Message) -> None:
+            if event["type"] == "http.response.start":
+                scope_state.response_started = True
+            await send(event)
+
         try:
-            await self.app(scope, receive, send)
-        except Exception as e:  # noqa: BLE001
+            await self.app(scope, receive, capture_response_started)
+        except Exception as e:
+            if scope_state.response_started:
+                raise LitestarException("Exception caught after response started") from e
+
             litestar_app = scope["app"]
 
             if litestar_app.logging_config and (logger := litestar_app.logger):
                 self.handle_exception_logging(logger=logger, logging_config=litestar_app.logging_config, scope=scope)
 
             for hook in litestar_app.after_exception:
                 await hook(e, scope)
@@ -248,20 +190,20 @@
             send: The ASGI send function.
             exc: The caught exception.
 
         Returns:
             None.
         """
 
-        headers = Headers.from_scope(scope=scope)
-        if litestar_app.cors_config and (origin := headers.get("origin")):
-            cors_middleware = CORSMiddleware(app=self.app, config=litestar_app.cors_config)
-            send = cors_middleware.send_wrapper(send=send, origin=origin, has_cookie="cookie" in headers)
-
-        exception_handler = get_exception_handler(self.exception_handlers, exc) or self.default_http_exception_handler
+        exception_handlers = (
+            value_or_raise(ScopeState.from_scope(scope).exception_handlers)
+            if self.exception_handlers is None
+            else self.exception_handlers
+        )
+        exception_handler = get_exception_handler(exception_handlers, exc) or self.default_http_exception_handler
         request: Request[Any, Any, Any] = litestar_app.request_class(scope=scope, receive=receive, send=send)
         response = exception_handler(request, exc)
         await response.to_asgi_response(app=None, request=request)(scope=scope, receive=receive, send=send)
 
     @staticmethod
     async def handle_websocket_exception(send: Send, exc: Exception) -> None:
         """Handle exception raised inside 'websocket' scope routes.
```

### Comparing `litestar-2.8.3/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.9.0/litestar/exceptions/responses/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.9.0/litestar/exceptions/responses/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/session/base.py` & `litestar-2.9.0/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/session/client_side.py` & `litestar-2.9.0/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/middleware/session/server_side.py` & `litestar-2.9.0/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/config.py` & `litestar-2.9.0/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/controller.py` & `litestar-2.9.0/litestar/openapi/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
         Returns:
             A Response instance with the YAML object rendered into a string.
         """
         from yaml import dump as dump_yaml
 
         if self.should_serve_endpoint(request):
-            if not self._dumped_json_schema:
+            if not self._dumped_yaml_schema:
                 schema_json = decode_json(self._get_schema_as_json(request))
                 schema_yaml = dump_yaml(schema_json, default_flow_style=False)
                 self._dumped_yaml_schema = schema_yaml.encode("utf-8")
             return ASGIResponse(body=self._dumped_yaml_schema, media_type=OpenAPIMediaType.OPENAPI_YAML)
         return ASGIResponse(body=b"", status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(
```

### Comparing `litestar-2.8.3/litestar/openapi/datastructures.py` & `litestar-2.9.0/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/plugins.py` & `litestar-2.9.0/litestar/openapi/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/__init__.py` & `litestar-2.9.0/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/base.py` & `litestar-2.9.0/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/callback.py` & `litestar-2.9.0/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/components.py` & `litestar-2.9.0/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/contact.py` & `litestar-2.9.0/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/discriminator.py` & `litestar-2.9.0/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/encoding.py` & `litestar-2.9.0/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/enums.py` & `litestar-2.9.0/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/example.py` & `litestar-2.9.0/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/external_documentation.py` & `litestar-2.9.0/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/header.py` & `litestar-2.9.0/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/info.py` & `litestar-2.9.0/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/license.py` & `litestar-2.9.0/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/link.py` & `litestar-2.9.0/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/media_type.py` & `litestar-2.9.0/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/oauth_flow.py` & `litestar-2.9.0/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/oauth_flows.py` & `litestar-2.9.0/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/open_api.py` & `litestar-2.9.0/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/operation.py` & `litestar-2.9.0/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/parameter.py` & `litestar-2.9.0/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/path_item.py` & `litestar-2.9.0/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/paths.py` & `litestar-2.9.0/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/reference.py` & `litestar-2.9.0/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/request_body.py` & `litestar-2.9.0/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/response.py` & `litestar-2.9.0/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/responses.py` & `litestar-2.9.0/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/schema.py` & `litestar-2.9.0/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/security_requirement.py` & `litestar-2.9.0/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/security_scheme.py` & `litestar-2.9.0/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/server.py` & `litestar-2.9.0/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/server_variable.py` & `litestar-2.9.0/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/tag.py` & `litestar-2.9.0/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/openapi/spec/xml.py` & `litestar-2.9.0/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/plugins/base.py` & `litestar-2.9.0/litestar/plugins/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,14 @@
 
 
 class CLIPlugin(CLIPluginProtocol):
     """Plugin protocol to extend the CLI Server Lifespan."""
 
     __slots__ = ()
 
-    def on_cli_init(self, cli: Group) -> None:
-        return super().on_cli_init(cli)
-
     @contextmanager
     def server_lifespan(self, app: Litestar) -> Iterator[None]:
         yield
 
 
 @runtime_checkable
 class SerializationPluginProtocol(Protocol):
```

### Comparing `litestar-2.8.3/litestar/plugins/core.py` & `litestar-2.9.0/litestar/plugins/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/plugins/flash.py` & `litestar-2.9.0/litestar/plugins/flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from litestar.template.base import _get_request_from_context
 from litestar.utils.predicates import is_class_and_subclass
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from litestar.config.app import AppConfig
+    from litestar.connection.base import AuthT, StateT, UserT
     from litestar.template import TemplateConfig
 
 
 @dataclass
 class FlashConfig:
     """Configuration for Flash messages."""
 
@@ -65,15 +66,15 @@
                 template_callable = _transform_state(get_flashes)
 
         self.config.template_config.engine_instance.register_template_callable("get_flashes", template_callable)  # pyright: ignore[reportGeneralTypeIssues]
         return app_config
 
 
 def flash(
-    request: Request,
+    request: Request[UserT, AuthT, StateT],
     message: Any,
     category: str,
 ) -> None:
     request.session.setdefault("_messages", []).append({"message": message, "category": category})
 
 
 def get_flashes(context: Mapping[str, Any]) -> Any:
```

### Comparing `litestar-2.8.3/litestar/plugins/structlog.py` & `litestar-2.9.0/litestar/plugins/structlog.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/repository/_filters.py` & `litestar-2.9.0/litestar/repository/_filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/repository/filters.py` & `litestar-2.9.0/litestar/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/repository/handlers.py` & `litestar-2.9.0/litestar/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/repository/abc/_async.py` & `litestar-2.9.0/litestar/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/repository/abc/_sync.py` & `litestar-2.9.0/litestar/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/repository/testing/generic_mock_repository.py` & `litestar-2.9.0/litestar/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/response/base.py` & `litestar-2.9.0/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/response/file.py` & `litestar-2.9.0/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/response/redirect.py` & `litestar-2.9.0/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/response/sse.py` & `litestar-2.9.0/litestar/response/sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/response/streaming.py` & `litestar-2.9.0/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/response/template.py` & `litestar-2.9.0/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/routes/asgi.py` & `litestar-2.9.0/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/routes/base.py` & `litestar-2.9.0/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/routes/http.py` & `litestar-2.9.0/litestar/routes/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 from itertools import chain
 from typing import TYPE_CHECKING, Any, cast
 
 from msgspec.msgpack import decode as _decode_msgpack_plain
 
-from litestar.constants import DEFAULT_ALLOWED_CORS_HEADERS
-from litestar.datastructures.headers import Headers
 from litestar.datastructures.upload_file import UploadFile
 from litestar.enums import HttpMethod, MediaType, ScopeType
 from litestar.exceptions import ClientException, ImproperlyConfiguredException, SerializationException
 from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.response import Response
 from litestar.routes.base import BaseRoute
-from litestar.status_codes import HTTP_204_NO_CONTENT, HTTP_400_BAD_REQUEST
+from litestar.status_codes import HTTP_204_NO_CONTENT
 from litestar.types.empty import Empty
 from litestar.utils.scope.state import ScopeState
 
 if TYPE_CHECKING:
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.cleanup import DependencyCleanupGroup
     from litestar.connection import Request
@@ -251,65 +249,14 @@
 
             Args:
                 scope: The ASGI Scope.
 
             Returns:
                 Response
             """
-            cors_config = scope["app"].cors_config
-            request_headers = Headers.from_scope(scope=scope)
-            origin = request_headers.get("origin")
-
-            if cors_config and origin:
-                pre_flight_method = request_headers.get("Access-Control-Request-Method")
-                failures = []
-
-                if not cors_config.is_allow_all_methods and (
-                    pre_flight_method and pre_flight_method not in cors_config.allow_methods
-                ):
-                    failures.append("method")
-
-                response_headers = cors_config.preflight_headers.copy()
-
-                if not cors_config.is_origin_allowed(origin):
-                    failures.append("Origin")
-                elif response_headers.get("Access-Control-Allow-Origin") != "*":
-                    response_headers["Access-Control-Allow-Origin"] = origin
-
-                pre_flight_requested_headers = [
-                    header.strip()
-                    for header in request_headers.get("Access-Control-Request-Headers", "").split(",")
-                    if header.strip()
-                ]
-
-                if pre_flight_requested_headers:
-                    if cors_config.is_allow_all_headers:
-                        response_headers["Access-Control-Allow-Headers"] = ", ".join(
-                            sorted(set(pre_flight_requested_headers) | DEFAULT_ALLOWED_CORS_HEADERS)  # pyright: ignore
-                        )
-                    elif any(
-                        header.lower() not in cors_config.allow_headers for header in pre_flight_requested_headers
-                    ):
-                        failures.append("headers")
-
-                return (
-                    Response(
-                        content=f"Disallowed CORS {', '.join(failures)}",
-                        status_code=HTTP_400_BAD_REQUEST,
-                        media_type=MediaType.TEXT,
-                    )
-                    if failures
-                    else Response(
-                        content=None,
-                        status_code=HTTP_204_NO_CONTENT,
-                        media_type=MediaType.TEXT,
-                        headers=response_headers,
-                    )
-                )
-
             return Response(
                 content=None,
                 status_code=HTTP_204_NO_CONTENT,
                 headers={"Allow": ", ".join(sorted(self.methods))},  # pyright: ignore
                 media_type=MediaType.TEXT,
             )
```

### Comparing `litestar-2.8.3/litestar/routes/websocket.py` & `litestar-2.9.0/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/base.py` & `litestar-2.9.0/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/jwt/__init__.py` & `litestar-2.9.0/litestar/security/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/jwt/auth.py` & `litestar-2.9.0/litestar/security/jwt/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/jwt/middleware.py` & `litestar-2.9.0/litestar/security/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/jwt/token.py` & `litestar-2.9.0/litestar/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/session_auth/auth.py` & `litestar-2.9.0/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/security/session_auth/middleware.py` & `litestar-2.9.0/litestar/security/session_auth/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Sequence
 
 from litestar.exceptions import NotAuthorizedException
+from litestar.middleware._internal.exceptions import ExceptionHandlerMiddleware
 from litestar.middleware.authentication import (
     AbstractAuthenticationMiddleware,
     AuthenticationResult,
 )
-from litestar.middleware.exceptions import ExceptionHandlerMiddleware
 from litestar.types import Empty, Method, Scopes
 
 __all__ = ("MiddlewareWrapper", "SessionAuthMiddleware")
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.security.session_auth.auth import SessionAuth
@@ -42,28 +42,23 @@
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
             None
         """
         if not self.has_wrapped_middleware:
-            litestar_app = scope["app"]
             auth_middleware = self.config.authentication_middleware_class(
                 app=self.app,
                 exclude=self.config.exclude,
                 exclude_http_methods=self.config.exclude_http_methods,
                 exclude_opt_key=self.config.exclude_opt_key,
                 scopes=self.config.scopes,
                 retrieve_user_handler=self.config.retrieve_user_handler,  # type: ignore[arg-type]
             )
-            exception_middleware = ExceptionHandlerMiddleware(
-                app=auth_middleware,
-                exception_handlers=litestar_app.exception_handlers or {},  # pyright: ignore
-                debug=None,
-            )
+            exception_middleware = ExceptionHandlerMiddleware(app=auth_middleware, debug=None)
             self.app = self.config.session_backend_config.middleware.middleware(
                 app=exception_middleware,
                 backend=self.config.session_backend,
             )
             self.has_wrapped_middleware = True
         await self.app(scope, receive, send)
```

### Comparing `litestar-2.8.3/litestar/serialization/msgspec_hooks.py` & `litestar-2.9.0/litestar/serialization/msgspec_hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 from pathlib import Path, PurePath
 from re import Pattern
 from typing import TYPE_CHECKING, Any, Callable, Mapping, TypeVar, overload
 from uuid import UUID
 
 import msgspec
 
+from litestar.datastructures.secret_values import SecretBytes, SecretString
 from litestar.exceptions import SerializationException
 from litestar.types import Empty, EmptyType, Serializer, TypeDecodersSequence
+from litestar.utils.typing import get_origin_or_inner_type
 
 if TYPE_CHECKING:
     from litestar.types import TypeEncodersMap
 
 __all__ = (
     "decode_json",
     "decode_msgpack",
@@ -48,14 +50,16 @@
     IPv6Network: str,
     datetime: lambda val: val.isoformat(),
     date: lambda val: val.isoformat(),
     time: lambda val: val.isoformat(),
     deque: list,
     Decimal: lambda val: int(val) if val.as_tuple().exponent >= 0 else float(val),
     Pattern: lambda val: val.pattern,
+    SecretBytes: lambda val: val.get_obscured().decode("utf-8"),
+    SecretString: lambda val: val.get_obscured(),
     # support subclasses of stdlib types, If no previous type matched, these will be
     # the last type in the mro, so we use this to (attempt to) convert a subclass into
     # its base class. # see https://github.com/jcrist/msgspec/issues/248
     # and https://github.com/litestar-org/litestar/issues/1003
     str: str,
     int: int,
     float: float,
@@ -100,25 +104,42 @@
 
     Returns:
         A ``msgspec``-supported type
     """
 
     from litestar.datastructures.state import ImmutableState
 
-    if isinstance(value, target_type):
-        return value
+    try:
+        if isinstance(value, target_type):
+            return value
+    except TypeError as exc:
+        # we might get a TypeError here if target_type is a subscribed generic. For
+        # performance reasons, we let this happen and only unwrap this when we're
+        # certain this might be the case
+        if (origin := get_origin_or_inner_type(target_type)) is not None:
+            target_type = origin
+            if isinstance(value, target_type):
+                return value
+        else:
+            raise exc
 
     if type_decoders:
         for predicate, decoder in type_decoders:
             if predicate(target_type):
                 return decoder(target_type, value)
 
     if issubclass(target_type, (Path, PurePath, ImmutableState, UUID)):
         return target_type(value)
 
+    if issubclass(target_type, SecretBytes) and isinstance(value, (bytes, str)):
+        return SecretBytes(value.encode("utf-8") if isinstance(value, str) else value)
+
+    if issubclass(target_type, SecretString) and isinstance(value, str):
+        return SecretString(value)
+
     raise TypeError(f"Unsupported type: {type(value)!r}")
 
 
 _msgspec_json_encoder = msgspec.json.Encoder(enc_hook=default_serializer)
 _msgspec_json_decoder = msgspec.json.Decoder(dec_hook=default_deserializer)
 _msgspec_msgpack_encoder = msgspec.msgpack.Encoder(enc_hook=default_serializer)
 _msgspec_msgpack_decoder = msgspec.msgpack.Decoder(dec_hook=default_deserializer)
```

### Comparing `litestar-2.8.3/litestar/static_files/base.py` & `litestar-2.9.0/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/static_files/config.py` & `litestar-2.9.0/litestar/static_files/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.file_system import BaseLocalFileSystem
 from litestar.handlers import asgi, get, head
 from litestar.response.file import ASGIFileResponse  # noqa: TCH001
 from litestar.router import Router
 from litestar.static_files.base import StaticFiles
-from litestar.types import Empty
 from litestar.utils import normalize_path, warn_deprecation
 
 __all__ = ("StaticFilesConfig",)
 
 if TYPE_CHECKING:
     from litestar.datastructures import CacheControlHeader
     from litestar.handlers.asgi_handlers import ASGIRouteHandler
@@ -115,15 +114,15 @@
     name: str = "static",
     after_request: AfterRequestHookHandler | None = None,
     after_response: AfterResponseHookHandler | None = None,
     before_request: BeforeRequestHookHandler | None = None,
     cache_control: CacheControlHeader | None = None,
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: list[Guard] | None = None,
-    include_in_schema: bool | EmptyType = Empty,
+    include_in_schema: bool | EmptyType = False,
     middleware: Sequence[Middleware] | None = None,
     opt: dict[str, Any] | None = None,
     security: Sequence[SecurityRequirement] | None = None,
     tags: Sequence[str] | None = None,
     router_class: type[Router] = Router,
     resolve_symlinks: bool = True,
 ) -> Router:
```

### Comparing `litestar-2.8.3/litestar/stores/base.py` & `litestar-2.9.0/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/stores/file.py` & `litestar-2.9.0/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/stores/memory.py` & `litestar-2.9.0/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/stores/redis.py` & `litestar-2.9.0/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/stores/registry.py` & `litestar-2.9.0/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/template/base.py` & `litestar-2.9.0/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/template/config.py` & `litestar-2.9.0/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/testing/__init__.py` & `litestar-2.9.0/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/testing/helpers.py` & `litestar-2.9.0/litestar/testing/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
             when the ASGI send function is called.
         cache_control: A ``cache-control`` header of type
             :class:`CacheControlHeader <litestar.datastructures.CacheControlHeader>` to add to route handlers of
             this app. Can be overridden by route handlers.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
-        cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
+        cors_config: If set, configures CORS handling for the application.
         csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
         debug: If ``True``, app errors rendered as HTML with a stack trace.
         dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
         dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
             validation of request data.
         etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             Can be overridden by route handlers.
@@ -426,15 +426,15 @@
         before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
             when the ASGI send function is called.
         cache_control: A ``cache-control`` header of type
             :class:`CacheControlHeader <litestar.datastructures.CacheControlHeader>` to add to route handlers of
             this app. Can be overridden by route handlers.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
-        cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
+        cors_config: If set, configures CORS handling for the application.
         csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
         debug: If ``True``, app errors rendered as HTML with a stack trace.
         dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
         dto: :class:`AbstractDTO <.dto.base_dto.AbstractDTO>` to use for (de)serializing and
             validation of request data.
         etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             Can be overridden by route handlers.
```

### Comparing `litestar-2.8.3/litestar/testing/life_span_handler.py` & `litestar-2.9.0/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/testing/request_factory.py` & `litestar-2.9.0/litestar/testing/request_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,17 @@
                     cast("dict[str, Any]", data), files=files or [], boundary=None
                 )
             else:
                 encoding_headers, stream = encode_urlencoded_data(decode_json(value=encode_json(data)))
             headers.update(encoding_headers)
             for chunk in stream:
                 body += chunk
-        ScopeState.from_scope(scope).body = body
+        scope_state = ScopeState.from_scope(scope)
+        scope_state.body = body
+        scope_state.exception_handlers = scope["route_handler"].resolve_exception_handlers()
         self._create_cookie_header(headers, cookies)
         scope["headers"] = self._build_headers(headers)
         return Request(scope=scope)
 
     def get(
         self,
         path: str = "/",
```

### Comparing `litestar-2.8.3/litestar/testing/transport.py` & `litestar-2.9.0/litestar/testing/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                 }
                 portal.call(
                     self.client.app,
                     scope,
                     self.create_receive(request=request, context=context),
                     self.create_send(request=request, context=context),
                 )
-        except BaseException as exc:  # noqa: BLE001
+        except BaseException as exc:
             if self.raise_server_exceptions:
                 raise exc
             return Response(
                 status_code=HTTP_500_INTERNAL_SERVER_ERROR, headers=[], stream=ByteStream(b""), request=request
             )
         else:
             if not context["response_started"]:  # pragma: no cover
```

### Comparing `litestar-2.8.3/litestar/testing/websocket_test_session.py` & `litestar-2.9.0/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/testing/client/__init__.py` & `litestar-2.9.0/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/testing/client/async_client.py` & `litestar-2.9.0/litestar/testing/client/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from contextlib import AsyncExitStack
-from typing import TYPE_CHECKING, Any, Generic, Mapping, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, Mapping, Sequence, TypeVar
+from urllib.parse import urljoin
 
 from httpx import USE_CLIENT_DEFAULT, AsyncClient, Response
 
 from litestar import HttpMethod
 from litestar.testing.client.base import BaseTestClient
 from litestar.testing.life_span_handler import LifeSpanHandler
-from litestar.testing.transport import TestClientTransport
+from litestar.testing.transport import ConnectionUpgradeExceptionError, TestClientTransport
 from litestar.types import AnyIOBackend, ASGIApp
 
 if TYPE_CHECKING:
     from httpx._client import UseClientDefault
     from httpx._types import (
         AuthTypes,
         CookieTypes,
@@ -23,14 +24,15 @@
         RequestFiles,
         TimeoutTypes,
         URLTypes,
     )
     from typing_extensions import Self
 
     from litestar.middleware.session.base import BaseBackendConfig
+    from litestar.testing.websocket_test_session import WebSocketTestSession
 
 
 T = TypeVar("T", bound=ASGIApp)
 
 
 class AsyncTestClient(AsyncClient, BaseTestClient, Generic[T]):  # type: ignore[misc]
     lifespan_handler: LifeSpanHandler[Any]
@@ -464,14 +466,67 @@
             cookies=cookies,
             auth=auth,
             follow_redirects=follow_redirects,
             timeout=timeout,
             extensions=None if extensions is None else dict(extensions),
         )
 
+    async def websocket_connect(
+        self,
+        url: str,
+        subprotocols: Sequence[str] | None = None,
+        params: QueryParamTypes | None = None,
+        headers: HeaderTypes | None = None,
+        cookies: CookieTypes | None = None,
+        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
+        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        extensions: Mapping[str, Any] | None = None,
+    ) -> WebSocketTestSession:
+        """Sends a GET request to establish a websocket connection.
+
+        Args:
+            url: Request URL.
+            subprotocols: Websocket subprotocols.
+            params: Query parameters.
+            headers: Request headers.
+            cookies: Request cookies.
+            auth: Auth headers.
+            follow_redirects: Whether to follow redirects.
+            timeout: Request timeout.
+            extensions: Dictionary of ASGI extensions.
+
+        Returns:
+            A `WebSocketTestSession <litestar.testing.WebSocketTestSession>` instance.
+        """
+        url = urljoin("ws://testserver", url)
+        default_headers: dict[str, str] = {}
+        default_headers.setdefault("connection", "upgrade")
+        default_headers.setdefault("sec-websocket-key", "testserver==")
+        default_headers.setdefault("sec-websocket-version", "13")
+        if subprotocols is not None:
+            default_headers.setdefault("sec-websocket-protocol", ", ".join(subprotocols))
+        try:
+            await AsyncClient.request(
+                self,
+                "GET",
+                url,
+                headers={**dict(headers or {}), **default_headers},  # type: ignore[misc]
+                params=params,
+                cookies=cookies,
+                auth=auth,
+                follow_redirects=follow_redirects,
+                timeout=timeout,
+                extensions=None if extensions is None else dict(extensions),
+            )
+        except ConnectionUpgradeExceptionError as exc:
+            return exc.session
+
+        raise RuntimeError("Expected WebSocket upgrade")  # pragma: no cover
+
     async def get_session_data(self) -> dict[str, Any]:
         """Get session data.
 
         Returns:
             A dictionary containing session data.
 
         Examples:
```

### Comparing `litestar-2.8.3/litestar/testing/client/base.py` & `litestar-2.9.0/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/testing/client/sync_client.py` & `litestar-2.9.0/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/__init__.py` & `litestar-2.9.0/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/asgi_types.py` & `litestar-2.9.0/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/builtin_types.py` & `litestar-2.9.0/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/callable_types.py` & `litestar-2.9.0/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/composite_types.py` & `litestar-2.9.0/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/file_types.py` & `litestar-2.9.0/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/helper_types.py` & `litestar-2.9.0/litestar/types/helper_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/internal_types.py` & `litestar-2.9.0/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/protocols.py` & `litestar-2.9.0/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/types/serialization.py` & `litestar-2.9.0/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/__init__.py` & `litestar-2.9.0/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/compat.py` & `litestar-2.9.0/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/dataclass.py` & `litestar-2.9.0/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/deprecation.py` & `litestar-2.9.0/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/helpers.py` & `litestar-2.9.0/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/module_loader.py` & `litestar-2.9.0/litestar/utils/module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/path.py` & `litestar-2.9.0/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/predicates.py` & `litestar-2.9.0/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/sequence.py` & `litestar-2.9.0/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/signature.py` & `litestar-2.9.0/litestar/utils/signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/sync.py` & `litestar-2.9.0/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/typing.py` & `litestar-2.9.0/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/version.py` & `litestar-2.9.0/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/warnings.py` & `litestar-2.9.0/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/scope/__init__.py` & `litestar-2.9.0/litestar/utils/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/litestar/utils/scope/state.py` & `litestar-2.9.0/litestar/utils/scope/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from litestar.utils.empty import value_or_default
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar.datastructures import URL, Accept, Headers
     from litestar.types.asgi_types import Scope
+    from litestar.types.composite_types import ExceptionHandlersMap
 
 CONNECTION_STATE_KEY: Final = "_ls_connection_state"
 
 
 @dataclass
 class ScopeState:
     """An object for storing connection state.
@@ -29,67 +30,73 @@
         "base_url",
         "body",
         "content_type",
         "cookies",
         "csrf_token",
         "dependency_cache",
         "do_cache",
+        "exception_handlers",
         "flash_messages",
         "form",
         "headers",
         "is_cached",
         "json",
         "log_context",
         "msgpack",
         "parsed_query",
         "response_compressed",
+        "response_started",
         "session_id",
         "url",
         "_compat_ns",
     )
 
     def __init__(self) -> None:
         self.accept = Empty
         self.base_url = Empty
         self.body = Empty
         self.content_type = Empty
         self.cookies = Empty
         self.csrf_token = Empty
         self.dependency_cache = Empty
         self.do_cache = Empty
+        self.exception_handlers = Empty
         self.form = Empty
         self.flash_messages = []
         self.headers = Empty
         self.is_cached = Empty
         self.json = Empty
         self.log_context: dict[str, Any] = {}
         self.msgpack = Empty
         self.parsed_query = Empty
         self.response_compressed = Empty
+        self.response_started = False
         self.session_id = Empty
         self.url = Empty
         self._compat_ns: dict[str, Any] = {}
 
     accept: Accept | EmptyType
     base_url: URL | EmptyType
     body: bytes | EmptyType
     content_type: tuple[str, dict[str, str]] | EmptyType
     cookies: dict[str, str] | EmptyType
     csrf_token: str | EmptyType
     dependency_cache: dict[str, Any] | EmptyType
     do_cache: bool | EmptyType
+    exception_handlers: ExceptionHandlersMap | EmptyType
     form: dict[str, str | list[str]] | EmptyType
     flash_messages: list[dict[str, str]]
     headers: Headers | EmptyType
     is_cached: bool | EmptyType
     json: Any | EmptyType
     log_context: dict[str, Any]
     msgpack: Any | EmptyType
     parsed_query: tuple[tuple[str, str], ...] | EmptyType
     response_compressed: bool | EmptyType
+    response_started: bool
     session_id: str | None | EmptyType
     url: URL | EmptyType
     _compat_ns: dict[str, Any]
 
     @classmethod
     def from_scope(cls, scope: Scope) -> Self:
         """Create a new `ConnectionState` object from a scope.
```

### Comparing `litestar-2.8.3/tests/conftest.py` & `litestar-2.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/docker_service_fixtures.py` & `litestar-2.9.0/tests/docker_service_fixtures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/helpers.py` & `litestar-2.9.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/models.py` & `litestar-2.9.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_advanced_alchemy.py` & `litestar-2.9.0/tests/e2e/test_advanced_alchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_exception_handlers.py` & `litestar-2.9.0/tests/e2e/test_exception_handlers/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_option_requests.py` & `litestar-2.9.0/tests/e2e/test_option_requests.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_regular_handler_under_asgi_mount_path.py` & `litestar-2.9.0/tests/e2e/test_regular_handler_under_asgi_mount_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_response_caching.py` & `litestar-2.9.0/tests/e2e/test_response_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_router_registration.py` & `litestar-2.9.0/tests/e2e/test_router_registration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_starlette_responses.py` & `litestar-2.9.0/tests/e2e/test_starlette_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_dependency_validation.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_dependency_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_classes.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_injection_of_classes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_inter_dependencies.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_inter_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_request_local_caching.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_request_local_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py` & `litestar-2.9.0/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_request.py` & `litestar-2.9.0/tests/e2e/test_life_cycle_hooks/test_after_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_response.py` & `litestar-2.9.0/tests/e2e/test_life_cycle_hooks/test_after_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,40 @@
-from typing import TYPE_CHECKING, Dict
+from unittest.mock import MagicMock, call
 
 import pytest
 
 from litestar import Controller, Request, Router, get
 from litestar.status_codes import HTTP_200_OK
 from litestar.testing import create_test_client
 
-state: Dict[str, str] = {}
 
-if TYPE_CHECKING:
-    from litestar.types import AfterResponseHookHandler
+@pytest.mark.parametrize("sync", [True, False])
+@pytest.mark.parametrize("layer", ["app", "router", "controller", "handler"])
+def test_after_response_resolution(layer: str, sync: bool) -> None:
+    mock = MagicMock()
 
+    if sync:
 
-def create_sync_test_handler(msg: str) -> "AfterResponseHookHandler":
-    def handler(_: Request) -> None:
-        state["msg"] = msg
+        def handler(_: Request) -> None:  # pyright: ignore
+            mock(layer)
 
-    return handler
+    else:
 
+        async def handler(_: Request) -> None:  # type: ignore[misc]
+            mock(layer)
 
-def create_async_test_handler(msg: str) -> "AfterResponseHookHandler":
-    async def handler(_: Request) -> None:
-        state["msg"] = msg
+    class MyController(Controller):
+        path = "/controller"
+        after_response = handler if layer == "controller" else None
 
-    return handler
+        @get("/", after_response=handler if layer == "handler" else None)
+        def my_handler(self) -> None:
+            return None
 
+    router = Router(
+        path="/router", route_handlers=[MyController], after_response=handler if layer == "router" else None
+    )
 
-@pytest.mark.parametrize("layer", ["app", "router", "controller", "handler"])
-def test_after_response_resolution(layer: str) -> None:
-    for handler in (create_sync_test_handler(layer), create_async_test_handler(layer)):
-        state.pop("msg", None)
-
-        class MyController(Controller):
-            path = "/controller"
-            after_response = handler if layer == "controller" else None
-
-            @get("/", after_response=handler if layer == "handler" else None)
-            def my_handler(self) -> None:
-                return None
-
-        router = Router(
-            path="/router", route_handlers=[MyController], after_response=handler if layer == "router" else None
-        )
-
-        with create_test_client(route_handlers=[router], after_response=handler if layer == "app" else None) as client:
-            response = client.get("/router/controller/")
-            assert response.status_code == HTTP_200_OK
-            assert state["msg"] == layer
+    with create_test_client(route_handlers=[router], after_response=handler if layer == "app" else None) as client:
+        response = client.get("/router/controller/")
+        assert response.status_code == HTTP_200_OK
+        assert all(c == call(layer) for c in mock.call_args_list)
```

### Comparing `litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_before_request.py` & `litestar-2.9.0/tests/e2e/test_life_cycle_hooks/test_before_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_logging/test_structlog_to_file.py` & `litestar-2.9.0/tests/e2e/test_logging/test_structlog_to_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_middleware/test_middleware_send_wrapper_called_on_error.py` & `litestar-2.9.0/tests/e2e/test_middleware/test_middleware_send_wrapper_called_on_error.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_openapi/test_spec_headers.py` & `litestar-2.9.0/tests/e2e/test_openapi/test_spec_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/conftest.py` & `litestar-2.9.0/tests/e2e/test_routing/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/test_asset_url_path.py` & `litestar-2.9.0/tests/e2e/test_routing/test_asset_url_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/test_path_mounting.py` & `litestar-2.9.0/tests/e2e/test_routing/test_path_mounting.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/test_path_resolution.py` & `litestar-2.9.0/tests/e2e/test_routing/test_path_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/test_route_indexing.py` & `litestar-2.9.0/tests/e2e/test_routing/test_route_indexing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/test_route_reverse.py` & `litestar-2.9.0/tests/e2e/test_routing/test_route_reverse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/e2e/test_routing/test_validations.py` & `litestar-2.9.0/tests/e2e/test_routing/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_cache_control_headers.py` & `litestar-2.9.0/tests/examples/test_cache_control_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_exceptions.py` & `litestar-2.9.0/tests/examples/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_lifecycle_hooks.py` & `litestar-2.9.0/tests/examples/test_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_request_data.py` & `litestar-2.9.0/tests/examples/test_request_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_routing.py` & `litestar-2.9.0/tests/examples/test_routing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_startup_and_shutdown.py` & `litestar-2.9.0/tests/examples/test_startup_and_shutdown.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_static_files.py` & `litestar-2.9.0/tests/examples/test_static_files.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_stores.py` & `litestar-2.9.0/tests/examples/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_todo_app.py` & `litestar-2.9.0/tests/examples/test_todo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_using_session_auth.py` & `litestar-2.9.0/tests/examples/test_using_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_application_hooks/test_application_after_exception_hook.py` & `litestar-2.9.0/tests/examples/test_application_hooks/test_application_after_exception_hook.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_application_hooks/test_lifespan_manager.py` & `litestar-2.9.0/tests/examples/test_application_hooks/test_lifespan_manager.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_application_state/test_using_application_state.py` & `litestar-2.9.0/tests/examples/test_application_state/test_using_application_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_contrib/test_piccolo_orm.py` & `litestar-2.9.0/tests/examples/test_contrib/test_piccolo_orm.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py` & `litestar-2.9.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py` & `litestar-2.9.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py` & `litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py` & `litestar-2.9.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_data_transfer_objects/test_defining_dtos_on_layers.py` & `litestar-2.9.0/tests/examples/test_data_transfer_objects/test_defining_dtos_on_layers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_problem_statement.py` & `litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_problem_statement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private_override.py` & `litestar-2.9.0/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private_override.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_dto/test_example_apps.py` & `litestar-2.9.0/tests/examples/test_dto/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_dto/test_tutorial.py` & `litestar-2.9.0/tests/examples/test_dto/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_middleware/test_abstract_middleware.py` & `litestar-2.9.0/tests/examples/test_middleware/test_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_middleware/test_logging_middleware.py` & `litestar-2.9.0/tests/examples/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_middleware/test_session_middleware.py` & `litestar-2.9.0/tests/examples/test_middleware/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_openapi/test_openapi.py` & `litestar-2.9.0/tests/examples/test_openapi/test_openapi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_openapi/test_plugins.py` & `litestar-2.9.0/tests/examples/test_openapi/test_plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_pagination/test_using_classic_pagination.py` & `litestar-2.9.0/tests/examples/test_pagination/test_using_classic_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_pagination/test_using_cursor_pagination.py` & `litestar-2.9.0/tests/examples/test_pagination/test_using_cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_pagination/test_using_offset_pagination.py` & `litestar-2.9.0/tests/examples/test_pagination/test_using_offset_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_parameters/test_header_and_cookies_parameters.py` & `litestar-2.9.0/tests/examples/test_parameters/test_header_and_cookies_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_parameters/test_layered_parameters.py` & `litestar-2.9.0/tests/examples/test_parameters/test_layered_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_parameters/test_path_parameters.py` & `litestar-2.9.0/tests/examples/test_parameters/test_path_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_parameters/test_query_parameters.py` & `litestar-2.9.0/tests/examples/test_parameters/test_query_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py` & `litestar-2.9.0/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_responses/test_background_tasks.py` & `litestar-2.9.0/tests/examples/test_responses/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_responses/test_response_cookies.py` & `litestar-2.9.0/tests/examples/test_responses/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_responses/test_response_headers.py` & `litestar-2.9.0/tests/examples/test_responses/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_auth.py` & `litestar-2.9.0/tests/examples/test_security/test_jwt/test_using_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py` & `litestar-2.9.0/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py` & `litestar-2.9.0/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_templating/test_engine_instance.py` & `litestar-2.9.0/tests/examples/test_templating/test_engine_instance.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_templating/test_returning_templates.py` & `litestar-2.9.0/tests/examples/test_templating/test_returning_templates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/examples/test_templating/test_template_functions.py` & `litestar-2.9.0/tests/examples/test_templating/test_template_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/conftest.py` & `litestar-2.9.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_app.py` & `litestar-2.9.0/tests/unit/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from unittest.mock import MagicMock, Mock, PropertyMock
 
 import pytest
 from click import Group
 from pytest import MonkeyPatch
 
 from litestar import Litestar, MediaType, Request, Response, get
+from litestar._asgi.asgi_router import ASGIRouter
 from litestar.config.app import AppConfig, ExperimentalFeatures
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.contrib.sqlalchemy.plugins import SQLAlchemySerializationPlugin
 from litestar.datastructures import MutableScopeHeaders, State
 from litestar.events.emitter import SimpleEventEmitter
 from litestar.exceptions import (
     ImproperlyConfiguredException,
@@ -168,14 +169,15 @@
         property_mocks.append((field.name, property_mock))
         monkeypatch.setattr(type(app_config_object), field.name, property_mock, raising=False)
 
     # Things that we don't actually need to call for this test
     monkeypatch.setattr(Litestar, "register", MagicMock())
     monkeypatch.setattr(Litestar, "_create_asgi_handler", MagicMock())
     monkeypatch.setattr(Router, "__init__", MagicMock())
+    monkeypatch.setattr(ASGIRouter, "__init__", MagicMock(return_value=None))
 
     # instantiates the app with an `on_app_config` that returns our patched `AppConfig` object.
     Litestar(on_app_init=[MagicMock(return_value=app_config_object)])
 
     # this ensures that each of the properties of the `AppConfig` object have been accessed within `Litestar.__init__()`
     for name, mock in property_mocks:
         assert mock.called, f"expected {name} to be called"
```

### Comparing `litestar-2.8.3/tests/unit/test_asgi_router.py` & `litestar-2.9.0/tests/unit/test_asgi/test_asgi_router.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from typing import TYPE_CHECKING, AsyncGenerator, Callable
 from unittest.mock import AsyncMock, MagicMock, call
 
 import anyio
 import pytest
 from pytest_mock import MockerFixture
 
-from litestar import Litestar, asgi
+from litestar import Litestar, asgi, get
 from litestar._asgi.asgi_router import ASGIRouter
-from litestar.exceptions import ImproperlyConfiguredException
+from litestar.exceptions import ImproperlyConfiguredException, NotFoundException
 from litestar.testing import TestClient, create_test_client
+from litestar.types.empty import Empty
 from litestar.utils.helpers import get_exception_group
+from litestar.utils.scope.state import ScopeState
 
 if TYPE_CHECKING:
     from contextlib import AbstractAsyncContextManager
 
     from litestar.types import Receive, Scope, Send
 
 _ExceptionGroup = get_exception_group()
@@ -221,7 +223,51 @@
     assert receive.call_count == 2
     send.assert_has_calls(
         [
             call({"type": "lifespan.startup.complete"}),
             call({"type": "lifespan.shutdown.failed", "message": mock_format_exc.return_value}),
         ]
     )
+
+
+async def test_asgi_router_set_exception_handlers_in_scope_routing_error(scope: Scope) -> None:
+    # If routing fails, the exception handlers that are set in scope should be the ones
+    # defined on the app instance.
+
+    app_exception_handlers_mock = MagicMock()
+    handler_exception_handlers_mock = MagicMock()
+
+    @get(exception_handlers={RuntimeError: handler_exception_handlers_mock})
+    async def handler() -> None:
+        return None
+
+    app = Litestar(route_handlers=[handler], exception_handlers={RuntimeError: app_exception_handlers_mock})
+    scope["path"] = "/nowhere-to-be-found"
+    with pytest.raises(NotFoundException):
+        await app.asgi_router(scope, AsyncMock(), AsyncMock())
+
+    state = ScopeState.from_scope(scope)
+    assert state.exception_handlers is not Empty
+    assert state.exception_handlers[RuntimeError] is app_exception_handlers_mock
+
+
+async def test_asgi_router_set_exception_handlers_in_scope_successful_routing(
+    scope: Scope, monkeypatch: pytest.MonkeyPatch
+) -> None:
+    # if routing is successful, the exception handlers that are set in scope should be the ones
+    # resolved from the handler.
+
+    app_exception_handlers_mock = MagicMock()
+    handler_exception_handlers_mock = MagicMock()
+
+    @get(exception_handlers={TypeError: handler_exception_handlers_mock})
+    async def handler() -> None:
+        return None
+
+    app = Litestar(route_handlers=[handler], exception_handlers={RuntimeError: app_exception_handlers_mock})
+    router = app.asgi_router
+    scope["path"] = "/"
+    await router(scope, AsyncMock(), AsyncMock())
+    state = ScopeState.from_scope(scope)
+    assert state.exception_handlers is not Empty
+    assert state.exception_handlers[RuntimeError] is app_exception_handlers_mock
+    assert state.exception_handlers[TypeError] is handler_exception_handlers_mock
```

### Comparing `litestar-2.8.3/tests/unit/test_background_tasks.py` & `litestar-2.9.0/tests/unit/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_concurrency.py` & `litestar-2.9.0/tests/unit/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_controller.py` & `litestar-2.9.0/tests/unit/test_controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_data_extractors.py` & `litestar-2.9.0/tests/unit/test_data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_di.py` & `litestar-2.9.0/tests/unit/test_di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_events.py` & `litestar-2.9.0/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_exceptions.py` & `litestar-2.9.0/tests/unit/test_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from litestar.exceptions import (
     HTTPException,
     ImproperlyConfiguredException,
     LitestarException,
     MissingDependencyException,
     ValidationException,
 )
-from litestar.middleware.exceptions.middleware import create_exception_response
+from litestar.exceptions.responses import create_exception_response
 from litestar.status_codes import HTTP_400_BAD_REQUEST, HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.testing import RequestFactory, create_test_client
 
 
 class CustomLitestarException(LitestarException):
     detail = "Custom Exception"
```

### Comparing `litestar-2.8.3/tests/unit/test_file_system.py` & `litestar-2.9.0/tests/unit/test_file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_guards.py` & `litestar-2.9.0/tests/unit/test_guards.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_pagination.py` & `litestar-2.9.0/tests/unit/test_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_params.py` & `litestar-2.9.0/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_parsers.py` & `litestar-2.9.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_request_class_resolution.py` & `litestar-2.9.0/tests/unit/test_request_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response_class_resolution.py` & `litestar-2.9.0/tests/unit/test_response_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_stores.py` & `litestar-2.9.0/tests/unit/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_typing.py` & `litestar-2.9.0/tests/unit/test_typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_websocket_class_resolution.py` & `litestar-2.9.0/tests/unit/test_websocket_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_channels/conftest.py` & `litestar-2.9.0/tests/unit/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_channels/test_backends.py` & `litestar-2.9.0/tests/unit/test_channels/test_backends.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_channels/test_plugin.py` & `litestar-2.9.0/tests/unit/test_channels/test_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_channels/test_subscriber.py` & `litestar-2.9.0/tests/unit/test_channels/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/__init__.py` & `litestar-2.9.0/tests/unit/test_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/conftest.py` & `litestar-2.9.0/tests/unit/test_cli/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_cli.py` & `litestar-2.9.0/tests/unit/test_cli/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,8 +85,8 @@
 
     importlib.reload(litestar.cli._utils)
     cli_command = importlib.reload(litestar.cli.main).litestar_group
 
     result = runner.invoke(cli_command, f"--app={app_file.stem}:app custom-group custom-command")
 
     assert result.exit_code == 0
-    mock_command_callback.assert_called_once_with()
+    mock_command_callback.assert_called_once()
```

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_cli_plugin.py` & `litestar-2.9.0/tests/unit/test_cli/test_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_core_commands.py` & `litestar-2.9.0/tests/unit/test_cli/test_core_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_env_resolution.py` & `litestar-2.9.0/tests/unit/test_cli/test_env_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_schema_commands.py` & `litestar-2.9.0/tests/unit/test_cli/test_schema_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_session_commands.py` & `litestar-2.9.0/tests/unit/test_cli/test_session_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_cli/test_ssl.py` & `litestar-2.9.0/tests/unit/test_cli/test_ssl.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_connection/test_base.py` & `litestar-2.9.0/tests/unit/test_connection/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_connection/test_connection_caching.py` & `litestar-2.9.0/tests/unit/test_connection/test_connection_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_connection/test_request.py` & `litestar-2.9.0/tests/unit/test_connection/test_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_connection/test_websocket.py` & `litestar-2.9.0/tests/unit/test_connection/test_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/conftest.py` & `litestar-2.9.0/tests/unit/test_contrib/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_minijinja.py` & `litestar-2.9.0/tests/unit/test_contrib/test_minijinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_msgspec.py` & `litestar-2.9.0/tests/unit/test_contrib/test_msgspec.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_opentelemetry.py` & `litestar-2.9.0/tests/unit/test_contrib/test_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_prometheus.py` & `litestar-2.9.0/tests/unit/test_contrib/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_repository.py` & `litestar-2.9.0/tests/unit/test_contrib/test_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_sqlalchemy.py` & `litestar-2.9.0/tests/unit/test_contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py` & `litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_plugin.py` & `litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py` & `litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_signature.py` & `litestar-2.9.0/tests/unit/test_contrib/test_attrs/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_request.py` & `litestar-2.9.0/tests/unit/test_contrib/test_htmx/test_htmx_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_response.py` & `litestar-2.9.0/tests/unit/test_contrib/test_htmx/test_htmx_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/endpoints.py` & `litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py` & `litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/tables.py` & `litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/tables.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py` & `litestar-2.9.0/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/conftest.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/models.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_dto.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_integration.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, List
+from unittest.mock import ANY
 
 import pydantic as pydantic_v2
 import pytest
 from pydantic import v1 as pydantic_v1
 from typing_extensions import Annotated
 
 from litestar import post
@@ -131,15 +132,15 @@
         assert extra == [
             {
                 "type": "value_error",
                 "loc": ["user_id"],
                 "msg": "Value error, user id must be greater than 0",
                 "input": -1,
                 "ctx": {"error": "ValueError"},
-                "url": "https://errors.pydantic.dev/2.6/v/value_error",
+                "url": ANY,
             }
         ]
 
 
 def test_signature_model_invalid_input(base_model: BaseModelType, pydantic_version: PydanticVersion) -> None:
     class OtherChild(base_model):  # type: ignore[misc, valid-type]
         val: List[int]
```

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_openapi.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_openapi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     encode_json,
     encode_msgpack,
     get_serializer,
 )
 
 from . import PydanticVersion
 
+TODAY = datetime.date.today()
+
 
 class CustomStr(str):
     pass
 
 
 class CustomInt(int):
     pass
@@ -80,15 +82,15 @@
     bytesize: pydantic_v1.ByteSize
     secret_str: pydantic_v1.SecretStr
     secret_bytes: pydantic_v1.SecretBytes
     payment_card_number: pydantic_v1.PaymentCardNumber
 
     constr: pydantic_v1.constr(min_length=1)  # type: ignore[valid-type]
     conbytes: pydantic_v1.conbytes(min_length=1)  # type: ignore[valid-type]
-    condate: pydantic_v1.condate(ge=datetime.date.today())  # type: ignore[valid-type]
+    condate: pydantic_v1.condate(ge=TODAY)  # type: ignore[valid-type]
     condecimal: pydantic_v1.condecimal(ge=Decimal("1"))  # type: ignore[valid-type]
     confloat: pydantic_v1.confloat(ge=0)  # type: ignore[valid-type]
 
     conint: pydantic_v1.conint(ge=0)  # type: ignore[valid-type]
 
     url: pydantic_v1.AnyUrl
     http_url: pydantic_v1.HttpUrl
@@ -108,15 +110,15 @@
     bytesize: pydantic_v2.ByteSize
     secret_str: pydantic_v2.SecretStr
     secret_bytes: pydantic_v2.SecretBytes
     payment_card_number: pydantic_v2.PaymentCardNumber
 
     constr: pydantic_v2.constr(min_length=1)  # type: ignore[valid-type]
     conbytes: pydantic_v2.conbytes(min_length=1)  # type: ignore[valid-type]
-    condate: pydantic_v2.condate(ge=datetime.date.today())  # type: ignore[valid-type]
+    condate: pydantic_v2.condate(ge=TODAY)  # type: ignore[valid-type]
     condecimal: pydantic_v2.condecimal(ge=Decimal("1"))  # type: ignore[valid-type]
     confloat: pydantic_v2.confloat(ge=0)  # type: ignore[valid-type]
 
     conint: pydantic_v2.conint(ge=0)  # type: ignore[valid-type]
 
     url: pydantic_v2.AnyUrl
     http_url: pydantic_v2.HttpUrl
@@ -140,15 +142,15 @@
             color=ColorV1("rgb(255, 255, 255)"),
             bytesize=pydantic_v1.ByteSize(100),
             secret_str=pydantic_v1.SecretStr("hello"),
             secret_bytes=pydantic_v1.SecretBytes(b"hello"),
             payment_card_number=pydantic_v1.PaymentCardNumber("4000000000000002"),
             constr="hello",
             conbytes=b"hello",
-            condate=datetime.date.today(),
+            condate=TODAY,
             condecimal=Decimal("3.14"),
             confloat=1.0,
             conset={1},
             confrozenset=frozenset([1]),
             conint=1,
             conlist=[1],
             url="some://example.org/",  # type: ignore[arg-type]
@@ -161,15 +163,15 @@
         color=ColorV2("rgb(255, 255, 255)"),
         bytesize=pydantic_v2.ByteSize(100),
         secret_str=pydantic_v2.SecretStr("hello"),
         secret_bytes=pydantic_v2.SecretBytes(b"hello"),
         payment_card_number=pydantic_v2.PaymentCardNumber("4000000000000002"),
         constr="hello",
         conbytes=b"hello",
-        condate=datetime.date.today(),
+        condate=TODAY,
         condecimal=Decimal("3.14"),
         confloat=1.0,
         conset={1},
         confrozenset=frozenset([1]),
         conint=1,
         conlist=[1],
         url="some://example.org/",  # type: ignore[arg-type]
@@ -186,15 +188,15 @@
         ("color", "white"),
         ("bytesize", 100),
         ("secret_str", "**********"),
         ("secret_bytes", "**********"),
         ("payment_card_number", "4000000000000002"),
         ("constr", "hello"),
         ("conbytes", b"hello"),
-        ("condate", datetime.date.today().isoformat()),
+        ("condate", TODAY.isoformat()),
         ("condecimal", 3.14),
         ("conset", {1}),
         ("confrozenset", frozenset([1])),
         ("conint", 1),
         ("url", "some://example.org/"),
         ("http_url", "http://example.org/"),
     ],
```

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_utils.py` & `litestar-2.9.0/tests/unit/test_contrib/test_pydantic/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_datastructures/test_cookie.py` & `litestar-2.9.0/tests/unit/test_datastructures/test_cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_datastructures/test_headers.py` & `litestar-2.9.0/tests/unit/test_datastructures/test_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_datastructures/test_multi_dicts.py` & `litestar-2.9.0/tests/unit/test_datastructures/test_multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_datastructures/test_state.py` & `litestar-2.9.0/tests/unit/test_datastructures/test_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_datastructures/test_upload_file.py` & `litestar-2.9.0/tests/unit/test_datastructures/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_datastructures/test_url.py` & `litestar-2.9.0/tests/unit/test_datastructures/test_url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/conftest.py` & `litestar-2.9.0/tests/unit/test_dto/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_integration.py` & `litestar-2.9.0/tests/unit/test_dto/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_base_dto.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_dataclass_dto.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_dataclass_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_integration.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -999,7 +999,62 @@
 """
     )
     openapi = cast("Litestar", module.app).openapi_schema
     schema = openapi.components.schemas["WithCount[litestar.dto._backend.GetUsersUserResponseBody]"]
     assert not_none(schema.properties).keys() == {"count", "data"}
     model_schema = openapi.components.schemas["GetUsersUserResponseBody"]
     assert not_none(model_schema.properties).keys() == {"id", "name"}
+
+
+def test_openapi_schema_for_dto_includes_body_examples(create_module: Callable[[str], ModuleType]) -> None:
+    module = create_module(
+        """
+from dataclasses import dataclass
+from uuid import UUID
+
+from typing_extensions import Annotated
+
+from litestar import Litestar, post
+from litestar.dto import DataclassDTO
+from litestar.openapi.spec import Example
+from litestar.params import Body
+
+
+@dataclass
+class Item:
+    id: UUID
+    name: str
+
+
+body = Body(
+    title="Create item",
+    description="Create a new item.",
+    examples=[
+        Example(
+            summary="Post is Ok",
+            value={
+                "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
+                "name": "Swatch",
+            },
+        )
+    ],
+)
+
+
+@post()
+async def create_item(data: Annotated[Item, body]) -> Item:
+    return data
+
+
+@post("dto", dto=DataclassDTO[Item])
+async def create_item_with_dto(data: Annotated[Item, body]) -> Item:
+    return data
+
+
+app = Litestar(route_handlers=[create_item, create_item_with_dto])
+"""
+    )
+
+    openapi_schema = module.app.openapi_schema
+    item_schema = openapi_schema.components.schemas["Item"]
+    item_with_dto_schema = openapi_schema.components.schemas["CreateItemWithDtoItemRequestBody"]
+    assert item_schema.examples == item_with_dto_schema.examples
```

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_utils.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_backends.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/test_backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ruff: noqa: UP006,UP007
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from types import ModuleType
-from typing import TYPE_CHECKING, Callable, List, Optional
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional
 from unittest.mock import MagicMock
 
 import pytest
 from msgspec import Meta, Struct, to_builtins
 
 from litestar import Litestar, Request, get, post
 from litestar._openapi.schema_generation import SchemaCreator
@@ -36,32 +36,40 @@
 
 
 @dataclass
 class DC:
     a: int
     nested: NestedDC
     nested_list: List[NestedDC]
+    nested_mapping: Dict[str, NestedDC]
     b: str = field(default="b")
     c: List[int] = field(default_factory=list)
     optional: Optional[str] = None
 
 
 DESTRUCTURED = {
     "a": 1,
     "b": "b",
     "c": [],
     "nested": {"a": 1, "b": "two"},
     "nested_list": [{"a": 1, "b": "two"}],
+    "nested_mapping": {"a": {"a": 1, "b": "two"}},
     "optional": None,
 }
-RAW = b'{"a":1,"nested":{"a":1,"b":"two"},"nested_list":[{"a":1,"b":"two"}],"b":"b","c":[],"optional":null}'
-COLLECTION_RAW = (
-    b'[{"a":1,"nested":{"a":1,"b":"two"},"nested_list":[{"a":1,"b":"two"}],"b":"b","c":[],"optional":null}]'
+RAW = b'{"a":1,"nested":{"a":1,"b":"two"},"nested_list":[{"a":1,"b":"two"}],"nested_mapping":{"a":{"a":1,"b":"two"}},"b":"b","c":[],"optional":null}'
+COLLECTION_RAW = b'[{"a":1,"nested":{"a":1,"b":"two"},"nested_list":[{"a":1,"b":"two"}],"nested_mapping":{"a":{"a":1,"b":"two"}},"b":"b","c":[],"optional":null}]'
+STRUCTURED = DC(
+    a=1,
+    b="b",
+    c=[],
+    nested=NestedDC(a=1, b="two"),
+    nested_list=[NestedDC(a=1, b="two")],
+    nested_mapping={"a": NestedDC(a=1, b="two")},
+    optional=None,
 )
-STRUCTURED = DC(a=1, b="b", c=[], nested=NestedDC(a=1, b="two"), nested_list=[NestedDC(a=1, b="two")], optional=None)
 
 
 @pytest.fixture(name="dto_factory")
 def fx_backend_factory(use_experimental_dto_backend: bool) -> type[DataclassDTO]:
     class Factory(DataclassDTO):
         config = DTOConfig(experimental_codegen_backend=use_experimental_dto_backend)
         model_type = DC
@@ -85,15 +93,18 @@
             backend_cls(
                 dto_factory=dto_factory,
                 field_definition=FieldDefinition.from_annotation(DC),
                 model_type=DC,
                 wrapper_attribute_name=None,
                 is_data_field=True,
                 handler_id="test",
-            ).parse_raw(b'{"a":1,"nested":{"a":1,"b":"two"},"nested_list":[{"a":1,"b":"two"}]}', asgi_connection)
+            ).parse_raw(
+                b'{"a":1,"nested":{"a":1,"b":"two"},"nested_list":[{"a":1,"b":"two"}],"nested_mapping":{"a":{"a":1,"b":"two"}}}',
+                asgi_connection,
+            )
         )
         == DESTRUCTURED
     )
 
 
 def test_backend_parse_raw_msgpack(dto_factory: type[DataclassDTO], backend_cls: type[DTOBackend]) -> None:
     @get("/", name="handler_id", media_type=MediaType.MESSAGEPACK)
@@ -108,15 +119,15 @@
                 dto_factory=dto_factory,
                 field_definition=FieldDefinition.from_annotation(DC),
                 model_type=DC,
                 wrapper_attribute_name=None,
                 is_data_field=True,
                 handler_id="test",
             ).parse_raw(
-                b"\x83\xa1a\x01\xa6nested\x82\xa1a\x01\xa1b\xa3two\xabnested_list\x91\x82\xa1a\x01\xa1b\xa3two",
+                b"\x87\xa1a\x01\xa6nested\x82\xa1a\x01\xa1b\xa3two\xabnested_list\x91\x82\xa1a\x01\xa1b\xa3two\xaenested_mapping\x81\xa1a\x82\xa1a\x01\xa1b\xa3two\xa1b\xa1b\xa1c\x90\xa8optional\xc0",
                 asgi_connection,
             )
         )
         == DESTRUCTURED
     )
```

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_utils.py` & `litestar-2.9.0/tests/unit/test_dto/test_factory/test_backends/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py` & `litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py` & `litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_validations.py` & `litestar-2.9.0/tests/unit/test_handlers/test_asgi_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_opt.py` & `litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/test_opt.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_resolution.py` & `litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/test_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_validations.py` & `litestar-2.9.0/tests/unit/test_handlers/test_base_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_defaults.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_head.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_head.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_media_type.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_sync.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_validations.py` & `litestar-2.9.0/tests/unit/test_handlers/test_http_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py` & `litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py` & `litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py` & `litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py` & `litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_validations.py` & `litestar-2.9.0/tests/unit/test_handlers/test_websocket_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/flower.jpeg` & `litestar-2.9.0/tests/unit/test_kwargs/flower.jpeg`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_cleanup_group.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_cleanup_group.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_cookie_params.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_cookie_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_defaults.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_dependency_batches.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_dependency_batches.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_generator_dependencies.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_generator_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_header_params.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_header_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_json_data.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_json_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_layered_params.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_layered_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_msgpack_data.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_msgpack_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_multipart_data.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_multipart_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_path_params.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_path_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_query_params.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_query_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_reserved_kwargs_injection.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_reserved_kwargs_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_url_encoded_data.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_url_encoded_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_kwargs/test_validations.py` & `litestar-2.9.0/tests/unit/test_kwargs/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_logging/test_logging_config.py` & `litestar-2.9.0/tests/unit/test_logging/test_logging_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -215,7 +215,20 @@
     root_logger_handler = root_logger.handlers[0]  # type: ignore[attr-defined]
     assert isinstance(root_logger_handler, expected_handler_class)
     if type(root_logger_handler) is QueueHandler:
         formatter = root_logger_handler.listener.handlers[0].formatter  # type: ignore[attr-defined]
     else:
         formatter = root_logger_handler.formatter
     assert formatter._fmt == log_format
+
+
+@pytest.mark.parametrize(
+    "traceback_line_limit, expected_warning_deprecation_called",
+    [
+        [-1, False],
+        [20, True],
+    ],
+)
+def test_traceback_line_limit_deprecation(traceback_line_limit: int, expected_warning_deprecation_called: bool) -> None:
+    with patch("litestar.logging.config.warn_deprecation") as mock_warning_deprecation:
+        LoggingConfig(traceback_line_limit=traceback_line_limit)
+        assert mock_warning_deprecation.called is expected_warning_deprecation_called
```

### Comparing `litestar-2.8.3/tests/unit/test_logging/test_structlog_config.py` & `litestar-2.9.0/tests/unit/test_logging/test_structlog_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import sys
 from typing import Callable
+from unittest.mock import patch
 
 import pytest
 import structlog
 from pytest import CaptureFixture
 from structlog import BytesLoggerFactory, get_logger
 from structlog.processors import JSONRenderer
 from structlog.types import BindableLogger, WrappedLogger
@@ -151,7 +152,23 @@
 
         log_messages = [decode_json(value=x) for x in capsys.readouterr().out.splitlines()]
 
         assert log_messages == [
             {"key": "value1", "event": "message1"},
             {"key": "value2", "event": "message2"},
         ]
+
+
+@pytest.mark.parametrize(
+    "isatty, pretty_print_tty, expected_as_json",
+    [
+        (True, True, False),
+        (True, False, True),
+        (False, True, True),
+        (False, False, True),
+    ],
+)
+def test_structlog_config_as_json(isatty: bool, pretty_print_tty: bool, expected_as_json: bool) -> None:
+    with patch("litestar.logging.config.sys.stderr.isatty") as isatty_mock:
+        isatty_mock.return_value = isatty
+        logging_config = StructLoggingConfig(pretty_print_tty=pretty_print_tty)
+        assert logging_config.as_json() is expected_as_json
```

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_allowed_hosts_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_allowed_hosts_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     unpacked_middleware = []
     cur = client.app.asgi_router.root_route_map_node.children["/"].asgi_handlers["GET"][0]
     while hasattr(cur, "app"):
         unpacked_middleware.append(cur)
         cur = cast("Any", cur.app)
     unpacked_middleware.append(cur)
 
-    assert len(unpacked_middleware) == 4
-    allowed_hosts_middleware = cast("Any", unpacked_middleware[1])
+    allowed_hosts_middleware, *_ = unpacked_middleware
     assert isinstance(allowed_hosts_middleware, AllowedHostsMiddleware)
     assert allowed_hosts_middleware.allowed_hosts_regex.pattern == ".*\\.example.com$|moishe.zuchmir.com"  # type: ignore[union-attr]
 
 
 def test_allowed_hosts_middleware_hosts_regex() -> None:
     config = AllowedHostsConfig(allowed_hosts=["*.example.com", "moishe.zuchmir.com"])
     middleware = AllowedHostsMiddleware(app=DummyApp(), config=config)  # type: ignore[abstract]
```

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_base_authentication_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_base_authentication_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_base_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_base_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_compression_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_compression_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_cors_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_cors_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Literal, Mapping, Optional, Union, cast
 
 import pytest
 
 from litestar import get
 from litestar.config.cors import CORSConfig
-from litestar.middleware.cors import CORSMiddleware
+from litestar.middleware._internal.cors import CORSMiddleware
 from litestar.status_codes import HTTP_200_OK, HTTP_404_NOT_FOUND
 from litestar.testing import create_test_client
 from litestar.types.asgi_types import Method
 
 
 def test_setting_cors_middleware() -> None:
     cors_config = CORSConfig()  # pyright: ignore
@@ -24,15 +24,15 @@
         unpacked_middleware = []
         cur = client.app.asgi_handler
         while hasattr(cur, "app"):
             unpacked_middleware.append(cur)
             cur = cast("Any", cur.app)
         unpacked_middleware.append(cur)
         assert len(unpacked_middleware) == 4
-        cors_middleware = cast("Any", unpacked_middleware[1])
+        cors_middleware = cast("Any", unpacked_middleware[0])
         assert isinstance(cors_middleware, CORSMiddleware)
         assert cors_middleware.config.allow_headers == ["*"]
         assert cors_middleware.config.allow_methods == ["*"]
         assert cors_middleware.config.allow_origins == cors_config.allow_origins
         assert cors_middleware.config.allow_origin_regex == cors_config.allow_origin_regex
```

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_csrf_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_csrf_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_exception_handler_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_exception_handler_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from inspect import getinnerframes
 from typing import TYPE_CHECKING, Any, Callable, Generator, Optional
+from unittest.mock import MagicMock
 
 import pytest
-from _pytest.capture import CaptureFixture
 from pytest_mock import MockerFixture
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from structlog.testing import capture_logs
 
 from litestar import Litestar, MediaType, Request, Response, get
-from litestar.exceptions import HTTPException, InternalServerException, ValidationException
+from litestar.exceptions import HTTPException, InternalServerException, LitestarException, ValidationException
+from litestar.exceptions.responses._debug_response import get_symbol_name
 from litestar.logging.config import LoggingConfig, StructLoggingConfig
-from litestar.middleware.exceptions import ExceptionHandlerMiddleware
-from litestar.middleware.exceptions._debug_response import get_symbol_name
-from litestar.middleware.exceptions.middleware import _starlette_exception_handler, get_exception_handler
+from litestar.middleware._internal.exceptions.middleware import (
+    ExceptionHandlerMiddleware,
+    _starlette_exception_handler,
+    get_exception_handler,
+)
 from litestar.status_codes import HTTP_400_BAD_REQUEST, HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.testing import TestClient, create_test_client
 from litestar.types import ExceptionHandlersMap
-from litestar.types.asgi_types import HTTPScope
+from litestar.types.asgi_types import HTTPReceiveMessage, HTTPScope, Message, Receive, Scope, Send
+from litestar.utils.scope.state import ScopeState
 from tests.helpers import cleanup_logging_impl
 
 if TYPE_CHECKING:
     from _pytest.logging import LogCaptureFixture
 
     from litestar.types import Scope
     from litestar.types.callable_types import GetLogger
@@ -39,15 +43,15 @@
 @pytest.fixture()
 def app() -> Litestar:
     return Litestar()
 
 
 @pytest.fixture()
 def middleware() -> ExceptionHandlerMiddleware:
-    return ExceptionHandlerMiddleware(dummy_app, None, {})
+    return ExceptionHandlerMiddleware(dummy_app, None)
 
 
 @pytest.fixture()
 def scope(create_scope: Callable[..., HTTPScope], app: Litestar) -> HTTPScope:
     return create_scope(app=app)
 
 
@@ -118,25 +122,32 @@
     assert response.content == {
         "detail": "Internal Server Error",
         "status_code": HTTP_500_INTERNAL_SERVER_ERROR,
     }
 
 
 def test_exception_handler_middleware_exception_handlers_mapping() -> None:
+    mock = MagicMock()
+
     @get("/")
-    def handler() -> None: ...
+    def handler(request: Request) -> None:
+        mock(ScopeState.from_scope(request.scope).exception_handlers)
 
     def exception_handler(request: Request, exc: Exception) -> Response:
         return Response(content={"an": "error"}, status_code=HTTP_500_INTERNAL_SERVER_ERROR)
 
     app = Litestar(route_handlers=[handler], exception_handlers={Exception: exception_handler}, openapi_config=None)
-    assert app.asgi_router.root_route_map_node.children["/"].asgi_handlers["GET"][0].exception_handlers == {  # type: ignore[attr-defined]
-        Exception: exception_handler,
-        StarletteHTTPException: _starlette_exception_handler,
-    }
+
+    with TestClient(app) as client:
+        client.get("/")
+        mock.assert_called_once()
+        assert mock.call_args[0][0] == {
+            Exception: exception_handler,
+            StarletteHTTPException: _starlette_exception_handler,
+        }
 
 
 def test_exception_handler_middleware_calls_app_level_after_exception_hook() -> None:
     @get("/test")
     def handler() -> None:
         raise RuntimeError()
 
@@ -189,20 +200,18 @@
             assert "Test debug exception" in response.text
         else:
             assert "Internal Server Error" in response.text
 
         if should_log:
             assert len(caplog.records) == 1
             assert caplog.records[0].levelname == "ERROR"
-            assert caplog.records[0].message.startswith(
-                "exception raised on http connection to route /test\n\nTraceback (most recent call last):\n"
-            )
+            assert caplog.records[0].message.startswith("Uncaught exception (connection_type=http, path=/test):")
         else:
             assert not caplog.records
-            assert "exception raised on http connection request to route /test" not in response.text
+            assert "Uncaught exception" not in response.text
 
 
 @pytest.mark.parametrize(
     "is_debug, logging_config, should_log",
     [
         (True, StructLoggingConfig(log_exceptions="debug"), True),
         (False, StructLoggingConfig(log_exceptions="debug"), False),
@@ -212,15 +221,14 @@
         (False, StructLoggingConfig(log_exceptions="never"), False),
         (True, None, False),
         (False, None, False),
     ],
 )
 def test_exception_handler_struct_logging(
     get_logger: "GetLogger",
-    capsys: CaptureFixture,
     is_debug: bool,
     logging_config: Optional[LoggingConfig],
     should_log: bool,
 ) -> None:
     @get("/test")
     def handler() -> None:
         raise ValueError("Test debug exception")
@@ -235,58 +243,20 @@
         else:
             assert "Internal Server Error" in response.text
 
         if should_log:
             assert len(cap_logs) == 1
             assert cap_logs[0].get("connection_type") == "http"
             assert cap_logs[0].get("path") == "/test"
-            assert cap_logs[0].get("traceback")
-            assert cap_logs[0].get("event") == "Uncaught Exception"
+            assert cap_logs[0].get("event") == "Uncaught exception"
             assert cap_logs[0].get("log_level") == "error"
         else:
             assert not cap_logs
 
 
-def test_traceback_truncate_default_logging(
-    get_logger: "GetLogger",
-    caplog: "LogCaptureFixture",
-) -> None:
-    @get("/test")
-    def handler() -> None:
-        raise ValueError("Test debug exception")
-
-    app = Litestar([handler], logging_config=LoggingConfig(log_exceptions="always", traceback_line_limit=1))
-
-    with caplog.at_level("ERROR", "litestar"), TestClient(app=app) as client:
-        client.app.logger = get_logger("litestar")
-        response = client.get("/test")
-        assert response.status_code == HTTP_500_INTERNAL_SERVER_ERROR
-        assert "Internal Server Error" in response.text
-
-        assert len(caplog.records) == 1
-        assert caplog.records[0].levelname == "ERROR"
-        assert caplog.records[0].message == (
-            "exception raised on http connection to route /test\n\nTraceback (most recent call last):\nValueError: Test debug exception\n"
-        )
-
-
-def test_traceback_truncate_struct_logging() -> None:
-    @get("/test")
-    def handler() -> None:
-        raise ValueError("Test debug exception")
-
-    app = Litestar([handler], logging_config=StructLoggingConfig(log_exceptions="always", traceback_line_limit=1))
-
-    with TestClient(app=app) as client, capture_logs() as cap_logs:
-        response = client.get("/test")
-        assert response.status_code == HTTP_500_INTERNAL_SERVER_ERROR
-        assert len(cap_logs) == 1
-        assert cap_logs[0].get("traceback") == "ValueError: Test debug exception\n"
-
-
 def handler(_: Any, __: Any) -> Any:
     return None
 
 
 def handler_2(_: Any, __: Any) -> Any:
     return None
 
@@ -315,15 +285,15 @@
 
 @pytest.mark.filterwarnings("ignore::litestar.utils.warnings.LitestarWarning:")
 def test_pdb_on_exception(mocker: MockerFixture) -> None:
     @get("/test")
     def handler() -> None:
         raise ValueError("Test debug exception")
 
-    mock_post_mortem = mocker.patch("litestar.middleware.exceptions.middleware.pdb.post_mortem")
+    mock_post_mortem = mocker.patch("litestar.middleware._internal.exceptions.middleware.pdb.post_mortem")
 
     app = Litestar([handler], pdb_on_exception=True)
 
     with TestClient(app=app) as client:
         response = client.get("/test")
 
     assert response.status_code == HTTP_500_INTERNAL_SERVER_ERROR
@@ -342,17 +312,15 @@
         client.app.logger = get_logger("litestar")
         response = client.get("/test")
 
         assert response.status_code == HTTP_500_INTERNAL_SERVER_ERROR
         assert "Test debug exception" in response.text
         assert len(caplog.records) == 1
         assert caplog.records[0].levelname == "ERROR"
-        assert caplog.records[0].message.startswith(
-            "exception raised on http connection to route /test\n\nTraceback (most recent call last):\n"
-        )
+        assert caplog.records[0].message.startswith("Uncaught exception (connection_type=http, path=/test):")
 
 
 def test_get_symbol_name_where_type_doesnt_support_bool() -> None:
     class Test:
         def __bool__(self) -> bool:
             raise TypeError("This type doesn't support bool")
 
@@ -384,7 +352,33 @@
     @get(media_type=media_type)
     def handler() -> None:
         raise ValidationException(extra={"foo": Foo("bar")})
 
     with create_test_client([handler], type_encoders={Foo: lambda f: f.value}) as client:
         res = client.get("/")
         assert res.json()["extra"] == {"foo": "bar"}
+
+
+async def test_exception_handler_middleware_response_already_started(scope: HTTPScope) -> None:
+    assert not ScopeState.from_scope(scope).response_started
+
+    async def mock_receive() -> HTTPReceiveMessage:  # type: ignore[empty-body]
+        pass
+
+    mock = MagicMock()
+
+    async def mock_send(message: Message) -> None:
+        mock(message)
+
+    start_message: Message = {"type": "http.response.start", "status": 200, "headers": []}
+
+    async def asgi_app(scope: Scope, receive: Receive, send: Send) -> None:
+        await send(start_message)
+        raise RuntimeError("Test exception")
+
+    mw = ExceptionHandlerMiddleware(asgi_app, None)
+
+    with pytest.raises(LitestarException):
+        await mw(scope, mock_receive, mock_send)
+
+    mock.assert_called_once_with(start_message)
+    assert ScopeState.from_scope(scope).response_started
```

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_logging_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_middleware_handling.py` & `litestar-2.9.0/tests/unit/test_middleware/test_middleware_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,16 @@
 
         unpacked_middleware = []
         cur = client.app.asgi_router.root_route_map_node.children["/"].asgi_handlers["GET"][0]
         while hasattr(cur, "app"):
             unpacked_middleware.append(cur)
             cur = cast("ASGIApp", cur.app)  # pyright: ignore
         unpacked_middleware.append(cur)
-        assert len(unpacked_middleware) == 4
 
-        middleware_instance = unpacked_middleware[1]
+        middleware_instance, *_ = unpacked_middleware
 
         assert isinstance(
             middleware_instance,
             (
                 MiddlewareProtocolRequestLoggingMiddleware,
                 BaseMiddlewareRequestLoggingMiddleware,
                 MiddlewareWithArgsAndKwargs,
```

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_rate_limit_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_rate_limit_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_session/conftest.py` & `litestar-2.9.0/tests/unit/test_middleware/test_session/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_session/test_client_side_backend.py` & `litestar-2.9.0/tests/unit/test_middleware/test_session/test_client_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_session/test_integration.py` & `litestar-2.9.0/tests/unit/test_middleware/test_session/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_session/test_middleware.py` & `litestar-2.9.0/tests/unit/test_middleware/test_session/test_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_middleware/test_session/test_server_side_backend.py` & `litestar-2.9.0/tests/unit/test_middleware/test_session/test_server_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/conftest.py` & `litestar-2.9.0/tests/unit/test_openapi/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_config.py` & `litestar-2.9.0/tests/unit/test_openapi/test_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_datastructures.py` & `litestar-2.9.0/tests/unit/test_openapi/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_endpoints.py` & `litestar-2.9.0/tests/unit/test_openapi/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_integration.py` & `litestar-2.9.0/tests/unit/test_openapi/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,31 @@
         assert client.app.openapi_schema
         openapi_schema = client.app.openapi_schema
         assert openapi_schema.paths
         response = client.get("/schema/openapi.json")
         assert response.status_code == HTTP_404_NOT_FOUND
 
 
+@pytest.mark.parametrize(
+    "schema_paths",
+    [
+        ("/schema/openapi.json", "/schema/openapi.yaml"),
+        ("/schema/openapi.yaml", "/schema/openapi.json"),
+    ],
+)
+def test_openapi_controller_internal_schema_conversion(schema_paths: list[str]) -> None:
+    openapi_config = OpenAPIConfig("Example API", "1.0.0", openapi_controller=OpenAPIController)
+
+    with create_test_client([], openapi_config=openapi_config) as client:
+        for schema_path in schema_paths:
+            response = client.get(schema_path)
+            assert response.status_code == HTTP_200_OK
+            assert "Example API" in response.text
+
+
 def test_openapi_custom_path(openapi_controller: type[OpenAPIController] | None) -> None:
     openapi_config = OpenAPIConfig(
         title="my title", version="1.0.0", path="/custom_schema_path", openapi_controller=openapi_controller
     )
     with create_test_client([], openapi_config=openapi_config) as client:
         response = client.get("/schema")
         assert response.status_code == HTTP_404_NOT_FOUND
```

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_parameters.py` & `litestar-2.9.0/tests/unit/test_openapi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_path_item.py` & `litestar-2.9.0/tests/unit/test_openapi/test_path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_request_body.py` & `litestar-2.9.0/tests/unit/test_openapi/test_request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_responses.py` & `litestar-2.9.0/tests/unit/test_openapi/test_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_schema.py` & `litestar-2.9.0/tests/unit/test_openapi/test_schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_security_schemes.py` & `litestar-2.9.0/tests/unit/test_openapi/test_security_schemes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_spec_generation.py` & `litestar-2.9.0/tests/unit/test_openapi/test_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_tags.py` & `litestar-2.9.0/tests/unit/test_openapi/test_tags.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_converter.py` & `litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/test_converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py` & `litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py` & `litestar-2.9.0/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_plugins/test_base.py` & `litestar-2.9.0/tests/unit/test_plugins/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_plugins/test_flash.py` & `litestar-2.9.0/tests/unit/test_plugins/test_flash.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_plugins/test_sqlalchemy.py` & `litestar-2.9.0/tests/unit/test_plugins/test_sqlalchemy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,49 @@
-from advanced_alchemy import base as sa_base
-from advanced_alchemy import filters as sa_filters
-from advanced_alchemy import types as sa_types
 from advanced_alchemy.extensions import litestar as sa_litestar
+from advanced_alchemy.extensions.litestar import base as sa_base
+from advanced_alchemy.extensions.litestar import exceptions as sa_exceptions
+from advanced_alchemy.extensions.litestar import filters as sa_filters
+from advanced_alchemy.extensions.litestar import mixins as sa_mixins
+from advanced_alchemy.extensions.litestar import repository as sa_repository
+from advanced_alchemy.extensions.litestar import service as sa_service
+from advanced_alchemy.extensions.litestar import types as sa_types
+from advanced_alchemy.extensions.litestar import utils as sa_utils
 
+from litestar.pagination import OffsetPagination
 from litestar.plugins import sqlalchemy
 
 
 def test_re_exports() -> None:
+    assert sqlalchemy.base is sa_base
     assert sqlalchemy.filters is sa_filters
     assert sqlalchemy.types is sa_types
-
-    assert sqlalchemy.AuditColumns is sa_base.AuditColumns
-    assert sqlalchemy.BigIntAuditBase is sa_base.BigIntAuditBase
-    assert sqlalchemy.BigIntBase is sa_base.BigIntBase
-    assert sqlalchemy.BigIntPrimaryKey is sa_base.BigIntPrimaryKey
-    assert sqlalchemy.CommonTableAttributes is sa_base.CommonTableAttributes
-    assert sqlalchemy.UUIDAuditBase is sa_base.UUIDAuditBase
-    assert sqlalchemy.UUIDBase is sa_base.UUIDBase
-    assert sqlalchemy.UUIDPrimaryKey is sa_base.UUIDPrimaryKey
-    assert sqlalchemy.orm_registry is sa_base.orm_registry
+    assert sqlalchemy.mixins is sa_mixins
+    assert sqlalchemy.utils is sa_utils
+    assert sqlalchemy.repository is sa_repository
+    assert sqlalchemy.service is sa_service
+    assert sqlalchemy.exceptions is sa_exceptions
+    assert OffsetPagination is sa_service.OffsetPagination
 
     assert sqlalchemy.AlembicAsyncConfig is sa_litestar.AlembicAsyncConfig
     assert sqlalchemy.AlembicCommands is sa_litestar.AlembicCommands
     assert sqlalchemy.AlembicSyncConfig is sa_litestar.AlembicSyncConfig
     assert sqlalchemy.AsyncSessionConfig is sa_litestar.AsyncSessionConfig
     assert sqlalchemy.EngineConfig is sa_litestar.EngineConfig
     assert sqlalchemy.SQLAlchemyAsyncConfig is sa_litestar.SQLAlchemyAsyncConfig
     assert sqlalchemy.SQLAlchemyDTO is sa_litestar.SQLAlchemyDTO
     assert sqlalchemy.SQLAlchemyDTOConfig is sa_litestar.SQLAlchemyDTOConfig
     assert sqlalchemy.SQLAlchemyInitPlugin is sa_litestar.SQLAlchemyInitPlugin
     assert sqlalchemy.SQLAlchemyPlugin is sa_litestar.SQLAlchemyPlugin
     assert sqlalchemy.SQLAlchemySerializationPlugin is sa_litestar.SQLAlchemySerializationPlugin
     assert sqlalchemy.SQLAlchemySyncConfig is sa_litestar.SQLAlchemySyncConfig
     assert sqlalchemy.SyncSessionConfig is sa_litestar.SyncSessionConfig
+
+    # deprecated, to be removed later
+    assert sqlalchemy.AuditColumns is sa_base.AuditColumns
+    assert sqlalchemy.BigIntAuditBase is sa_base.BigIntAuditBase
+    assert sqlalchemy.BigIntBase is sa_base.BigIntBase
+    assert sqlalchemy.BigIntPrimaryKey is sa_base.BigIntPrimaryKey
+    assert sqlalchemy.CommonTableAttributes is sa_base.CommonTableAttributes
+    assert sqlalchemy.UUIDAuditBase is sa_base.UUIDAuditBase
+    assert sqlalchemy.UUIDBase is sa_base.UUIDBase
+    assert sqlalchemy.UUIDPrimaryKey is sa_base.UUIDPrimaryKey
+    assert sqlalchemy.orm_registry is sa_base.orm_registry
```

### Comparing `litestar-2.8.3/tests/unit/test_repository/models_bigint.py` & `litestar-2.9.0/tests/unit/test_repository/models_bigint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Example domain objects for testing."""
 
 from __future__ import annotations
 
 from datetime import date, datetime
 from typing import List
 
-from advanced_alchemy import SQLAlchemyAsyncRepository, SQLAlchemySyncRepository
 from advanced_alchemy.base import BigIntAuditBase, BigIntBase
+from advanced_alchemy.repository import SQLAlchemyAsyncRepository, SQLAlchemySyncRepository
 from sqlalchemy import Column, FetchedValue, ForeignKey, String, Table, func
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 
 class BigIntAuthor(BigIntAuditBase):
     """The Author domain object."""
```

### Comparing `litestar-2.8.3/tests/unit/test_repository/models_uuid.py` & `litestar-2.9.0/tests/unit/test_repository/models_uuid.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 
 from __future__ import annotations
 
 from datetime import date, datetime
 from typing import List
 from uuid import UUID
 
-from advanced_alchemy import SQLAlchemyAsyncRepository, SQLAlchemySyncRepository, base
-from advanced_alchemy.base import UUIDAuditBase, UUIDBase
+from advanced_alchemy import base
+from advanced_alchemy.repository import SQLAlchemyAsyncRepository, SQLAlchemySyncRepository
 from sqlalchemy import Column, FetchedValue, ForeignKey, String, Table, func
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 
-class UUIDAuthor(UUIDAuditBase):
+class UUIDAuthor(base.UUIDAuditBase):
     """The UUIDAuthor domain object."""
 
     name: Mapped[str] = mapped_column(String(length=100))  # pyright: ignore
     dob: Mapped[date] = mapped_column(nullable=True)  # pyright: ignore
     books: Mapped[List[UUIDBook]] = relationship(  # noqa
         lazy="selectin",
         back_populates="author",
         cascade="all, delete",
     )
 
 
-class UUIDBook(UUIDBase):
+class UUIDBook(base.UUIDBase):
     """The Book domain object."""
 
     title: Mapped[str] = mapped_column(String(length=250))  # pyright: ignore
     author_id: Mapped[UUID] = mapped_column(ForeignKey("uuid_author.id"))  # pyright: ignore
     author: Mapped[UUIDAuthor] = relationship(lazy="joined", innerjoin=True, back_populates="books")  # pyright: ignore
 
 
-class UUIDEventLog(UUIDAuditBase):
+class UUIDEventLog(base.UUIDAuditBase):
     """The event log domain object."""
 
     logged_at: Mapped[datetime] = mapped_column(default=datetime.now())  # pyright: ignore
     payload: Mapped[dict] = mapped_column(default={})  # pyright: ignore
 
 
-class UUIDModelWithFetchedValue(UUIDBase):
+class UUIDModelWithFetchedValue(base.UUIDBase):
     """The ModelWithFetchedValue UUIDBase."""
 
     val: Mapped[int]  # pyright: ignore
     updated: Mapped[datetime] = mapped_column(  # pyright: ignore
         server_default=func.current_timestamp(),
         onupdate=func.current_timestamp(),
         server_onupdate=FetchedValue(),
@@ -54,28 +54,28 @@
     "uuid_item_tag",
     base.orm_registry.metadata,
     Column("item_id", ForeignKey("uuid_item.id"), primary_key=True),
     Column("tag_id", ForeignKey("uuid_tag.id"), primary_key=True),
 )
 
 
-class UUIDItem(UUIDBase):
+class UUIDItem(base.UUIDBase):
     name: Mapped[str] = mapped_column(String(length=50))  # pyright: ignore
     description: Mapped[str] = mapped_column(String(length=100), nullable=True)  # pyright: ignore
     tags: Mapped[List[UUIDTag]] = relationship(secondary=lambda: uuid_item_tag, back_populates="items")  # noqa
 
 
-class UUIDTag(UUIDAuditBase):
+class UUIDTag(base.UUIDAuditBase):
     """The event log domain object."""
 
     name: Mapped[str] = mapped_column(String(length=50))  # pyright: ignore
     items: Mapped[List[UUIDItem]] = relationship(secondary=lambda: uuid_item_tag, back_populates="tags")  # noqa
 
 
-class UUIDRule(UUIDAuditBase):
+class UUIDRule(base.UUIDAuditBase):
     """The rule domain object."""
 
     name: Mapped[str] = mapped_column(String(length=250))  # pyright: ignore
     config: Mapped[dict] = mapped_column(default=lambda: {})  # pyright: ignore
 
 
 class RuleAsyncRepository(SQLAlchemyAsyncRepository[UUIDRule]):
```

### Comparing `litestar-2.8.3/tests/unit/test_repository/test_generic_mock_repository.py` & `litestar-2.9.0/tests/unit/test_repository/test_generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_base_response.py` & `litestar-2.9.0/tests/unit/test_response/test_base_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_file_response.py` & `litestar-2.9.0/tests/unit/test_response/test_file_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_redirect_response.py` & `litestar-2.9.0/tests/unit/test_response/test_redirect_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_response_cookies.py` & `litestar-2.9.0/tests/unit/test_response/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_response_headers.py` & `litestar-2.9.0/tests/unit/test_response/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_response_to_asgi_response.py` & `litestar-2.9.0/tests/unit/test_response/test_response_to_asgi_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_serialization.py` & `litestar-2.9.0/tests/unit/test_response/test_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_sse.py` & `litestar-2.9.0/tests/unit/test_response/test_sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_streaming_response.py` & `litestar-2.9.0/tests/unit/test_response/test_streaming_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_type_decoders.py` & `litestar-2.9.0/tests/unit/test_response/test_type_decoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_response/test_type_encoders.py` & `litestar-2.9.0/tests/unit/test_response/test_type_encoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_security/test_security.py` & `litestar-2.9.0/tests/unit/test_security/test_security.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_security/test_session_auth.py` & `litestar-2.9.0/tests/unit/test_security/test_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_security/test_jwt/test_auth.py` & `litestar-2.9.0/tests/unit/test_security/test_jwt/test_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_security/test_jwt/test_integration.py` & `litestar-2.9.0/tests/unit/test_security/test_jwt/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_security/test_jwt/test_token.py` & `litestar-2.9.0/tests/unit/test_security/test_jwt/test_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_signature/test_parsing.py` & `litestar-2.9.0/tests/unit/test_signature/test_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_signature/test_validation.py` & `litestar-2.9.0/tests/unit/test_signature/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import Generic, List, Optional, TypeVar
 
 import pytest
 from attr import define
 from typing_extensions import Annotated, TypedDict
 
 from litestar import get, post
 from litestar._signature import SignatureModel
@@ -285,7 +285,21 @@
     with pytest.raises(ValidationException) as exc:
         model.parse_values_from_connection_kwargs(connection=RequestFactory().get(), a=0, b=9)
 
     assert exc.value.extra == [
         {"message": "Expected `int` >= 6", "key": "a", "source": ParamType.QUERY},
         {"message": "Expected `int` <= 4", "key": "b", "source": ParamType.QUERY},
     ]
+
+
+def test_validate_subscribed_generics() -> None:
+    T = TypeVar("T")
+
+    class Foo(Generic[T]):
+        pass
+
+    @get("/")
+    async def something(foo: Foo[str] = Foo()) -> None:
+        return None
+
+    with create_test_client([something]) as client:
+        assert client.get("/").status_code == 200
```

### Comparing `litestar-2.8.3/tests/unit/test_static_files/conftest.py` & `litestar-2.9.0/tests/unit/test_static_files/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_static_files/test_create_static_router.py` & `litestar-2.9.0/tests/unit/test_static_files/test_create_static_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_static_files/test_file_serving_resolution.py` & `litestar-2.9.0/tests/unit/test_static_files/test_file_serving_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_static_files/test_html_mode.py` & `litestar-2.9.0/tests/unit/test_static_files/test_html_mode.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_static_files/test_static_files_validation.py` & `litestar-2.9.0/tests/unit/test_static_files/test_static_files_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from pathlib import Path, PosixPath
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, List, cast
 
 import pytest
 
 from litestar import HttpMethod, Litestar, MediaType, get
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.static_files import StaticFilesConfig, create_static_files_router
@@ -142,10 +142,10 @@
 
     # Resolve file path with the StaticFiles handler
     string_path = Path("test.txt").as_posix()
 
     coroutine = static_files_handler.get_fs_info(directories=static_files_handler.directories, file_path=string_path)
     resolved_path, fs_info = asyncio.run(coroutine)
 
-    expected_resolved_path = PosixPath(str(tmpdir / "test.txt"))
+    expected_resolved_path = tmpdir / "test.txt"
     assert resolved_path == expected_resolved_path  # Because the resolved path is inside the static directory
     assert fs_info is not None  # Because the file exists, so there is info
```

### Comparing `litestar-2.8.3/tests/unit/test_template/test_built_in.py` & `litestar-2.9.0/tests/unit/test_template/test_built_in.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_template/test_builtin_functions.py` & `litestar-2.9.0/tests/unit/test_template/test_builtin_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_template/test_context.py` & `litestar-2.9.0/tests/unit/test_template/test_context.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_template/test_csrf_token.py` & `litestar-2.9.0/tests/unit/test_template/test_csrf_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_template/test_template.py` & `litestar-2.9.0/tests/unit/test_template/test_template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_testing/test_lifespan_handler.py` & `litestar-2.9.0/tests/unit/test_testing/test_lifespan_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_testing/test_request_factory.py` & `litestar-2.9.0/tests/unit/test_testing/test_request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_testing/test_test_client.py` & `litestar-2.9.0/tests/unit/test_testing/test_test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from queue import Empty
 from typing import TYPE_CHECKING, Callable, Dict, NoReturn, Optional, Union, cast
 
 from _pytest.fixtures import FixtureRequest
 
 from litestar import Controller, WebSocket, delete, head, patch, put, websocket
 from litestar.status_codes import HTTP_200_OK, HTTP_201_CREATED, HTTP_204_NO_CONTENT
-from litestar.testing import AsyncTestClient, WebSocketTestSession, create_test_client
+from litestar.testing import AsyncTestClient, WebSocketTestSession, create_async_test_client, create_test_client
 
 if TYPE_CHECKING:
     from litestar.middleware.session.base import BaseBackendConfig
     from litestar.types import (
         AnyIOBackend,
         HTTPResponseBodyEvent,
         HTTPResponseStartEvent,
@@ -257,7 +257,56 @@
     async def handler(socket: WebSocket) -> None:
         pass
 
     with create_test_client(handler, backend=anyio_backend, timeout=0.1) as client, pytest.raises(
         Empty
     ), client.websocket_connect("/"):
         pass
+
+
+@pytest.mark.parametrize("block,timeout", [(False, None), (False, 0.001), (True, 0.001)])
+@pytest.mark.parametrize(
+    "receive_method",
+    [
+        WebSocketTestSession.receive,
+        WebSocketTestSession.receive_json,
+        WebSocketTestSession.receive_text,
+        WebSocketTestSession.receive_bytes,
+    ],
+)
+async def test_websocket_test_session_block_timeout_async(
+    receive_method: Callable[..., Any], block: bool, timeout: Optional[float], anyio_backend: "AnyIOBackend"
+) -> None:
+    @websocket()
+    async def handler(socket: WebSocket) -> None:
+        await socket.accept()
+
+    with pytest.raises(Empty):
+        async with create_async_test_client(handler, backend=anyio_backend) as client:
+            with await client.websocket_connect("/") as ws:
+                receive_method(ws, timeout=timeout, block=block)
+
+
+async def test_websocket_accept_timeout_async(anyio_backend: "AnyIOBackend") -> None:
+    @websocket()
+    async def handler(socket: WebSocket) -> None:
+        pass
+
+    async with create_async_test_client(handler, backend=anyio_backend, timeout=0.1) as client:
+        with pytest.raises(Empty):
+            with await client.websocket_connect("/"):
+                pass
+
+
+async def test_websocket_connect_async(anyio_backend: "AnyIOBackend") -> None:
+    @websocket()
+    async def handler(socket: WebSocket) -> None:
+        await socket.accept()
+        data = await socket.receive_json()
+        await socket.send_json(data)
+        await socket.close()
+
+    async with create_async_test_client(handler, backend=anyio_backend, timeout=0.1) as client:
+        with await client.websocket_connect("/", subprotocols="wamp") as ws:
+            ws.send_json({"data": "123"})
+            data = ws.receive_json()
+            assert data == {"data": "123"}
```

### Comparing `litestar-2.8.3/tests/unit/test_types/test_protocols.py` & `litestar-2.9.0/tests/unit/test_types/test_protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_dataclass.py` & `litestar-2.9.0/tests/unit/test_utils/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_deprecation.py` & `litestar-2.9.0/tests/unit/test_utils/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_helpers.py` & `litestar-2.9.0/tests/unit/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_module_loader.py` & `litestar-2.9.0/tests/unit/test_utils/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_path.py` & `litestar-2.9.0/tests/unit/test_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_predicates.py` & `litestar-2.9.0/tests/unit/test_utils/test_predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_scope.py` & `litestar-2.9.0/tests/unit/test_utils/test_scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_sequence.py` & `litestar-2.9.0/tests/unit/test_utils/test_sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_signature.py` & `litestar-2.9.0/tests/unit/test_utils/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_sync.py` & `litestar-2.9.0/tests/unit/test_utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_typing.py` & `litestar-2.9.0/tests/unit/test_utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/tests/unit/test_utils/test_version.py` & `litestar-2.9.0/tests/unit/test_utils/test_version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.3/LICENSE` & `litestar-2.9.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021, 2022, 2023 Litestar Org.
+Copyright (c) 2021, 2022, 2023, 2024 Litestar Org.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `litestar-2.8.3/README.md` & `litestar-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -554,14 +554,19 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.b-list.org/"><img src="https://avatars.githubusercontent.com/u/12384?v=4?s=100" width="100px;" alt="James Bennett"/><br /><sub><b>James Bennett</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Aubernostrum" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sherbang"><img src="https://avatars.githubusercontent.com/u/275015?v=4?s=100" width="100px;" alt="sherbang"/><br /><sub><b>sherbang</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sherbang" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlsmedstad"><img src="https://avatars.githubusercontent.com/u/6952324?v=4?s=100" width="100px;" alt="Carl Smedstad"/><br /><sub><b>Carl Smedstad</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=carlsmedstad" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/maintain0404"><img src="https://avatars.githubusercontent.com/u/50428534?v=4?s=100" width="100px;" alt="Taein Min"/><br /><sub><b>Taein Min</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=maintain0404" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wallseat"><img src="https://avatars.githubusercontent.com/u/26143672?v=4?s=100" width="100px;" alt="Stanislav Lyu."/><br /><sub><b>Stanislav Lyu.</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Awallseat" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tibor-reiss"><img src="https://avatars.githubusercontent.com/u/75096465?v=4?s=100" width="100px;" alt="Tibor Reiss"/><br /><sub><b>Tibor Reiss</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tibor-reiss" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=tibor-reiss" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=tibor-reiss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://pogrom.dev"><img src="https://avatars.githubusercontent.com/u/11032969?v=4?s=100" width="100px;" alt="Alex"/><br /><sub><b>Alex</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3A0xE111" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/litestar/commits?author=0xE111" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://0110.be"><img src="https://avatars.githubusercontent.com/u/60453?v=4?s=100" width="100px;" alt="Joren Six"/><br /><sub><b>Joren Six</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=JorenSix" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.8.3/pyproject.toml` & `litestar-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 authors = [
-  {name = "Cody Fincher", email = "cody.fincher@gmail.com"},
-  {name = "Jacob Coffee", email = "jacob@z7x.org"},
-  {name = "Janek Nouvertné", email = "provinzkraut@posteo.de"},
+  {name = "Cody Fincher", email = "cody@litestar.dev"},
+  {name = "Jacob Coffee", email = "jacob@litestar.dev"},
+  {name = "Janek Nouvertné", email = "janek@litestar.dev"},
   {name = "Na'aman Hirschfeld", email = "nhirschfeld@gmail.com"},
-  {name = "Peter Schutt", email = "peter.github@proton.me"},
+  {name = "Peter Schutt", email = "peter@litestar.dev"},
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
@@ -48,23 +48,23 @@
 description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 keywords = ["api", "rest", "asgi", "litestar", "starlite"]
 license = {text = "MIT"}
 maintainers = [
   {name = "Litestar Developers", email = "hello@litestar.dev"},
   {name = "Cody Fincher", email = "cody@litestar.dev"},
   {name = "Jacob Coffee", email = "jacob@litestar.dev"},
-  {name = "Janek Nouvertné", email = "provinzkraut@litestar.dev"},
+  {name = "Janek Nouvertné", email = "janek@litestar.dev"},
   {name = "Peter Schutt", email = "peter@litestar.dev"},
   {name = "Visakh Unnikrishnan", email = "guacs@litestar.dev"},
   {name = "Alc", email = "alc@litestar.dev"}
 ]
 name = "litestar"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
-version = "2.8.3"
+version = "2.9.0"
 
 [project.urls]
 Blog = "https://blog.litestar.dev"
 Changelog = "https://github.com/litestar-org/litestar/releases/"
 Discord = "https://discord.gg/litestar"
 Documentation = "https://docs.litestar.dev/"
 Homepage = "https://litestar.dev/"
@@ -88,15 +88,15 @@
 minijinja = ["minijinja>=1.0.0"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 piccolo = ["piccolo"]
 picologging = ["picologging"]
 prometheus = ["prometheus-client"]
 pydantic = ["pydantic", "email-validator", "pydantic-extra-types"]
 redis = ["redis[hiredis]>=4.4.4"]
-sqlalchemy = ["advanced-alchemy>=0.2.2,<0.9.0"]
+sqlalchemy = ["advanced-alchemy>=0.2.2"]
 standard = ["jinja2", "jsbeautifier", "uvicorn[standard]", "uvloop>=0.18.0; sys_platform != 'win32'", "fast-query-parsers>=1.0.2"]
 structlog = ["structlog"]
 
 [project.scripts]
 litestar = "litestar.__main__:run_cli"
 
 [tool.hatch.metadata]
@@ -108,15 +108,25 @@
   '/Makefile',
   '/litestar',
   '/tests',
   '/CHANGELOG.rst',
 ]
 
 [tool.pdm]
-ignore_package_warnings = ["sphinx", "slotscheck"]
+ignore_package_warnings = [
+  "alabaster",
+  "sphinxcontrib-*",
+  "sphinx-*",
+  "sphinx",
+  "pre-commit",
+  "pydata-sphinx-*",
+  "slotscheck",
+  "autobahn",
+  "accessible-pygments"
+]
 
 [tool.pdm.dev-dependencies]
 dev = [
   "beanie>=1.21.0",
   "beautifulsoup4",
   "fsspec",
   "greenlet",
@@ -381,14 +391,15 @@
 
 [tool.ruff.lint.per-file-ignores]
 "docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET"]
 "docs/examples/**" = ["T201"]
 "docs/examples/application_hooks/before_send_hook.py" = ["UP006"]
 "docs/examples/contrib/sqlalchemy/plugins/**/*.*" = ["UP006"]
 "docs/examples/data_transfer_objects**/*.*" = ["UP006"]
+"docs/examples/contrib/sqlalchemy/sqlalchemy_declarative_models.py" = ["UP006"]
 "litestar/_openapi/schema_generation/schema.py" = ["C901"]
 "litestar/exceptions/*.*" = ["N818"]
 "litestar/handlers/**/*.*" = ["N801"]
 "litestar/params.py" = ["N802"]
 "test_apps/**/*.*" = ["D", "TRY", "EM", "S", "PTH"]
 "tests/**/*.*" = [
   "A",
```

### Comparing `litestar-2.8.3/PKG-INFO` & `litestar-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: litestar
-Version: 2.8.3
+Version: 2.9.0
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Project-URL: Blog, https://blog.litestar.dev
 Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
 Project-URL: Discord, https://discord.gg/litestar
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Homepage, https://litestar.dev/
 Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Reddit, https://www.reddit.com/r/LitestarAPI
 Project-URL: Repository, https://github.com/litestar-org/litestar
 Project-URL: Twitter, https://twitter.com/LitestarAPI
-Author-email: Cody Fincher <cody.fincher@gmail.com>, Jacob Coffee <jacob@z7x.org>, Janek Nouvertné <provinzkraut@posteo.de>, Na'aman Hirschfeld <nhirschfeld@gmail.com>, Peter Schutt <peter.github@proton.me>
-Maintainer-email: Litestar Developers <hello@litestar.dev>, Cody Fincher <cody@litestar.dev>, Jacob Coffee <jacob@litestar.dev>, Janek Nouvertné <provinzkraut@litestar.dev>, Peter Schutt <peter@litestar.dev>, Visakh Unnikrishnan <guacs@litestar.dev>, Alc <alc@litestar.dev>
+Author-email: Cody Fincher <cody@litestar.dev>, Jacob Coffee <jacob@litestar.dev>, Janek Nouvertné <janek@litestar.dev>, Na'aman Hirschfeld <nhirschfeld@gmail.com>, Peter Schutt <peter@litestar.dev>
+Maintainer-email: Litestar Developers <hello@litestar.dev>, Cody Fincher <cody@litestar.dev>, Jacob Coffee <jacob@litestar.dev>, Janek Nouvertné <janek@litestar.dev>, Peter Schutt <peter@litestar.dev>, Visakh Unnikrishnan <guacs@litestar.dev>, Alc <alc@litestar.dev>
 License: MIT
 License-File: LICENSE
 Keywords: api,asgi,litestar,rest,starlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -61,15 +61,15 @@
 Provides-Extra: cli
 Requires-Dist: jsbeautifier; extra == 'cli'
 Requires-Dist: uvicorn[standard]; extra == 'cli'
 Requires-Dist: uvloop>=0.18.0; (sys_platform != 'win32') and extra == 'cli'
 Provides-Extra: cryptography
 Requires-Dist: cryptography; extra == 'cryptography'
 Provides-Extra: full
-Requires-Dist: advanced-alchemy<0.9.0,>=0.2.2; extra == 'full'
+Requires-Dist: advanced-alchemy>=0.2.2; extra == 'full'
 Requires-Dist: annotated-types; extra == 'full'
 Requires-Dist: attrs; extra == 'full'
 Requires-Dist: brotli; extra == 'full'
 Requires-Dist: cryptography; extra == 'full'
 Requires-Dist: email-validator; extra == 'full'
 Requires-Dist: fast-query-parsers>=1.0.2; extra == 'full'
 Requires-Dist: jinja2; extra == 'full'
@@ -108,15 +108,15 @@
 Provides-Extra: pydantic
 Requires-Dist: email-validator; extra == 'pydantic'
 Requires-Dist: pydantic; extra == 'pydantic'
 Requires-Dist: pydantic-extra-types; extra == 'pydantic'
 Provides-Extra: redis
 Requires-Dist: redis[hiredis]>=4.4.4; extra == 'redis'
 Provides-Extra: sqlalchemy
-Requires-Dist: advanced-alchemy<0.9.0,>=0.2.2; extra == 'sqlalchemy'
+Requires-Dist: advanced-alchemy>=0.2.2; extra == 'sqlalchemy'
 Provides-Extra: standard
 Requires-Dist: fast-query-parsers>=1.0.2; extra == 'standard'
 Requires-Dist: jinja2; extra == 'standard'
 Requires-Dist: jsbeautifier; extra == 'standard'
 Requires-Dist: uvicorn[standard]; extra == 'standard'
 Requires-Dist: uvloop>=0.18.0; (sys_platform != 'win32') and extra == 'standard'
 Provides-Extra: structlog
@@ -679,14 +679,19 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.b-list.org/"><img src="https://avatars.githubusercontent.com/u/12384?v=4?s=100" width="100px;" alt="James Bennett"/><br /><sub><b>James Bennett</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Aubernostrum" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sherbang"><img src="https://avatars.githubusercontent.com/u/275015?v=4?s=100" width="100px;" alt="sherbang"/><br /><sub><b>sherbang</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sherbang" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlsmedstad"><img src="https://avatars.githubusercontent.com/u/6952324?v=4?s=100" width="100px;" alt="Carl Smedstad"/><br /><sub><b>Carl Smedstad</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=carlsmedstad" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/maintain0404"><img src="https://avatars.githubusercontent.com/u/50428534?v=4?s=100" width="100px;" alt="Taein Min"/><br /><sub><b>Taein Min</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=maintain0404" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wallseat"><img src="https://avatars.githubusercontent.com/u/26143672?v=4?s=100" width="100px;" alt="Stanislav Lyu."/><br /><sub><b>Stanislav Lyu.</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Awallseat" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tibor-reiss"><img src="https://avatars.githubusercontent.com/u/75096465?v=4?s=100" width="100px;" alt="Tibor Reiss"/><br /><sub><b>Tibor Reiss</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tibor-reiss" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=tibor-reiss" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=tibor-reiss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://pogrom.dev"><img src="https://avatars.githubusercontent.com/u/11032969?v=4?s=100" width="100px;" alt="Alex"/><br /><sub><b>Alex</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3A0xE111" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/litestar/commits?author=0xE111" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://0110.be"><img src="https://avatars.githubusercontent.com/u/60453?v=4?s=100" width="100px;" alt="Joren Six"/><br /><sub><b>Joren Six</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=JorenSix" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

