# Comparing `tmp/g4f-0.3.0.2.tar.gz` & `tmp/g4f-0.3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.0.2.tar", last modified: Sat Apr 20 18:13:41 2024, max compression
+gzip compressed data, was "g4f-0.3.0.3.tar", last modified: Sun Apr 21 05:47:37 2024, max compression
```

## Comparing `g4f-0.3.0.2.tar` & `g4f-0.3.0.3.tar`

### file list

```diff
@@ -1,244 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.588012 g4f-0.3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-20 18:13:30.000000 g4f-0.3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-20 18:13:30.000000 g4f-0.3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-20 18:13:41.588012 g4f-0.3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47160 2024-04-20 18:13:30.000000 g4f-0.3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.552012 g4f-0.3.0.2/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.560012 g4f-0.3.0.2/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.560012 g4f-0.3.0.2/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.568012 g4f-0.3.0.2/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.568012 g4f-0.3.0.2/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.568012 g4f-0.3.0.2/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    32305 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.548012 g4f-0.3.0.2/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    45822 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:13:41.588012 g4f-0.3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-20 18:13:30.000000 g4f-0.3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.791786 g4f-0.3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-21 05:47:34.000000 g4f-0.3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 05:47:34.000000 g4f-0.3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-21 05:47:37.791786 g4f-0.3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47160 2024-04-21 05:47:34.000000 g4f-0.3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.755786 g4f-0.3.0.3/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.763786 g4f-0.3.0.3/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21279 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.763786 g4f-0.3.0.3/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.771786 g4f-0.3.0.3/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.771786 g4f-0.3.0.3/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.771786 g4f-0.3.0.3/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31934 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.775786 g4f-0.3.0.3/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.775786 g4f-0.3.0.3/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.775786 g4f-0.3.0.3/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.775786 g4f-0.3.0.3/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.775786 g4f-0.3.0.3/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.775786 g4f-0.3.0.3/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/unfinished/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.751786 g4f-0.3.0.3/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.779786 g4f-0.3.0.3/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.783786 g4f-0.3.0.3/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.783786 g4f-0.3.0.3/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45952 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.783786 g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.787786 g4f-0.3.0.3/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.787786 g4f-0.3.0.3/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.787786 g4f-0.3.0.3/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.787786 g4f-0.3.0.3/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.787786 g4f-0.3.0.3/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-21 05:47:34.000000 g4f-0.3.0.3/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:47:37.787786 g4f-0.3.0.3/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-21 05:47:37.000000 g4f-0.3.0.3/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-21 05:47:37.000000 g4f-0.3.0.3/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:47:37.000000 g4f-0.3.0.3/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-21 05:47:37.000000 g4f-0.3.0.3/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 05:47:37.000000 g4f-0.3.0.3/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 05:47:37.000000 g4f-0.3.0.3/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 05:47:37.791786 g4f-0.3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-21 05:47:34.000000 g4f-0.3.0.3/setup.py
```

### Comparing `g4f-0.3.0.2/LICENSE` & `g4f-0.3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/PKG-INFO` & `g4f-0.3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.2
+Version: 0.3.0.3
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.3 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.0.2/README.md` & `g4f-0.3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Aichatos.py` & `g4f-0.3.0.3/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Aura.py` & `g4f-0.3.0.3/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Bing.py` & `g4f-0.3.0.3/g4f/Provider/Bing.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import random
 import json
 import uuid
 import time
 import asyncio
 from urllib import parse
 from datetime import datetime, date
-from aiohttp import ClientSession, ClientTimeout, BaseConnector, WSMsgType
 
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from ..image import ImageRequest
-from ..errors import ResponseStatusError, RateLimitError
+from ..errors import ResponseError, ResponseStatusError, RateLimitError
+from ..requests import StreamSession, DEFAULT_HEADERS
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from .helper import get_connector, get_random_hex
+from .helper import get_random_hex
 from .bing.upload_image import upload_image
 from .bing.conversation import Conversation, create_conversation, delete_conversation
 from .BingCreateImages import BingCreateImages
 from .. import debug
 
 class Tones:
     """
@@ -45,15 +45,14 @@
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         timeout: int = 900,
         api_key: str = None,
         cookies: Cookies = None,
-        connector: BaseConnector = None,
         tone: str = None,
         image: ImageType = None,
         web_search: bool = False,
         context: str = None,
         **kwargs
     ) -> AsyncResult:
         """
