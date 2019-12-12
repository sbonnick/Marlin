
## Prereqs
1. Install platform.io on VS Code
2. Plug board into USB and power on

## Build and Upload
1. Under platform IO project tasks
    1. Build
    2. Upload

## After uploading firmware
1. Control => Restore failsafe
2. *Install Z Probe*
3. Prepare => Delta Calibration => Auto Calibration
4. Prepare => Level Bed
5. Prepare => Delta Calibration => Set Delta Height
6. *Remove Z Probe*
7. Control => Temperature => PID Autotune: 200
8. *wait for it to heat up and then start to cool down*
8. Control => Store settings
9. Check if Z=0 is the right height(Use a piece of paper or two). If not, modify Z-offeset(This will not change Delta Height) and do "Set Delta Height"(This changes Delta Height) again.


*All operations above can be executed by lcd menu.*
*DO NOT USE THE "PROBE Z OFFSET" IN LCD MENU (1.1.9). IT'S FOR PROBE LIKE INDUCTIVE SENSOR*
