# Mobile-First
## É uma metodologia de desenvolvimento web que prioriza a experiência do usuário em dispositivos móveis. Em vez de criar um site para desktop e depois adaptá-lo para dispositivos menores, a ideia é começar o desenvolvimento pensando nas telas menores e depois escalar para as maiores.
### layouts: Tem Dois Tipos que são os adaptativo e responsivo
### adaptativo: E Quando ele se adapta com o dispositivo, para celular o site vai ter um tamanho, para computador outro tamanho.
### responsivo: Quando ele se flexbiliza com o tamanho da tela do dispositivo.
## Imagens Responsivas: picture e source, são imagens que mudam de acordo com o tamanho da tela do aparelho
## picture: Um lugar para as diferentes versões de imagens
## source: Define as condições para as imagens aparecer
```html
<picture>
  <source media="(min-width: 768px)" srcset="imagem-grande.jpg"> <!-- Se a largura do site for maior ou igual a 768px vai ter essa imagem -->
  <source media="(min-width: 480px)" srcset="imagem-media.jpg"> <!-- Se a largura do site for maior ou igual a 480px vai ter essa imagem -->
  <img src="imagem-pequena.jpg" alt="Descrição da imagem"> <!-- Se a largura do site for menor a 480px vai ter essa imagem -->
</picture>
```
## Imagens Responsivas:Propriedade Object-fit, define como um elemento da imagem ou vídeo deve ser redimensionado para que consiga caber dentro do contêiner em que está inserido
## fill: vai ser redirecionada para conseguir ver ela toda na área Disponível
```css
img{
height:400px;
width:400px;
object-fit:fill;
}
```
## contain: vai diminuir a imagem, mantendo a proporção, para aparecer a imagem toda
```css
img{
height:400px;
width:400px;
object-fit:contain;
}
```
## cover: vai manter a proporção da imagem, mais vai cortar a imagem
```css
img{
height:400px;
width:400px;
object-fit:contain;
}
```
