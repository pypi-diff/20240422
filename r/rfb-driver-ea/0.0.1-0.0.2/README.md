# Comparing `tmp/rfb-driver-ea-0.0.1.tar.gz` & `tmp/rfb_driver_ea-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb-driver-ea-0.0.1.tar", last modified: Thu Mar  7 08:29:35 2024, max compression
+gzip compressed data, was "rfb_driver_ea-0.0.2.tar", last modified: Mon Apr 22 07:19:44 2024, max compression
```

## Comparing `rfb-driver-ea-0.0.1.tar` & `rfb_driver_ea-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:29:35.802165 rfb-driver-ea-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-03-07 08:29:35.802165 rfb-driver-ea-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 08:29:35.802165 rfb-driver-ea-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:29:35.798164 rfb-driver-ea-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:29:35.798164 rfb-driver-ea-0.0.1/src/rfb_driver_ea/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 08:29:35.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-03-07 08:29:14.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea/drv_ea.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:29:35.802165 rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-03-07 08:29:35.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-07 08:29:35.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 08:29:35.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-07 08:29:35.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-07 08:29:35.000000 rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.644804 rfb_driver_ea-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-04-22 07:19:44.644804 rfb_driver_ea-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:19:44.644804 rfb_driver_ea-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.640804 rfb_driver_ea-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.640804 rfb_driver_ea-0.0.2/src/rfb_driver_ea/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-04-22 07:19:25.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea/drv_ea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:19:44.640804 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 07:19:44.000000 rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/top_level.txt
```

### Comparing `rfb-driver-ea-0.0.1/LICENSE.txt` & `rfb_driver_ea-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfb-driver-ea-0.0.1/PKG-INFO` & `rfb_driver_ea-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-driver-ea
-Version: 0.0.1
+Version: 0.0.2
 Summary: Driver to control EA Power Electronics devices.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Maintainer-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rfb-driver-ea-0.0.1/pyproject.toml` & `rfb_driver_ea-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rfb-driver-ea-0.0.1/src/rfb_driver_ea/context.py` & `rfb_driver_ea-0.0.2/src/rfb_driver_ea/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 from rfb_config_tool import sys_conf_update_config_params
 
 #######################          MODULE IMPORTS          #######################
 
 ######################             CONSTANTS              ######################
 # For further information check out README.md
 DEFAULT_MAX_MSG : int           = 100 # Max number of allowed message per chan
-DEFAULT_MAX_MESSAGE_SIZE : int  = 400 # Size of message sent through IPC message queue
+DEFAULT_MAX_MESSAGE_SIZE : int  = 550 # Size of message sent through IPC message queue
 DEFAULT_TX_CHAN : str           = 'TX_SCPI' #'TX_SCPI' # Name of the TX channel in CAN
-DEFAULT_RX_CHAN: str            = 'RX_SCPI_EA'  #Name of the RX channel for epc
-DEFAULT_MAX_READS: int = 10
+DEFAULT_RX_CHAN: str            = 'RX_SCPI'  #Name of the RX channel for epc
+DEFAULT_MAX_READS: int          = 10 # Number of maximum reads made when reading the queue
+DEFAULT_MAX_REQUESTS: int       = 10 # Number of requests made after sending again the message
 
 CONSTANTS_NAMES = ('DEFAULT_MAX_READS','DEFAULT_MAX_MSG', 'DEFAULT_MAX_MESSAGE_SIZE',
                    'DEFAULT_TX_CHAN', 'DEFAULT_RX_CHAN')
 sys_conf_update_config_params(context=globals(),
                               constants_names=CONSTANTS_NAMES)
```

### Comparing `rfb-driver-ea-0.0.1/src/rfb_driver_ea/drv_ea.py` & `rfb_driver_ea-0.0.2/src/rfb_driver_ea/drv_ea.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,33 +23,33 @@
 from rfb_scpi_sniffer import DrvScpiSerialConfC, DrvScpiCmdDataC, DrvScpiCmdTypeE
 from rfb_driver_bases import (DrvBaseStatusE, DrvBaseStatusC, DrvBasePwrModeE, DrvBasePwrDeviceC,
                                 DrvBasePwrPropertiesC, DrvBasePwrDataC)
 
 #######################          MODULE IMPORTS          #######################
 ######################             CONSTANTS              ######################
 from .context import (DEFAULT_TX_CHAN, DEFAULT_RX_CHAN, DEFAULT_MAX_MSG, DEFAULT_MAX_MESSAGE_SIZE,
-                      DEFAULT_MAX_READS)
+                      DEFAULT_MAX_READS, DEFAULT_MAX_REQUESTS)
 #######################              ENUMS               #######################
 _MILI_UNITS = 1000
 
