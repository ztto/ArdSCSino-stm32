# ArdSCSino-stm32

ArdSCSino-stm32 is the STM32 version of ArdSCSino.
ArdSxSino is hardware that replicates SCSI storage devices using Arduino.

SASI Support for Sharp X68000
Note 1: It works with ACE and EXPERT, but there are issues with PRO, such as DSKBENCH not exiting properly.
Note 2: Operation confirmation has not been performed on SHARP X1turbo, NEC PC98.

You can now describe various parameters in the "scsi-config.txt" file.
Sample is provided.

SCSI Description format:
Column 1: Vendor Name (8 characters)
Column 2: Product Name (16 characters)
Column 3: Version (4 characters)
Column 4: Type (1 character) <0 for STANDARD, 1 for SHARP X1turbo>
Column 5: WAIT time (3 characters) <For SASI, set a value around 80 to prevent abnormal termination>

Example: Please consider '.' as a half-width space<br>
--------------<br>
NECGATE･<br>
ST410800N･･･････<br>
1.0･<br>
0<br>
000<br>
--------------<br>

# Setup<br>
Using platformio.
Using the following as a MicroSDCARD adapter:
<br>
Hirose DM3AT-SF-PEJM5<br>