@@ -75,15 +74,14 @@
         if tone is None:
             tone = tone if model.startswith("gpt-4") else model
         tone = cls.get_model("" if tone is None else tone)
         gpt4_turbo = True if model.startswith("gpt-4-turbo") else False
 
         return stream_generate(
             prompt, tone, image, context, cookies, api_key,
-            get_connector(connector, proxy, True),
             proxy, web_search, gpt4_turbo, timeout,
             **kwargs
         )
 
 def create_context(messages: Messages) -> str:
     """
     Creates a context string from a list of messages.
@@ -98,33 +96,61 @@
         for message in messages
     ) + "\n\n"
 
 def get_ip_address() -> str:
     return f"13.{random.randint(104, 107)}.{random.randint(0, 255)}.{random.randint(0, 255)}"
 
 def get_default_cookies():
+    #muid = get_random_hex().upper()
+    sid = get_random_hex().upper()
+    guid = get_random_hex().upper()
+    isodate = date.today().isoformat()
+    timestamp = int(time.time())
+    zdate = "0001-01-01T00:00:00.0000000"
     return {
-        'SRCHD'         : 'AF=NOFORM',
-        'PPLState'      : '1',
-        'KievRPSSecAuth': '',
-        'SUID'          : '',
-        'SRCHUSR'       : f'DOB={date.today().strftime("%Y%m%d")}&T={int(time.time())}',
-        'SRCHHPGUSR'    : f'HV={int(time.time())}',
-        'BCP'           : 'AD=1&AL=1&SM=1',
-        '_Rwho'         : f'u=d&ts={date.today().isoformat()}',
+        "_C_Auth": "",
+        #"MUID": muid,
+        #"MUIDB":  muid,
+        "_EDGE_S": f"F=1&SID={sid}",
+        "_EDGE_V": "1",
+        "SRCHD": "AF=hpcodx",
+        "SRCHUID": f"V=2&GUID={guid}&dmnchg=1",
+        "_RwBf": (
+            f"r=0&ilt=1&ihpd=0&ispd=0&rc=3&rb=0&gb=0&rg=200&pc=0&mtu=0&rbb=0&g=0&cid="
+            f"&clo=0&v=1&l={isodate}&lft={zdate}&aof=0&ard={zdate}"
+            f"&rwdbt={zdate}&rwflt={zdate}&o=2&p=&c=&t=0&s={zdate}"
+            f"&ts={isodate}&rwred=0&wls=&wlb="
+            "&wle=&ccp=&cpt=&lka=0&lkt=0&aad=0&TH="
+        ),
+        '_Rwho': f'u=d&ts={isodate}',
+        "_SS": f"SID={sid}&R=3&RB=0&GB=0&RG=200&RP=0",
+        "SRCHUSR": f"DOB={date.today().strftime('%Y%m%d')}&T={timestamp}",
+        "SRCHHPGUSR": f"HV={int(time.time())}",
+        "BCP": "AD=1&AL=1&SM=1",
+        "ipv6": f"hit={timestamp}",
+        '_C_ETH' : '1',
     }
 
-def create_headers(cookies: Cookies = None, api_key: str = None) -> dict:
+async def create_headers(cookies: Cookies = None, api_key: str = None) -> dict:
     if cookies is None:
+        # import nodriver as uc
+        # browser = await uc.start(headless=False)
+        # page = await browser.get(Defaults.home)
+        # await asyncio.sleep(10)
+        # cookies = {}
+        # for c in await page.browser.cookies.get_all():
+        #     if c.domain.endswith(".bing.com"):
+        #         cookies[c.name] = c.value
+        # user_agent = await page.evaluate("window.navigator.userAgent")
+        # await page.close()
         cookies = get_default_cookies()
     if api_key is not None:
         cookies["_U"] = api_key
     headers = Defaults.headers.copy()
     headers["cookie"] = "; ".join(f"{k}={v}" for k, v in cookies.items())
-    headers["x-forwarded-for"] = get_ip_address()
     return headers
 
 class Defaults:
     """
     Default settings and configurations for the Bing provider.
     """
     delimiter = "\x1e"
@@ -242,33 +268,21 @@
             "timezoneoffset": 8, "countryConfidence": 8,
             "Center": {"Latitude": 34.0536909, "Longitude": -118.242766},
             "RegionType": 2, "SourceType": 1
         }],
     }
 
     # Default headers for requests
-    home = 'https://www.bing.com/chat?q=Bing+AI&FORM=hpcodx'
+    home = "https://www.bing.com/chat?q=Microsoft+Copilot&FORM=hpcodx"
     headers = {
-        'sec-ch-ua': '"Chromium";v="122", "Not(A:Brand";v="24", "Google Chrome";v="122"',
-        'sec-ch-ua-mobile': '?0',
-        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36',
-        'sec-ch-ua-arch': '"x86"',
-        'sec-ch-ua-full-version': '"122.0.6261.69"',
-        'accept': 'application/json',
-        'sec-ch-ua-platform-version': '"15.0.0"',
+        **DEFAULT_HEADERS,
+        "accept": "application/json",
+        "referer": home,
         "x-ms-client-request-id": str(uuid.uuid4()),
-        'sec-ch-ua-full-version-list': '"Chromium";v="122.0.6261.69", "Not(A:Brand";v="24.0.0.0", "Google Chrome";v="122.0.6261.69"',
-        'x-ms-useragent': 'azsdk-js-api-client-factory/1.0.0-beta.1 core-rest-pipeline/1.12.3 OS/Windows',
-        'sec-ch-ua-model': '""',
-        'sec-ch-ua-platform': '"Windows"',
-        'sec-fetch-site': 'same-origin',
-        'sec-fetch-mode': 'cors',
-        'sec-fetch-dest': 'empty',
-        'referer': home,
-        'accept-language': 'en-US,en;q=0.9',
+        "x-ms-useragent": "azsdk-js-api-client-factory/1.0.0-beta.1 core-rest-pipeline/1.15.1 OS/Windows",
     }
 
 def format_message(msg: dict) -> str:
     """
     Formats a message dictionary into a JSON string with a delimiter.
 
     :param msg: The message dictionary to format.
