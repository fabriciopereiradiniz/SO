<p align="center">
  <img src="https://i.imgur.com/xnhjM7o.gif" alt="OS" />
</p>

TripOS é um sistema operacional basico desenvolvido utilizando assembly para a matéria de sistemas operacionais, o desenvolvimento do mesmo só foi possível graças ao canal [Tutorial KiddieOS](https://www.youtube.com/watch?v=Jws7BHrts6g&list=PLsoiO2Be-2z8BfsSkspJfDiuKeC9-LSca&index=2).

## Execução do SO

Para execução do tripOS será necessário os seguintes itens:
- NASM para conversão do `.asm` para `.bin`
- FergoRaw utilizado para inserir os arquivos binários em diferentes partições realizando a conversão para `.img`
- Rufus ou outro builder de `.img` para `.iso` de sua preferência
> Quer apenas executar o os? Basta apenas bootar o `boot.iso` utilizando Rufus no seu pendrive.

## Implementações atuais

- Tela inicial
- Interface gráfica com borda
- Interface gráfica borderless window
- Lib's para monitor/wmemory
