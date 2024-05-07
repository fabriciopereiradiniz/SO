#### _Read this in other languages_

<kbd>[<img title="English" alt="English" src="https://i.imgur.com/K0sBZSD.png" width="22">](README.md)</kbd>
<kbd>[<img title="Portuguese" alt="Brazillian portuguese" src="https://i.imgur.com/MZMUUJ6.png" width="22">](translations/README-PTBR.md)</kbd>

<p align="center">
  <img src="https://i.imgur.com/xnhjM7o.gif" alt="OS" />
</p>

_TripOS is a basic operating system developed using assembly language for the Operating Systems course. Its development was made possible thanks to the [KiddieOS Tutorial](https://www.youtube.com/watch?v=Jws7BHrts6g&list=PLsoiO2Be-2z8BfsSkspJfDiuKeC9-LSca&index=2) channel.
To execute TripOS, you need several tools: NASM for converting .asm files to .bin, FergoRaw for manipulating binary files into .img format (with a note to update the necessary DLLs), and Rufus or another ISO builder to convert .img files to .iso format._

## OS Execution

To execute tripOS you need this:
- NASM to convert `.asm` to `.bin`
- FergoRaw to manipulate binary files into `.img` (update your dlls! -> "MSCOMCTL.OCX")
- Rufus or other iso builder to convert `.img` to `.iso` 
<br>

`/Assembler.bat/` use nasm for file conversion;
`/binary/` nasm converted files;
`/Hardware/` assembly libraries.
<details>
<summary>Need some help?</summary>
<tr>
  <td>Link to NASM: <a href="https://www.nasm.us/index.php"><img alt="NASM" src="https://www.nasm.us/images/nasm.png" width="25"></a></td>
  <td>Link to RUFUS: <a href="https://rufus.ie/pt_BR/"><img alt="Rufus" src="https://rufus.ie/pics/rufus-128.png" width="25"></a></td>
  <td>Link to FERGORAW: <a href="https://www.fergonez.net/softwares/fraw"><img alt="Fergoraw" src="https://images.gofreedownload.net/hardware-floppy-34989.jpg" width="25"></a></td>
</tr>
</details>
<div align="right">
  <img src="https://i.imgur.com/9f0AnpO.gif" alt="window" width="150">
</div>

## Implementações atuais

- Main Window <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>
- Graphic Interface (border) <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>
- Graphic Interface (borderless) <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>
- Monitor/wmemory lib's <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>

### How to install and configure your VM

Open your VM.

Press CRTL + N.

CHOOSE YOUR VM NAME/FOLDERS.

<p align="center">
  <img src="https://i.imgur.com/19b1kej.png" alt="OS" />
</p>

CHANGE THE VALUES IF NEEDED

CHOOSE: "use an existing virtual hard disk file", AND USE THE o `usb.vmdk`.

<p align="center">
  <img src="https://i.imgur.com/gklLM5i.png" alt="OS" />
</p>

### Classes 

### 01
In the first class, we began by downloading NASM, Fergo Raw, and Rufus 3.9. Then, we installed NASM, initiated Rufus 3.9, and extracted the Fergo Raw zip file. However, we encountered an issue when trying to open the extracted file due to a missing or invalid component, "MSCOMCTL.OCX". Although a solution using a virtual machine was suggested, it remains unresolved. After resolving this issue in the future, we configured environment variables, organized OS files into directories, created a BAT file using Notepad++, and learned to assemble .ASM files with NASM.

### 02
In the second class, we solved the initial issue with Fergo Raw by installing a missing library and activating an ActiveX control. Subsequently, we encountered a new error related to "COMDLG32.OCX", which was resolved similarly to the previous issue. Both solutions involved installing necessary files and registering them using specific commands.

### 03
In the third class, we continued by installing compatible versions of Rufus and VirtualBox, configuring the virtual machine to recognize the USB drive, creating an initial boot.asm code, and using FergoRaw to create a bootable image file named System. Finally, we used Rufus to transfer this image to the USB drive. The process involved creating a virtual machine in VirtualBox with specific settings and executing the bootable image, resulting in the display of "Hello World" messages.
