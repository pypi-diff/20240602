# Comparing `tmp/pih-mio-0.30.1.tar.gz` & `tmp/pih-mio-0.30.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.30.1.tar", last modified: Tue May 21 20:16:08 2024, max compression
+gzip compressed data, was "pih-mio-0.30.2.tar", last modified: Sun Jun  2 06:21:26 2024, max compression
```

## Comparing `pih-mio-0.30.1.tar` & `pih-mio-0.30.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:08.214922 pih-mio-0.30.1/
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:07.557547 pih-mio-0.30.1/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.30.1/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.30.1/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   377190 2024-05-21 20:13:45.000000 pih-mio-0.30.1/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5930 2024-05-18 23:10:23.000000 pih-mio-0.30.1/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      303 2024-05-17 06:23:22.000000 pih-mio-0.30.1/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4472 2024-05-21 20:14:00.000000 pih-mio-0.30.1/MobileHelperService/const.py
--rw-rw-rw-   0        0        0     1009 2024-05-21 00:17:20.000000 pih-mio-0.30.1/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    18213 2024-05-20 00:19:11.000000 pih-mio-0.30.1/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      381 2024-05-17 06:41:58.000000 pih-mio-0.30.1/MobileHelperService/tools.py
--rw-rw-rw-   0        0        0      331 2024-05-21 20:16:08.199223 pih-mio-0.30.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 20:16:08.121096 pih-mio-0.30.1/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      331 2024-05-21 20:16:06.000000 pih-mio-0.30.1/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2024-05-21 20:16:06.000000 pih-mio-0.30.1/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:16:06.000000 pih-mio-0.30.1/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-21 20:16:06.000000 pih-mio-0.30.1/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-21 20:16:06.000000 pih-mio-0.30.1/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-21 20:16:06.000000 pih-mio-0.30.1/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:16:08.230470 pih-mio-0.30.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 06:21:27.054531 pih-mio-0.30.2/
+drwxrwxrwx   0        0        0        0 2024-06-02 06:21:26.685430 pih-mio-0.30.2/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.30.2/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.30.2/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   376914 2024-06-02 04:39:11.000000 pih-mio-0.30.2/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5930 2024-05-18 23:10:23.000000 pih-mio-0.30.2/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      303 2024-05-17 06:23:22.000000 pih-mio-0.30.2/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4472 2024-06-02 06:21:08.000000 pih-mio-0.30.2/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0     1009 2024-05-21 00:17:20.000000 pih-mio-0.30.2/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    18213 2024-05-21 23:56:06.000000 pih-mio-0.30.2/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      381 2024-05-17 06:41:58.000000 pih-mio-0.30.2/MobileHelperService/tools.py
+-rw-rw-rw-   0        0        0      331 2024-06-02 06:21:27.038909 pih-mio-0.30.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 06:21:27.007662 pih-mio-0.30.2/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      331 2024-06-02 06:21:25.000000 pih-mio-0.30.2/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-06-02 06:21:26.000000 pih-mio-0.30.2/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:21:25.000000 pih-mio-0.30.2/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-06-02 06:21:25.000000 pih-mio-0.30.2/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 06:21:25.000000 pih-mio-0.30.2/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-06-02 06:21:25.000000 pih-mio-0.30.2/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 06:21:27.070162 pih-mio-0.30.2/setup.cfg
```

### Comparing `pih-mio-0.30.1/MobileHelperService/api.py` & `pih-mio-0.30.2/MobileHelperService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,17 @@
     UserOutput,
     MarkOutput,
     OutputStub,
     SessionBase,
 )
 from pih.console_api import LINE
 
-def arg_value_is_file(value: str) -> bool:    
-    return value.startswith(FILE_PATTERN_LIST)
 
+def arg_value_is_file(value: str) -> bool:
+    return value.startswith(FILE_PATTERN_LIST)
 
 
 class MobileOutputBase(OutputStub):
 
     def b(self, value: str) -> str:
         return b(value)
 
@@ -134,18 +134,20 @@
             j((" ", A.CT_V.BLUE_ROMB, " ", lines[0])),
             jnl((A.D.map(lambda item: js((space, item)), lines[1:]))),  # type: ignore
         )
     )
 
 
 class MobileHelperUserSettiongsHolder:
-    
+
     @staticmethod
     def get(login_holder: str | User) -> MobileHelperUserSettings:
