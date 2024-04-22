# Comparing `tmp/ValWrap-0.8.1.tar.gz` & `tmp/ValWrap-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValWrap-0.8.1.tar", last modified: Thu Jan 11 20:09:42 2024, max compression
+gzip compressed data, was "ValWrap-0.9.1.tar", last modified: Mon Feb  5 00:52:11 2024, max compression
```

## Comparing `ValWrap-0.8.1.tar` & `ValWrap-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:09:42.824908 ValWrap-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-11 20:09:42.824908 ValWrap-0.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:09:42.824908 ValWrap-0.8.1/ValWrap/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-11 20:09:28.000000 ValWrap-0.8.1/ValWrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43685 2024-01-11 20:09:28.000000 ValWrap-0.8.1/ValWrap/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:09:42.824908 ValWrap-0.8.1/ValWrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-11 20:09:42.000000 ValWrap-0.8.1/ValWrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-11 20:09:42.000000 ValWrap-0.8.1/ValWrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:09:42.000000 ValWrap-0.8.1/ValWrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-11 20:09:42.000000 ValWrap-0.8.1/ValWrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-11 20:09:42.000000 ValWrap-0.8.1/ValWrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-11 20:09:28.000000 ValWrap-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 20:09:42.824908 ValWrap-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 00:52:11.922935 ValWrap-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-05 00:52:11.922935 ValWrap-0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 00:52:11.918935 ValWrap-0.9.1/ValWrap/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 00:52:01.000000 ValWrap-0.9.1/ValWrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46001 2024-02-05 00:52:02.000000 ValWrap-0.9.1/ValWrap/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 00:52:11.922935 ValWrap-0.9.1/ValWrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-05 00:52:11.000000 ValWrap-0.9.1/ValWrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-05 00:52:11.000000 ValWrap-0.9.1/ValWrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 00:52:11.000000 ValWrap-0.9.1/ValWrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 00:52:11.000000 ValWrap-0.9.1/ValWrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 00:52:11.000000 ValWrap-0.9.1/ValWrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-05 00:52:02.000000 ValWrap-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 00:52:11.922935 ValWrap-0.9.1/setup.cfg
```

### Comparing `ValWrap-0.8.1/ValWrap/requests.py` & `ValWrap-0.9.1/ValWrap/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import List, Any, TypedDict
+from typing import List, TypedDict, Any
 from typing_extensions import NotRequired
 
 class All(TypedDict):
     AccountXP: AccountXPType
     ActivateContract: ActivateContractType
     ChangeQueue: ChangeQueueType
     ChangeQueueBody: ChangeQueueBodyType
@@ -24,15 +24,18 @@
     MatchHistory: MatchHistoryType
     NameService: List[NameServiceType]
     NameServiceBody: List[str]
     OwnedItems: OwnedItemsType
     Party: PartyType
     PartyChatToken: PartyChatTokenType
     PartyDecline: PartyDeclineType
+    PartyDisableCode: PartyDisableCodeType
+    PartyGenerateCode: PartyGenerateCodeType
     PartyInvite: PartyInviteType
+    PartyJoinByCode: PartyJoinByCodeType
     PartyPlayer: PartyPlayerType
     PartySetMemberReady: PartySetMemberReadyType
     PartySetMemberReadyBody: PartySetMemberReadyBodyType
     PartyVoiceToken: PartyVoiceTokenType
     Penalties: PenaltiesType
     PlayerLoadout: PlayerLoadoutType
     PlayerMMR: PlayerMMRType
@@ -268,18 +271,18 @@
 
 class AesselectionsType(TypedDict):
     AssetID: str
     SocketID: str
     TypeID: str
 
 class SpraysType(TypedDict):
+    SpraySelections: NotRequired[List[SpraySelectionsType]]
     EquipSlotID: NotRequired[str]
     SprayID: NotRequired[str]
     SprayLevelID: NotRequired[None]
-    SpraySelections: NotRequired[List[SpraySelectionsType]]
 
 class SpraySelectionsType(TypedDict):
     LevelID: str
     SocketID: str
     SprayID: str
 
 class CurrentGameMatchType(TypedDict):
@@ -305,36 +308,33 @@
     GameServerHost: str
     GameServerHosts: List[str]
     GameServerObfuscatedIP: float
     GameServerPort: float
     PlayerKey: str
 
 class PlayersType(TypedDict):
