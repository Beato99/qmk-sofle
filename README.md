# Default QMK firmware for ErgoFrets Sofle Keyboard

Download QMK software using the source code: https://docs.qmk.fm/#/newbs  
Alternatively, install the  WSL version for Windows: https://wsl.qmk.fm/

Make the changes you'd like to the keyboard and compile it using  
```qmk compile -kb <keyboard> -km <keymap>```  
Use QMK toolbox to easily load the firmware onto the microcontroller

*If the microcontroller is RP2040 based, add the following parameter  
```qmk compile -kb <keyboard> -km <keymap> -e CONVERT_TO=promicro_rp2040```  
Then drag and drop the .uf2 file directly to the microcontroller massive storage unit that appears when putting it into boot mode