-        login_holder = login_holder.login if isinstance(login_holder, User) else login_holder
+        login_holder = (
+            login_holder.login if isinstance(login_holder, User) else login_holder
+        )
         value: MobileHelperUserSettings = MobileHelperUserSettings()
         result: MobileHelperUserSettings | None = A.S_U.get(
             login_holder, MOBILE_HELPER_USER_SETTINGS_NAME, value
         )
         if n(result):
             if MobileHelperUserSettiongsHolder.set(login_holder, value):
                 result = value
@@ -153,16 +155,18 @@
 
     @staticmethod
     def set(login: str, value: MobileHelperUserSettings) -> bool:
         return A.S_U.set(login, MOBILE_HELPER_USER_SETTINGS_NAME, value)
 
 
 class UserSettings:
-    def __init__(self, login_holder:  str | User):
-        self.login: str = login_holder.login if isinstance(login_holder, User) else login_holder
+    def __init__(self, login_holder: str | User):
+        self.login: str = (
+            login_holder.login if isinstance(login_holder, User) else login_holder
+        )
 
     def get(self) -> MobileHelperUserSettings:
         return MobileHelperUserSettiongsHolder.get(self.login)
 
     def set(self, value: int) -> bool:
         return MobileHelperUserSettiongsHolder.set(
             self.login, MobileHelperUserSettings(value)
@@ -174,34 +178,34 @@
     def remove(self, value: int) -> bool:
         return self.set(BM.remove(self.get().flags, value))
 
     def add(self, value: int) -> bool:
         return self.set(BM.add(self.get().flags, value))
 
 
-
-
 def get_command_variant_name(value: str | None) -> str:
     if n(value):
         return ""
     return nns(value).replace(COMMAND_NAME_VARIANT_SPLITTER, "")
 
 
-def command_node_name_equals_to(name: str, value: str, ) -> bool:
-    command_node_name_variant_index: int = name.find(
-        COMMAND_NAME_VARIANT_SPLITTER
-    )
+def command_node_name_equals_to(
+    name: str,
+    value: str,
+) -> bool:
+    command_node_name_variant_index: int = name.find(COMMAND_NAME_VARIANT_SPLITTER)
     if command_node_name_variant_index != -1:
         name = name[0:command_node_name_variant_index]
         command_node_name_length: int = len(name)
         if len(value) < command_node_name_length:
             return False
         value = value[0:command_node_name_length]
     return A.D.equal(value, name)
 
+
 def flag_name_list(value: Flags, all: bool = False) -> list[str]:
     result: list[str] = [
         item[0]
         for item in A.D.filter(lambda item: item[1] == value, list(FLAG_MAP.items()))
     ]
     return result if all else [result[0]]
 
@@ -389,17 +393,15 @@
     def break_line(self) -> None:
         pass
 
     def message_send(self, value: str) -> bool:
         return self.message_send_to_whatsapp(value)
 
     def message_send_to_whatsapp(self, value: str) -> bool:
-        return A.ME_WH_W.send(
-            self.get_recipient(), value, self.profile
-        )
+        return A.ME_WH_W.send(self.get_recipient(), value, self.profile)
 
     @contextmanager
     def make_send_to_group(self, group: A.CT.MESSAGE.WHATSAPP.GROUP):
         try:
             while_not_do(lambda: e(self.message_buffer))
             self.recipient = A.D.get(group)
             yield True
@@ -676,15 +678,16 @@
         self, group: MarkGroup, result: Result, use_index: bool
     ) -> None:
         group_name: str = nns(group.GroupName)
         self.write_line(
             j(
                 (
                     "Свободные карты доступа для группы доступа ",
-                    esc(group_name), ":",
+                    esc(group_name),
+                    ":",
                 )
             )
         )
         self.write_result(
             result,
             use_index=False,
             data_label_function=lambda index, _, __, data_value: j((index + 1, ". "))
@@ -1376,33 +1379,31 @@
         return 0 if n(self.arg_list) else len(self.arg_list)  # type: ignore
 
     @property
     def none_command(self) -> bool:
         return n(self.current_command)
 
     def ws_ping_handler(self) -> None:
+        host: str = self.arg() or self.input.input("Введите название хоста")
         with self.output.make_loading(loading_timeout=0.5):
             self.write_line(
                 js(
                     (
                         "Результат:",
                         A.D_F.yes_no(
-                            A.C_R.accessibility_by_smb_port(
-                                self.arg() or self.input.input("Введите название хоста")
-                            ),
+                            A.C_R.accessibility_by_smb_port(host),
                             True,
                         ),
                     )
                 )
             )
 
     @property
     def am_i_doctor(self) -> bool:
-        return self.session.am_i_admin or A.C_U.doctor(self.session.user) 
-
+        return self.session.am_i_admin or A.C_U.doctor(self.session.user)
 
     def yes_no_adapted(
         self,
         text: str,
         _: bool = False,
         yes_label: str = YES_LABEL,
         no_label: str = NO_LABEL,
@@ -1761,15 +1762,19 @@
                         "Памятка: Установка датчиков, карты и аккумулятора"
                     )
                 ],
                 holter_study_course_help_content_image_list,
             ),
             HelpContentHolder(
                 "nn5",
-                [self.output.italics("Памятка: Расположение датчиков на теле пациента")],
+                [
+                    self.output.italics(
+                        "Памятка: Расположение датчиков на теле пациента"
+                    )
+                ],
                 [
                     HelpImageContent(
                         lambda: MEDIA_CONTENT.IMAGE.HOLTER_DETECTORS_MAP, title=""
                     )
                 ],
             ),
             HelpContentHolder(
@@ -2922,28 +2927,27 @@
                                 nl(
                                     "Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации:"
                                 ),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
                                 # self.output.bold("P"),
-                                "Pacific ",
+                                "PIH: Pacific ",
                                 # self.output.bold("I"),
                                 "International ",
                                 # self.output.bold("H"),
                                 nl("Hospital "),
                                 nl("или"),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
                                 # self.output.bold("П"),
-                                "Пасифик ",
+                                "ПИХ: Пасифик ",
                                 # self.output.bold("И"),
                                 "Интернешнл ",
-                                self.output.bold("Х"),
                                 nl("Хоспитал.", count=2),
                                 self.output.bold("Автор"),
                                 ": ",
                                 nl("Караченцев Никита Александрович"),
                                 self.output.bold("Версия"),
                                 ": ",
                                 nl(VERSION),
@@ -3669,23 +3673,19 @@
         return self.pih.input
 
     def bold(self, value: Any) -> str:
         return self.output.bold(value)
 
     @property
     def arg_list_exclude_file(self) -> list[str]:
-        return A.D.filter(
-            lambda item: not arg_value_is_file(item), self.arg_list
-        )
-        
+        return A.D.filter(lambda item: not arg_value_is_file(item), self.arg_list)
+
     @property
     def arg_list_only_file(self) -> list[str]:
-        return A.D.filter(
-            arg_value_is_file, self.arg_list
-        )
+        return A.D.filter(arg_value_is_file, self.arg_list)
 
     @property
     def check_for_arg_list_include_file(self) -> bool:
         return (self.arg_len - len(self.arg_list_exclude_file)) != 0
 
     def arg(
         self,
@@ -3942,38 +3942,41 @@
                             self.user_given_name,
                             ", запущен тестовый процесс создания дампа базы данных",
                         )
                     )
                 )
             )
         else:
