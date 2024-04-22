# Comparing `tmp/pih-mio-0.28.tar.gz` & `tmp/pih-mio-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.28.tar", last modified: Wed Apr 10 05:34:35 2024, max compression
+gzip compressed data, was "pih-mio-0.29.1.tar", last modified: Mon Apr 22 04:12:03 2024, max compression
```

## Comparing `pih-mio-0.28.tar` & `pih-mio-0.29.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 05:34:35.375046 pih-mio-0.28/
-drwxrwxrwx   0        0        0        0 2024-04-10 05:34:34.980333 pih-mio-0.28/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.28/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.28/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   361191 2024-04-10 05:19:48.000000 pih-mio-0.28/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.28/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.28/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4461 2024-04-10 05:33:31.000000 pih-mio-0.28/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.28/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    16542 2024-04-10 05:18:33.000000 pih-mio-0.28/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      329 2024-04-10 05:34:35.312535 pih-mio-0.28/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 05:34:35.281287 pih-mio-0.28/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-10 05:34:33.000000 pih-mio-0.28/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-10 05:34:34.000000 pih-mio-0.28/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 05:34:33.000000 pih-mio-0.28/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-10 05:34:33.000000 pih-mio-0.28/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-04-10 05:34:33.000000 pih-mio-0.28/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 05:34:33.000000 pih-mio-0.28/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 05:34:35.390659 pih-mio-0.28/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 04:12:03.135127 pih-mio-0.29.1/
+drwxrwxrwx   0        0        0        0 2024-04-22 04:12:02.690916 pih-mio-0.29.1/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.1/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.1/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   374073 2024-04-22 03:14:50.000000 pih-mio-0.29.1/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.1/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.1/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4465 2024-04-22 04:11:21.000000 pih-mio-0.29.1/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.29.1/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    16542 2024-04-10 05:18:33.000000 pih-mio-0.29.1/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      331 2024-04-22 04:12:03.088251 pih-mio-0.29.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 04:12:03.056998 pih-mio-0.29.1/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      331 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-22 04:12:02.000000 pih-mio-0.29.1/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 04:12:03.166460 pih-mio-0.29.1/setup.cfg
```

### Comparing `pih-mio-0.28/MobileHelperService/api.py` & `pih-mio-0.29.1/MobileHelperService/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     j,
     jp,
     nl,
     lw,
     js,
     nn,
     ne,
+    nnt,
     nns,
     one,
     esc,
     jnl,
     nnb,
     nnl,
     escs,
@@ -71,15 +72,15 @@
     while_not_do,
 )
 from pih.consts import (
     CheckableSections,
     Actions,
     JournalType,
     Tags,
-    EmailVerificationMethods
+    EmailVerificationMethods,
 )
 from MobileHelperService.collection import MobileHelperUserSettings
 from pih.consts.polibase import PolibaseDocumentTypes
 from pih.consts.ssh_hosts import SSHHosts
 from MobileHelperService.const import *
 
 from pih.consts.errors import BarcodeNotFound, NotFound, Error
@@ -91,16 +92,16 @@
     Output,
     Session,
     PIHThread,
     MarkInput,
     UserInput,
     UserOutput,
     MarkOutput,
-    SessionBase,
     OutputStub,
+    SessionBase,
 )
 from pih.console_api import LINE
 
 
 class MobileOutputBase(OutputStub):
 
     def b(self, value: str) -> str:
@@ -158,53 +159,44 @@
     def remove(self, value: int) -> bool:
         return self.set(BM.remove(self.get().flags, value))
 
     def add(self, value: int) -> bool:
         return self.set(BM.add(self.get().flags, value))
 
 
-def command_name_base(value: str) -> str:
-    return value.split(COMMAND_NAME_BASE_DELEMITER)[0]
+def get_command_base_name(value: str) -> str:
+    return value.split(COMMAND_NAME_VARIANT_SPLITTER)[0]
+
+
+def get_command_variant_name(value: str | None) -> str:
+    if n(value):
+        return ""
+    return value.replace(COMMAND_NAME_VARIANT_SPLITTER, "")
+
+
+def command_node_name_equal(value1: str, value2: str) -> bool:
+    return A.D.equal(value1, get_command_base_name(value2)) or A.D.equal(
+        value1, get_command_variant_name(value2)
+    )
 
 
 def mio_command(value: list[str] | str) -> str:
     if isinstance(value, str):
-        return command_name_base(value)
+        return get_command_base_name(value)
     return mio_command(one(value))
 
 
 def flag_name_list(value: Flags, all: bool = False) -> list[str]:
     result: list[str] = [
         item[0]
         for item in A.D.filter(lambda item: item[1] == value, list(FLAG_MAP.items()))
     ]
     return result if all else [result[0]]
 
 
-def flag_string_represent(value: Flags, all: bool = True) -> str:
-    return js(
-        (
-            "[",
-            j(
-                A.D.map(lambda item: b(item), flag_name_list(value, all)),
-                j((" ", i("или"), " ")),
-            ),
-            "]",
-        )
-    )
-
-
-def format_given_name(
-    session: Session, _: Output | None, name: str | None = None
-) -> str | None:
-    if e(session.login):
-        return None
-    return b(name or session.user_given_name)
-
-
 class InternalInterrupt(Exception):
     @property
     def type(self) -> int:
         return self.args[0]
 
 
 class AddressedInterruption(Exception):
@@ -230,19 +222,19 @@
         self,
         result: Result[list[User]],
         caption: str | None = None,
         use_index: bool = False,
         root_location: str = A.CT_AD.ACTIVE_USERS_CONTAINER_DN,
     ) -> None:
         if ne(caption):
-            self.parent.write_line(b(caption))
+            self.parent.write_line(self.parent.bold(caption))
         self.parent.write_result(result, use_index=use_index)
 
     def get_formatted_given_name(self, value: str | None = None) -> str:
-        return b(value)
+        return self.parent.bold(value)
 
 
 class MobileSession(SessionBase):
     def __init__(self, recipient: str, flags: int | None = 0):
         super().__init__(name="mobile", flags=flags)  # type: ignore
         self.recipient: str = recipient
         self.user: User | None = None
@@ -277,27 +269,27 @@
     def exit(self, _1: int | None = None, _2: str | None = None) -> None:
         raise InternalInterrupt(InterruptionTypes.EXIT)
 
     @property
     def argv(self) -> list[str] | None:
         return self.arg_list
 
-    def arg(self, index: int = 0, default_value: Any | None = None) -> str | Any | None:
+    def arg(self, index: int = 0, default_value: Any = None) -> str | Any:
         return A.D.by_index(self.argv, index, default_value)
 
 
 class MobileMarkOutput(MarkOutput):
     def result(
         self,
         result: Result[list[Mark]],
         caption: str | None = None,
         use_index: bool = False,
     ) -> None:
         if ne(caption):
-            self.parent.write_line(b(caption))
+            self.parent.write_line(self.parent.bold(caption))
         self.parent.write_result(result, use_index=use_index)
 
 
 @dataclass
 class MessageHolder:
     body: str | None = None
     text_before: str = ""
@@ -368,14 +360,15 @@
         text: str,
         text_before: str | None = None,
         text_after: str | None = None,
     ) -> str:
         return text
 
     def whatsapp_send(self, text: str) -> bool:
+        A.L.debug_bot(text)
         return A.ME_WH_W.send(self.get_recipient(), text, self.profile)
 
     @contextmanager
     def make_send_to_group(self, group: A.CT.MESSAGE.WHATSAPP.GROUP):
         try:
             while_not_do(lambda: e(self.message_buffer))
             self.recipient = A.D.get(group)
@@ -562,15 +555,15 @@
     ) -> str:
         return i(
             js(
                 (
                     title,
                     j(
                         A.D.map(
-                            lambda item: b(A.D.capitalize(item)),
+                            lambda item: self.bold(A.D.capitalize(item)),
                             keywords,
                         ),
                         " или ",
                     ),
                 )
             )
         )
@@ -583,15 +576,15 @@
                 if self.show_exit_message:
                     with self.make_indent(2):
                         with self.make_personalized(False):
                             self.write_line(self.exit_line or self.create_exit_line())
 
     def value(self, caption: str, value: Any, text_before: str | None = None) -> None:
         self.separated_line()
-        self.write_line(j((b(caption), ": ", value)))
+        self.write_line(j((self.bold(caption), ": ", value)))
 
     def good(self, value: str) -> None:
         self.write_line(nl(js((A.CT_V.GOOD, value))))
 
     def error(self, value: str | Any) -> None:
         if self.show_error:
             self.separated_line()
@@ -603,30 +596,30 @@
                             (value if isinstance(value, str) else value.get_details()),
                         )
                     )
                 )
             )
 
     def head(self, value: str) -> None:
-        self.write_line(nl(b(value.upper())))
+        self.write_line(nl(self.bold(value.upper())))
 
     def head1(self, value: str) -> None:
-        self.write_line(nl(b(value)))
+        self.write_line(nl(self.bold(value)))
 
     def head2(self, value: str) -> None:
-        self.write_line(b(value))
+        self.write_line(self.bold(value))
 
     def new_line(self) -> None:
         return
 
     def separated_line(self) -> None:
         self.type = BM.add(self.type, MessageType.SEPARATE_ONCE)
 
     def header(self, value: str) -> None:
-        self.write_line(js(("", A.CT_V.BULLET, nl(b(value)))))
+        self.write_line(js(("", A.CT_V.BULLET, nl(self.bold(value)))))
 
     def bold(self, value: str) -> str:
         return b(value)
 
     def italic(self, value: str) -> str:
         return i(value)
 
