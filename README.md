# - Bootlogos-SM8350-AC (2) -
> ⛔ : THIS PROJECT IS NOT FINISHED!!! (I think)
> 
> ⚠️ : If you are here just out of curiosity or you barely know how to install a ROM, you should not touch it.

This is the Bootlogos repository for the **Xpeng**, better known as **Moto G200 5G and Edge S30** phones. That's all I can describe for a README. Now, let's move on to the bootlogo previews of the ROMs.

| Murena (/e/OS) | Evolution X | LineageOS | LMODroid |
| --- | --- | --- | --- |
| ![logo](https://image2url.com/images/1765377043947-20ad6470-81b5-4c29-a36b-25030f0b030f.png) | ![logo](https://image2url.com/images/1765377080529-8653e91b-051e-4b8a-9c57-6ebbf429a3a0.png) | ![logo](https://image2url.com/images/1765377125086-7dec12cd-94f0-4720-87aa-f11037521048.png) | ![logo](https://image2url.com/images/1765377182841-41558492-2740-4789-8686-15dd687f8ee1.png) |

# - FAQ -
1. Why two repositories from the same family? (SM8350-AC)
**R**. The difference between the Edge 30 Fusion and the Moto G200/Edge S30 is that the Edge 30 Fusion is 60px larger; in other words, the Edge 30 Fusion has a resolution of 1080x2400, while the G200 has 1080x2460 (basically 60px larger).

2. Why does it have less bootlogo than repository Bootlogos-SM8350-AC.1?
**R**. Because these are the most official ROMs I've found, if you want to help me find more official or unofficial ROMs, contact me on Telegram. [Kultrinhaa_](t.me/KultrinhaaKKKK)

# - Requirements -
- Unlocked Bootloader
- Root (For mobile method)
- PC or OTG with other phone (Use Bugjaeger)
- Android Platform Tools (with installed Motorola USB driver on Windows)

# - How to flash? (PC Method) -
1. Reboot the phone to fastboot/bootloader mode
2. Insert command to flash bootlogo
```bash
fastboot flash logo <path/to/logo.bin>
```
3. Reboot the phone

# - How to flash? (Mobile Method) -
1. Download and install the ReTermimal
[Download Here](https://github.com/RohitKushvaha01/ReTerminal/releases) - Credits to [RohitKushvaha01](https://github.com/RohitKushvaha01)
3. Open it until you reach this screen:
<img width="400" alt="Screenshot_20251201-041431_ReTerminal" src="https://github.com/user-attachments/assets/bbb805c9-8b86-47e3-bbd0-975322c381a6" />

4. Click on "+" and then "Android"
<img width="400" alt="Screenshot_20251201-041437_ReTerminal" src="https://github.com/user-attachments/assets/d92f2a15-023a-4ab0-b178-3e3ef9e537ac" />

5. Insert command
```bash
su
```
> (Note: if you are in Magisk, it will ask you on your screen, but if you are in APatch/KernelSU, you have to open the root manager, superuser and activate ReTerminal for the super user to be active)

5. Enter the directory where the downloaded logo.bin is located, using cd
 ```bash
cd <path/to/directory>
```
> For example, if your downloaded logo.bin is in the "Download" folder of the internal storage, enter the command
```bash
cd /storage/emulated/0/Download
```
6. Insert command to flash a bootlogo
```bash
dd if=<logo>.bin of=/dev/block/by-name/logo_<current slot> bs=16777216
```
7. Reboot the phone and you will see the new bootlogo!