-
 class _ScpiCmds(Enum):
     "Modes of the device"
     READ_INFO = '*IDN?'
     GET_MEAS  = 'MEASure:ARRay?'
     GET_OUTPUT = 'OUTPut?'
     CURR_NOM  = 'SYSTem:NOMinal:CURRent?'
     VOLT_NOM  = 'SYSTem:NOMinal:VOLTage?'
     POWER = 'SYSTem:NOMinal:POWer?'
     LOCK_ON = 'SYSTem:LOCK: ON'
     LOCK_OFF = 'SYSTem:LOCK: OFF'
     OUTPUT_ON = 'OUTPut: ON'
     OUTPUT_OFF = 'OUTPut: OFF'
     SEND_CURR = 'CURRent '
     SEND_VOLT = 'VOLTage '
+    CHECK_ERROR = ':SYST:ERR?'
 
 
 #######################             CLASSES              #######################
 class DrvEaPropertiesC(DrvBasePwrPropertiesC):
     "Properties of power supply device"
     def __init__(self, model: str, serial_number: int, max_volt_limit: int, \
                  max_current_limit: int, max_power_limit: int) -> None:
@@ -84,15 +84,15 @@
             - None.
         '''
         stat: DrvBaseStatusC = DrvBaseStatusC(status)
         super().__init__(status = stat, mode = mode, voltage = voltage,
                          current = current, power = power)
 
 
-class DrvEaDeviceC(DrvBasePwrDeviceC):
+class DrvEaDeviceC(DrvBasePwrDeviceC): #pylint: disable=too-many-instance-attributes
     "Principal class of ea power supply device"
     __instances = []
 
     def __change_last_mode(self, mode: DrvBasePwrModeE) -> None:
         ''' Change the last mode of the device.
         Args:
             - mode (DrvBasePwrModeE): Mode of the device.
@@ -121,14 +121,15 @@
         add_msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.ADD_DEV,
                                   port = config.port,
                                   payload = config,
                                   rx_chan_name = DEFAULT_RX_CHAN+'_'+config.port.split('/')[-1])
         self.__tx_chan.send_data(add_msg)
         self.__rx_chan.delete_until_last()
         self.__wait_4_response: bool = False