@@ -364,15 +378,14 @@
 async def stream_generate(
     prompt: str,
     tone: str,
     image: ImageType = None,
     context: str = None,
     cookies: dict = None,
     api_key: str = None,
-    connector: BaseConnector = None,
     proxy: str = None,
     web_search: bool = False,
     gpt4_turbo: bool = False,
     timeout: int = 900,
     conversation: Conversation = None,
     return_conversation: bool = False,
     raise_apology: bool = False,
@@ -389,36 +402,34 @@
     :param context: Additional context for the prompt.
     :param cookies: Cookies for the session.
     :param web_search: Flag to enable web search.
     :param gpt4_turbo: Flag to enable GPT-4 Turbo.
     :param timeout: Timeout for the request.
     :return: An asynchronous generator yielding responses.
     """
-    headers = create_headers(cookies, api_key)
+    headers = await create_headers(cookies, api_key)
     new_conversation = conversation is None
     max_retries = (5 if new_conversation else 0) if max_retries is None else max_retries
-    async with ClientSession(
-        timeout=ClientTimeout(total=timeout), connector=connector
-    ) as session:
-        first = True
-        while first or conversation is None:
+    first = True
+    while first or conversation is None:
+        async with StreamSession(timeout=timeout, proxy=proxy) as session:
             first = False
             do_read = True
             try:
                 if conversation is None:
                     conversation = await create_conversation(session, headers, tone)
                 if return_conversation:
                     yield conversation
-            except ResponseStatusError as e:
+            except (ResponseStatusError, RateLimitError) as e:
                 max_retries -= 1
                 if max_retries < 1:
                     raise e
                 if debug.logging:
                     print(f"Bing: Retry: {e}")
-                headers = create_headers()
+                headers = await create_headers()
                 await asyncio.sleep(sleep_retry)
                 continue
 
             image_request = await upload_image(
                 session,
                 image,
                 "Balanced" if tone == Tones.copilot else tone,
@@ -430,43 +441,42 @@
                 'wss://sydney.bing.com/sydney/ChatHub',
                 autoping=False,
                 params={'sec_access_token': conversation.conversationSignature},
                 headers=headers
             ) as wss:
                 await wss.send_str(format_message({'protocol': 'json', 'version': 1}))
                 await wss.send_str(format_message({"type": 6}))
-                await wss.receive(timeout=timeout)
+                await wss.receive_str()
                 await wss.send_str(create_message(
                     conversation, prompt, tone,
                     context if new_conversation else None,
                     image_request, web_search, gpt4_turbo,
                     new_conversation
                 ))
                 response_txt = ''
                 returned_text = ''
                 message_id = None
                 while do_read:
-                    msg = await wss.receive(timeout=timeout)
-                    if msg.type == WSMsgType.CLOSED:
-                        break
-                    if msg.type != WSMsgType.TEXT or not msg.data:
-                        continue
-                    objects = msg.data.split(Defaults.delimiter)
+                    msg = await wss.receive_str()
+                    objects = msg.split(Defaults.delimiter)
                     for obj in objects:
                         if obj is None or not obj:
                             continue
-                        response = json.loads(obj)
+                        try:
+                            response = json.loads(obj)
+                        except json.JSONDecodeError:
+                            continue
                         if response and response.get('type') == 1 and response['arguments'][0].get('messages'):
                             message = response['arguments'][0]['messages'][0]
                             if message_id is not None and message_id != message["messageId"]:
                                 returned_text = ''
                             message_id = message["messageId"]
                             image_response = None
                             if (raise_apology and message['contentOrigin'] == 'Apology'):
-                                raise RuntimeError("Apology Response Error")
+                                raise ResponseError("Apology Response Error")
                             if 'adaptiveCards' in message:
                                 card = message['adaptiveCards'][0]['body'][0]
                                 if "text" in card:
                                     response_txt = card.get('text')
                                 if message.get('messageType') and "inlines" in card:
                                     inline_txt = card['inlines'][0].get('text')
                                     response_txt += f"{inline_txt}\n"
@@ -484,23 +494,26 @@
                                 if new not in ("", "\n"):
                                     yield new
                                     returned_text = response_txt
                             if image_response is not None:
                                 yield image_response
                         elif response.get('type') == 2:
                             result = response['item']['result']
+                            do_read = False
                             if result.get('error'):
                                 max_retries -= 1
                                 if max_retries < 1:
                                     if result["value"] == "CaptchaChallenge":
                                         raise RateLimitError(f"{result['value']}: Use other cookies or/and ip address")
                                     else:
                                         raise RuntimeError(f"{result['value']}: {result['message']}")
                                 if debug.logging:
                                     print(f"Bing: Retry: {result['value']}: {result['message']}")
-                                headers = create_headers()
-                                do_read = False
+                                headers = await create_headers()
                                 conversation = None
                                 await asyncio.sleep(sleep_retry)
-                                break
-                            return
-        await delete_conversation(session, conversation, headers)
+                            break
+                        elif response.get('type') == 3:
+                            do_read = False
+                            break
+            if conversation is not None:
+                await delete_conversation(session, conversation, headers)
```

### Comparing `g4f-0.3.0.2/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.3/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Blackbox.py` & `g4f-0.3.0.3/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.3/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.3/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.3/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.3/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.3/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.3/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Cnote.py` & `g4f-0.3.0.3/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Cohere.py` & `g4f-0.3.0.3/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.3/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.3/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.3/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Ecosia.py` & `g4f-0.3.0.3/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Feedough.py` & `g4f-0.3.0.3/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.3/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.3/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.3/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.3/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.3/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/GigaChat.py` & `g4f-0.3.0.3/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.3/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.3/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.3/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Koala.py` & `g4f-0.3.0.3/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Liaobots.py` & `g4f-0.3.0.3/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Llama.py` & `g4f-0.3.0.3/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Local.py` & `g4f-0.3.0.3/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.3/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Pi.py` & `g4f-0.3.0.3/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.3/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/Vercel.py` & `g4f-0.3.0.3/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.3/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/You.py` & `g4f-0.3.0.3/g4f/Provider/You.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import uuid
 
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import format_prompt
 from ..image import ImageResponse, to_bytes, is_accepted_format
 from ..requests import StreamSession, FormData, raise_for_status
-from .you.har_file import get_dfp_telemetry_id
+from .you.har_file import get_telemetry_ids
+from .. import debug
 
 class You(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://you.com"
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     default_model = "gpt-3.5-turbo"
@@ -31,14 +32,15 @@
         "dall-e",
     ]
     model_aliases = {
         "claude-v2": "claude-2"
     }
     _cookies = None
     _cookies_used = 0
+    _telemetry_ids = []
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         stream: bool = True,
@@ -155,26 +157,31 @@
         auth_uuid = "507a52ad-7e69-496b-aee0-1c9863c7c819"
         auth_token = f"public-token-live-{auth_uuid}:public-token-live-{auth_uuid}"
         auth = base64.standard_b64encode(auth_token.encode()).decode()
         return f"Basic {auth}"
 
     @classmethod
     async def create_cookies(cls, client: StreamSession) -> Cookies:
+        if not cls._telemetry_ids:
+            cls._telemetry_ids = await get_telemetry_ids()
         user_uuid = str(uuid.uuid4())
+        telemetry_id = cls._telemetry_ids.pop()
+        if debug.logging:
+            print(f"Use telemetry_id: {telemetry_id}")
         async with client.post(
             "https://web.stytch.com/sdk/v1/passwords",
             headers={
                 "Authorization": cls.get_auth(),
                 "X-SDK-Client": cls.get_sdk(),
                 "X-SDK-Parent-Host": cls.url,
                 "Origin": "https://you.com",
                 "Referer": "https://you.com/"
             },
             json={
-                "dfp_telemetry_id": await get_dfp_telemetry_id(),
+                "dfp_telemetry_id": telemetry_id,
                 "email": f"{user_uuid}@gmail.com",
                 "password": f"{user_uuid}#{user_uuid}",
                 "session_duration_minutes": 129600
             }
         ) as response:
             await raise_for_status(response)
             session = (await response.json())["data"]
```

### Comparing `g4f-0.3.0.2/g4f/Provider/__init__.py` & `g4f-0.3.0.3/g4f/Provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from .HuggingChat      import HuggingChat
 from .HuggingFace      import HuggingFace
 from .Koala            import Koala
 from .Liaobots         import Liaobots
 from .Llama            import Llama
 from .Local            import Local
 from .MetaAI           import MetaAI
+from .MetaAIAccount    import MetaAIAccount
 from .PerplexityLabs   import PerplexityLabs
 from .Pi               import Pi
 from .ReplicateImage   import ReplicateImage
 from .Vercel           import Vercel
 from .WhiteRabbitNeo   import WhiteRabbitNeo
 from .You              import You
```

### Comparing `g4f-0.3.0.2/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.3/g4f/Provider/bing/conversation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
-from aiohttp import ClientSession
-from ...requests import raise_for_status
+from ...requests import StreamSession, raise_for_status
 from ...errors import RateLimitError
 from ...providers.conversation import BaseConversation
 
 class Conversation(BaseConversation):
     """
     Represents a conversation with specific attributes.
     """
@@ -18,15 +17,15 @@
         clientId (str): Client identifier.
         conversationSignature (str): Signature for the conversation.
         """
         self.conversationId = conversationId
         self.clientId = clientId
         self.conversationSignature = conversationSignature
 
-async def create_conversation(session: ClientSession, headers: dict, tone: str) -> Conversation:
+async def create_conversation(session: StreamSession, headers: dict, tone: str) -> Conversation:
     """
     Create a new conversation asynchronously.
 
     Args:
     session (ClientSession): An instance of aiohttp's ClientSession.
     proxy (str, optional): Proxy URL. Defaults to None.
 
@@ -45,30 +44,30 @@
     conversationId = data.get('conversationId')
     clientId = data.get('clientId')
     conversationSignature = response.headers.get('X-Sydney-Encryptedconversationsignature')
     if not conversationId or not clientId or not conversationSignature:
         raise RuntimeError('Empty fields: Failed to create conversation')
     return Conversation(conversationId, clientId, conversationSignature)
         
-async def list_conversations(session: ClientSession) -> list:
+async def list_conversations(session: StreamSession) -> list:
     """
     List all conversations asynchronously.
 
     Args:
     session (ClientSession): An instance of aiohttp's ClientSession.
 
     Returns:
     list: A list of conversations.
     """
     url = "https://www.bing.com/turing/conversation/chats"
     async with session.get(url) as response:
         response = await response.json()
         return response["chats"]
 
-async def delete_conversation(session: ClientSession, conversation: Conversation, headers: dict) -> bool:
+async def delete_conversation(session: StreamSession, conversation: Conversation, headers: dict) -> bool:
     """
     Delete a conversation asynchronously.
 
     Args:
     session (ClientSession): An instance of aiohttp's ClientSession.
     conversation (Conversation): The conversation to delete.
     proxy (str, optional): Proxy URL. Defaults to None.
```

### Comparing `g4f-0.3.0.2/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.3/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.3/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.3/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from selenium.webdriver.support import expected_conditions as EC
 except ImportError:
     pass
 
 from ..base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from ...webdriver import get_browser
 from ...typing import AsyncResult, Messages, Cookies, ImageType, AsyncIterator
-from ...requests import get_args_from_browser, raise_for_status
+from ...requests import DEFAULT_HEADERS, get_args_from_browser, raise_for_status
 from ...requests.aiohttp import StreamSession
 from ...image import to_image, to_bytes, ImageResponse, ImageRequest
 from ...errors import MissingAuthError, ResponseError
 from ...providers.conversation import BaseConversation
 from ..openai.har_file import getArkoseAndAccessToken, NoValidHarFileError
 from ... import debug
 
@@ -356,15 +356,14 @@
                         cls.default_model = cls.get_model(model)
                 except Exception as e:
                     api_key = cls._api_key = None
                     cls._create_request_args()
                     if debug.logging:
                         print("OpenaiChat: Load default_model failed")
                         print(f"{e.__class__.__name__}: {e}")
-                        
 
             arkose_token = None
             if cls.default_model is None:
                 try:
                     arkose_token, api_key, cookies = await getArkoseAndAccessToken(proxy)
                     cls._create_request_args(cookies)
                     cls._set_api_key(api_key)
@@ -373,26 +372,27 @@
                 if cls._api_key is None:
                     await cls.nodriver_access_token()
                 if cls._api_key is None and cls.needs_auth:
                     raise e
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
             async with session.post(
-                f"{cls.url}/backend-anon/sentinel/chat-requirements" if not cls._api_key else
+                f"{cls.url}/backend-anon/sentinel/chat-requirements"
+                if not cls._api_key else
                 f"{cls.url}/backend-api/sentinel/chat-requirements",
                 json={"conversation_mode_kind": "primary_assistant"},
                 headers=cls._headers
             ) as response:
                 cls._update_request_args(session)
                 await raise_for_status(response)
                 data = await response.json()
                 blob = data["arkose"]["dx"]
                 need_arkose = data["arkose"]["required"]
                 chat_token = data["token"]
-                
+
                 if debug.logging:
                     print(f'Arkose: {need_arkose} Turnstile: {data["turnstile"]["required"]}')
 
             if need_arkose and arkose_token is None:
                 arkose_token, api_key, cookies = await getArkoseAndAccessToken(proxy)
                 cls._create_request_args(cookies)
                 cls._set_api_key(api_key)
@@ -591,16 +591,15 @@
             user_data_dir = user_config_dir("g4f-nodriver")
         except:
             user_data_dir = None
         if debug.logging:
             print(f"Open nodriver with user_dir: {user_data_dir}")
         browser = await uc.start(user_data_dir=user_data_dir)
         page = await browser.get("https://chat.openai.com/")
-        while await page.find("[id^=headlessui-menu-button-]") is None:
-            await asyncio.sleep(1)
+        await page.select("[id^=headlessui-menu-button-]", 240)
         api_key = await page.evaluate(
             "(async () => {"
             "let session = await fetch('/api/auth/session');"
             "let data = await session.json();"
             "let accessToken = data['accessToken'];"
             "let expires = new Date(); expires.setTime(expires.getTime() + 60 * 60 * 4 * 1000);"
             "document.cookie = 'access_token=' + accessToken + ';expires=' + expires.toUTCString() + ';path=/';"
@@ -658,24 +657,18 @@
                 data = await response.json()
                 if "accessToken" in data:
                     return data["accessToken"]
 
     @staticmethod
     def get_default_headers() -> dict:
         return {
-            "accept-language": "en-US",
+            **DEFAULT_HEADERS,
             "content-type": "application/json",
             "oai-device-id": str(uuid.uuid4()),
             "oai-language": "en-US",
-            "sec-ch-ua": "\"Google Chrome\";v=\"123\", \"Not:A-Brand\";v=\"8\", \"Chromium\";v=\"123\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Linux\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin"
         }
 
     @staticmethod
     def _format_cookies(cookies: Cookies):
         return "; ".join(f"{k}={v}" for k, v in cookies.items() if k != "access_token")
 
     @classmethod
@@ -692,19 +685,19 @@
             cls._cookies[c.key if hasattr(c, "key") else c.name] = c.value
         cls._update_cookie_header()
 
     @classmethod
     def _set_api_key(cls, api_key: str):
         cls._api_key = api_key
         cls._expires = int(time.time()) + 60 * 60 * 4
-        cls._headers["Authorization"] = f"Bearer {api_key}"
+        cls._headers["authorization"] = f"Bearer {api_key}"
 
     @classmethod
     def _update_cookie_header(cls):
-        cls._headers["Cookie"] = cls._format_cookies(cls._cookies)
+        cls._headers["cookie"] = cls._format_cookies(cls._cookies)
 
 class Conversation(BaseConversation):
     """
     Class to encapsulate response fields.
     """
     def __init__(self, conversation_id: str = None, message_id: str = None, finish_reason: str = None):
         self.conversation_id = conversation_id
```

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.3/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.3/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.3/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.3/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.3/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.3/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.3/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.3/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.3/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.3/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.3/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.3/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.3/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.3/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.3/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.3/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.3/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.3/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.3/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.3/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.3/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.3/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.3/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.3/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.0.3/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.3/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.3/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.3/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/unfinished/Replicate.py` & `g4f-0.3.0.3/g4f/Provider/unfinished/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/Provider/you/har_file.py` & `g4f-0.3.0.3/g4f/Provider/you/har_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import json
 import os
+import os.path
 import random
-import uuid
-import asyncio
 import requests
 
 from ...requests import StreamSession, raise_for_status
+from ...errors import MissingRequirementsError
+from ... import debug
 
 class NoValidHarFileError(Exception):
     ...
 
 class arkReq:
     def __init__(self, arkURL, arkHeaders, arkBody, arkCookies, userAgent):
         self.arkURL = arkURL
@@ -63,68 +64,49 @@
 async def sendRequest(tmpArk: arkReq, proxy: str = None):
     async with StreamSession(headers=tmpArk.arkHeaders, cookies=tmpArk.arkCookies, proxies={"all": proxy}) as session:
         async with session.post(tmpArk.arkURL, data=tmpArk.arkBody) as response:
             await raise_for_status(response)
             return await response.text()
 
 async def get_dfp_telemetry_id(proxy: str = None):
-    return await telemetry_id_with_driver(proxy)
     global chatArks
     if chatArks is None:
         chatArks = readHAR()
     return await sendRequest(random.choice(chatArks), proxy)
 
-async def telemetry_id_with_driver(proxy: str = None):
-    from ...debug import logging
-    if logging:
-        print('getting telemetry_id for you.com with nodriver')
+async def get_telemetry_ids(proxy: str = None) -> list:
+    if debug.logging:
+        print('Getting telemetry_id for you.com with nodriver')
     try:
-        import nodriver as uc
-        from nodriver import start, cdp, loop
+        from nodriver import start
     except ImportError:
-        if logging:
-            print('nodriver not found, random uuid (may fail)')
-        return str(uuid.uuid4())
-
-    CAN_EVAL = False
-    payload_received = False
-    payload = None
-
+        raise MissingRequirementsError('Install "nodriver" package | pip install -U nodriver')
     try:
         browser = await start()
         tab = browser.main_tab
-
-        async def send_handler(event: cdp.network.RequestWillBeSent):
-            nonlocal CAN_EVAL, payload_received, payload
-            if 'telemetry.js' in event.request.url:
-                CAN_EVAL = True
-            if "/submit" in event.request.url:
-                payload = event.request.post_data
-                payload_received = True
-
-        tab.add_handler(cdp.network.RequestWillBeSent, send_handler)
         await browser.get("https://you.com")
 
-        while not CAN_EVAL:
+        while not await tab.evaluate('"GetTelemetryID" in this'):
             await tab.sleep(1)
 
-        await tab.evaluate('window.GetTelemetryID("public-token-live-507a52ad-7e69-496b-aee0-1c9863c7c819", "https://telemetry.stytch.com/submit");')
-
-        while not payload_received:
-            await tab.sleep(.1)
-
-    except Exception as e:
-        print(f"Error occurred: {str(e)}")
+        async def get_telemetry_id():
+            public_token = "public-token-live-507a52ad-7e69-496b-aee0-1c9863c7c819"
+            telemetry_url = "https://telemetry.stytch.com/submit"
+            return await tab.evaluate(f'this.GetTelemetryID("{public_token}", "{telemetry_url}");', await_promise=True)
+
+        # for _ in range(500):
+        #     with open("hardir/you.com_telemetry_ids.txt", "a") as f:
+        #         f.write((await get_telemetry_id()) + "\n")
 
+        return [await get_telemetry_id() for _ in range(4)]
     finally:
         try:
             await tab.close()
         except Exception as e:
             print(f"Error occurred while closing tab: {str(e)}")
-
         try:
             await browser.stop()
         except Exception as e:
             pass
 
     headers = {
         'Accept': '*/*',
```

### Comparing `g4f-0.3.0.2/g4f/__init__.py` & `g4f-0.3.0.3/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/api/__init__.py` & `g4f-0.3.0.3/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/api/_logging.py` & `g4f-0.3.0.3/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/cli.py` & `g4f-0.3.0.3/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/async_client.py` & `g4f-0.3.0.3/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/client.py` & `g4f-0.3.0.3/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/helper.py` & `g4f-0.3.0.3/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/image_models.py` & `g4f-0.3.0.3/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/service.py` & `g4f-0.3.0.3/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/stubs.py` & `g4f-0.3.0.3/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/client/types.py` & `g4f-0.3.0.3/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/cookies.py` & `g4f-0.3.0.3/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/errors.py` & `g4f-0.3.0.3/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/__init__.py` & `g4f-0.3.0.3/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/index.html` & `g4f-0.3.0.3/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.3/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.3/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.3/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.3/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.3/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.3/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.3/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/chat.v1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,17 @@
 appStorage = window.localStorage || {
     setItem: (key, value) => self[key] = value,
     getItem: (key) => self[key],
     removeItem: (key) => delete self[key],
     length: 0
 }
 
-const markdown = window.markdownit();
+const markdown = window.markdownit({
+    html: true,
+});
 const markdown_render = (content) => {
     return markdown.render(content
             .replaceAll(/<!-- generated images start -->|<!-- generated images end -->/gm, "")
             .replaceAll(/<img data-prompt="[^>]+">/gm, "")
         )
         .replaceAll("<a href=", '<a target="_blank" href=')
         .replaceAll('<code>', '<code class="language-plaintext">')
@@ -309,14 +311,16 @@
         `
     } else if (message.type == "message") {
         console.error(message.message)
     } else if (message.type == "error") {
         window.error = message.error
         console.error(message.error);
         content_inner.innerHTML += `<p><strong>An error occured:</strong> ${message.error}</p>`;
+    } else if (message.type == "preview") {
+        content_inner.innerHTML = markdown_render(message.preview);
     } else if (message.type == "content") {
         window.text += message.content;
         html = markdown_render(window.text);
         let lastElement, lastIndex = null;
         for (element of ['</p>', '</code></pre>', '</p>\n</li>\n</ol>', '</li>\n</ol>', '</li>\n</ul>']) {
             const index = html.lastIndexOf(element)
             if (index - element.length > lastIndex) {
@@ -545,15 +549,15 @@
     let elements = "";
     let last_model = null;
     for (i in messages) {
         let item = messages[i];
         last_model = item.provider?.model;
         let next_i = parseInt(i) + 1;
         let next_provider = item.provider ? item.provider : (messages.length > next_i ? messages[next_i].provider : null);
-        let provider_label = item.provider?.label ? item.provider?.label : item.provider?.name;
+        let provider_label = item.provider?.label ? item.provider.label : item.provider?.name;
         let provider_link = item.provider?.name ? `<a href="${item.provider.url}" target="_blank">${provider_label}</a>` : "";
         let provider = provider_link ? `
             <div class="provider">
                 ${provider_link}
                 ${item.provider.model ? ' with ' + item.provider.model : ''}
             </div>
         ` : "";
```

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.3/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.3/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/server/api.py` & `g4f-0.3.0.3/g4f/gui/server/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import json
 from typing import Iterator
 
 from g4f import version, models
 from g4f import get_last_provider, ChatCompletion
 from g4f.errors import VersionNotFoundError
+from g4f.image import ImagePreview
 from g4f.Provider import ProviderType, __providers__, __map__
 from g4f.providers.base_provider import ProviderModelMixin, FinishReason
 from g4f.providers.conversation import BaseConversation
 
 conversations: dict[dict[str, BaseConversation]] = {}
 
 class Api():
@@ -142,14 +143,16 @@
                     if provider not in conversations:
                         conversations[provider] = {}
                     conversations[provider][conversation_id] = chunk
                     yield self._format_json("conversation", conversation_id)
                 elif isinstance(chunk, Exception):
                     logging.exception(chunk)
                     yield self._format_json("message", get_error_message(chunk))
+                elif isinstance(chunk, ImagePreview):
+                    yield self._format_json("preview", chunk.to_string())
                 elif not isinstance(chunk, FinishReason):
                     yield self._format_json("content", str(chunk))
         except Exception as e:
             logging.exception(e)
             yield self._format_json('error', get_error_message(e))
 
     def _format_json(self, response_type: str, content):
```

### Comparing `g4f-0.3.0.2/g4f/gui/server/backend.py` & `g4f-0.3.0.3/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/server/config.py` & `g4f-0.3.0.3/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/server/internet.py` & `g4f-0.3.0.3/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/server/js_api.py` & `g4f-0.3.0.3/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/server/website.py` & `g4f-0.3.0.3/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/gui/webview.py` & `g4f-0.3.0.3/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/image.py` & `g4f-0.3.0.3/g4f/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,17 @@
     """
     if isinstance(images, str):
         result = f"[![{alt}]({preview.replace('{image}', images) if preview else images})]({images})"
     else:
         if not isinstance(preview, list):
             preview = [preview.replace('{image}', image) if preview else image for image in images]
         result = "\n".join(
-            f"[![#{idx+1} {alt}]({preview[idx]})]({image})" for idx, image in enumerate(images)
+            #f"[![#{idx+1} {alt}]({preview[idx]})]({image})"
+            f'[<img src="{preview[idx]}" width="200" alt="#{idx+1} {alt}">]({image})'
+            for idx, image in enumerate(images)
         )
     start_flag = "<!-- generated images start -->\n"
     end_flag = "<!-- generated images end -->\n"
     return f"\n{start_flag}{result}\n{end_flag}\n"
 
 def to_bytes(image: ImageType) -> bytes:
     """
@@ -255,14 +257,21 @@
 
     def get(self, key: str):
         return self.options.get(key)
 
     def get_list(self) -> list[str]:
         return [self.images] if isinstance(self.images, str) else self.images
 
+class ImagePreview(ImageResponse):
+    def __str__(self):
+        return ""
+
+    def to_string(self):
+        return super().__str__()
+
 class ImageRequest:
     def __init__(
         self,
         options: dict = {}
     ):
         self.options = options
```

### Comparing `g4f-0.3.0.2/g4f/local/__init__.py` & `g4f-0.3.0.3/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/locals/models.py` & `g4f-0.3.0.3/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/locals/provider.py` & `g4f-0.3.0.3/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/models.py` & `g4f-0.3.0.3/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/providers/base_provider.py` & `g4f-0.3.0.3/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/providers/create_images.py` & `g4f-0.3.0.3/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/providers/helper.py` & `g4f-0.3.0.3/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/providers/retry_provider.py` & `g4f-0.3.0.3/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/providers/types.py` & `g4f-0.3.0.3/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/requests/__init__.py` & `g4f-0.3.0.3/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/requests/aiohttp.py` & `g4f-0.3.0.3/g4f/requests/aiohttp.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,36 @@
 
 class StreamSession(ClientSession):
     def __init__(
         self,
         headers: dict = {},
         timeout: int = None,
         connector: BaseConnector = None,
+        proxy: str = None,
         proxies: dict = {},
         impersonate = None,
         **kwargs
     ):
         if impersonate:
             headers = {
                 **DEFAULT_HEADERS,
                 **headers
             }
         connect = None
         if isinstance(timeout, tuple):
             connect, timeout = timeout;
         if timeout is not None:
             timeout = ClientTimeout(timeout, connect)
+        if proxy is None:
+            proxy = proxies.get("all", proxies.get("https"))
         super().__init__(
             **kwargs,
             timeout=timeout,
             response_class=StreamResponse,
-            connector=get_connector(connector, proxies.get("all", proxies.get("https"))),
+            connector=get_connector(connector, proxy),
             headers=headers
         )
 
 def get_connector(connector: BaseConnector = None, proxy: str = None, rdns: bool = False) -> Optional[BaseConnector]:
     if proxy and not connector:
         try:
             from aiohttp_socks import ProxyConnector
```

### Comparing `g4f-0.3.0.2/g4f/requests/curl_cffi.py` & `g4f-0.3.0.3/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/requests/defaults.py` & `g4f-0.3.0.3/g4f/requests/defaults.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,31 @@
+try:
+    import brotli
+    has_brotli = True
+except ImportError:
+    has_brotli = False
+
 DEFAULT_HEADERS = {
-    "sec-ch-ua": '"Chromium";v="122", "Not(A:Brand";v="24", "Google Chrome";v="122"',
-    "sec-ch-ua-mobile": "?0",
-    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
-    "ec-ch-ua-arch": '"x86"',
-    "sec-ch-ua-full-version": '"122.0.6261.69"',
     "accept": "*/*",
-    "sec-ch-ua-platform-version:": '"6.5.0"',
-    "sec-ch-ua-full-version-list": '"Chromium";v="122.0.6261.69", "Not(A:Brand";v="24.0.0.0", "Google Chrome";v="122.0.6261.69"',
-    "sec-ch-ua-bitness": '"64"',
-    "sec-ch-ua-model": '""',
-    "sec-ch-ua-platform": '"Windows"',
-    "sec-fetch-site": "same-site",
-    "sec-fetch-mode": "cors",
-    "sec-fetch-dest": "empty",
-    "referer": "",
-    "accept-encoding": "gzip, deflate, br",
+    "accept-encoding": "gzip, deflate" + (", br" if has_brotli else ""),
     "accept-language": "en-US",
+    "referer": "",
+    "sec-ch-ua": "\"Google Chrome\";v=\"123\", \"Not:A-Brand\";v=\"8\", \"Chromium\";v=\"123\"",
+    "sec-ch-ua-arch": "\"x86\"",
+    "sec-ch-ua-bitness": "\"64\"",
+    "sec-ch-ua-full-version": "\"123.0.6312.122\"",
+    "sec-ch-ua-full-version-list": "\"Google Chrome\";v=\"123.0.6312.122\", \"Not:A-Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"123.0.6312.122\"",
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-model": "\"\"",
+    "sec-ch-ua-platform": "\"Windows\"",
+    "sec-ch-ua-platform-version": '"15.0.0"',
+    "sec-fetch-dest": "empty",
+    "sec-fetch-mode": "cors",
+    "sec-fetch-site": "same-origin",
+    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
 }
 WEBVIEW_HAEDERS = {
     "Accept": "*/*",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "",
     "Referer": "",
     "Sec-Fetch-Dest": "empty",
```

### Comparing `g4f-0.3.0.2/g4f/requests/raise_for_status.py` & `g4f-0.3.0.3/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/stubs.py` & `g4f-0.3.0.3/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/typing.py` & `g4f-0.3.0.3/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/version.py` & `g4f-0.3.0.3/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f/webdriver.py` & `g4f-0.3.0.3/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.3/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.2
+Version: 0.3.0.3
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.3 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.0.2/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.3/g4f.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 g4f/Provider/HuggingChat.py
 g4f/Provider/HuggingFace.py
 g4f/Provider/Koala.py
 g4f/Provider/Liaobots.py
 g4f/Provider/Llama.py
 g4f/Provider/Local.py
 g4f/Provider/MetaAI.py
+g4f/Provider/MetaAIAccount.py
 g4f/Provider/PerplexityLabs.py
 g4f/Provider/Pi.py
 g4f/Provider/ReplicateImage.py
 g4f/Provider/Vercel.py
 g4f/Provider/WhiteRabbitNeo.py
 g4f/Provider/You.py
 g4f/Provider/__init__.py
```

### Comparing `g4f-0.3.0.2/g4f.egg-info/requires.txt` & `g4f-0.3.0.3/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.2/setup.py` & `g4f-0.3.0.3/setup.py`

 * *Files identical despite different names*

