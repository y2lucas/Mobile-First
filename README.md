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
## @media: são códigos que podem alterar o css do site, dependendo de características como largura da tela
## sintaxe básica
```css
@media(){
}
```
## Largura da Tela: permitem que você aplique estilos específicos a um elemento HTML dependendo da largura da tela do dispositivo onde a página está sendo visualizada. usamos o min-width ou max-width.
## min-width: define o valor mínimo que a largura da tela (viewport) deve ter para que os estilos dentro da media query sejam aplicados, Em outras palavras, se a tela for maior ou igual ao valor especificado, os estilos serão ativados
```css
@media(min-width:500px){
body{
background-color:red;
}
}
```
## max-width: define o valor máximo que a largura da tela pode ter para que os estilos sejam aplicados. Se a tela for menor ou igual ao valor especificado, os estilos serão ativados
```css
@media(max-width:500px){
body{
background-color:red;
}
}
```
## Orientação: Essas condições dentro das @media em CSS permitem que você aplique estilos específicos dependendo da orientação da tela do dispositivo.
## (orientation: landscape): Aplica os estilos quando a tela estiver na orientação paisagem (mais larga que alta)
## (orientation: portrait): Aplica os estilos quando a tela estiver na orientação retrato (mais alta que larga)
```css
@media (orientation: landscape) {
  /* Estilos para orientação paisagem */
  .image {
    width: 100%; /* A imagem ocupará toda a largura da tela */
  }
}

@media (orientation: portrait) {
  /* Estilos para orientação retrato */
  .image {
    max-width: 500px; /* Limita a largura máxima da imagem */
  }
}
```