-    CharacterID: NotRequired[str]
-    CharacterSelectionState: NotRequired[str]
-    CompetitiveTier: NotRequired[float]
-    IsCaptain: NotRequired[bool]
-    PlayerIdentity: NotRequired[PlayerIdentityType]
-    PregamePlayerState: NotRequired[str]
-    SeasonalBadgeInfo: NotRequired[SeasonalBadgeInfoType]
-    Subject: NotRequired[str]
     IsAnonymized: NotRequired[bool]
     IsBanned: NotRequired[bool]
     PlayerCardID: NotRequired[str]
     TitleID: NotRequired[str]
     competitiveTier: NotRequired[float]
     gameName: NotRequired[str]
     leaderboardRank: NotRequired[float]
     numberOfWins: NotRequired[float]
     puuid: NotRequired[str]
     rankedRating: NotRequired[float]
     tagLine: NotRequired[str]
-    IsAssociated: NotRequired[bool]
-    IsCoach: NotRequired[bool]
-    TeamID: NotRequired[Any]
+    CharacterID: NotRequired[str]
+    CharacterSelectionState: NotRequired[str]
+    CompetitiveTier: NotRequired[float]
+    IsCaptain: NotRequired[bool]
+    PlayerIdentity: NotRequired[PlayerIdentityType]
+    PregamePlayerState: NotRequired[str]
+    SeasonalBadgeInfo: NotRequired[SeasonalBadgeInfoType]
+    Subject: NotRequired[str]
     accountLevel: NotRequired[float]
     behaviorFactors: NotRequired[BehaviorFactorsType]
     characterId: NotRequired[str]
     isObserver: NotRequired[bool]
     newPlayerExperienceDetails: NotRequired[NewPlayerExperienceDetailsType]
     partyId: NotRequired[str]
     platformInfo: NotRequired[PlatformInfoType]
@@ -343,14 +343,17 @@
     preferredLevelBorder: NotRequired[Any]
     roundDamage: NotRequired[Any]
     sessionPlaytimeMinutes: NotRequired[Any]
     stats: NotRequired[Any]
     subject: NotRequired[str]
     teamId: NotRequired[Any]
     xpModifications: NotRequired[List[XpModificationsType]]
+    IsAssociated: NotRequired[bool]
+    IsCoach: NotRequired[bool]
+    TeamID: NotRequired[Any]
 
 class SeasonalBadgeInfoType(TypedDict):
     LeaderboardRank: float
     NumberOfWins: float
     Rank: float
     SeasonID: Any
     WinsByTier: None
@@ -719,14 +722,62 @@
     RestrictedSeconds: float
     State: str
     StateTransitionReason: str
     Version: float
     VoiceRoomID: str
     XPBonuses: List[Any]
 
+class PartyDisableCodeType(TypedDict):
+    Accessibility: str
+    CheatData: CheatDataType
+    ClientVersion: str
+    CustomGameData: CustomGameDataType
+    EligibleQueues: List[str]
+    ErrorNotification: ErrorNotificationType
+    ID: str
+    InviteCode: str
+    Invites: None
+    MUCName: str
+    MatchmakingData: MatchmakingDataType
+    Members: List[MembersType]
+    PreviousState: str
+    QueueEntryTime: str
+    QueueIneligibilities: List[str]
+    Requests: List[Any]
+    RestrictedSeconds: float
+    State: str
+    StateTransitionReason: str
+    Version: float
+    VoiceRoomID: str
+    XPBonuses: List[Any]
+
+class PartyGenerateCodeType(TypedDict):
+    Accessibility: str
+    CheatData: CheatDataType
+    ClientVersion: str
+    CustomGameData: CustomGameDataType
+    EligibleQueues: List[str]
+    ErrorNotification: ErrorNotificationType
+    ID: str
+    InviteCode: str
+    Invites: None
+    MUCName: str
+    MatchmakingData: MatchmakingDataType
+    Members: List[MembersType]
+    PreviousState: str
+    QueueEntryTime: str
+    QueueIneligibilities: List[str]
+    Requests: List[Any]
+    RestrictedSeconds: float
+    State: str
+    StateTransitionReason: str
+    Version: float
+    VoiceRoomID: str
+    XPBonuses: List[Any]
+
 class PartyInviteType(TypedDict):
     Accessibility: str
     CheatData: CheatDataType
     ClientVersion: str
     CustomGameData: CustomGameDataType
     EligibleQueues: List[str]
     ErrorNotification: ErrorNotificationType
@@ -743,15 +794,15 @@
     RestrictedSeconds: float
     State: str
     StateTransitionReason: str
     Version: float
     VoiceRoomID: str
     XPBonuses: List[Any]
 
-class PartyPlayerType(TypedDict):
+class PartyJoinByCodeType(TypedDict):
     CurrentPartyID: str
     Invites: None
     PlatformInfo: PlatformInfoType
     Requests: List[RequestsType]
     Subject: str
     Version: float
 
@@ -760,14 +811,22 @@
     ExpiresIn: float
     ID: str
     PartyID: str
     RefreshedAt: str
     RequestedBySubject: str
     Subjects: List[str]
 