@@ -642,15 +635,15 @@
                 )
             )
         )
         self.write_result(
             result,
             use_index=False,
             data_label_function=lambda index, _, __, data_value: j((index + 1, ". "))
-            + b(data_value),
+            + self.bold(data_value),
         )
 
     def table_with_caption(
         self,
         result: Result,
         caption: str | None = None,
         use_index: bool = False,
@@ -668,24 +661,24 @@
             if not isinstance(data, list):
                 data = [data]
             length: int = len(data)
             if length == 1:
                 use_index = False
             if use_index:
                 field_list.list.insert(0, A.CT_FC.INDEX)
-            item_data: Any | None = None
+            item_data: Any = None
             result_text_list: list[list[str]] = []
             for index, item in enumerate(data):
                 row_data: list = []
                 for field_item_obj in field_list.get_list():
                     field_item: FieldItem = field_item_obj
                     if field_item.visible:
                         if field_item == A.CT_FC.INDEX:
                             row_data.append(
-                                j((b(index + 1), "."))
+                                j((self.bold(index + 1), "."))
                                 + " "
                                 * (
                                     len(str(length))
                                     - len(str(index + 1))
                                     + 1
                                     + (1 if index < 9 and len(str(length)) > 1 else 0)
                                 )
@@ -850,15 +843,15 @@
             else:
                 self.output.error("Неверный формат номера телефона!")
 
     def input(
         self,
         caption: str | None = None,
         _: bool = True,
-        check_function: Callable[[str], Any | None] | None = None,
+        check_function: Callable[[str], Any] | None = None,
     ) -> str:
         input_data: str | None = None
         while True:
             if ne(caption):
                 with self.output.make_indent(0):
                     self.output.input(caption)
             self.stdin.wait_for_data_input = True
@@ -971,15 +964,15 @@
 
     def polibase_person_card_registry_folder(
         self, value: str | None = None, title: str | None = None
     ) -> str:
         return self.wait_for_polibase_person_card_registry_folder_input(
             lambda: super(MobileInput, self).polibase_person_card_registry_folder(
                 value,
-                f"Введите:\n  {A.CT_V.BULLET} название папки с картами пациентов\n  {A.CT_V.BULLET} символ {b('!')} для автоматического выбора папки\n или\n  {A.CT_V.BULLET} отсканируйте QR-код на папке реестра карт пациентов",
+                f"Введите:\n  {A.CT_V.BULLET} название папки с картами пациентов\n  {A.CT_V.BULLET} символ {self.output.bold('!')} для автоматического выбора папки\n или\n  {A.CT_V.BULLET} отсканируйте QR-код на папке реестра карт пациентов",
             )  # type: ignore
         )
 
     def polibase_person_any(self, title: str | None = None) -> str:
         return self.wait_for_polibase_person_pin_input(
             lambda: self.input(
                 title
@@ -992,15 +985,15 @@
 class CommandNode:
     name_list: list[str] | None = None
     title_and_label: list[str] | Callable[[], list[str]] | None = None
     handler: Callable[[], None] | None = None
     allowed_groups: list[Groups] | None = None
     wait_for_input: bool = True
     show_in_main_menu: bool = False
-    parent: Any | None = None
+    parent: Any = None
     text: str | Callable[[], str] | None = None
     visible: bool = True
     show_always: bool = False
     description: str | Callable[[], str] | None = None
     order: int | None = None
     filter_function: Callable[[], bool] | None = None
     help_text: Callable[[], str] | None = None
@@ -1118,27 +1111,43 @@
     FROM_FILE_REDIRECT: str = FROM_FILE_REDIRECT_SYMBOL
 
 
 def get_file_pattern_index(value: str | None) -> int | None:
     if e(value):
         return None
     for file_pattern_index, pattern in enumerate(FILE_PATTERN_LIST):
-        if value.find(pattern) == 0:
+        if nnt(value).find(pattern) == 0:
             return file_pattern_index
     return None
 
 
 def check_for_arg_is_file(self, value: str) -> bool:
     return nn(get_file_pattern_index(value))
 
 
 class MobileHelper(OutputStub):
 
-    command_name_set: set[str] | None = None
-    allowed_group_set: set[Groups] | None = None
+    command_base_name_collection: tuple[str, ...] | None = None
+    command_node_name_collection: tuple[str, ...] | None = None
+    allowed_group_collection: set[Groups] | None = None
+
+    def flag_string_represent(self, value: Flags, all: bool = True) -> str:
+        return js(
+            (
+                "[",
+                j(
+                    A.D.map(
+                        self.output.bold,
+                        flag_name_list(value, all),
+                    ),
+                    j((" ", i("или"), " ")),
+                ),
+                "]",
+            )
+        )
 
     def create_study_course_item(
         self,
         index: int,
         item: HelpContentHolder,
         item_list: dict[CommandNode, None],
         content_list: list[HelpContentHolder],
@@ -1192,17 +1201,17 @@
             )
         ]
 
     def get_it_telephone_number_text(self) -> str:
         return j(
             (
                 "Общий телефон: ",
-                nl(b("709")),
+                nl(self.output.bold("709")),
                 "Сотовый телефон: ",
-                b(A.D_TN.by_login("Administrator")),
+                self.output.bold(A.D_TN.by_login("Administrator")),
             )
         )
 
     def long_operation_handler(self) -> None:
         self.write_line(i("Ожидайте получения результата..."))
 
     @staticmethod
@@ -1306,25 +1315,25 @@
         self.current_command: list[CommandNode] | None = None
         self.command_list: list[list[CommandNode]] = []
         self.command_history: list[list[CommandNode]] = []
         self.recipient_user_list: list[User] | None = None
         self.line: str | None = None
         self.show_good_bye: bool | None = None
         self.language_index: int | None = None
-        self.comandless_line_part_list: list[str] | None
+        self.commandless_part_list: list[str] | None
         self.menu = MENU()
         self.keywords = KEYWORDS()
         self.return_result_key: str | None = None
         self.user_settings: UserSettings = UserSettings(self.session.login)
         # output stub rewrite
         self.b = b
         self.i = i
 
         def get_formatted_given_name(name: str | None = None) -> str | None:
-            return format_given_name(self.session, None, name)
+            return self.output.bold(name or self.session.user_given_name)
 
         self.output.user.get_formatted_given_name = get_formatted_given_name
         #######################
         self.study_node: CommandNode = self.create_command_link(
             A.D.map(lambda item: j((COMMAND_LINK_SYMBOL, item)), ["study", "обучение"]),
             "study",
             ["Обучение"],
@@ -1682,15 +1691,15 @@
                     item,
                     HOLTER_STUDY_COURSE_COLLECTION,
                     HOLTER_STUDY_COURSE_CONTENT_LIST,
                 )
             ] = None
         #######################
         reboot_workstation_node: CommandNode = CommandNode(
-            ["reboot", "перезагруз^ить"],
+            ["reboot", "перезагруз|ить"],
             lambda: [
                 "перезагрузить компьютер",
                 "перезагрузить" + (" компьютер" if self.in_choose_command else ""),
             ],
             self.reboot_workstation_handler,
             ADMIN_GROUPS,
             filter_function=lambda: self.is_not_all or self.in_main_menu,
@@ -1700,18 +1709,18 @@
             lambda: [
                 "перезагрузка всех компьютеров",
                 "перезагрузить все" + (" компьютеры" if self.in_choose_command else ""),
             ],
             lambda: self.reboot_workstation_handler(True),
             ADMIN_GROUPS,
             filter_function=lambda: self.is_all or self.in_main_menu,
-            help_text=lambda: flag_string_represent(Flags.ALL),
+            help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         shutdown_workstation_node: CommandNode = CommandNode(
-            ["shutdown", "выключ^ить"],
+            ["shutdown", "выключ|ить"],
             lambda: [
                 "выключение компьютера",
                 "выключить" + (" компьютер" if self.is_all else ""),
             ],
             self.shutdown_workstation_handler,
             ADMIN_GROUPS,
             filter_function=lambda: self.is_not_all or self.in_main_menu,
@@ -1721,15 +1730,15 @@
             lambda: [
                 "выключение всех компьютеров",
                 "выключить все" + (" компьютеры" if self.is_all else ""),
             ],
             lambda: self.shutdown_workstation_handler(True),
             ADMIN_GROUPS,
             filter_function=lambda: self.is_all,
-            help_text=lambda: flag_string_represent(Flags.ALL),
+            help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         find_workstation_node: CommandNode = CommandNode(
             self.keywords.command.FIND,
             lambda: [
                 "Поиск компьютера",
                 "Найти" + (" компьютер" if self.in_choose_command else ""),
             ],
@@ -1744,15 +1753,15 @@
                     "Показать весь список компьютеров"
                     if self.in_choose_command
                     else "Весь список"
                 ),
             ],
             lambda: self.find_workstation_handler(True),
             filter_function=lambda: self.is_all,
-            help_text=lambda: flag_string_represent(Flags.ALL),
+            help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         msg_to_node: CommandNode = CommandNode(
             ["msg", "сообщение", "message"],
             lambda: [
                 "Отправка сообщения пользователю",
                 "Отправить сообщение"
                 + (" пользователю" if self.in_choose_command else ""),
@@ -1791,24 +1800,24 @@
                 "все компьютеры на доступность",
             ],
             lambda: self.check_resources_and_indications_handler(
                 [CheckableSections.WS], True
             ),
             ADMIN_GROUPS,
             filter_function=lambda: self.is_all,
-            help_text=lambda: flag_string_represent(Flags.ALL),
+            help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         process_kill_node: CommandNode = CommandNode(
             ["kill", "завершить"],
             ["Завершение процесса", "Завершить процесс"],
             lambda: self.console_apps_api.process_kill(self.arg(), self.arg(1)),
             filter_function=lambda: self.is_not_all or self.in_main_menu,
         )
         disks_report_node: CommandNode = CommandNode(
-            ["disk^s", "диски"],
+            ["disk|s", "диски"],
             ["Показать информацию о дисках"],
             lambda: self.console_apps_api.disks_report(self.arg()),
             filter_function=lambda: self.is_not_all or self.in_main_menu,
         )
         self.menu.workstation = [
             reboot_workstation_node,
             reboot_all_workstations_node,
@@ -1899,15 +1908,15 @@
                     (
                         "Показать весь список",
                         " заметок" if self.in_choose_command else "",
                     )
                 ),
             ],
             self.note_find_handler,
-            help_text=lambda: flag_string_represent(Flags.ALL),
+            help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         self.menu.notes = [
             create_note_node,
             self.find_note_node,
             self.show_all_note_node,
         ]
         self.menu.journals = [add_journal_record_node, show_journal_node]
@@ -1928,95 +1937,109 @@
             ["tt", "урв"], ["учёт рабочего времени"], self.time_tracking_report_handler
         )
         my_time_tracking_report_node: CommandNode = CommandNode(
             ["my_tt", "мой_урв"],
             ["Мои отметки ухода и прихода"],
             lambda: self.time_tracking_report_handler(True),
         )
-        marketer_statistics: CommandNode = CommandNode(
+        marketer_reviews_statistics: CommandNode = CommandNode(
             ["statistics", "статистика"],
-            ["Статистика по отзывам"],
-            self.marketer_statistics_handler,
+            ["Статистика по отзывам", "Статистика"],
+            self.marketer_review_statistics_handler,
+        )
+        marketer_reviews_settings: CommandNode = CommandNode(
+            ["settings", "настройка"],
+            ["Настройка отзывов", "Настройка"],
+            self.marketer_review_settings_handler,
+        )
+        marketer_reviews_menu: CommandNode = CommandNode(
+            ["review|s", "отзыв|ы"],
+            ["Отзывы"],
+            lambda: self.menu_handler(
+                [marketer_reviews_statistics, marketer_reviews_settings]
+            ),
         )
         self.menu.hr_unit = [my_time_tracking_report_node]
-        self.menu.marketer_unit = [marketer_statistics]
+        self.menu.marketer_unit = [marketer_reviews_menu]
         hr_unit_node: CommandNode = CommandNode(
-            ["hr", "кадр^ов"],
+            ["hr", "кадр|ов"],
             ["Отдел кадров"],
             lambda: self.menu_handler(self.menu.hr_unit),
             text=lambda: j(
                 (
                     "Руководитель: ",
-                    b(
+                    self.output.bold(
                         one(
                             A.R.filter(
                                 lambda item: not item.samAccountName.startswith(
                                     A.CT_AD.TEMPLATED_USER_SERACH_TEMPLATE[0]
                                 )
                                 and not item.samAccountName.endswith(
                                     A.CT_AD.TEMPLATED_USER_SERACH_TEMPLATE[-1]
                                 ),
                                 A.R_U.by_job_position(A.CT_AD.JobPositions.HR),
                             )
                         ).name
                     ),
                     nl("."),
                     "Телефон: ",
-                    b("706"),
+                    self.output.bold("706"),
                     ".",
                 )
             ),
         )
         marketer_unit_node: CommandNode = CommandNode(
-            ["marketing", "маркет^олог", "marketer"],
+            ["marketing", "маркет|олог", "marketer"],
             ["Отдел маркетинга"],
             lambda: self.menu_handler(self.menu.marketer_unit),
             text=lambda: j(
                 (
                     "Руководитель: ",
-                    b(one(A.R_U.by_job_position(A.CT_AD.JobPositions.MARKETER)).name),
+                    self.output.bold(
+                        one(A.R_U.by_job_position(A.CT_AD.JobPositions.MARKETER)).name
+                    ),
                     ".",
                     nl() * 2,
                     A.D_F.wappi_status(A.CT_ME_WH_W.Profiles.MARKETER, self.output),
                 )
             ),
         )
         self.menu.unit = [
             it_unit_node,
             call_centre_unit_node,
             hr_unit_node,
             marketer_unit_node,
         ]
         #######################
         robocopy_node: CommandNode = CommandNode(
-            ["rb^k", "robocopy"],
+            ["rb|k", "robocopy"],
             ["Запуск Robocopy-задания"],
             self.robocopy_job_run_handler,
         )
         polibase_backup_node: CommandNode = CommandNode(
-            ["pb^k"],
+            ["pb|k"],
             [
                 "Создание бекапа базы данных Polibase",
                 "Создать бекап базы данных Polibase",
             ],
             self.create_polibase_db_backup_handler,
         )
         self.menu.backup = [robocopy_node, polibase_backup_node]
 
         #######################
         polibase_person_information_node: CommandNode = CommandNode(
-            ["info^rmation", "инфо^рмация"],
+            ["info|rmation", "инфо|рмация"],
             lambda: [
                 "Информация о пациенте",
                 "Информация" + (" о пациенте" if self.in_choose_command else ""),
             ],
             self.polibase_person_show_information_handler,
         )
         polibase_doctor_visits_node: CommandNode = CommandNode(
-            ["visit^s", "приём^ы", "визит^ы", "прием^ы"],
+            ["visit|s", "приём|ы", "визит|ы", "прием|ы"],
             lambda: ["Список моих приёмов", "Показать список моих приёмов"],
             self.polibase_visit_handler,
             filter_function=lambda: self.am_i_doctor,
         )
         polibase_person_find_card_registry_or_folder_node: CommandNode = CommandNode(
             self.keywords.command.FIND,
             lambda: [
@@ -2026,28 +2049,28 @@
                 + " или папку",
             ],
             self.polibase_person_card_registry_folder_find_handler,
             filter_function=lambda: self.is_not_all or self.in_main_menu,
         )
 
         check_email_node: CommandNode = CommandNode(
-            ["email", "почт^ы", "mail"],
+            ["email", "почт|ы", "mail"],
             lambda: [
                 "Проверка адресса электронной почты",
                 (
                     "Проверить адресс электронной почты"
                     if self.in_choose_command
                     else "Адресса электронной почты"
                 ),
             ],
             lambda: self.check_email_address_handler(),
         )
 
         check_valenta_node: CommandNode = CommandNode(
-            ["valenta", "валент^у"],
+            ["valenta", "валент|у"],
             lambda: [
                 "Проверка наличия новых исследований в Валенте",
                 j(
                     (
                         (
                             "Проверить наличие новых исследований в Валенте"
                             if self.in_choose_command
@@ -2059,15 +2082,15 @@
             ],
             lambda: self.check_resources_and_indications_handler(
                 [CheckableSections.VALENTA]
             ),
         )
 
         check_printers_node: CommandNode = CommandNode(
-            ["printer^s", "принтер^ы"],
+            ["printer|s", "принтер|ы"],
             lambda: [
                 "Проверка принтеров",
                 "Проверить принтеры" if self.in_choose_command else "Принтеров",
             ],
             lambda: self.check_resources_and_indications_handler(
                 [CheckableSections.PRINTERS]
             ),
@@ -2151,43 +2174,43 @@
                 "Поиск пользователя",
                 j(("Найти", (" пользователя" if self.in_choose_command else ""))),
             ],
             self.user_find_handler,
             filter_function=lambda: self.is_not_all or self.in_choose_command,
         )
         change_user_telephone_number_node: CommandNode = CommandNode(
-            ["phone", "телефон^е"],
+            ["phone", "телефон|е"],
             lambda: [
                 "Изменение телефонного номера пользователя",
                 j(
                     (
                         "Изменить телефонный номер",
                         (" пользователя" if self.in_main_menu else ""),
                     )
                 ),
             ],
             lambda: self.user_property_set_handler(0),
             ADMIN_GROUPS,
             filter_function=lambda: self.is_not_all or self.in_choose_command,
         )
         change_all_user_telephone_number_node: CommandNode = CommandNode(
-            ["phone", "телефон^е"],
+            ["phone", "телефон|е"],
             lambda: [
                 "Редактирование всех телефонных номеров",
                 j(
                     (
                         "Изменить все телефонные номера",
                         (" пользователей" if self.in_choose_command else ""),
                     )
                 ),
             ],
             lambda: self.user_property_set_handler(0),
             ADMIN_GROUPS,
             filter_function=lambda: self.is_all,
-            help_text=lambda: flag_string_represent(Flags.ALL),
+            help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         change_user_password_node: CommandNode = CommandNode(
             self.keywords.command.PASSWORD,
             lambda: [
                 "Изменение пароля пользователя",
                 j(
                     (
@@ -2275,45 +2298,45 @@
                 A.D.get(A.CT_CMDT.SSH)[1:],
                 self.get_run_title_and_label(A.CT_CMDT.SSH),
                 lambda: self.run_command_handler(A.CT_CMDT.SSH),
             ),
         ]
         #######################
         check_resources_node: CommandNode = CommandNode(
-            ["resource^s", "ресурс^ы"],
+            ["resource|s", "ресурс|ы"],
             lambda: [
                 "Проверка основных ресурсов",
                 (
                     "Проверить основные ресурсы"
                     if self.in_choose_command
                     else "основных ресурсов"
                 ),
             ],
             lambda: self.check_resources_and_indications_handler(
                 [CheckableSections.RESOURCES]
             ),
             ADMIN_GROUPS + [Groups.RD, Groups.IndicationWatcher],
         )
         check_indications_node: CommandNode = CommandNode(
-            ["indication^s", "показан^ия"],
+            ["indication|s", "показания"],
             lambda: [
                 "Проверка показаний отделения лучевой диагностики",
                 (
                     "Проверить показания отделения лучевой диагностики"
                     if self.in_choose_command
                     else "Показаний отделения лучевой диагностики"
                 ),
             ],
             lambda: self.check_resources_and_indications_handler(
                 [CheckableSections.INDICATIONS]
             ),
             ADMIN_GROUPS + [Groups.RD, Groups.IndicationWatcher],
         )
         check_backups_node: CommandNode = CommandNode(
-            ["backup^s", "бекап^ы", "rbk"],
+            ["backup|s", "бекап|ы", "rbk"],
             lambda: [
                 "Список Robocopy-заданий",
                 (
                     "Проверить Robocopy-задания"
                     if self.in_choose_command
                     else "Robocopy-заданий"
                 ),
@@ -2348,15 +2371,15 @@
                     else "Отсканированого документа"
                 ),
             ],
             self.check_scanned_document_handler,
             # filter_function=lambda: not self.argless,
         )
         check_disks_node: CommandNode = CommandNode(
-            ["disk^s", "диск^и"],
+            ["disk|s", "диск|и"],
             lambda: [
                 "Проверка свободного места на всех наблюдаемых дисках",
                 (
                     "Проверить свободное места на всех наблюдаемых дисках"
                     if self.in_choose_command
                     else "свободного места на всех наблюдаемых дисках"
                 ),
@@ -2376,18 +2399,18 @@
                     if self.in_choose_command
                     else "Всех компонентов"
                 ),
             ],
             None,
             True,
         )
-        check_all_node.help_text = lambda: flag_string_represent(Flags.ALL)
+        check_all_node.help_text = lambda: self.flag_string_represent(Flags.ALL)
         #######################
         polibase_restart_node: CommandNode = CommandNode(
-            ["restart", "перезагруз^ить"],
+            ["restart", "перезагруз|ить"],
             A.D.map(
                 lambda item: js((item, "Polibase")),
                 ["Перезагрузка сервера", "Перезагрузить сервер"],
             ),
             self.console_apps_api.polibase_restart,
             ADMIN_GROUPS,
         )
@@ -2643,16 +2666,16 @@
             "wiki",
             ["Наша Вики", "Наша Вики - источник знаний!"],
             WIKI_BASE_CONTENT_LIST
             + [
                 HelpImageContent(
                     lambda: MEDIA_CONTENT.IMAGE.WIKI_PAGE,
                     None,
-                    f"Откроется браузер и отобразится страница.\n\n_{b('Важное дополнение')}: получить доступ к сайту можно, введя в адресной строке браузера текст: "
-                    + b(A.CT_ADDR.WIKI_SITE_ADDRESS)
+                    f"Откроется браузер и отобразится страница.\n\n_{self.output.bold('Важное дополнение')}: получить доступ к сайту можно, введя в адресной строке браузера текст: "
+                    + self.output.bold(A.CT_ADDR.WIKI_SITE_ADDRESS)
                     + "_",
                     False,
                 )
             ],  # type: ignore
         )
         IT_HELP_CONTENT_HOLDER_LIST: list[HelpContentHolder] = [
             HelpContentHolder(
@@ -2708,15 +2731,17 @@
         ]
 
         self.main_menu_node: CommandNode = CommandNode(
             ["menu", "меню"],
             ["Меню"],
             self.main_menu_handler,
             text=lambda: nl(
-                b("Все команды:") if self.is_all else b("Список разделов:")
+                self.output.bold("Все команды:")
+                if self.is_all
+                else self.output.bold("Список разделов:")
             ),
         )
         #######################
         self.address_node: CommandNode = self.create_command_link(
             j(("to", FLAG_KEYWORDS.ADDRESS_SYMBOL), "|"),
             FLAG_KEYWORDS.ADDRESS_SYMBOL,
             i("Адресовать команду"),
@@ -2731,15 +2756,15 @@
             i("Адресовать ссылку на команду"),
             ADMIN_GROUPS,
             True,
         )
         self.address_as_link_node.order = 3
         #######################
         self.all_commands_node: CommandNode = self.create_command_link(
-            j((COMMAND_LINK_SYMBOL, j((flag_string_represent(Flags.ALL, True))))),
+            j((COMMAND_LINK_SYMBOL, j((self.flag_string_represent(Flags.ALL, True))))),
             FLAG_KEYWORDS.ALL_SYMBOL,
             [i("Все команды")],
             None,
             True,
         )
         self.all_commands_node.order = 1
         self.all_commands_node.filter_function = lambda: not self.in_choose_command
@@ -2760,35 +2785,35 @@
                             (
                                 nl(
                                     "Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации:"
                                 ),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
-                                b("P"),
+                                self.output.bold("P"),
                                 " acific ",
-                                b("I"),
+                                self.output.bold("I"),
                                 " nternational ",
-                                b("H"),
+                                self.output.bold("H"),
                                 nl(" ospital "),
                                 nl("или"),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
-                                b("П"),
+                                self.output.bold("П"),
                                 " асифик ",
-                                b("И"),
+                                self.output.bold("И"),
                                 " нтернейшнл ",
-                                b("Х"),
+                                self.output.bold("Х"),
                                 nl(" оспитал.", count=2),
-                                b("Автор: "),
+                                self.output.bold("Автор: "),
                                 nl("Караченцев Никита Александрович"),
-                                b("Версия: "),
+                                self.output.bold("Версия: "),
                                 nl(VERSION),
-                                b("Сервер: "),
+                                self.output.bold("Сервер: "),
                                 A.SYS.host(),
                                 nl(),
                                 LINE,
                                 nl(),
                                 get_wappi_status("  ", A.CT_ME_WH_W.Profiles.IT),
                                 nl() * 2,
                                 get_wappi_status(
@@ -2823,20 +2848,22 @@
             self.exit_node.name_list,
             self.exit_node.title_and_label,
             self.exit_node.handler,
             wait_for_input=False,
         )
         #######################
         self.ws_node: CommandNode = CommandNode(
-            ["ws", "комп^ьютер"],
+            ["ws", "комп|ьютер"],
             ["Компьютер"],
             lambda: self.menu_handler(self.menu.workstation),
             text_decoration_before="🖥️ ",
             show_in_main_menu=True,
-            help_text=lambda: flag_string_represent(Flags.ALL) if self.is_all else "",
+            help_text=lambda: (
+                self.flag_string_represent(Flags.ALL) if self.is_all else ""
+            ),
             text="Наши компьютеры",
         )
         self.menu.check = [
             check_all_node,
             check_resources_node,
             check_ws_node.clone_as(
                 self.ws_node.name_list,
@@ -2958,23 +2985,23 @@
             or A.C_J.exists(self.arg(), self.arg()),
         )
 
         all_passwords_node: CommandNode = self.create_command_link(
             change_user_password_node.name_list,
             js(
                 (
-                    command_name_base(self.note_node.name_list[0]),
+                    get_command_base_name(self.note_node.name_list[0]),
                     flag_name_list(Flags.SILENCE)[0],
                     esc("password"),
                 )
             ),
             ["Список всех паролей"],
             ADMIN_GROUPS,
         )
-        all_passwords_node.help_text = lambda: flag_string_represent(Flags.ALL)
+        all_passwords_node.help_text = lambda: self.flag_string_represent(Flags.ALL)
         self.execute_python_file_silence("@on_before_command_node_tree_creation")
 
         #######################
         self.command_node_tree = {
             CommandNode(
                 ["where", "где"],
                 lambda: [
@@ -3008,15 +3035,15 @@
             CommandNode(
                 self.run_command_node.name_list, [""]
             ): A.D.to_dict_with_none_value(self.menu.run_command),
             CommandNode(self.user_node.name_list, [""]): A.D.to_dict_with_none_value(
                 self.menu.user
             ),
             self.ws_node: None,
-            CommandNode(["ws", "комп^ьютер"], [""]): A.D.to_dict_with_none_value(
+            CommandNode(["ws", "комп|ьютер"], [""]): A.D.to_dict_with_none_value(
                 self.menu.workstation
             ),
             CommandNode(["study", "обучение"], [""]): {
                 self.wiki_node: None,
                 infinity_study_course_node: None,
                 basic_polibase_study_course_node: None,
                 holter_study_course_node: None,
@@ -3173,15 +3200,15 @@
                 show_in_main_menu=True,
             ): None,
             it_unit_node: None,
             hr_unit_node: None,
             call_centre_unit_node: None,
             marketer_unit_node: None,
             CommandNode(
-                ["indication^s", "показания"],
+                ["indication|s", "показания"],
                 ["Показания"],
                 lambda: self.check_resources_and_indications_handler(
                     [CheckableSections.INDICATIONS]
                 ),
                 ADMIN_GROUPS + [Groups.RD, Groups.IndicationWatcher],
                 text_decoration_before="📈 ",
                 show_in_main_menu=True,
@@ -3222,32 +3249,32 @@
                     ADMIN_GROUPS,
                 ): None,
             },
             CommandNode([""], [""]): all_passwords_node,
             CommandNode(
                 ["set"],
                 ["Установить значение переменной"],
-                self.get_or_set_variable_handler,
+                self.variable_value_getter_and_setter_handler,
             ): None,
             CommandNode(["door", "дверь"], [""]): {
                 CommandNode(
                     ["open"],
                     ["Открытие дверей холодного прохода"],
                     lambda: self.door_open_handler("cold_pass"),
                 ),
                 CommandNode(
                     ["close"],
                     ["Закрытие дверей холодного прохода"],
                     lambda: self.door_close_handler("cold_pass"),
-                )
+                ),
             },
             CommandNode(
                 ["get"],
                 ["Показать значение переменной"],
-                lambda: self.get_or_set_variable_handler(True),
+                lambda: self.variable_value_getter_and_setter_handler(True),
             ): None,
             CommandNode(["qr"], [""]): {
                 CommandNode(["code", "код"], ["Создание QR-кода", "Создать QR-код"]): {
                     CommandNode(
                         ["command", "команды"],
                         ["для команды мобильного помощника"],
                         self.create_qr_code_for_mobile_helper_command_handler,
@@ -3306,15 +3333,15 @@
                                 ),
                             )
                             if with_error
                             else (
                                 " ",
                                 A.CT_V.ROBOT,
                                 " ",
-                                b(keyword.upper()),
+                                self.output.bold(keyword.upper()),
                                 ": до свидания, ",
                                 self.get_user_given_name(),
                                 ".",
                             )
                         )
                     )
                     if not with_error:
@@ -3322,28 +3349,28 @@
                             self.write_line(
                                 js(
                                     (
                                         nl("Всегда буду рад видеть Вас вновь:"),
                                         " ",
                                         A.CT_V.BULLET,
                                         "повторить",
-                                        esc(b(self.get_command_title())),
+                                        esc(self.output.bold(self.get_command_title())),
                                         A.CT_V.ARROW,
                                         "отправьте",
-                                        b(keyword),
-                                        b(
+                                        self.output.bold(keyword),
+                                        self.output.bold(
                                             self.get_command_name(
                                                 use_language_index=True
                                             )
                                         ),
                                         nl(),
                                         "     ",
                                         A.CT_V.HAND_INDICATE,
                                         nl(
-                                            b(
+                                            self.output.bold(
                                                 A.D_F.whatsapp_send_message_to_it(
                                                     js(
                                                         (
                                                             keyword,
                                                             self.get_command_name(),
                                                         )
                                                     )
@@ -3351,19 +3378,19 @@
                                             )
                                         ),
                                         "или",
                                         nl(),
                                         " ",
                                         A.CT_V.BULLET,
                                         "отправьте",
-                                        b(keyword),
+                                        self.output.bold(keyword),
                                         nl(),
                                         "     ",
                                         A.CT_V.HAND_INDICATE,
-                                        b(link_text),
+                                        self.output.bold(link_text),
                                     )
                                 )
                             )
 
     def choose_file(
         self,
         search_request: str | None = None,
@@ -3384,23 +3411,27 @@
                     else search_request[0:splitter_index]
                 )
 
         def label_function(file: File, _) -> str:
             title_list: list[str] = file.title.split(A.CT.SPLITTER)
             if len(title_list) == 3:
                 return j(
-                    ([b(title_list[0].upper()), ": "] if n(filter_function) else [])
+                    (
+                        [self.output.bold(title_list[0].upper()), ": "]
+                        if n(filter_function)
+                        else []
+                    )
                     + [
-                        b(title_list[-1]),
+                        self.output.bold(title_list[-1]),
                         " (",
                         title_list[-2],
                         ")",
                     ]
                 )
-            return b(title_list[1])
+            return self.output.bold(title_list[1])
 
         with self.output.make_loading(text="Идет загрузка файлов. Ожидайте"):
             file_list: list[File] = A.R_F.find(
                 search_request,
                 command_type=command_type,
                 exclude_private_files=True,
             ).data  # type: ignore
@@ -3431,15 +3462,15 @@
         if not (self.is_silence or self.is_only_result):
             self.output.head1(
                 js(
                     (
                         (
                             None
                             if n(command_type)
-                            else j((b(A.D.get(command_type)[0]), ": "))
+                            else j((self.output.bold(A.D.get(command_type)[0]), ": "))
                         ),
                         title_list[-1] if n(command_type) else esc(title_list[-1]),
                     )
                 )
             )
         return file
 
@@ -3456,15 +3487,15 @@
         return CommandNode(
             [name] if isinstance(name, str) else name,
             title_and_label,
             lambda: self.do_pih(
                 js(
                     (
                         self.current_pih_keyword,
-                        js((js(self.comandless_line_part_list), link)),
+                        js((js(self.commandless_part_list), link)),
                     )
                 )
             ),
             allowed_groups=allowed_groups,
             wait_for_input=True,
             show_in_main_menu=show_in_main_menu,
             text_decoration_before=text_decoration_before,
@@ -3489,33 +3520,33 @@
         return self.pih.output
 
     @property
     def input(self) -> MobileInput:
         return self.pih.input
 
     def bold(self, value: str) -> str:
-        return b(value)
+        return self.output.bold(value)
 
     @property
     def arg_list_exclude_file(self) -> list[str]:
         return A.D.filter(
             lambda item: not item.startswith(FILE_PATTERN_LIST), self.arg_list
         )
 
     @property
     def check_for_arg_list_include_file(self) -> bool:
         return (self.arg_len - len(self.arg_list_exclude_file)) != 0
 
     def arg(
         self,
         index: int = 0,
-        default_value: Any | None = None,
+        default_value: Any = None,
         as_file: bool = False,
         filter_function: Callable[[str], bool] | None = None,
-    ) -> Any | None:
+    ) -> Any:
         result: str | None = (
             A.D.by_index(
                 (
                     self.arg_list
                     if n(filter_function)
                     else A.D.filter(filter_function, self.arg_list)
                 ),
@@ -3598,15 +3629,15 @@
                 )
             else:
                 state: bool = not self.user_settings.has(A.CT_AD_UP.Jokeless)
                 self.write_line(
                     j(
                         (
                             "Отправка анегдота при входе или выходе ",
-                            b(["выключена", "включена"][state]),
+                            self.output.bold(["выключена", "включена"][state]),
                             ".",
                         )
                     )
                 )
                 if self.yes_no(
                     js(
                         (
@@ -3619,15 +3650,15 @@
                     if [self.user_settings.add, self.user_settings.remove][state](
                         A.CT_AD_UP.Jokeless
                     ):
                         self.write_line(
                             j(
                                 (
                                     "Отправка анегдота при входе или выходе ",
-                                    b(["выключена", "включена"][state]),
+                                    self.output.bold(["выключена", "включена"][state]),
                                     ".",
                                 )
                             )
                         )
         else:
             self.write_line(A.R_DS.joke().data)
 
@@ -3650,40 +3681,40 @@
                     or self.input.input(
                         f"Введите:\n  {A.CT_V.BULLET} Адресс электронной почты\nили\n  {A.CT_V.BULLET} Поисковый запрос для поиска пациента"
                     )
                 )
             polibase_person_string: str = ""
             if ne(polibase_person):
                 polibase_person_string = j(
-                    ("клиента ", b(polibase_person.FullName), A.CT.SPLITTER)  # type: ignore
+                    ("клиента ", self.output.bold(polibase_person.FullName), A.CT.SPLITTER)  # type: ignore
                 )
             if not only_for_polibase_person:
                 if ne(value):
                     if A.C.email(nns(value)):
                         result = A.C_EML.accessability(value, not self.is_forced, EmailVerificationMethods.NORMAL if self.is_test else None)  # type: ignore
                         self.output.separated_line()
                         text: str = js(
                             (
                                 "Адресс электронной почты",
                                 polibase_person_string,
-                                b(value),
+                                self.output.bold(value),
                                 j(("" if result else "не", "доступен")),
                             )
                         )
                         if result:
                             self.output.good(text)
                         else:
                             self.output.error(text)
                         return result
                     elif ne(polibase_person):
                         self.output.error(
                             js(
                                 (
                                     "Адресс электронной почты:",
-                                    b(value),
+                                    self.output.bold(value),
                                     "имеет неверный формат",
                                 )
                             )
                         )
                         return None
                 else:
                     self.output.error("Адресс электронной почты отстутствует")
@@ -3762,29 +3793,36 @@
                         )
                     )
                 )
             )
         else:
             answer = self.yes_no(
                 "Изменить имя файла дампа базы данных",
-                b("Отправьте имя"),
-                js(("Использовать имя:", b(name), "- отправьте", A.O.get_number(0))),
+                self.output.bold("Отправьте имя"),
+                js(
+                    (
+                        "Использовать имя:",
+                        self.output.bold(name),
+                        "- отправьте",
+                        A.O.get_number(0),
+                    )
+                ),
             )
             self.write_line(
                 i(
                     j(
                         (
                             self.user_given_name,
                             ", ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе: ",
-                            b("Backup Console"),
+                            self.output.bold("Backup Console"),
                         )
                     )
                 )
             )
-        A.A_P.DB.backup(self.input.answer if answer else name, test, self.is_forced)
+        A.A_P.DB.backup(self.input.answer if answer else name, test)
 
     def show_polibase_password_handler(self) -> None:
         LOGIN: str = "login"
         PASSWORD: str = "password"
         result: dict[str, Any] | None = None
 
         def execute_query_for_password(condition: str) -> dict[str, Any] | None:
@@ -3829,199 +3867,283 @@
             result = get_by_login(self.session.login)  # type: ignore
         if e(result):
             self.output.error("Пользователь Полибейс не найден")
         else:
             self.write_line(
                 j(
                     (
-                        b("Логин"),
+                        self.output.bold("Логин"),
                         ": ",
                         result[LOGIN],
                         nl(),
-                        b("Пароль"),
+                        self.output.bold("Пароль"),
                         ": ",
                         result[PASSWORD],
                     )
                 )
             )
 
     def robocopy_job_run_handler(self) -> None:
         forced: bool = self.is_forced
-        source_job_name: str | None = self.arg()
-        if ne(source_job_name):
-            source_job_name = lw(source_job_name)
-        job_name_set: set = set()
-        job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = defaultdict(list)
-        job_status_list: list[RobocopyJobStatus] = A.R_B.robocopy_job_status_list().data
-        if self.is_all and n(source_job_name):
-            filtered_job_status_list: list[RobocopyJobStatus] = A.D.filter(
-                lambda item: not (item.exclude or (item.active and not self.is_forced)),
-                job_status_list,
-            )
-            length: int = len(filtered_job_status_list)
-            if length > 0 and self.yes_no(js(("Запустить все", length, "заданий"))):
-                job_status: RobocopyJobStatus
-                for job_status in filtered_job_status_list:
-                    A.A_B.start_robocopy_job(
-                        job_status.name,
-                        job_status.source,
-                        job_status.destination,
-                        forced,
-                    )
-                self.write_line(
-                    i(
-                        js(
-                            (
-                                j((self.user_given_name, ",")),
-                                "ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе",
-                                b("Backup Console"),
-                            )
-                        )
-                    )
-                )
-                return
-        job_status_map: dict[str, RobocopyJobStatus] = {}
-        for job_status in job_status_list:
+        source_job_name: str | None = None
+        source_job_status_status: int | None = None
+        for index, arg in enumerate(self.arg_list):
+            if index > 1:
+                break
+            if A.D_C.decimal(arg):
+                source_job_status_status = A.D_Ex.decimal(arg)
+                continue
+            source_job_name = lw(arg)
+        source_job_name_set: set = set()
+        source_job_status_map: dict[str, RobocopyJobStatus] = {}
+        source_job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = defaultdict(
+            list
+        )
+        source_job_status_list: list[RobocopyJobStatus] = (
+            A.R_B.robocopy_job_status_list().data
+        )
+        for job_status in source_job_status_list:
             job_name: str = job_status.name
-            job_name_set.add(job_name)
-            job_status_map_by_name[job_name].append(job_status)
-            job_status_map[
+            source_job_name_set.add(job_name)
+            source_job_status_map_by_name[job_name].append(job_status)
+            source_job_status_map[
                 A.D_F_B.job_full_name(
                     job_status.name, job_status.source, job_status.destination
                 )
             ] = job_status
-        job_name_list: list[str] = list(job_name_set)
-        job_name_list.sort()
-        if ne(source_job_name) and source_job_name not in job_name_list:
-            source_job_name = None
+
+        source_job_name_list: list[str] = list(source_job_name_set)
+        source_job_name_list.sort()
+
+        action_job_status_list: list[RobocopyJobStatus] = source_job_status_list
+        action_job_status_map: dict[str, RobocopyJobStatus] = source_job_status_map
+        action_job_name_list: list[str] = source_job_name_list
+        action_job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = (
+            source_job_status_map_by_name
+        )
+        # filtering
+        filtered_job_name_set: set = set()
+        filtered_job_status_map: dict[str, RobocopyJobStatus] = {}
+        filtered_job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = (
+            defaultdict(list)
+        )
+        filtered_job_status_list: list[RobocopyJobStatus] | None = None
+        filter_exists: bool = (
+            not (n(source_job_name) and n(source_job_status_status)) or self.is_all
+        )
 
         def is_active(job_name: str) -> bool:
-            inacitve_count: int = 0
-            for job_status in job_status_list:
+            inactive_count: int = 0
+            for job_status in action_job_status_list:
                 if job_status.name == job_name:
-                    inacitve_count += 1
+                    inactive_count += 1
                     if job_status.active:
-                        inacitve_count -= 1
-            return inacitve_count == 0
+                        inactive_count -= 1
+            return inactive_count == 0
 
-        if ne(source_job_name) and is_active(source_job_name) and not forced:
-            self.output.error(
-                js(("Robocopy-задание", escs(source_job_name), "уже выполняется"))
+        if filter_exists:
+            filtered_job_status_list = source_job_status_list
+            if nn(source_job_status_status):
+                filtered_job_status_list = A.D.filter(
+                    lambda item: item.last_status == source_job_status_status,
+                    filtered_job_status_list,
+                )
+            if nn(source_job_name):
+                filtered_job_status_list = A.D.filter(
+                    lambda item: A.D.contains(item.name, source_job_name)
+                    and (forced or not is_active(item.name)),
+                    filtered_job_status_list,
+                )
+
+        self.write_line(nl(self.output.bold("Список Robocopy-заданий:")))
+
+        def job_status_item_label_function(
+            name: str,
+            job_status: RobocopyJobStatus,
+        ) -> str:
+            source: str = job_status.source
+            destination: str = job_status.destination
+            job_status = action_job_status_map[
+                A.D_F_B.job_full_name(name, source, destination)
+            ]
+            status: int | None = None
+            date: str | None = None
+            if job_status.active:
+                date = self.output.bold("выполняется")
+            else:
+                if job_status.last_created is not None:
+                    date = A.D_F.datetime(job_status.last_created)
+                status = job_status.last_status
+            return j(
+                (
+                    j(
+                        (
+                            "   ",
+                            A.CT.VISUAL.BULLET,
+                            " ",
+                            source,
+                            A.CT.VISUAL.ARROW,
+                            destination,
+                        )
+                    ),
+                    ("" if n(status) else j((": ", self.output.bold(status)))),
+                    ("" if n(date) else nl(j((" " * 6, date)), reversed=True)),
+                )
             )
-        else:
-            if source_job_name not in job_name_list:
-                self.write_line(nl(b("Список Robocopy-заданий:")))
-
-            def job_status_list_label_function(name: str) -> str:
-                job_list: list[RobocopyJobStatus] = job_status_map_by_name[name]
 
-                def job_status_item_label_function(
-                    job_status: RobocopyJobStatus,
-                ) -> str:
-                    source: str = job_status.source
-                    destination: str = job_status.destination
-                    job_status = job_status_map[
-                        A.D_F_B.job_full_name(name, source, destination)
-                    ]
-                    status: int | None = None
-                    date: str | None = None
-                    if job_status.active:
-                        date = "выполняется"
-                    else:
-                        if job_status.last_created is not None:
-                            date = A.D_F.datetime(job_status.last_created)
-                        status = job_status.last_status
-                    return (
-                        j(
-                            (
-                                "   ",
-                                A.CT.VISUAL.BULLET,
-                                " ",
-                                source,
-                                A.CT.VISUAL.ARROW,
-                                destination,
-                            )
-                        )
-                        + ("" if status is None else f" [ {b(status)} ]")
-                        + (
-                            ""
-                            if date is None
-                            else nl(j((" " * 5, date)), reversed=True)
-                        )
+        def job_status_list_label_function(name: str) -> str:
+            return nl(
+                jnl(
+                    A.D.map(
+                        lambda item: job_status_item_label_function(name, item),
+                        action_job_status_map_by_name[name],
                     )
+                ),
+                reversed=True,
+            )
 
-                return nl(
-                    jnl(A.D.map(job_status_item_label_function, job_list)),
-                    reversed=True,
+        def job_label_function(name: str) -> str:
+            return j(
+                (
+                    self.output.bold(name),
+                    A.CT.SPLITTER,
+                    job_status_list_label_function(name),
                 )
+            )
+
+        if filter_exists:
+            if ne(filtered_job_status_list):
+                filtered_job_status_list = A.D.filter(
+                    lambda item: not (item.exclude and self.is_all),
+                    filtered_job_status_list,
+                )
+                for job_status in filtered_job_status_list:
+                    job_name: str = job_status.name
+                    filtered_job_name_set.add(job_name)
+                    filtered_job_status_map_by_name[job_name].append(job_status)
+                    filtered_job_status_map[
+                        A.D_F_B.job_full_name(
+                            job_status.name, job_status.source, job_status.destination
+                        )
+                    ] = job_status
+                action_job_status_list = filtered_job_status_list
+                action_job_name_list = list(filtered_job_name_set)
+                action_job_name_list.sort()
+                action_job_status_map_by_name = filtered_job_status_map_by_name
+                action_job_status_map = filtered_job_status_map
+                if self.is_all:
+                    index: int = 0
+                    for job_name in filtered_job_status_map_by_name:
+                        if job_name in filtered_job_name_set:
+                            index += 1
+                            self.write_line(
+                                j(
+                                    (
+                                        index,
+                                        ". ",
+                                        self.output.bold(job_name),
+                                        job_status_list_label_function(job_name),
+                                    )
+                                )
+                            )
+                    length: int = len(filtered_job_status_list)
+                    if length > 0 and self.yes_no(
+                        js(("Запустить все", length, "заданий"))
+                    ):
+                        job_status: RobocopyJobStatus
+                        for job_status in filtered_job_status_list:
+                            A.A_B.start_robocopy_job(
+                                job_status.name,
+                                job_status.source,
+                                job_status.destination,
+                                forced,
+                            )
+                        self.write_line(
+                            i(
+                                js(
+                                    (
+                                        j((self.user_given_name, ",")),
+                                        "ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе",
+                                        self.output.bold("Backup Console"),
+                                    )
+                                )
+                            )
+                        )
+                        return
+            else:
+                self.output.error("Список отфильтрованных Robocopy-заданий пуст")
+        job_name: str = self.input.item_by_index(
+            "Пожалуйста, выберите Robocopy-задание, которое необходимо запустить",
+            action_job_name_list,
+            lambda name, _: job_label_function(name),
+        )
+        job_list: list[RobocopyJobStatus] = action_job_status_map_by_name[job_name]
 
-            def job_label_function(name: str) -> str:
-                return j((b(name), A.CT.SPLITTER, job_status_list_label_function(name)))
+        job_list = (
+            job_list
+            if forced
+            else A.D.filter(lambda item: not item.active or item.live, job_list)
+        )
 
-            job_name: str = source_job_name or self.input.item_by_index(
-                "Пожалуйста, выберите Robocopy-задание, которое необходимо запустить",
-                job_name_list,
-                lambda name, _: job_label_function(name),
-            )
-            job_list: list[RobocopyJobStatus] = job_status_map_by_name[job_name]
-            job_list = (
-                job_list
-                if forced
-                else A.D.filter(lambda item: not item.active or item.live, job_list)
+        if len(job_list) > 0:
+            self.write_line(
+                nl(j((self.output.bold("Robocopy-задание"), ": ", job_name)))
             )
-            if len(job_list) > 0:
-                self.write_line(nl(j((b("Robocopy-задание"), ": ", job_name))))
+            job_item: RobocopyJobStatus | None = None
+            if len(job_list) > 1:
                 all_job_item: RobocopyJobStatus = RobocopyJobStatus("Все")
-                job_item: RobocopyJobStatus = (
+                job_item = (
                     all_job_item
                     if self.is_all
                     else self.input.item_by_index(
                         "Пожалуйста, выберите направление",
                         job_list + ([] if len(job_list) <= 1 else [all_job_item]),
                         lambda item, _: (
-                            b(item.name)
+                            self.output.bold(item.name)
                             if n(item.destination)
-                            else b(
+                            else self.output.bold(
                                 j((item.source, A.CT.VISUAL.ARROW, item.destination))
                             )
                         ),
                     )
                 )
-                if A.A_B.start_robocopy_job(
-                    job_name, job_item.source, job_item.destination, forced
-                ):
-                    self.write_line(
-                        i(
-                            j(
-                                (
-                                    self.user_given_name,
-                                    ", ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе ",
-                                    b("Backup Console"),
-                                )
-                            )
-                        )
-                    )
-                else:
-                    self.output.error(
+            else:
+                job_item = job_list[0]
+            if A.A_B.start_robocopy_job(
+                job_name, job_item.source, job_item.destination, forced
+            ):
+                self.write_line(
+                    i(
                         j(
                             (
                                 self.user_given_name,
-                                ", Robocopy-задание не может быть выполнено",
+                                ", ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе ",
+                                self.output.bold("Backup Console"),
                             )
                         )
                     )
+                )
             else:
                 self.output.error(
                     j(
                         (
                             self.user_given_name,
-                            ", все направления для Robocopy-задания в процессе выполнения",
+                            ", Robocopy-задание не может быть выполнено",
                         )
                     )
                 )
+        else:
+            self.output.error(
+                j(
+                    (
+                        self.user_given_name,
+                        ", все направления для Robocopy-задания в процессе выполнения",
+                    )
+                )
+            )
 
     def yes_no(
         self,
         text: str,
         yes_label: str = YES_LABEL,
         no_label: str = NO_LABEL,
         yes_checker: Callable[[str], bool] | None = None,
@@ -4140,15 +4262,15 @@
         if non_search_action:
             if all:
                 if not self.yes_no(
                     j(
                         (
                             ("Перезагрузить" if action_index == 0 else "Выключить"),
                             " все компьютеры, которые помечены как разрешенные",
-                            b("Да"),
+                            self.output.bold("Да"),
                             " (Введите слово ",
                             esc(WORKSTATION_CHECK_WORD),
                             ")",
                         )
                     ),
                     yes_checker=(lambda item: item == WORKSTATION_CHECK_WORD),
                 ):
@@ -4159,28 +4281,30 @@
                 workstations_result = A.R_WS.by_any(None if all else value)
                 if e(workstations_result):
                     if A.C_R.accessibility_by_smb_port(value, None, 2):
                         if self.is_forced:
                             if action_index == 0:
                                 A.A_WS.reboot(value, True)
                                 self.write_line(
-                                    b(
+                                    self.output.bold(
                                         j(
                                             (
                                                 "Идет перезагрузка компьютера ",
                                                 value,
                                                 "...",
                                             )
                                         )
                                     )
                                 )
                             else:
                                 A.A_WS.shutdown(value, True)
                                 self.write_line(
-                                    b(j(("Идет выключение компьютера ", value, "...")))
+                                    self.output.bold(
+                                        j(("Идет выключение компьютера ", value, "..."))
+                                    )
                                 )
                         else:
                             self.output.error(
                                 js(("Компьютер", value, "нельзя перезагрузить"))
                             )
                     else:
                         self.output.error(js(("Компьютер", value, "не найден")))
@@ -4195,15 +4319,15 @@
                             if all or (
                                 A.C_WS.rebootable(workstation)
                                 or (
                                     self.yes_no(
                                         js(
                                             (
                                                 "Компьютер",
-                                                b(workstation.name),
+                                                self.output.bold(workstation.name),
                                                 "не отмечен как разрешенный для перезагрузки, Вы уверены, что хотите его перезагрузить",
                                             )
                                         )
                                     )
                                 )
                                 and (
                                     not has_user
@@ -4216,36 +4340,36 @@
                                             )
                                         )
                                     )
                                 )
                             ):
                                 if A.A_WS.reboot(workstation.name, True):
                                     self.write_line(
-                                        b(
+                                        self.output.bold(
                                             f"Идет перезагрузка компьютера {workstation.name}..."
                                         )
                                     )
                         else:
                             if all or (
                                 A.C_WS.shutdownable(workstation)
                                 or (
                                     self.yes_no(
-                                        f"Компьютер {b('не отмечен')} как разрешенный для выключения, Вы уверены, что хотите его выключить"
+                                        f"Компьютер {self.output.bold('не отмечен')} как разрешенный для выключения, Вы уверены, что хотите его выключить"
                                     )
                                 )
                                 and (
                                     not has_user
                                     or self.yes_no(
                                         f"Выключить компьютер {workstation.name}{user_string}"
                                     )
                                 )
                             ):
                                 if A.A_WS.shutdown(workstation.name, True):
                                     self.write_line(
-                                        b(
+                                        self.output.bold(
                                             f"Идет выключение компьютер {workstation.name}..."
                                         )
                                     )
 
                     A.R.every(every_action, workstations_result)
             else:
                 try:
@@ -4261,25 +4385,25 @@
                 try:
 
                     def data_label_function(
                         index: int, field: FieldItem, data: Any, item_data: Any
                     ) -> tuple[bool, str]:
                         if field.name == A.CT_FNC.ACCESSABLE:
                             accessable: bool = item_data
-                            return True, f"{b(field.caption)}: " + (
+                            return True, f"{self.output.bold(field.caption)}: " + (
                                 "Да" if accessable else "Нет"
                             )
                         if field.name == A.CT_FNC.LOGIN:
                             login: str | None = item_data
                             return (
                                 True,
                                 (
                                     None
                                     if e(item_data)
-                                    else f"{b('Пользователь')}: {A.R_U.by_login(login).data.name} ({login})"
+                                    else f"{self.output.bold('Пользователь')}: {A.R_U.by_login(login).data.name} ({login})"
                                 ),
                             )
                         return False, None
 
                     self.output.write_result(
                         workstations_result,
                         False,
@@ -4295,15 +4419,15 @@
         except NotFound as error:
             if raise_exception:
                 raise error
             else:
                 self.output.error(error)
 
     def return_result(
-        self, value: Any | None = None, interrupt_type: InterruptionTypes | None = None
+        self, value: Any = None, interrupt_type: InterruptionTypes | None = None
     ) -> None:
         if nn(self.return_result_key):
             A.E.send(
                 A.CT_E.RESULT_WAS_RETURNED,
                 (
                     self.return_result_key,
                     value if n(interrupt_type) else "",
@@ -4346,15 +4470,15 @@
                         polibase_person.ChartFolder
                     )
                     if ne(polibase_person_card_registry_folder):
                         result = j(
                             (
                                 j(
                                     (
-                                        b(
+                                        self.output.bold(
                                             A.CT_FC.POLIBASE.CARD_REGISTRY_FOLDER.caption
                                         ),
                                         ": ",
                                         polibase_person_card_registry_folder,
                                     )
                                 ),
                                 self.get_polibase_person_card_place_label(
@@ -4367,33 +4491,38 @@
                         )
                     if e(result):
                         with self.output.make_allow_show_error(True):
                             self.write_line(
                                 js(
                                     (
                                         "Найдена карта пациента:",
-                                        b(polibase_person.FullName),
+                                        self.output.bold(polibase_person.FullName),
                                     )
                                 )
                             )
                             with self.output.make_indent(2, True):
                                 self.output.error(
                                     j(
                                         (
                                             "Карта пациента: ",
-                                            b(value),
+                                            self.output.bold(value),
                                             " ",
                                             A.CT_FC.POLIBASE.CARD_REGISTRY_FOLDER.default_value.lower(),
                                         )
                                     )
                                 )
                         was_found = True
                     else:
                         self.write_line(
-                            js(("Найдена карта пациента:", b(polibase_person.FullName)))
+                            js(
+                                (
+                                    "Найдена карта пациента:",
+                                    self.output.bold(polibase_person.FullName),
+                                )
+                            )
                         )
                         with self.output.make_indent(2, True):
                             self.write_line(result)
                         was_found = True
                 else:
                     pass
             except NotFound as _:
@@ -4426,15 +4555,15 @@
     def run_command_handler(self, command_type: A.CT_CMDT | None = None) -> None:
         def filter_function(item: Note) -> bool:
             title_list: list[str] = item.title.split(A.CT.SPLITTER)  # type: ignore
             if len(title_list) > 1:
                 return title_list[0].lower() in A.D.get(command_type)[1:]
             return True
 
-        arg: Any | None = None
+        arg: Any = None
         if n(command_type):
             for i in range(max(1, self.arg_len)):
                 arg = self.arg(
                     i,
                     as_file=True,
                     filter_function=None if n(command_type) else filter_function,
                 )
@@ -4504,15 +4633,17 @@
             for index, parameter in enumerate(DH.parameters_map):
                 DH.parameters_map[parameter][0] = A.D.if_is_in(
                     fileless_arg_list, index
                 ) or self.input.input(
                     js(
                         (
                             "Введите значение для параметра",
-                            b(DH.parameters_map[parameter][1] or parameter),
+                            self.output.bold(
+                                DH.parameters_map[parameter][1] or parameter
+                            ),
                         )
                     )
                 )
 
             def put_parameters(value: Match[str]) -> str:
                 return DH.parameters_map[get_name_and_title(value)[0]][0]
 
@@ -4526,31 +4657,39 @@
                     search_request,
                     command_type=command_type,
                 ).text
 
         if command_type == A.CT_CMDT.SSH:
             host = lw(self.arg())
             if ne(host) and host not in A.D.to_list(SSHHosts):
-                self.output.error(js(("Хост", b(host), "не найден")))
+                self.output.error(js(("Хост", self.output.bold(host), "не найден")))
                 host = None
             if e(host):
                 host = A.D.get(
                     self.input.item_by_index(
                         "Выберите хост",
                         A.D.to_list(SSHHosts),  # type: ignore
                         lambda item, _: A.D.get(item),
                     )
                 )
             while True:
                 if ne(text):
                     text = extract_parameters(text)  # type: ignore
-                text = text or self.input.input(js(("Введите команду для", b(host))))
+                text = text or self.input.input(
+                    js(("Введите команду для", self.output.bold(host)))
+                )
                 try:
                     with self.output.make_loading(
-                        text=j(("Выполнение запроса на ", b(host), ". Ожидайте"))
+                        text=j(
+                            (
+                                "Выполнение запроса на ",
+                                self.output.bold(host),
+                                ". Ожидайте",
+                            )
+                        )
                     ):
                         self.write_line(
                             jnl(
                                 (
                                     A.R_SSH.execute(
                                         text,
                                         host,  # type: ignore
@@ -4626,41 +4765,43 @@
                     process_result: CompletedProcess | None = None
                     if use_psexec_executor:
                         if e(host):
                             if self.yes_no(
                                 j(
                                     (
                                         "Использовать хост ",
-                                        b(default_host),
+                                        self.output.bold(default_host),
                                         ", для выполнения команды",
                                     )
                                 ),
-                                no_label=b("Или введите название хоста"),
+                                no_label=self.output.bold("Или введите название хоста"),
                             ):
                                 host = default_host
                             else:
                                 host = self.input.answer
                         while True:
                             host = lw(host)
                             if host == default_host or A.C_R.accessibility_by_ping(
                                 host, count=1
                             ):
                                 self.write_line(
                                     nl(
                                         js(
                                             (
                                                 "Команда будет запущена на хосте",
-                                                b(host),
+                                                self.output.bold(host),
                                             )
                                         )
                                     )
                                 )
                                 break
                             else:
-                                self.output.error(js(("Хост", b(host), "не доступен")))
+                                self.output.error(
+                                    js(("Хост", self.output.bold(host), "не доступен"))
+                                )
                                 host = self.input.input(
                                     "Введите имя хоста, на котором будет выполнена команда"
                                 )
                     if n(host_is_local):
                         host_is_local = A.SYS.host_is_local(host)
                     self.write_line(
                         js(
@@ -4725,15 +4866,15 @@
                     command_line_list: list[str] = []
                     line_count: int = 0
                     while e(text):
                         if line_count == 0 or self.yes_no(
                             "Ввести следующую строку код",
                             no_label=j(
                                 (
-                                    b("Завершить ввод кода"),
+                                    self.output.bold("Завершить ввод кода"),
                                     " - ",
                                     A.CT_V.NUMBER_SYMBOLS[0],
                                 )
                             ),
                         ):
                             command_line_list.append(
                                 self.input.input("Введите строку кода")
@@ -4767,15 +4908,15 @@
                 command_line_list: list[str] = []
                 line_count: int = 0
                 while e(text):
                     if line_count == 0 or self.yes_no(
                         "Ввести следующую строку запроса",
                         no_label=j(
                             (
-                                b("Завершить ввод текста запроса"),
+                                self.output.bold("Завершить ввод текста запроса"),
                                 " - ",
                                 A.CT_V.NUMBER_SYMBOLS[0],
                             )
                         ),
                     ):
                         command_line_list.append(
                             self.input.input("Введите текст запрос")
@@ -4787,15 +4928,15 @@
                 command_part_list: list[str] = text.split("$\\n")
                 command_part_list_is_single: bool = len(command_part_list) == 1
                 if not command_part_list_is_single:
                     self.write_line(
                         js(
                             (
                                 "Команда состоит из",
-                                b(len(command_part_list)),
+                                self.output.bold(len(command_part_list)),
                                 "запросов",
                             )
                         )
                     )
                 for command_part_index, command_part_item in enumerate(
                     command_part_list
                 ):
@@ -4836,20 +4977,24 @@
                                         not need_show_result
                                         or not self.yes_no(
                                             j(
                                                 (
                                                     "Результат состоит из ",
                                                     len(result),
                                                     nl(" элементов."),
-                                                    b("Выгрузить в виде EXCEL файла"),
+                                                    self.output.bold(
+                                                        "Выгрузить в виде EXCEL файла"
+                                                    ),
                                                 )
                                             ),
                                             no_label=j(
                                                 (
-                                                    b("Показать результат"),
+                                                    self.output.bold(
+                                                        "Показать результат"
+                                                    ),
                                                     " - ",
                                                     A.CT_V.NUMBER_SYMBOLS[0],
                                                 )
                                             ),
                                         )
                                     )
 
@@ -4865,15 +5010,17 @@
                                                 else j(
                                                     (
                                                         " ",
                                                         A.CT_V.BULLET,
                                                         " ",
                                                         field.name,
                                                         ": ",
-                                                        b((data_value or "").strip()),
+                                                        self.output.bold(
+                                                            (data_value or "").strip()
+                                                        ),
                                                     )
                                                 )
                                             ),
                                         ),
                                         separated_result_item=True,
                                     )
 
@@ -4882,15 +5029,22 @@
                                         show_result()
                                     else:
                                         first_field: FieldItem = result.fields.list[0]
                                         if first_field.name == A.CT_P.DBMS_OUTPUT:
                                             show_result()
                                         else:
                                             self.write_line(
-                                                j((b(first_field.caption), ":"))
+                                                j(
+                                                    (
+                                                        self.output.bold(
+                                                            first_field.caption
+                                                        ),
+                                                        ":",
+                                                    )
+                                                )
                                             )
                                             A.R.every(
                                                 lambda data: self.write_line(
                                                     js(
                                                         (
                                                             "",
                                                             A.CT_V.BULLET,
@@ -4942,15 +5096,15 @@
                                 else:
                                     break
                         if nn(error_catched):
                             break
 
     def show_free_marks(self) -> None:
         def label_function(data_item: Mark, _: int) -> str:
-            return f" {A.CT.VISUAL.BULLET} {b(data_item.TabNumber)} - {data_item.GroupName}"
+            return f" {A.CT.VISUAL.BULLET} {self.output.bold(data_item.TabNumber)} - {data_item.GroupName}"
 
         self.output.write_result(
             A.R_M.free_list(),
             False,
             separated_result_item=False,
             label_function=label_function,
         )
@@ -4977,17 +5131,25 @@
                 text_list_result: list[str] = []
                 for text_item in text_list:
                     if text_item.strip() != "_" * len(text_item.strip()):
                         text_list_result.append(text_item)
                 if ne(note.title) and not A.D.equal(gkeep_item.title, note.title):
                     if len(text_list_result) > 1:
                         return [
-                            j((b(note.title), nl(count=2), text_list_result[0]))
+                            j(
+                                (
+                                    self.output.bold(note.title),
+                                    nl(count=2),
+                                    text_list_result[0],
+                                )
+                            )
                         ] + text_list_result[1:]
-                    return A.D.as_list(j((b(note.title), nl(count=2), text)))
+                    return A.D.as_list(
+                        j((self.output.bold(note.title), nl(count=2), text))
+                    )
                 return text_list_result
 
             def label_function_for_command_menu(
                 item: list[CommandNode], _
             ) -> list[str]:
                 if item == [self.exit_node]:
                     return self.exit_node.title_and_label[1] + A.D.as_value(
@@ -5007,15 +5169,17 @@
                 gkeep_item_list: list[GKeepItem] = (
                     gkeep_item_list_result.data
                     if strict_equality or (not strict_equality and self.is_all)
                     else [
                         self.input.item_by_index(
                             "Выберите заметку",
                             gkeep_item_list_result.data,
-                            lambda item, _: j((b(item.title), ": ", item.name)),
+                            lambda item, _: j(
+                                (self.output.bold(item.title), ": ", item.name)
+                            ),
                         )
                     ]
                 )
                 for gkeep_item in gkeep_item_list:
                     note_result: Result[Note] | None = None
                     with self.output.make_loading(1, "Идет загрузка заметки. Ожидайте"):
                         note_result = A.R_N.get_by_id(gkeep_item.id)
@@ -5052,15 +5216,17 @@
                                     js(("Изображение", index + 1)),
                                     A.D_CO.bytes_to_base64(
                                         BytesIO(response.content).getvalue()
                                     ),
                                 )
 
                     if len(gkeep_item_list) == 1 and ne(command_menu):
-                        self.write_line(nl(b("Доступные команды:"), count=2))
+                        self.write_line(
+                            nl(self.output.bold("Доступные команды:"), count=2)
+                        )
                         with self.output.make_indent(2, True):
                             self.do_pih(
                                 js(
                                     (
                                         self.current_pih_keyword,
                                         self.get_command_name(
                                             self.command_by_index(
@@ -5135,26 +5301,28 @@
                 forced = True
             if A.A_ACT.was_done(action, self.session.login, parameters, forced):
                 if not action_description.silence:
                     self.output.good(
                         js(
                             (
                                 "Действие",
-                                b(action_description.description),
+                                self.output.bold(action_description.description),
                                 "зарегистрировано.",
                             )
                         )
                     )
 
     def choice_journal(self, name: str | None) -> JournalType:
         def choice_journal_internal(value: list[JournalType]) -> int:
             index: int = self.input.index(
                 "Выберите журнал",
                 value,
-                lambda item, _: js((b(item[1].caption), j(("(", item[1].name, ")")))),
+                lambda item, _: js(
+                    (self.output.bold(item[1].caption), j(("(", item[1].name, ")")))
+                ),
             )  # type: ignore
             return A.D.get(value[index])[0]
 
         journal_list: list[JournalType] = A.D.to_list(A.CT_J)  # type: ignore
         journal_list = A.D.sort(lambda item: item[1].order, journal_list)
         return one(
             A.D_J.type_by_any(
@@ -5168,15 +5336,15 @@
             )  # type: ignore
         )  # type: ignore
 
     def add_journal_record_handler(self) -> None:
         journal_type: JournalType | None = self.choice_journal(self.arg())
 
         if nn(journal_type):
-            journal_name: str = b(A.D.get(journal_type)[1].caption)
+            journal_name: str = self.output.bold(A.D.get(journal_type)[1].caption)
             with self.output.make_separated_lines():
                 self.write_line(j(("Вы выбрали журнал: ", journal_name)))
 
             def get(item: Enum) -> IconedOrderedNameCaptionDescription:
                 return A.D.get(item)[1]
 
             tag: Tags = A.D_J.tag_by_id(
@@ -5199,15 +5367,15 @@
                         (
                             'SELECT parameters->"$.title" title FROM pih_db.events where name =',
                             esc(A.CT_E.ADD_JOURNAL_RECORD.name),
                             'and parameters->"$.type"=',
                             A.D.get(journal_type)[0],
                             'and parameters->"$.tag"=',
                             A.D.get(tag)[0],
-                            'group by parameters->"$.title"',
+                            "group by 1 order by 1",
                         )
                     )
                 ),
             ).data
             title: str | None = None
             if ne(variants):
                 title_index: int | str | None = None
@@ -5259,15 +5427,20 @@
         name = self.arg() or name
         title = self.arg(1) or title
         text = self.arg(2) or text
         self.drop_args()
         while True:
             if e(name):
                 name = self.input.input(
-                    js(("Введите название заметки:", b("оно должно быть уникальным")))
+                    js(
+                        (
+                            "Введите название заметки:",
+                            self.output.bold("оно должно быть уникальным"),
+                        )
+                    )
                 )
             if A.C_N.exists(name, None, True):
                 self.output.error(
                     js(
                         (
                             "Заметка с названием",
                             esc(name),
@@ -5294,15 +5467,15 @@
                         self.input.input("Введите заголовок QR-кода"),
                         False,
                     )
                 )
                 if ne(qr_code_image_path):
                     if self.yes_no(
                         "Распечатать QR-код",
-                        js((b("Да"), "- укажите количество копий")),
+                        js((self.output.bold("Да"), "- укажите количество копий")),
                         yes_checker=lambda value: A.D_Ex.decimal(value) > 0,
                     ):
                         self.output.good("QR-код заметки отправлен на печать")
                         for _ in range(
                             if_else(
                                 self.is_silence,
                                 1,
@@ -5320,29 +5493,67 @@
             self.console_apps_api.send_workstation_message(
                 self.arg(), self.arg(1), not self.is_silence
             )
 
     def who_lost_the_mark_handler(self) -> None:
         self.console_apps_api.who_lost_the_mark(self.arg())
 
-    def marketer_statistics_handler(self) -> None:
+    def marketer_review_statistics_handler(self) -> None:
         self.execute_python_file(
             "marketer_statistics_create",
             redirect_to_mobile_output=True,
             loading_text="Создание статистики. Ожидайте",
         )
         self.output.write_image(
             "Статистика по отзывам",
             A.D_CO.file_to_base64(
                 A.PTH_STAT.get_file_path(
                     A.CT_STAT.Types.POLIBASE_PERSON_REVIEW_NOTIFICATION
                 )
             ),
         )
-        A.R_F.execute("doctor_list_review_partipant")
+        # A.R_F.execute("doctor_list_review_partipant")
+
+    def marketer_review_settings_handler(self) -> None:
+        def show_settings() -> None:
+            self.write_line(
+                js(
+                    (
+                        "Состояние:",
+                        self.output.bold(
+                            ["Выключен", "Включен"][
+                                A.S.get(A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON)
+                            ]
+                        ),
+                    )
+                )
+            )
+            self.write_line(
+                js(
+                    (
+                        "Время запуска:",
+                        self.output.bold(
+                            A.S.get(
+                                A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME,
+                            )
+                        ),
+                    )
+                )
+            )
+        show_settings()
+        if self.yes_no("Запустить мастер настройки"):
+            if self.set_variable_value(A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON):
+                self.set_variable_value(A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME)
+            self.output.good("Настройка завершена")
+            show_settings()
+
+    def set_variable_value(self, value: A.CT_S) -> Any:
+        return self.variable_value_getter_and_setter_handler(
+            False, variable_name=A.D.get(value).key_name, silence=True
+        )
 
     def time_tracking_report_handler(self, for_me_report_only: bool = False) -> None:
         def get_date_format(value: str) -> str:
             value = value.strip()
             return (
                 A.CT.YEARLESS_DATE_FORMAT
                 if value.count(A.CT.DATE_PART_DELIMITER) == 1 or value.count(" ") == 1
@@ -5371,15 +5582,15 @@
                 end_date = end_date.replace(today.year)
         while True:
             if e(start_date):
                 value = self.input.input(
                     j(
                         (
                             "Введите начало периода, в формате ",
-                            b("ДЕНЬ.МЕСЯЦ"),
+                            self.output.bold("ДЕНЬ.МЕСЯЦ"),
                             ", например ",
                             A.D.today_string(A.CT.YEARLESS_DATE_FORMAT),
                         )
                     )
                 )
                 value = A.D_F.to_date(value)
                 format = get_date_format(value)
@@ -5390,15 +5601,15 @@
                     continue
             if e(end_date) or start_date > end_date:
                 if not self.yes_no(
                     "Использовать сегодняшнюю дату",
                     no_label=j(
                         (
                             "Введите окончание периода, в формате ",
-                            b("ДЕНЬ.МЕСЯЦ"),
+                            self.output.bold("ДЕНЬ.МЕСЯЦ"),
                             ", например ",
                             A.D.today_string(A.CT.YEARLESS_DATE_FORMAT),
                         )
                     ),
                 ):
                     value = A.D_F.to_date(self.input.answer)
                     format = get_date_format(value)
@@ -5452,15 +5663,17 @@
             )
 
     def menu_handler(self, menu_command_node_list: list[CommandNode]) -> None:
         def label_function(command_node: CommandNode) -> str:
             return j(
                 (
                     A.D.as_value(command_node.text_decoration_before),
-                    b(A.D.capitalize(self.get_command_node_label(command_node))),
+                    self.output.bold(
+                        A.D.capitalize(self.get_command_node_label(command_node))
+                    ),
                     (
                         j(
                             (
                                 nl(),
                                 " ",
                                 A.CT_V.BULLET,
                                 " ",
@@ -5528,15 +5741,15 @@
         )
         if e(image_path):
             pass
         elif self.yes_no("Показать результат"):
             self.output.write_image("Результат", A.D_CO.file_to_base64(image_path))
         if self.yes_no(
             "Распечатать",
-            js((b("Да"), "- укажите количество копий")),
+            js((self.output.bold("Да"), "- укажите количество копий")),
             yes_checker=lambda value: A.D_Ex.decimal(value) > 0,
         ):
             self.output.good("QR код отправлен на печать")
             for _ in range(1 if self.is_silence else A.D_Ex.decimal(self.input.answer)):
                 A.A_QR.print(image_path)
 
     def study_course_handler(
@@ -5548,15 +5761,17 @@
     ) -> None:
         if e(index):
             action_index: int = self.input.index(
                 "Пожалуйста, выберите пункт меню",
                 [
                     j(
                         (
-                            b(A.D.capitalize(self.keywords.command.EXIT[1])),
+                            self.output.bold(
+                                A.D.capitalize(self.keywords.command.EXIT[1])
+                            ),
                             nl("...", reversed=True),
                         )
                     ),
                     "Пройти обучающий курс",
                     "Выбрать раздел обучающего курса",
                 ]
                 + (
@@ -5626,27 +5841,29 @@
                     )
                     if ne(main_title):
                         self.output.head(main_title) is not None
                     self.study_course_handler(
                         self.input.index(
                             "Пожалуйста, выберите раздел обучения",
                             A.D.to_list(node_list, True),
-                            lambda item, _: b(self.get_command_node_title(item)),
+                            lambda item, _: self.output.bold(
+                                self.get_command_node_title(item)
+                            ),
                         ),
                         node_list,
                         help_content_holder_list,
                     )
             else:
-                title: str = b(self.get_command_title())
+                title: str = self.output.bold(self.get_command_title())
                 self.execute_command([self.study_wiki_location_node])
                 self.output.write_image(
                     js(
                         (
                             "На странице найдите раздел",
-                            b("Обучение"),
+                            self.output.bold("Обучение"),
                             "и выберите пункт меню:",
                             title,
                         )
                     ),
                     wiki_location(),
                 )
         else:
@@ -5715,15 +5932,19 @@
             def represent_data() -> str | None:
                 if field.name == A.CT_FNC.FULL_NAME:
                     index_string: str = nl(index + 1)
                     return (
                         field.default_value
                         if e(data)
                         else j(
-                            (index_string, " " * (len(str(length)) + 3), b(person.pin))
+                            (
+                                index_string,
+                                " " * (len(str(length)) + 3),
+                                self.output.bold(person.pin),
+                            )
                         )
                     )
                 if field.name in [
                     A.CT_FNC.PIN,
                     A.CT_FNC.CARD_REGISTRY_FOLDER,
                     A.CT_FNC.EMAIL,
                 ]:
@@ -5804,18 +6025,18 @@
                     remainder_length: int = length - stack_count * base
                     if remainder_length > 0:
                         polibase_person_card_registry_map[stack_count] = (
                             polibase_person_pin_list[stack_count * base :]
                         )
                     length = len(polibase_person_card_registry_map)
                     text: str = (
-                        f"Разложите все карты пациентов, находящиеся в папке на {b(length)} стопок по {base} в каждой стопке."
+                        f"Разложите все карты пациентов, находящиеся в папке на {self.output.bold(length)} стопок по {base} в каждой стопке."
                     )
                     if remainder_length > 0:
-                        text += f"В последней стопке будет {b(remainder_length)} карт пациентов."
+                        text += f"В последней стопке будет {self.output.bold(remainder_length)} карт пациентов."
                     self.write_line(text)
                     names: list[str] = [
                         "1",
                         "2",
                         "3",
                         "4",
                         "5",
@@ -5869,16 +6090,16 @@
                                         (
                                             A.CT_V.BULLET,
                                             (
                                                 "Возьмите карту пациента c номером "
                                                 if step_limit == 1
                                                 else ""
                                             ),
-                                            j((b(min_pin_value), ": ")),
-                                            b(names[index]),
+                                            j((self.output.bold(min_pin_value), ": ")),
+                                            self.output.bold(names[index]),
                                             "стопка",
                                             js(
                                                 (
                                                     names[
                                                         A.D.check(
                                                             position > 4,
                                                             len(
@@ -5887,15 +6108,15 @@
                                                                 ]
                                                             )
                                                             - position,
                                                             position,
                                                         )
                                                     ],
                                                     "карта",
-                                                    b(
+                                                    self.output.bold(
                                                         A.D.check(
                                                             position + 1
                                                             > int(
                                                                 len(
                                                                     polibase_person_card_registry_map[
                                                                         index
                                                                     ]
@@ -6022,15 +6243,15 @@
                             A.D.list_to_string(
                                 A.D.map(
                                     lambda item: j(
                                         (
                                             " " * 8,
                                             A.CT_V.BULLET,
                                             " ",
-                                            b(item.name),
+                                            self.output.bold(item.name),
                                             " (",
                                             item.count,
                                             ")",
                                         )
                                     ),
                                     folder_list,
                                 ),
@@ -6067,15 +6288,15 @@
                                         )
                                         if not titled
                                         else ""
                                     ),
                                     " " * 4,
                                     A.CT_V.BULLET,
                                     " ",
-                                    b(folder_name),
+                                    self.output.bold(folder_name),
                                     ": ",
                                     A.D.list_to_string(diff_list),
                                 )
                             )
                         )
                         titled = True
 
@@ -6168,34 +6389,38 @@
                                     ):
                                         self.drop_args()
                                         self.output.separated_line()
                                         self.write_line(
                                             js(
                                                 (
                                                     "Карта пациента с персональным номером",
-                                                    b(polibase_person.pin),
+                                                    self.output.bold(
+                                                        polibase_person.pin
+                                                    ),
                                                     "добавлена в папку",
-                                                    b(
+                                                    self.output.bold(
                                                         polibase_person_card_registry_folder
                                                     ),
                                                 )
                                             )
                                         )
                                     else:
                                         pass
                                 else:
                                     self.drop_args()
                                     self.output.separated_line()
                                     self.write_line(
                                         js(
                                             (
                                                 "Карта пациента с персональным номером",
-                                                b(polibase_person.pin),
+                                                self.output.bold(polibase_person.pin),
                                                 "уже находится в папке",
-                                                b(polibase_person_card_registry_folder),
+                                                self.output.bold(
+                                                    polibase_person_card_registry_folder
+                                                ),
                                             )
                                         )
                                     )
                                     A.CR.set_folder_for_person(
                                         polibase_person_card_registry_folder,
                                         polibase_person,
                                         A.R_P.person_by_login(
@@ -6246,24 +6471,24 @@
                 is_new: bool = (
                     e(polibase_person_pin_list)
                     or polibase_person.pin not in polibase_person_pin_list
                 )
                 result: str = (
                     f"{index + 1}. {'Добавлена ' if is_new else ''}{polibase_person.pin}: {polibase_person.FullName}"
                 )
-                return result if is_new else b(result)
+                return result if is_new else self.output.bold(result)
 
             self.output.write_result(
                 Result(A.CT_FC.POLIBASE.PERSON, polibase_person_list_result),
                 False,
                 label_function=label_function,
                 title=js(
                     (
                         "Список карт пациентов в папке",
-                        b(polibase_person_card_registry_folder),
+                        self.output.bold(polibase_person_card_registry_folder),
                     )
                 ),
             )
             if ne(interruption):
                 raise interruption
 
     def create_password_handler(self) -> None:
@@ -6284,15 +6509,15 @@
             variable_is_exists: bool = ne(variable_storage_list)
             if variable_is_exists:
 
                 def label_function(
                     item: StorageVariableHolder, _: int | None = None
                 ) -> str:
                     return j(
-                        [b(item.key_name)]
+                        [self.output.bold(item.key_name)]
                         + [
                             "" if e(item.description) else " (",
                             item.description,
                             ")",
                         ]
                     )
 
@@ -6304,15 +6529,15 @@
                 if self.yes_no(
                     js(("Обновить временную метку:", label_function(timestamp_holder)))
                 ):
                     if self.yes_no(
                         "Использовать текущую дату",
                         no_label=js(
                             (
-                                b("Ввести дату самостоятельно"),
+                                self.output.bold("Ввести дату самостоятельно"),
                                 "- отправьте",
                                 A.O.get_number(0),
                             )
                         ),
                     ):
                         A.D_V_T.update(timestamp_holder)
                         if A.C_V_T_E.exists_by_timestamp(timestamp_holder.key_name):
@@ -6325,15 +6550,15 @@
                     timestamp_name,
                     (
                         None
                         if self.yes_no(
                             "Использовать текущую дату",
                             no_label=js(
                                 (
-                                    b("Ввести дату самостоятельно"),
+                                    self.output.bold("Ввести дату самостоятельно"),
                                     "- отправьте",
                                     A.O.get_number(0),
                                 )
                             ),
                         )
                         else self.input.datetime(use_time=None, ask_time_input=False)
                     ),
@@ -6342,24 +6567,36 @@
                 self.output.good("Временная метка создана")
                 break
         note_name: str | None = None
         if self.yes_no("Создать заметку для временной метки"):
             self.output.header("Создание заметки для временной метки")
             note_name: str | None = None
             if self.yes_no(
-                js(("Использовать название", b(timestamp_name), "для заметки"))
+                js(
+                    (
+                        "Использовать название",
+                        self.output.bold(timestamp_name),
+                        "для заметки",
+                    )
+                )
             ):
                 note_name = timestamp_name
             else:
                 while True:
                     if A.C_N.exists(
                         note_name := self.input.input("Введите название заметки")
                     ):
                         self.output.error(
-                            js(("Заметка с названием", b(note_name), "уже существует"))
+                            js(
+                                (
+                                    "Заметка с названием",
+                                    self.output.bold(note_name),
+                                    "уже существует",
+                                )
+                            )
                         )
                     else:
                         break
 
             with self.output.make_indent(2):
                 note_name = self.create_note_handler(
                     note_name,
@@ -6386,26 +6623,26 @@
             expired_timestamp_name: str | None = None
             with self.output.make_indent(2):
                 life_time_holder = self.input.item_by_index(
                     "Выберите продолжительность (в месяцах)",
                     A.D_V.find("life_time") + A.D_V.find("duration"),
                     lambda item, _: j(
                         (
-                            b(item.description),
+                            self.output.bold(item.description),
                             ": ",
                             item.default_value,
                             " месяцев",
                         )
                     ),
                 )
                 if self.yes_no(
                     js(
                         (
                             "Использовать название",
-                            b(timestamp_name),
+                            self.output.bold(timestamp_name),
                             "для истекающей временной метки",
                         )
                     )
                 ):
                     expired_timestamp_name = timestamp_name
                 else:
                     while True:
@@ -6414,15 +6651,15 @@
                                 "Введите название истекающей временной метки"
                             )
                         ):
                             self.output.error(
                                 js(
                                     (
                                         "Истекающая временная метка с названием",
-                                        b(expired_timestamp_name),
+                                        self.output.bold(expired_timestamp_name),
                                         "уже существет",
                                     )
                                 )
                             )
                         else:
                             break
             A.D_V_T_E.set(
@@ -6434,15 +6671,15 @@
             )
             self.output.good("Истекающая заметка создана")
 
     def print_handler(self) -> None:
         image_path: str = self.arg() or self.input.input("Отправьте изображение")
         if self.yes_no(
             "Распечатать",
-            f"{b('Да')} - укажите количество копий",
+            f"{self.output.bold('Да')} - укажите количество копий",
             yes_checker=lambda value: A.D_Ex.decimal(value) > 0,
         ):
             self.output.good("Изображение отправлено на печать")
             image_path_list: tuple = A.D.separate_unquoted_and_quoted(image_path)
             image_path = j(
                 A.D.not_empty_items([js(image_path_list[0])] + image_path_list[1])
             )
@@ -6451,15 +6688,15 @@
 
     def about_it_handler(self) -> None:
         it_user_list: Result[list[User]] = A.R_U.by_job_position(
             A.CT_AD.JobPositions.IT
         )
 
         def label_function(user: User, _) -> str:
-            result: str = nl(js(("", A.CT.VISUAL.BULLET, b(user.name))))
+            result: str = nl(js(("", A.CT.VISUAL.BULLET, self.output.bold(user.name))))
             if ne(user.description):
                 user_description_list: list[str] = A.D_F.description_list(
                     user.description
                 )
                 workstation_name: str = user_description_list[1]
                 workstation: Workstation = A.R_WS.by_name(workstation_name).data
                 result += nl(j((" ", user_description_list[0])))
@@ -6468,15 +6705,15 @@
                         internal_telephone_number: str = str(
                             A.D_Ex.decimal(workstation.description.split("(")[-1])
                         )
                         result += nl(
                             js(
                                 (
                                     "   Внутренний номер телефона:",
-                                    b(internal_telephone_number),
+                                    self.output.bold(internal_telephone_number),
                                 )
                             )
                         )
             return result
 
         self.output.write_result(
             it_user_list,
@@ -6495,25 +6732,25 @@
 
     def find_free_mark_handler(self) -> None:
         value: str | None = self.arg()
         try:
             result_mark: Mark = one(A.R_M.by_any(value or self.input.mark.any()))
 
             def label_function(data_item: Mark, _: int) -> str:
-                return j((A.CT.VISUAL.BULLET, b(data_item.TabNumber)))
+                return j((A.CT.VISUAL.BULLET, self.output.bold(data_item.TabNumber)))
 
             def filter_function(mark: Mark) -> bool:
                 return mark.GroupID == result_mark.GroupID
 
             self.write_line(
                 nl(
                     j(
                         (
                             "Свободные карты доступа для группы доступа ",
-                            b(result_mark.GroupName),
+                            self.output.bold(result_mark.GroupName),
                             ":",
                         )
                     )
                 )
             )
             self.output.write_result(
                 A.R.filter(A.R_M.free_list(), filter_function),
@@ -6524,18 +6761,24 @@
             )
         except NotFound as error:
             self.output.error(error)
 
     def show_all_free_marks_handler(self) -> None:
         sort_by_tab_number: bool = self.yes_no(
             "Как отсортировать",
-            js((b("по табельному номеру"), "- отправьте", A.O.get_number(1))),
             js(
                 (
-                    b("по названию группы доступа"),
+                    self.output.bold("по табельному номеру"),
+                    "- отправьте",
+                    A.O.get_number(1),
+                )
+            ),
+            js(
+                (
+                    self.output.bold("по названию группы доступа"),
                     "- отправьте",
                     A.O.get_number(0),
                 )
             ),
         )
 
         def sort_function(item: Mark) -> str:
@@ -6549,20 +6792,23 @@
 
     def door_close_handler(self, name: str) -> None:
         A.A_DR.close(name)
 
     def door_open_handler(self, name: str) -> None:
         A.A_DR.open(name)
 
-    def get_or_set_variable_handler(self, get_action: bool = False) -> None:
-        variable_name: str | None = (
+    def variable_value_getter_and_setter_handler(
+        self, get_action: bool = False, variable_name: str | None = None, silence=False
+    ) -> Any:
+        variable_name = (
             None
             if self.is_all and (not get_action or self.argless)
             else (
-                self.arg()
+                variable_name
+                or self.arg()
                 or self.input.input("Введите название или часть названия переменной")
             )
         )
         variable_value_holder_list: list[
             A.CT_S | A.CT_MR.Types | StorageVariableHolder
         ] = A.D_V.find(variable_name)
 
@@ -6593,15 +6839,17 @@
             return j(
                 A.D.filter(
                     lambda item: ne(item),
                     [
                         (
                             ""
                             if e(variable_holder.description)
-                            else j((b(variable_holder.description), ": "))
+                            else j(
+                                (self.output.bold(variable_holder.description), ": ")
+                            )
                         ),
                         (
                             None
                             if n(variable_holder.section)
                             else j(
                                 (variable_holder.section, A.D_V.SECTION_DELIMITER_ALT)
                             )
@@ -6612,15 +6860,15 @@
                 )
             )
 
         if e(variable_value_holder_list):
             self.output.error(f"Значение с именем '{variable_name}' не найдено")
             return
         variable_value_holder: A.CT_S | A.CT_MR.Types | None = None
-        value: Any | None = None
+        value: Any = None
 
         def get_value(
             variable_holder: A.CT_S | A.CT_MR.Types | StorageVariableHolder,
         ) -> Any:
             if isinstance(variable_holder, StorageVariableHolder):
                 return variable_holder.default_value
             if isinstance(variable_holder, A.CT_S):
@@ -6643,18 +6891,21 @@
                             value = A.D_F.datetime(value)
                         else:
                             group_name = "Переменная"
                     if isinstance(variable_holder, A.CT_S):
                         group_name = "Настройка"
                     if isinstance(variable_holder, A.CT_MR.Types):
                         group_name = "Материальный ресурс"
-                    self.write_line(j((A.CT_V.BULLET, " ", group_name, A.CT.SPLITTER)))
-                    with self.output.make_indent(3, True):
-                        self.write_line(f"{label_function(variable_holder)}:")
-                        self.write_line(js(("Значение: ", b(value))))
+                    if not silence:
+                        self.write_line(
+                            j((A.CT_V.BULLET, " ", group_name, A.CT.SPLITTER))
+                        )
+                        with self.output.make_indent(3, True):
+                            self.write_line(f"{label_function(variable_holder)}:")
+                            self.write_line(js(("Значение: ", self.output.bold(value))))
 
         if self.is_all:
             with self.output.make_personalized(False):
                 for variable_value_holder in variable_value_holder_list:
                     show_variable(variable_value_holder)
         else:
             with self.output.make_personalized(False):
@@ -6684,33 +6935,35 @@
                 value = A.D.datetime_to_string(value, format)
             elif isinstance(type, BoolStorageVariableHolder):
 
                 def check_function(value: str) -> bool | None:
                     return A.D_Ex.boolean(value)
 
                 value = self.input.input(
-                    "Введите булево значение (0 или 1)",
+                    "Введите значение (0 или 1)",
                     check_function=check_function,
                 )
             elif isinstance(type, StorageVariableHolder):
                 value = self.input.input("Введите строку")
             if ne(value):
                 if isinstance(variable_value_holder, A.CT_S):
                     A.S.set(variable_value_holder, value)
                 if isinstance(variable_value_holder, A.CT_MR.Types):
                     A.D_MR.set_quantity(variable_value_holder, value)
-            self.output.good(
-                js(
-                    (
-                        "Переменная",
-                        label_function(variable_value_holder, None),
-                        "установлена",
+            if not silence:
+                self.output.good(
+                    js(
+                        (
+                            "Переменная",
+                            label_function(variable_value_holder, None),
+                            "установлена",
+                        )
                     )
                 )
-            )
+            return value
 
     def polibase_person_card_registry_folder_find_handler(self) -> None:
         value: str | None = self.arg()
         while True:
             try:
                 value = value or self.input.polibase_person_any(
                     j(
@@ -6783,15 +7036,15 @@
                                 A.CT_FNC.FULL_NAME,
                             ]:
                                 is_full_name_field: bool = (
                                     field.name == A.CT_FNC.FULL_NAME
                                 )
                                 result[1] = j(
                                     (
-                                        b(field.caption),
+                                        self.output.bold(field.caption),
                                         ": ",
                                         (field.default_value if e(data) else data),
                                         (
                                             j((" (", person.pin, ")"))
                                             if is_full_name_field
                                             else ""
                                         ),
@@ -6842,15 +7095,15 @@
             )["timestamp"]
         )
         timestamp_from_db += timedelta(hours=PERIOD)
         if self.yes_no(
             js(
                 (
                     "Использовать дату и время для дальнейшего заполения информации:",
-                    b(
+                    self.output.bold(
                         A.D_F.datetime(
                             timestamp_from_db, A.CT.DATETIME_ONLY_HOUR_FORMAT
                         )
                     ),
                 )
             )
         ):
@@ -6858,15 +7111,17 @@
             use_preset = True
 
         def log(timestamp: datetime) -> None:
             self.write_line(
                 js(
                     (
                         "Показания для дата и время:",
-                        b(A.D_F.datetime(timestamp, A.CT.DATETIME_ONLY_HOUR_FORMAT)),
+                        self.output.bold(
+                            A.D_F.datetime(timestamp, A.CT.DATETIME_ONLY_HOUR_FORMAT)
+                        ),
                     )
                 )
             )
             preasure_list: list[str] = []
             helium_level: str = self.input.input(
                 "Введите уровень гелия",
                 check_function=lambda item: (
@@ -6964,15 +7219,15 @@
                                                     )
                                                 timestamp = log(timestamp)
                                                 if int(timestamp.hour) == 24:
                                                     self.write_line(
                                                         js(
                                                             (
                                                                 "Переход на следующий день:",
-                                                                b(
+                                                                self.output.bold(
                                                                     A.D_F.date(
                                                                         timestamp
                                                                     )
                                                                 ),
                                                             )
                                                         )
                                                     )
@@ -7025,28 +7280,34 @@
             else person_or_folder_name.ChartFolder
         )
         if ne(folder) and A.CR.is_person_card_registry_folder(folder):
             folder = A.D_F.polibase_person_card_registry_folder(folder)
             result_label_list.append(
                 j(
                     (
-                        b(A.CT_FC.POSITION.caption),
+                        self.output.bold(A.CT_FC.POSITION.caption),
                         if_else(
                             display_only_card_folder_label,
-                            lambda: js(("", b("папки"), b(folder))),
+                            lambda: js(
+                                (
+                                    "",
+                                    self.output.bold("папки"),
+                                    self.output.bold(folder),
+                                )
+                            ),
                             "",
                         ),
                         A.CT.SPLITTER,
                     )
                 )
             )
             card_folder_first_letter: str | None = folder[0]
             if card_folder_first_letter in A.CT_CR.PLACE_NAME:
                 result_label_list.append(
-                    f" {A.CT_V.BULLET} Место: {b(A.CT_CR.PLACE_NAME[card_folder_first_letter])}"
+                    f" {A.CT_V.BULLET} Место: {self.output.bold(A.CT_CR.PLACE_NAME[card_folder_first_letter])}"
                 )
             card_registry_folder_was_registered_event: EventDS | None = one(
                 A.R_E.get(*A.E_B.card_registry_folder_was_registered(folder))
             )
             if nn(polibase_person_pin_list):
                 card_index_source: int = polibase_person_pin_list.index(
                     person_or_folder_name.pin
@@ -7061,28 +7322,30 @@
                 result_label_list.append(
                     if_else(
                         e(polibase_person_pin_list),
                         js(
                             (
                                 "",
                                 A.CT_V.WARNING,
-                                b(i(A.CT_FC.POSITION.default_value)),
+                                self.output.bold(i(A.CT_FC.POSITION.default_value)),
                             )
                         ),
                         lambda: j(
                             (
                                 nl(
                                     js(
                                         (
                                             "",
                                             A.CT_V.BULLET,
                                             "Карта в папке:",
-                                            b(card_index_source + 1),
+                                            self.output.bold(card_index_source + 1),
                                             "из",
-                                            b(len(polibase_person_pin_list)),
+                                            self.output.bold(
+                                                len(polibase_person_pin_list)
+                                            ),
                                         )
                                     )
                                 ),
                                 j(
                                     [nl("    -------------")]
                                     + [
                                         js(
@@ -7090,15 +7353,15 @@
                                                 "   ",
                                                 (
                                                     A.CT_V.ARROW
                                                     if item == person_or_folder_name.pin
                                                     else A.CT_V.BULLET
                                                 ),
                                                 nl(
-                                                    b(item)
+                                                    self.output.bold(item)
                                                     if item == person_or_folder_name.pin
                                                     else item
                                                 ),
                                             )
                                         )
                                         for item in [
                                             polibase_person_pin_list[card_index - 1],
@@ -7118,24 +7381,24 @@
                     CardRegistryFolderPosition(),
                     card_registry_folder_was_registered_event.parameters,
                 )
                 if display_only_card_folder_label:
                     result_label_list.append(
                         j(
                             (
-                                f" {A.CT_V.BULLET} Шкаф: {b(position.p_a)}\n {A.CT_V.BULLET} Полка: {b(position.p_b)}",
+                                f" {A.CT_V.BULLET} Шкаф: {self.output.bold(position.p_a)}\n {A.CT_V.BULLET} Полка: {self.output.bold(position.p_b)}",
                                 if_else(
                                     position.p_c > 0,
                                     nl(
                                         js(
                                             (
                                                 "",
                                                 A.CT_V.BULLET,
                                                 "Позиция на полке:",
-                                                b(position.p_c),
+                                                self.output.bold(position.p_c),
                                             )
                                         )
                                     ),
                                     "",
                                 ),
                             )
                         )
@@ -7144,25 +7407,25 @@
                 result_label_list.append(
                     j(
                         (
                             js(
                                 (
                                     "",
                                     A.CT_V.BULLET,
-                                    b("Папка:"),
+                                    self.output.bold("Папка:"),
                                     nl(),
                                     "     шкаф:",
-                                    nl(b(position.p_a)),
+                                    nl(self.output.bold(position.p_a)),
                                     "     полка:",
-                                    b(position.p_b),
+                                    self.output.bold(position.p_b),
                                 )
                             ),
                             if_else(
                                 lambda: position.p_c > 0,
-                                f"\n     позиция на полке: {b(position.p_c)}",
+                                f"\n     позиция на полке: {self.output.bold(position.p_c)}",
                                 "",
                             ),
                         )
                     )
                 )
 
             return nl(jnl(result_label_list), reversed=True)
@@ -7266,15 +7529,17 @@
                 pass
 
         result: Result[list[EventDS]] | None = None
         event_builder: Callable = (
             A.E_B.polibase_person_with_inaccessable_email_was_detected
         )
         count: int = len(A.R_E.get(event_builder()))
-        if n(self.arg()) and self.yes_no(js(("Проверить все события:", b(count)))):
+        if n(self.arg()) and self.yes_no(
+            js(("Проверить все события:", self.output.bold(count)))
+        ):
             result = A.R_E.get(event_builder())
         else:
             while True:
                 try:
                     polibase_person: PolibasePerson = one(
                         self.input.polibase_persons_by_any(self.arg())
                     )
@@ -7283,15 +7548,15 @@
                 except NotFound as _:
                     self.output.error("Пациент не найден")
         if A.R.is_empty(result):
             self.output.error(
                 js(
                     (
                         "Событие о добавление недоступной почты для пациента:",
-                        b(polibase_person.FullName),
+                        self.output.bold(polibase_person.FullName),
                         j(("(", polibase_person.pin, ")")),
                         "отсутствует.",
                     )
                 )
             )
         else:
             A.R.every(every_action, result)
@@ -7379,15 +7644,17 @@
                         person_pin_list: list[int] = A.CR.persons_pin_by_folder(
                             person.ChartFolder
                         )
                         return (
                             True,
                             j(
                                 (
-                                    b(A.CT_FC.POLIBASE.CARD_REGISTRY_FOLDER.caption),
+                                    self.output.bold(
+                                        A.CT_FC.POLIBASE.CARD_REGISTRY_FOLDER.caption
+                                    ),
                                     ": ",
                                     data,
                                     (
                                         self.get_polibase_person_card_place_label(
                                             person, person_pin_list
                                         )
                                         if person.pin in person_pin_list
@@ -7448,37 +7715,43 @@
             result: list[CommandNode] = self.command_node_tail_list[command_node]
             parent: CommandNode = result[0].parent
             while nn(parent):
                 result.insert(0, parent)
                 parent = parent.parent
             self.command_list.append(result)
         self.command_list.sort(key=self.command_sort_function)
-        if n(MobileHelper.command_name_set):
-            command_node_name_set: set[str] = set()
+        if n(MobileHelper.command_base_name_collection):
+            command_node_base_name_list: list[str] = []
+            command_node_name_list: list[str] = []
             allowed_group_set: set[Groups] = set()
             for command_item in self.command_list:
                 for command_node in command_item:
                     if ne(command_node.allowed_groups):
                         for group in command_node.allowed_groups:
                             allowed_group_set.add(group)
-                    name_list: list[str] = A.D.map(
-                        lambda item: command_name_base(item),
+                    command_node_base_name_list += A.D.map(
+                        get_command_base_name,
                         command_node.name_list or [],
                     )
-                    for name_item in name_list:
-                        command_node_name_set.add(name_item)
-            MobileHelper.command_name_set = set(
-                A.D.filter(ne, command_node_name_set) + self.keywords.command.EXIT
+                    command_node_name_list += command_node.name_list or []
+            MobileHelper.command_base_name_collection = tuple(
+                set(
+                    A.D.filter(ne, command_node_base_name_list)
+                    + self.keywords.command.EXIT
+                )
             )
-            MobileHelper.allowed_group_set = allowed_group_set
+            MobileHelper.command_node_name_collection = tuple(
+                set(A.D.filter(ne, command_node_name_list) + self.keywords.command.EXIT)
+            )
+            MobileHelper.allowed_group_collection = allowed_group_set
         self.fill_allowed_group_list()
 
     def fill_allowed_group_list(self, session: Session | None = None) -> None:
         session = session or self.session
-        for group in MobileHelper.allowed_group_set:
+        for group in MobileHelper.allowed_group_collection:
             A.C_A.by_group(group, False, session, False, False)
 
     def command_sort_function(self, value: list[CommandNode]) -> str:
         name_list: list[str] = []
         for item in value:
             name_list.append(
                 self.get_command_node_label(item)
@@ -7530,65 +7803,65 @@
         value = value.lower()
         for index, item in enumerate(self.keywords.command.PIH):
             if value.find(item) == 0:
                 self.language_index = index
                 return True
         return False
 
-    def parse_arguments(self, line: str) -> list[str]:
-        line = line[len(PIH.NAME) :]
-        line_part_list: list[str] | None = None
-        line = line.replace("\xa0", " ")
-        line_part_list, self.arg_list = A.D.separate_unquoted_and_quoted(line)
-        self.comandless_line_part_list = list(line_part_list)
-        self.line_part_list = A.D.not_empty_items(line.split(" "))
-        line_part_list = A.D.filter(
+    def parse_arguments(self, value: str) -> list[str]:
+        part_list: list[str] | None = None
+        value = A.D.space_format(value[len(PIH.NAME) :])
+        part_list, self.arg_list = A.D.separate_unquoted_and_quoted(value)
+        self.commandless_part_list = list(part_list)
+        self.line_part_list = A.D.not_empty_items(value.split(" "))
+        part_list = A.D.filter(
             lambda item: item.lower() not in (PIH.NAME, PIH.NAME_ALT),
-            line_part_list,
+            part_list,
         )
-
-        ################################
         self.flags = 0
-
         self.flag_information = []
-        for index, arg_item in enumerate(line_part_list):
+        for index, arg_item in enumerate(part_list):
             arg_item = lw(arg_item)
             if arg_item in FLAG_MAP:
                 flag: Flags = FLAG_MAP[arg_item]
                 self.flags = BM.add(self.flags, flag)
                 self.flag_information.append((index, arg_item, flag))
         if ne(self.flag_information):
-            line_part_list = [
+            part_list = [
                 item
-                for item in line_part_list
+                for item in part_list
                 if lw(item)
                 not in A.D.map(
                     lambda flag_information_item: flag_information_item[1],
                     self.flag_information,
                 )
             ]
-        non_reserved_keyword_list: list[str] = []
-        for arg_item in line_part_list:
-            reserved_keyword_exists: bool = False
-            for system_keyword in MobileHelper.command_name_set:
-                reserved_keyword_exists = (
-                    reserved_keyword_exists
-                    or arg_item.lower().startswith(system_keyword)
+        non_command_node_name_list: list[str] = []
+        for arg_item in part_list:
+            command_node_name_exists: bool = False
+            for command_node_name in MobileHelper.command_node_name_collection:
+                command_node_name_has_variants: bool = (
+                    command_node_name.find(COMMAND_NAME_VARIANT_SPLITTER) != -1
+                )
+                command_node_name_exists = command_node_name_exists or (
+                    (command_node_name_equal(arg_item, command_node_name))
+                    if command_node_name_has_variants
+                    else A.D.equal(arg_item, command_node_name)
                 )
-                if reserved_keyword_exists:
-                    self.comandless_line_part_list.remove(arg_item)
+                if command_node_name_exists:
+                    self.commandless_part_list.remove(arg_item)
                     break
-            if not reserved_keyword_exists:
-                non_reserved_keyword_list.append(arg_item)
-        for arg_item in non_reserved_keyword_list:
-            line_part_list.remove(arg_item)
+            if not command_node_name_exists:
+                non_command_node_name_list.append(arg_item)
+        for arg_item in non_command_node_name_list:
+            part_list.remove(arg_item)
             self.arg_list.append(arg_item)
         self.session.flags = BM.add(self.session.flags, self.flags)
         self.session.arg_list = self.arg_list
-        return line_part_list
+        return part_list
 
     def do_pih(
         self,
         line: str = PIH.NAME,
         sender_user: User | None = None,
         external_flags: int | None = None,
         return_result_key: str | None = None,
@@ -7605,59 +7878,57 @@
 
                 if nn(external_flags):
                     self.external_flags = external_flags
 
                 self.current_command = None
                 command_list: list[list[CommandNode]] = []
                 #
-                line_part_list: list[str] = self.parse_arguments(line)
+                part_list: list[str] = self.parse_arguments(line)
                 #
 
                 if nn(arguments):
                     self.session.arg_list.extend(arguments)
 
-                source_line_part_list: list[str] = A.D.map(
-                    str.lower, list(line_part_list)
-                )
-                line_part_list_length: int = len(line_part_list)
+                source_part_list: list[str] = A.D.map(str.lower, list(part_list))
+                part_list_length: int = len(part_list)
 
-                if line_part_list_length > 0:
+                if part_list_length > 0:
                     filtered_command_list: list[list[CommandNode]] = A.D.filter(
                         self.command_list_filter_function, self.command_list
                     )
+                    command_item: list[CommandNode]
                     for command_item in filtered_command_list:
-                        command_item: list[CommandNode] = command_item
                         command_len: int = len(command_item)
-                        if line_part_list_length > command_len:
+                        if part_list_length > command_len:
                             continue
                         command_node_name_list: list[str] = []
                         for command_node in command_item:
-                            command_node_name_list += A.D.map(
-                                lambda item: command_name_base(item),
-                                command_node.name_list,
-                            )
-                        work_arg_list: list[str] = list(source_line_part_list)
-                        for arg_item in source_line_part_list:
+                            command_node_name_list += command_node.name_list
+
+                        temp_part_list: list[str] = list(source_part_list)
+                        for source_part_item in source_part_list:
                             has_result: bool = False
                             for command_node_name in command_node_name_list:
                                 has_result = ne(
                                     command_node_name
-                                ) and arg_item.startswith(command_node_name)
+                                ) and command_node_name_equal(
+                                    source_part_item, command_node_name
+                                )
                                 if has_result:
                                     break
                             if has_result:
-                                work_arg_list.remove(arg_item)
-                                if arg_item in line_part_list:
-                                    line_part_list.remove(arg_item)
+                                temp_part_list.remove(source_part_item)
+                                if source_part_item in part_list:
+                                    part_list.remove(source_part_item)
                                 command_len -= 1
                             if command_len == 0:
                                 self.current_command = list(command_item)
                         if not self.current_command:
                             if command_len > 0:
-                                if len(work_arg_list) == 0:
+                                if len(temp_part_list) == 0:
                                     command_list.append(command_item)
                 else:
                     self.current_command = [self.main_menu_node]
                 is_addressed: bool = self.has_flag(Flags.ADDRESS)
                 is_addressed_as_link: bool = self.has_flag(Flags.ADDRESS_AS_LINK)
                 if is_addressed or is_addressed_as_link:
                     with self.output.make_indent(2):
@@ -7696,15 +7967,18 @@
                         and nn(flag_information_item_index)
                         and len(self.line_part_list) > flag_information_item_index,
                         lambda: self.line_part_list[flag_information_item_index],
                     )
                     while True:
                         try:
                             self.recipient_user_list = self.input.user.by_any(
-                                recipient, True, b("Выберите получателя команды"), True
+                                recipient,
+                                True,
+                                self.output.bold("Выберите получателя команды"),
+                                True,
                             )
                         except NotFound as error:
                             recipient = None
                             self.output.error(error)
                         else:
                             if len(self.recipient_user_list) == 1:
                                 if (
@@ -7749,15 +8023,17 @@
                         if command_list_len > 1:
                             self.output.separated_line()
                             with self.output.make_indent(2):
                                 self.write_line(
                                     nl(
                                         js(
                                             (
-                                                b(self.current_pih_keyword.upper()),
+                                                self.output.bold(
+                                                    self.current_pih_keyword.upper()
+                                                ),
                                                 "нашёл следующие разделы:",
                                             )
                                         )
                                     )
                                 )
                         with self.output.make_indent(4):
 
@@ -7767,15 +8043,17 @@
                                 command_node: CommandNode = command[-1]
                                 return (
                                     j(
                                         (
                                             A.D.as_value(
                                                 command_node.text_decoration_before
                                             ),
-                                            b(self.get_command_label(command)),
+                                            self.output.bold(
+                                                self.get_command_label(command)
+                                            ),
                                             A.D.as_value(
                                                 command_node.text_decoration_after
                                             ),
                                         )
                                     )
                                     if len(command_list) > 1
                                     else None
@@ -7836,15 +8114,15 @@
                     value_string_list[0]
                     if len(value_string_list) == 1
                     else value_string_list[1]
                 )
         else:
             result = value
         return A.D.map(
-            lambda item: (item or "").replace(COMMAND_NAME_BASE_DELEMITER, ""),
+            get_command_variant_name,
             result,
         )
 
     def get_command_node_text(self, value: str | CommandNode) -> str:
         result: str | None = None
         if isinstance(value, CommandNode):
             if nn(value.text):
@@ -7863,48 +8141,48 @@
             A.D.map(
                 lambda item: item[item.startswith(COMMAND_LINK_SYMBOL) :],
                 value.name_list,
             )
         )
 
         def name(value: str) -> str:
-            index: int = value.find(COMMAND_NAME_BASE_DELEMITER)
+            index: int = value.find(COMMAND_NAME_VARIANT_SPLITTER)
             if index != -1:
                 return j((value[:index], "(", value[index + 1 :], ")"))
             return value
 
         name_list = A.D.map(name, name_list)
         return j(
             (
                 A.D.check(
                     len(name_list) > 1,
                     lambda: j(
                         (
                             "[ ",
                             j(
-                                A.D.map(lambda item: b(item), name_list),
+                                A.D.map(lambda item: self.output.bold(item), name_list),
                                 j((" ", i("или"), " ")),
                             ),
                             " ]",
                         )
                     ),
                     A.D.check(
                         len(name_list) > 0
                         and value.name_list != self.exit_node.name_list,
-                        lambda: b(name_list[0]),
+                        lambda: self.output.bold(name_list[0]),
                         "",
                     ),
                 )
             )
         )
 
     def get_command_node_name(
         self, value: CommandNode, use_language_index: bool = False
     ) -> str:
-        return command_name_base(
+        return get_command_base_name(
             A.D.by_index(
                 A.D.not_empty_items(
                     A.D.map(
                         lambda item: item[item.startswith(COMMAND_LINK_SYMBOL) :],
                         value.name_list,
                     )
                 ),
@@ -7965,15 +8243,15 @@
             self.fill_allowed_group_list(session)
 
         def label_function(command: list[CommandNode], _: int) -> str:
             command_node: CommandNode = command[0]
             return j(
                 (
                     A.D.as_value(command_node.text_decoration_before),
-                    b(self.get_command_label(command)),
+                    self.output.bold(self.get_command_label(command)),
                     A.D.as_value(command_node.description),
                     A.D.as_value(command_node.text_decoration_after),
                 )
             )
 
         command: list[CommandNode] = self.command_by_index(
             "Пожалуйста, выберите пункт меню",
@@ -8040,15 +8318,15 @@
                                 break
                     if is_cyclic:
                         self.output.separated_line()
                         self.write_line(
                             i(
                                 js(
                                     (
-                                        b(PIH.NAME.upper()),
+                                        self.output.bold(PIH.NAME.upper()),
                                         "будет выполнять команду в зацикленном режиме.",
                                     )
                                 )
                             )
                         )
                     if nn(handler):
                         with self.output.make_indent(2, True):
@@ -8077,17 +8355,17 @@
 
     def get_command_title_or_label(
         self,
         value: list[CommandNode] | None = None,
         function: Callable[[str], str] | None = None,
     ) -> str:
         value = value or self.current_command
-        filtered: list[str] = A.D.filter(lambda item: str(item).startswith("|"), value)
-        if len(filtered) > 0:
-            value = filtered
+        # filtered: list[str] = A.D.filter(lambda item: str(item).startswith("|"), value)
+        # if len(filtered) > 0:
+        #    value = filtered
         return j(
             (
                 A.D.capitalize(
                     A.D.list_to_string(
                         A.D.map(function, value),  # type: ignore
                         separator=" ",
                         filter_empty=True,
```

### Comparing `pih-mio-0.28/MobileHelperService/client.py` & `pih-mio-0.29.1/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.28/MobileHelperService/const.py` & `pih-mio-0.29.1/MobileHelperService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.28"
+VERSION: str = "0.29.1"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
@@ -73,25 +73,25 @@
     EXIT: list[str] = ["exit", "выход"]
     BACK: list[str] = ["back", "назад"]
     FIND: list[str] = ["find", "поиск", "search", "найти"]
     CREATE: list[str] = ["create", "создать", "+"]
     CHECK: list[str] = ["check", "проверить"]
     ADD: list[str] = ["add", "добавить", "+"]
     PASSWORD: list[str] = ["password", "пароль"]
-    USER: list[str] = ["user^s", "пользовател^ь"]
+    USER: list[str] = ["user|s", "пользовател|ь"]
     POLIBASE: list[str] = ["polibase", "полибейс"]
-    NOTES: list[str] = ["note^s", "заметк^и"]
-    JOURNALS: list[str] = ["journal^s", "журнал^ы"]
+    NOTES: list[str] = ["note|s", "заметк|и"]
+    JOURNALS: list[str] = ["journal|s", "журнал|ы"]
     RUN: list[str] = ["run", "запуск"]
     PATIENT: list[str] = ["patient", "пациент"]
-    DOCTOR: list[str] = ["doc^tor", "доктор", "врач"]
+    DOCTOR: list[str] = ["doc|tor", "доктор", "врач"]
     JOKE: list[str] = ["joke", "шутка", "анекдот"]
     ASK: list[str] = ["ask"]
     ASK_YES_NO: list[str] = ["ask_yes_no"]
-    SCAN: list[str] = ["scan^ed"]
+    SCAN: list[str] = ["scan|ed"]
     REGISTRY: list[str] = ["registry", "реестр"]
     CARD: list[str] = ["card", "карт"]
 
 
 YES_VARIANTS: tuple[str, ...] = ("1", "yes", "ok", "да")
 YES_LABEL: str = js(("", A.CT.VISUAL.BULLET, b("Да"), "- отправьте", A.O.get_number(1)))
 NO_LABEL: str = js(("", A.CT.VISUAL.BULLET, b("Нет"), "- отправьте", A.O.get_number(0)))
@@ -143,13 +143,13 @@
     FLAG_KEYWORDS.LINK_SYMBOL: Flags.ADDRESS_AS_LINK,
     "?": Flags.HELP,
     "-s": Flags.SETTINGS,
 }
 
 ADMIN_GROUPS: list[Groups] = [Groups.Admin]
 
-COMMAND_NAME_BASE_DELEMITER: str = "^"
+COMMAND_NAME_VARIANT_SPLITTER: str = "|"
 
 WORKSTATION_CHECK_WORD: str = "Workstation"
 
 VERSION_STRING: str = js((VERSION, "⚙️"))
 MODULE_NAME: str = j((A.root.NAME, "mio"), "-")
```

### Comparing `pih-mio-0.28/MobileHelperService/service.py` & `pih-mio-0.29.1/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.28/MobileHelperService/service_api.py` & `pih-mio-0.29.1/MobileHelperService/service_api.py`

 * *Files identical despite different names*