+        self.__request_data: int = 0
         self.__last_mode: DrvBasePwrModeE = DrvBasePwrModeE.DISABLE
         self.last_data: DrvEaDataC = DrvEaDataC(mode = DrvBasePwrModeE.DISABLE,
                                                 status = DrvBaseStatusE.OK,
                                                 current = 0, voltage = 0, power = 0)
 
         self.properties: DrvEaPropertiesC = DrvEaPropertiesC(model = None, serial_number = 0,
                                                                 max_volt_limit = 0,
@@ -160,21 +161,22 @@
         """
         i = 0
         while i < DEFAULT_MAX_READS and not self.__rx_chan.is_empty(): #pylint: disable=too-many-nested-blocks
             msg: DrvScpiCmdDataC = self.__rx_chan.receive_data_unblocking()
             if msg is not None and msg.data_type == DrvScpiCmdTypeE.RESP: #pylint: disable=too-many-nested-blocks
                 if hasattr(msg, 'status') and msg.status.value == DrvBaseStatusE.COMM_ERROR: #pylint: disable=attribute-defined-outside-init
                     log.critical("ERROR READING DEVICE")
-                    self.last_data.status = DrvBaseStatusE.COMM_ERROR #pylint: disable=attribute-defined-outside-init
+                    self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.COMM_ERROR) #pylint: disable=attribute-defined-outside-init
                 for data in msg.payload: #pylint: disable=too-many-nested-blocks #pylint: disable=attribute-defined-outside-init
                     if len(data) >0 and not str(data).startswith(":"):
                         if 'No error' in data:
-                            self.last_data.status = DrvBaseStatusE.OK #pylint: disable=attribute-defined-outside-init
+                            self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.OK) #pylint: disable=attribute-defined-outside-init
                         elif all (x in data for x in ("error", "Error", "ERROR")):
-                            self.last_data.status = DrvBaseStatusE.COMM_ERROR #pylint: disable=attribute-defined-outside-init
+                            log.error(f"Error reading device: {data}")
+                            self.last_data.status = DrvBaseStatusC(DrvBaseStatusE.COMM_ERROR) #pylint: disable=attribute-defined-outside-init
                         elif 'OFF' in data:
                             self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
                         elif ('ON' in data and self.last_data.mode in (DrvBasePwrModeE.WAIT,
                                                                     DrvBasePwrModeE.DISABLE)):
                             self.last_data.mode = self.__last_mode #pylint: disable=attribute-defined-outside-init
                         elif data.startswith('EA') or data.startswith('EPS'):
                             data = data.split(',')
@@ -278,37 +280,47 @@
             - None.
         Returns:
             - result (DrvEaDataC): Returns the device data.
         Raises:
             - None.
         '''
         log.debug("Get meas...")
+        if self.__request_data >= DEFAULT_MAX_REQUESTS:
+            self.__wait_4_response = False
+            self.__request_data = 0
+        self.__tx_chan.close()
+        self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         if not self.__wait_4_response:
             self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
                                 port = self.__port,
                                 payload = _ScpiCmds.GET_MEAS.value))
             self.__wait_4_response = True
+        else:
+            self.__request_data += 1
         self.read_buffer()
         return self.last_data
 
 
+
     def set_cc_mode(self, curr_ref: int, voltage_limit: int|None= None) -> None:
         '''
         Use source in constant current mode.
         Sink mode will be set with negative current values.
         Security voltage limit can be also set.
         Args:
             - curr_ref (int): current reference (mili Amps)
             - voltage_limit (int): voltage limit (milivolts)
                 if None, the maximum voltage limit will be used.
         Returns:
             - None
         Raises:
             - None
         '''
+        self.__tx_chan.close()
+        self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         curr_ref = abs(curr_ref)
         self.__change_last_mode(DrvBasePwrModeE.CC_MODE)
         current = round(float(curr_ref) / _MILI_UNITS, 2)
         current = min(self.properties.max_current_limit,current)
         if voltage_limit is None or voltage_limit > self.properties.max_volt_limit:
             voltage_limit = self.properties.max_volt_limit
         voltage = round(float(voltage_limit / _MILI_UNITS), 2)
@@ -356,14 +368,16 @@
             - current_limit (int): current limit (mili Amps),
                 if None the maximum current limit will be used.
         Returns:
             - None
         Raises:
             - None
         '''
+        self.__tx_chan.close()
+        self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         self.__change_last_mode(DrvBasePwrModeE.CV_MODE)
         voltage = round(float(volt_ref)/_MILI_UNITS, 2)
         current = round(float(current_limit/_MILI_UNITS), 2)
         #Check if the power limit is exceeded
         if self.properties.max_power_limit != 0:
             max_power_limit = self.properties.max_power_limit/_MILI_UNITS
             if voltage * current > max_power_limit:
@@ -402,15 +416,17 @@
         Args:
             - None
         Returns:
             - None
         Raises:
             - None 
         '''
-        log.critical("Disabling SOURCE...")
+        log.debug("Disabling SOURCE...")
+        self.__tx_chan.close()
+        self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         self.__change_last_mode(DrvBasePwrModeE.WAIT)
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
                                 port = self.__port,
                                 payload = _ScpiCmds.OUTPUT_OFF.value)
         self.__tx_chan.send_data(msg)
         self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
                                 port = self.__port,
@@ -421,15 +437,17 @@
         Args:
             - None
         Returns:
             - None
         Raises:
             - None 
         '''
-        log.critical("Disabling SOURCE...")
+        log.debug("Disabling SOURCE...")
+        self.__tx_chan.close()
+        self.__tx_chan = SysShdIpcChanC(name = DEFAULT_TX_CHAN)
         self.__change_last_mode(DrvBasePwrModeE.DISABLE)
         msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
                                 port = self.__port,
                                 payload = _ScpiCmds.OUTPUT_OFF.value)
         self.__tx_chan.send_data(msg)
         self.__tx_chan.send_data(DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE_READ,
                                 port = self.__port,
```

### Comparing `rfb-driver-ea-0.0.1/src/rfb_driver_ea.egg-info/PKG-INFO` & `rfb_driver_ea-0.0.2/src/rfb_driver_ea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-driver-ea
-Version: 0.0.1
+Version: 0.0.2
 Summary: Driver to control EA Power Electronics devices.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Maintainer-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