+class PartyPlayerType(TypedDict):
+    CurrentPartyID: str
+    Invites: None
+    PlatformInfo: PlatformInfoType
+    Requests: List[RequestsType]
+    Subject: str
+    Version: float
+
 class PartySetMemberReadyType(TypedDict):
     Accessibility: str
     CheatData: CheatDataType
     ClientVersion: str
     CustomGameData: CustomGameDataType
     EligibleQueues: List[str]
     ErrorNotification: ErrorNotificationType
@@ -1373,14 +1432,29 @@
 	return res
 
 def get_party_voice_token(auth: ExtraAuth, party_id: str) -> PartyVoiceTokenType:
 	api_url = f"https://glz-{auth.region}-1.{auth.shard}.a.pvp.net//parties/v1/parties/{party_id}/voicetoken"
 	res = get(api_url, auth)
 	return res
 
+def delete_party_disable_code(auth: ExtraAuth, party_id: str) -> PartyDisableCodeType:
+	api_url = f"https://glz-{auth.region}-1.{auth.shard}.a.pvp.net/parties/v1/parties/{party_id}/invitecode"
+	res = delete(api_url, auth)
+	return res
+
+def post_party_generate_code(auth: ExtraAuth, party_id: str) -> PartyGenerateCodeType:
+	api_url = f"https://glz-{auth.region}-1.{auth.shard}.a.pvp.net/parties/v1/parties/{party_id}/invitecode"
+	res = post(api_url, auth)
+	return res
+
+def post_party_join_by_code(auth: ExtraAuth, code: str) -> PartyJoinByCodeType:
+	api_url = f"https://glz-{auth.region}-1.{auth.shard}.a.pvp.net/parties/v1/players/joinbycode/{code}"
+	res = post(api_url, auth)
+	return res
+
 def get_prices(auth: ExtraAuth) -> PricesType:
 	api_url = f"https://pd.{auth.shard}.a.pvp.net/store/v1/offers"
 	res = get(api_url, auth)
 	return res
 
 def get_storefront(auth: ExtraAuth, puuid: Optional[str] = None) -> StorefrontType:
 	api_url = f"https://pd.{auth.shard}.a.pvp.net/store/v2/storefront/{puuid or auth.user_id}"
@@ -1473,8 +1547,8 @@
 	return res
 
 def get_riot_client_config(auth: Auth) -> Any:
 	api_url = "https://clientconfig.rpg.riotgames.com/api/v1/config/player?app=Riot%20Client"
 	res = get(api_url, auth)
 	return res
 
-__all__ = ["get_fetch_content","get_account_xp","get_player_loadout","put_set_player_loadout","get_player_mmr","get_match_history","get_match_details","get_competitive_updates","get_leaderboard","get_penalties","put_name_service","get_party","get_party_player","delete_party_remove_player","post_party_set_member_ready","post_refresh_competitive_tier","post_refresh_player_identity","post_refresh_pings","post_change_queue","post_start_custom_game","post_enter_matchmaking_queue","post_leave_matchmaking_queue","post_set_party_accessibility","post_set_custom_game_settings","post_party_invite","post_party_request","post_party_decline","get_custom_game_configs","get_party_chat_token","get_party_voice_token","get_prices","get_storefront","get_wallet","get_owned_items","get_pregame_player","get_pregame_match","get_pregame_loadouts","post_select_character","post_lock_character","post_pregame_quit","get_current_game_player","get_current_game_match","get_current_game_loadouts","post_current_game_quit","get_item_upgrades","get_contracts","post_activate_contract","put_riot_geo","get_pas_token","get_riot_client_config"]
+__all__ = ["get_fetch_content","get_account_xp","get_player_loadout","put_set_player_loadout","get_player_mmr","get_match_history","get_match_details","get_competitive_updates","get_leaderboard","get_penalties","put_name_service","get_party","get_party_player","delete_party_remove_player","post_party_set_member_ready","post_refresh_competitive_tier","post_refresh_player_identity","post_refresh_pings","post_change_queue","post_start_custom_game","post_enter_matchmaking_queue","post_leave_matchmaking_queue","post_set_party_accessibility","post_set_custom_game_settings","post_party_invite","post_party_request","post_party_decline","get_custom_game_configs","get_party_chat_token","get_party_voice_token","delete_party_disable_code","post_party_generate_code","post_party_join_by_code","get_prices","get_storefront","get_wallet","get_owned_items","get_pregame_player","get_pregame_match","get_pregame_loadouts","post_select_character","post_lock_character","post_pregame_quit","get_current_game_player","get_current_game_match","get_current_game_loadouts","post_current_game_quit","get_item_upgrades","get_contracts","post_activate_contract","put_riot_geo","get_pas_token","get_riot_client_config"]
```