-            answer = self.yes_no(
-                "Изменить имя файла дампа базы данных",
-                self.output.bold("Отправьте имя"),
-                js(
-                    (
-                        "Использовать имя:",
-                        self.output.bold(name),
-                        "- отправьте",
-                        A.O.get_number(0),
-                    )
-                ),
-            )
-            self.write_line(
-                self.output.italics(
-                    j(
+            if A.C_COMP.process_is_running(A.CT_H.POLIBASE.NAME):
+                return
+            else:
+                answer = self.yes_no(
+                    "Изменить имя файла дампа базы данных",
+                    js(
                         (
-                            self.user_given_name,
-                            ", ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе: ",
-                            self.output.bold("Backup Console"),
+                            "Использовать имя:",
+                            self.output.bold(name),
+                            "- отправьте",
+                            A.O.get_number(1),
+                        )
+                    ),
+                    self.output.bold("Отправьте имя"),
+                )
+                self.write_line(
+                    self.output.italics(
+                        j(
+                            (
+                                self.user_given_name,
+                                ", ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе: ",
+                                self.output.bold("Backup Console"),
+                            )
                         )
                     )
                 )
-            )
-        A.A_P.DB.backup(self.input.answer if answer else name, test)
+        A.A_P.DB.backup(name if answer else self.input.answer, test)
 
     def show_polibase_password_handler(self) -> None:
         LOGIN: str = "login"
         PASSWORD: str = "password"
         result: dict[str, Any] | None = None
 
         def execute_query_for_password(condition: str) -> dict[str, Any] | None:
@@ -4712,15 +4715,17 @@
         def filter_function(item: Note) -> bool:
             title_list: list[str] = item.title.split(A.CT.SPLITTER)  # type: ignore
             if len(title_list) > 1:
                 return title_list[0].lower() in A.D.get(command_type)[1:]
             return True
 
         arg: Any = None
-        self.arg_list = A.D.sort(lambda item: int(not arg_value_is_file(item)), self.arg_list)
+        self.arg_list = A.D.sort(
+            lambda item: int(not arg_value_is_file(item)), self.arg_list
+        )
         if n(command_type):
             for i in range(max(1, self.arg_len)):
                 arg = self.arg(
                     i,
                     as_file=True,
                     filter_function=None if n(command_type) else filter_function,
                 )
@@ -4904,17 +4909,15 @@
                         command_text_line if ne(command_text_line) else None,
                         for_cmd=True,
                     )
                     if n(use_psexec_executor):
                         use_psexec_executor = e(
                             [
                                 value
-                                for value in A.D.map(
-                                    lambda item: lw(item), command_text_line
-                                )
+                                for value in lw(command_text_line)
                                 if value in A.CT.PSTOOLS.COMMAND_LIST
                             ]
                         )
                     process_result: CompletedProcess | None = None
                     if use_psexec_executor:
                         if e(host):
                             if self.yes_no(
@@ -4951,27 +4954,17 @@
                                     js(("Хост", self.output.bold(host), "не доступен"))
                                 )
                                 host = self.input.input(
                                     "Введите имя хоста, на котором будет выполнена команда"
                                 )
                     if n(host_is_local):
                         host_is_local = A.SYS.host_is_local(host)
-                    self.write_line(
-                        js(
+                    with self.output.make_loading(0.5, "Выполнение команды. Ожидайте"):
+                        process_result = A.EXC.execute(
                             (
-                                self.get_formatted_given_name(),
-                                "ожидайте окончания выполнения команды...",
-                            )
-                        )
-                    )
-                    if use_psexec_executor:
-                        with self.output.make_loading(
-                            0.5, "Выролнение команды. Ожидайте"
-                        ):
-                            process_result = A.EXC.execute(
                                 (
                                     A.EXC.create_command_for_powershell(
                                         command_text_line
                                     )
                                     if is_powershell
                                     else (
                                         command_text_line
@@ -4979,31 +4972,24 @@
                                         else A.EXC.create_command_for_psexec_powershell(
                                             command_text_line,
                                             host,
                                             interactive=None,
                                             run_from_system_account=True,
                                         )
                                     )
-                                ),  # type: ignore
-                                True,
-                                True,
-                                False,
-                            )
-                    else:
-                        with self.output.make_loading(
-                            0.5, "Выполнение команды. Ожидайте"
-                        ):
-                            process_result = A.EXC.execute(
-                                A.EXC.create_command_for_executor(
+                                )
+                                if use_psexec_executor
+                                else A.EXC.create_command_for_executor(
                                     nnl(text)[0], nnl(command_text_line)[1:]
-                                ),
-                                True,
-                                True,
-                                False,
-                            )
+                                )
+                            ),
+                            True,
+                            True,
+                            False,
+                        )
 
                     def decode(value: bytes | None) -> str | None:
                         if e(value):
                             return None
                         return nnb(value).decode(A.CT_WINDOWS.CHARSETS.ALTERNATIVE)
 
                     output: str | None = decode(process_result.stdout)
