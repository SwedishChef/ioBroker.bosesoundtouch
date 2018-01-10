# ioBroker.bosesoundtouch ![Logo](admin/bosesoundtouch.png) 

Bose SoundTouch adapter for ioBroker IoT platform

## Usage
The following objects can be written:

| State          | Description |
| :---           | :---        |
| key            | One of the following keys to send: <br><br> PLAY <br> PAUSE <br> STOP <br> PREV_TRACK <br> NEXT_TRACK <br> THUMBS_UP <br> THUMBS_DOWN <br> BOOKMARK <br> POWER <br> MUTE <br> VOLUME_UP <br> VOLUME_DOWN <br> PRESET_1 <br> PRESET_2 <br> PRESET_3 <br> PRESET_4  <br> PRESET_5 <br> PRESET_6 <br> AUX_INPUT <br> SHUFFLE_OFF <br> SHUFFLE_ON <br> REPEAT_OFF <br> REPEAT_ONE <br> REPEAT_ALL <br> PLAY_PAUSE <br> ADD_FAVORITE <br> REMOVE_FAVORITE <br> INVALID_KEY |
| muted          | Mute or unmute the device. |
| on             | Power on or off the device. |
| playEverywhere | Define speaker as zone master and play its content on all other speakers. |
| volume         | Change device volume between 0 and 100. |

## changelog
### 0.1.5 (06.01.2018)
* added 'TUNEIN' to now playing info
* state playEverywhere falls back to false after activation
* admin/bose.png renamed to admin/bosesoundtouch.png to be shown corretly in adapter list
* added short adapter description in io-package.json

### 0.1.4 (30.12.2017)
* playEverywhere: support multi room (zones) to define one speaker as master for all others

### 0.1.3 (22.12.2017)
* revert last change

### 0.1.2 (22.12.2017)
* fixed typo in package.json

### 0.1.1 (20.12.2017)
* now playing: added state 'art' (URL to cover image if available)
* merged pull request from Apollon77 (basic config files for testing)
* renamed repository to 'ioBroker.bosesoundtouch'

### 0.1.0 (26.11.2017)
* objectChange/stateChange: log level 'debug'
* added 'STORED_MUSIC' to now playing info.

### 0.0.9 (22.11.2017)
* Merge pull request #1 from Apollon77/master: Add testing and fix things...

### 0.0.8 (19.11.2017)
* send value to correct instance when having multiple adapters installed
* first version of README.md

### 0.0.7 (09.11.2017)
* fixed logging in soundtouchsocket.js

### 0.0.6 (09.11.2017)
* renamed main.js to bosesoundtouch.js
* line ending: LF
* strings: single quote

### 0.0.5 and earlier (01.11.2017)
* Initial versions
