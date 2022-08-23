---
title: lolMiner
minVer: 1.12
releases: https://github.com/Lolliedieb/lolMiner-releases/releases
---

```
#!/bin/bash

#################################
## Begin of user-editable part ##
#################################

POOL=STRATUM_HOST
# Address to send funds to. Change this address to yours!
WALLET=0x99CFa888E8e4EC8e6C4CE9E4fD2a8cBD30b841d9

#################################
##  End of user-editable part  ##
#################################

cd "$(dirname "$0")"

./lolMiner -c OCTA --pool $POOL --user $WALLET --ethstratum=ETHPROXY $@
```