@@ -5730,15 +5716,15 @@
         report_file_path: str = A.PTH.join(
             A.PTH.MOBILE_HELPER.TIME_TRACKING_REPORT_FOLDER, report_file_name
         )
         allowed_report_for_all_persons: bool = (
             not for_me_report_only
             and not self.is_forced
             and A.C_A.action_for_group(
-                Groups.TimeTrackingReport, self.session,  False, True, False
+                Groups.TimeTrackingReport, self.session, False, True, False
             )
         )
 
         if A.A_TT.save_report(
             report_file_path,
             start_date,
             end_date,
@@ -6791,32 +6777,37 @@
             A.CT_AD.JobPositions.IT
         )
 
         def label_function(user: User, _) -> str:
             result: str = nl(js(("", A.CT.VISUAL.BULLET, self.output.bold(user.name))))
             if ne(user.description):
                 user_description_list: list[str] = A.D_F.description_list(
-                    user.description
+                    nnt(user.description)
                 )
-                workstation_name: str = user_description_list[1]
-                workstation: Workstation = A.R_WS.by_name(workstation_name).data
-                result += nl(j((" ", user_description_list[0])))
-                if nn(workstation):
-                    if ne(workstation.description):
-                        internal_telephone_number: str = str(
-                            A.D_Ex.decimal(workstation.description.split("(")[-1])
-                        )
-                        result += nl(
-                            js(
-                                (
-                                    "   Внутренний номер телефона:",
-                                    self.output.bold(internal_telephone_number),
+                result = j((result, nl(j((" ", user_description_list[0])))))
+                workstation_name: str | None = A.D.by_index(user_description_list, 1)
+                if nn(workstation_name):
+                    workstation: Workstation | None = A.R_WS.by_name(
+                        nnt(workstation_name)
+                    ).data
+                    if nn(workstation):
+                        if ne(nnt(workstation).description):
+                            internal_telephone_number: str = str(
+                                A.D_Ex.decimal(
+                                    nnt(nnt(workstation).description).split("(")[-1]
+                                )
+                            )
+                            result += nl(
+                                js(
+                                    (
+                                        "   Внутренний номер телефона:",
+                                        self.output.bold(internal_telephone_number),
+                                    )
                                 )
                             )
-                        )
             return result
 
         self.output.write_result(
             it_user_list,
             False,
             label_function=label_function,
             title="ИТ отдел это:",
@@ -7857,15 +7848,22 @@
             )
             MobileHelper.allowed_group_collection = allowed_group_set
         self.fill_allowed_group_list()
 
     def fill_allowed_group_list(self, session: Session | None = None) -> None:
         session = session or self.session
         for group in MobileHelper.allowed_group_collection:
-            A.C_A.action_for_group(group, session=session,exit_on_access_denied=False,  notify_on_fail=False, notify_on_success=False, cached=True)
+            A.C_A.action_for_group(
+                group,
+                session=session,
+                exit_on_access_denied=False,
+                notify_on_fail=False,
+                notify_on_success=False,
+                cached=True,
+            )
 
     def command_sort_function(self, value: list[CommandNode]) -> str:
         name_list: list[str] = []
         for item in value:
             name_list.append(
                 self.get_command_node_label(item) if n(item.order) else chr(item.order)
             )
@@ -7946,15 +7944,17 @@
                     self.flag_information,
                 )
             ]
         non_command_node_name_list: list[str] = []
         for arg_item in part_list:
             command_node_name_exists: bool = False
             for command_node_name_item in MobileHelper.command_node_name_collection:
