# Risorse

- [GALAsm](https://github.com/daveho/GALasm)
- [Lattice ispGAL & ispLSI](https://www.ythiee.com/2023/01/08/lattice-ispgal-isplsi/)
- [GAL specific information](https://www.ythiee.com/2021/06/06/gal-specific-information/)
- [PLD Compilers](https://www.ythiee.com/2021/06/06/pld-compilers/)

- [VirtualBox](https://www.virtualbox.org/)
- [Windows XP Professional SP3](https://archive.org/details/WinXPProSP3x86)
- [Windows XP Product Key](https://github.com/Fuwn/xp)



## Alcuni articoli interessanti:
- [KIM-64](https://www.ythiee.com/2025/01/05/kim-64/)
- [GAL22V10](https://www.ythiee.com/tag/gal22v10/)

# High Performance E2CMOS PLD Generic Array Logic™

- [GAL26V12C](https://github.com/LucaEstiva/Hobby_8088_PC/blob/main/GAL/26CV12.PDF)

- [GAL20RA10](https://github.com/LucaEstiva/Hobby_8088_PC/blob/main/GAL/GAL20RA10.PDF)

## Alcune peculiarità del chip GAL 20RA10

- Reset Asincrono indipendente per ogni Flip Flop:

Each GAL20RA10 macrocell has an independent asynchronous\
reset and preset control product term. The reset and preset product\
terms are level sensitive, and will hold the flip-flop in the reset or\
preset state while the product term is active independent of the clock\
or D-inputs. It should be noted that the reset and preset term alter\
the state of the flip-flop whose output is inverted by the output\
buffer. A reset of the flip-flop will result in the output pin becoming\
a logic high and a preset will result in a logic low.\

- Sogenti clock indipenti:

An independent clock control product term is provided for each\
GAL20RA10 macrocell. Data is clocked into the flip-flop on the\
active edge of the clock product term. The use of individual clock\
control product terms allow up to ten separate clocks. These clocks\
can be derived from any pin or combination of pins and/or feedback\
from other flip-flops. Multiple clock sources allow a number of\
asynchronous register functions to be combined into a single\
GAL20RA10. This allows the designer to combine discrete logic\
functions into a single device.\

# ABEL
ABEL (Advanced Boolean Expression Language)\
Può essere utilizzato su macchina virtuale con Windows XP.
E' possibile scaricare ABEL direttamente da questo repository.

- Utilizzare ABEL GUI:

![alt text](https://github.com/LucaEstiva/Hobby_8088_PC/blob/main/Images/ABEL/VirtualBox_Win_XP_ABEL_1.png?raw=true "ABEL ON XP")

Per generare il file jed, sarà necessario eseguire gli step:

![alt text](https://github.com/LucaEstiva/Hobby_8088_PC/blob/main/Images/ABEL/VirtualBox_Win_XP_ABEL_2.png?raw=true "ABEL COMPILE")

- Compile
- Optimize
- Fit
- FPGA/PLDmap

Per utilizzare ABEL utlizzando la riga di comando dal prompt di MS-Dos sarà necessario aggiungere al path i seguenti percorsi ( Pannello di controllo - Sistema - Avanzate - Variabili ambiente )\

- ahdl2pla

![alt text](https://github.com/LucaEstiva/Hobby_8088_PC/blob/main/Images/ABEL/VirtualBox_Win_XP_ABEL.png?raw=true "ABEL ON XP")

set ABELDEV=D:\ABEL\LIB4\
set PATH=%PATH%;D:\ABEL\

ovvero aggiungere al path ( Se ABEL si trova, ad esempio nella root del disco C il path sarà C:\ABEL ):\
C:\ABEL;C:\ABEL\LIB4

Quindi sarà possibile compilare un progamma:

- ahdl2pla "pathtoablfile.abl"

Aprire "editare" il file RUNME.bat ( usando un editor di testo ad esempio Notepad++, Blocco Note, Visual studio Code o altro... ) che si trova nella cartella ABEL per verificare i valori del parametri set.
