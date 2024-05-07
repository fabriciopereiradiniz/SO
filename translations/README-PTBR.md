#### _Leia em outras línguas_

<kbd>[<img title="Inglês" alt="Inglês" src="https://i.imgur.com/K0sBZSD.png" width="22">](/README.md)</kbd>
<kbd>[<img title="Português" alt="Português brasileiro" src="https://i.imgur.com/MZMUUJ6.png" width="22">](README-PTBR.md)</kbd>

<p align="center">
  <img src="https://i.imgur.com/xnhjM7o.gif" alt="OS" />
</p>

_TripOS é um sistema operacional basico desenvolvido utilizando assembly para a matéria de sistemas operacionais, o desenvolvimento do mesmo só foi possível graças ao canal [Tutorial KiddieOS](https://www.youtube.com/watch?v=Jws7BHrts6g&list=PLsoiO2Be-2z8BfsSkspJfDiuKeC9-LSca&index=2)._

## Execução do SO

Para execução do tripOS será necessário os seguintes itens:
- NASM para conversão do `.asm` para `.bin`
- FergoRaw utilizado para inserir os arquivos binários em diferentes partições realizando a conversão para `.img`
- Rufus ou outro builder de `.img` para `.iso` de sua preferência
<br>

`/Assembler.bat/` utiliza o nasm para a conversão;
`/binary/` contém os arquivos convertidos pelo nasm;
`/Hardware/` contém as bibliotecas.
<details>
<summary>Precisa de ajuda com links?</summary>
<tr>
  <td>Link para NASM: <a href="https://www.nasm.us/index.php"><img alt="NASM" src="https://www.nasm.us/images/nasm.png" width="25"></a></td>
  <td>Link para RUFUS: <a href="https://rufus.ie/pt_BR/"><img alt="Rufus" src="https://rufus.ie/pics/rufus-128.png" width="25"></a></td>
  <td>Link para FERGORAW: <a href="https://www.fergonez.net/softwares/fraw"><img alt="Fergoraw" src="https://images.gofreedownload.net/hardware-floppy-34989.jpg" width="25"></a></td>
</tr>
</details>
<div align="right">
  <img src="https://i.imgur.com/9f0AnpO.gif" alt="window" width="150">
</div>

## Implementações atuais

- Tela inicial <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>
- Interface gráfica com borda <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>
- Interface gráfica borderless window <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>
- Libs para monitor/wmemory <a><img alt="checked" src="https://cdn3.emoji.gg/emojis/4562_AlienPls.gif" width="12"></a>

### 01
Na primeira aula, começamos baixando NASM, Fergo Raw e Rufus 3.9. Em seguida, instalamos o NASM, iniciamos o Rufus 3.9 e extraímos o arquivo zip do Fergo Raw. No entanto, encontramos um problema ao tentar abrir o arquivo extraído devido a um componente ausente ou inválido, "MSCOMCTL.OCX". Embora uma solução usando uma máquina virtual tenha sido sugerida, ela permanece sem solução. Após resolvermos esse problema no futuro, configuramos as variáveis de ambiente, organizamos os arquivos do sistema operacional em diretórios, criamos um arquivo BAT usando o Notepad++ e aprendemos a montar arquivos .ASM com o NASM.

### 02
Na segunda aula, resolvemos o problema inicial com o Fergo Raw instalando uma biblioteca ausente e ativando um controle ActiveX. Posteriormente, encontramos um novo erro relacionado ao "COMDLG32.OCX", que foi resolvido de maneira semelhante ao problema anterior. Ambas as soluções envolveram a instalação de arquivos necessários e o registro deles usando comandos específicos.

### 03
Na terceira aula, continuamos instalando versões compatíveis do Rufus e do VirtualBox, configurando a máquina virtual para reconhecer o pendrive USB, criando um código inicial boot.asm e usando o FergoRaw para criar um arquivo de imagem bootável chamado System. Por fim, usamos o Rufus para transferir essa imagem para o pendrive USB. O processo envolveu a criação de uma máquina virtual no VirtualBox com configurações específicas e a execução da imagem de inicialização, resultando na exibição de mensagens "Hello World".