-                command_node_name_exists = command_node_name_equals_to(command_node_name_item, arg_item)
+                command_node_name_exists = command_node_name_equals_to(
+                    command_node_name_item, arg_item
+                )
                 if command_node_name_exists:
                     self.commandless_part_list.remove(arg_item)
                     break
             if not command_node_name_exists:
                 non_command_node_name_list.append(arg_item)
         for arg_item in non_command_node_name_list:
             part_list.remove(arg_item)
@@ -8091,16 +8091,15 @@
                                 ):
                                     self.output.error("Нельзя адресовать самому себе!")
                                     recipient = None
                                 else:
                                     break
                             else:
                                 self.recipient_user_list = A.D.filter(
-                                    lambda item: item.login
-                                    != self.session.get_login()
+                                    lambda item: item.login != self.session.get_login()
                                     and A.C.telephone_number(item.telephoneNumber),
                                     self.recipient_user_list,
                                 )
                                 if len(self.recipient_user_list) == 0:
                                     self.output.error("Нельзя адресовать самому себе!")
                                     recipient = None
                                 else:
```

### Comparing `pih-mio-0.30.1/MobileHelperService/client.py` & `pih-mio-0.30.2/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.30.1/MobileHelperService/const.py` & `pih-mio-0.30.2/MobileHelperService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.30.1"
+VERSION: str = "0.30.2"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
```

### Comparing `pih-mio-0.30.1/MobileHelperService/service.py` & `pih-mio-0.30.2/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.30.1/MobileHelperService/service_api.py` & `pih-mio-0.30.2/MobileHelperService/service_api.py`

 * *Files identical despite different names*

