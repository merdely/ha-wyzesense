## Changelog

### 0.0.19 - Revert to 0.0.13

### 0.0.18 - Undo two previous changes

### 0.0.17 - Fix string concatenation bug with alarm_data

### 0.0.16 - Fix string concatenation bug

### 0.0.15 - Fix breakage accidentially changing wyzesense requirement

### 0.0.14 - Bring in some changes from wyzesense2mqtt
https://github.com/raetha/wyzesense2mqtt

### 0.0.13 - Add stability change
from https://github.com/kevinvincent/ha-wyzesense/issues/189

### 0.0.12 - Move from property device_state_attributes to extra_state_attributes
property device_state_attributes is deprecated

### 0.0.9 - More stability fixes
Prevents wyzesense from stopping when receiving an unparseable packet. Should help with stability issues.
Thanks to @raetha for the fix.

### 0.0.7 - Major Stability and Error fix
**WHEN UPGRADING TO THIS VERSION YOU WILL HAVE TO RETRIGGER EACH SENSOR TO HAVE IT DISPLAY AGAIN**

This is a one time thing you have to do once updating and restarting HomeAssistant. Once you do this, stability on restarts should improve dramatically. This specifically solves any errors that contain `result = ws.List()` in the error message. This is the vast majority of errors reported.
