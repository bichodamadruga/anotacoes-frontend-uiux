

 # Propriedades de texto CSS


Nessa sessão veremos algumas das principais propriedades utilizadas para customizar textos em páginas HTML.


- **`text`**
    
    A propriedade `text` e suas variações são propriedades independentes que são utilidadas para controlar diferentes aspectos do texto em um elemento HTML.
    
    - `text-align`
        
        Controla o alinhamento do texto dentro de um elemento. Pode ter valores como **`left`**, **`right`**, **`center`** e **`justify`**.

```css

p {
    text-align: center;
}


p {
    text-transform: uppercase;
}


p {
    text-transform: lowercase;
}


p {
    text-transform: capitalize;
}


p {
    text-transform: none;
}

/* text-indent: Define o recuo da primeira linha de um bloco de texto

Nota: Os valores podem ser definidos em pixels, em porcentagem,
 e em valores relativos. (Mais detalhes em Unidades de Medidas)


COLOR! A propriedade color é utilizada para definir a cor de um texto. 

As cores podem ser especificadas de diversas maneiras, 
incluindo os formatos RGB, hexadecimal, nome da cor e 
outros. Abaixo temos alguns exemplos.

1. **Hexadecimal:**
    
    O formato hexadecimal é uma maneira comum de representar cores no
     CSS. Consiste em seis caracteres, onde os dois primeiros
      representam a intensidade da cor vermelha, os dois seguintes
       a intensidade da cor verde, e os dois últimos a intensidade
        da cor azul.

    font! 

    A propriedade `font` é uma propriedade composta 
    que permite ao desenvolvedor definir várias propriedades
     em uma únida declaração.

Dentre as mais usadas variações das propriedades relacionadas a
 fonte temos abaixo: 
*/

p {
    text-indent: 20px;
}


p {
    font-style: italic;
}

/* 
font-variant: Define a variante da fonte, como normal ou small-caps.
*/
p {
    font-variant: small-caps;
}


p {
    font-weight: bold;
}


p {
    font-size: 16px;
}

cssCopy code
p {
    font-family: "Helvetica", sans-serif;
}

cssCopy code
p {
    font-style: italic;
    font-weight: bold;
    font-size: 18px;
    font-family: "Times New Roman", serif;
}

cssCopy code
p {
    font: italic bold 18px "Times New Roman", serif;
}


p {
    letter-spacing: 2px; /* Aumenta o espaçamento entre os caracteres 
    em 2 pixels */
}


p {
    letter-spacing: -1px; /* Reduz o espaçamento entre os 
    caracteres em 1 pixel */
}

h1 {
    letter-spacing: 4.9px;
}

/*
A propriedade line-height define a altura da linha em um bloco de texto.
 Pode ser definida como um número puro (múltiplo da altura da fonte) ou
  como uma unidade específica.

  O line-height é crucial para o espaçamento vertical entre linhas de texto.
   Um valor adequado pode melhorar a legibilidade do texto e afetar a aparência
    geral do layout. Quando o valor é unitless (um número puro), ele é
     multiplicado pelo tamanho da fonte do elemento, o que permite que a
      altura da linha seja proporcional ao tamanho da fonte.

*/


p {
    line-height: 1.5; /* Define a altura da linha como 1,5 vezes a 
    altura da fonte */
}


p {
    line-height: 24px; /* Define a altura da linha como 24 pixels */
}

/*  UNIDADES DE MEDIDA:

As unidades de medida no CSS são utilizadas para especificar tamanhos
 e distâncias em propriedades como largura, altura, margens, espaçamento,
  entre outras. Existem diferentes tipos de unidades de medida no CSS, e
   elas podem ser classificadas em unidades absolutas e unidades relativas.

*/

/*
    unidade de medida absolutas

*/


p {
    font-size: 16px;
    margin-left: 10px;
}


div {
    width: 2in; /* POLEGADAS FÍSICAS*/
}


img {
    height: 5cm;
}


section {
    margin-top: 10mm;
}


h1 {
    font-size: 18pt;  /* 1 PONTO = 1/72 POLEGADA */
}


p {
    line-height: 1.5pc;  /* Uma unidade absoluta usada principalmente
     em impressão, onde 1 pica é igual a 12 pontos.  */
}


/*  UNIDADES DE MEDIDA RELATIVAS */

p {
    margin-left: 2em;  /* Representa o tamanho da fonte do elemento pai.*/ 
}


/* 
         Representa o tamanho da fonte do elemento raiz
          (normalmente, o tamanho da fonte do elemento <html>).
*/
body {
    font-size: 16px;
}

p {
    margin-left: 1.5rem; /* Será 1.5 vezes o tamanho da fonte do elemento
     raiz (16px) */
}


div {
    width: 50%;  /* Representa uma porcentagem do valor da propriedade do
     elemento pai.  */
}


section {
    width: 50vw;  /* Representa uma porcentagem da largura da viewport.  */
}


aside {
    height: 80vh; /* Representa uma porcentagem da altura da viewport.  */ 
}

/* vmin é a menor das unidades vw e vh, enquanto vmax é a maior.  */ 
img {
    width: 50vmin;
}

/*
    CONSIDERAÇÕES FINAIS

    -Escolha da Unidade:
    -Escolha a unidade de medida com base nos requisitos de design
     e no comportamento desejado.
    -Unidades relativas são frequentemente preferidas para criar
     layouts responsivos.
    -Combinação de Unidades:
    - É possível combinar unidades em propriedades diferentes para
     obter resultados mais complexos.

    Lembre-se de que a escolha da unidade depende do contexto e das
     necessidades específicas do seu projeto. As unidades relativas
      são frequentemente preferidas em ambientes responsivos, pois ajudam
       a manter proporções consistentes em relação ao tamanho da fonte ou
        à largura/altura da janela de exibição.

*/


div {
    margin: 1em 2rem; /* Margem superior/inferior de 1em e margem
     esquerda/direita de 2rem */
}

/*
    OPACIDADE E TRANSPARÊNCIA: 

    1- A propriedade opacity permite ajustar a opacidade de um elemento,
     variando de 0 (totalmente transparente) a 1 (totalmente opaco).

    2- ransparência de Cores:
    Outra maneira de alcançar a transparência é utilizando cores RGBA
     (Red, Green, Blue, Alpha), onde o componente alfa (A) controla
      a opacidade da cor. O valor alfa varia de 0 (totalmente transparente)
       a 1 (totalmente opaco).

    3- Transições de Opacidade:
    É possível criar efeitos de transição suaves na opacidade usando a
     propriedade transition.

    4- Pseudo-elemento ::before e ::after` com Opacidade:

    É possível aplicar opacidade a pseudo-elementos ::before e ::after para
    criar camadas adicionais de elementos com diferentes níveis de transparência.

    No exemplo abaixo, um pseudo-elemento ::before é adicionado a um elemento
     <div>, criando uma camada azul com 80% de opacidade.

    5- A propriedade backdrop-filter permite aplicar efeitos visuais,
     como desfoque ou escurecimento, na área atrás de um elemento.

*/

div {
    opacity: 0.7; /* Define a opacidade para 70% */
}


p {
    background-color: rgba(255, 0, 0, 0.5); /* Fundo vermelho com 50%
    de opacidade */
}


div {
    opacity: 1;
    transition: opacity 0.5s ease-in-out;
}

div:hover {
    opacity: 0.5; /* Opacidade reduzida ao passar o mouse
    
    OBS: Neste exemplo, a opacidade da <div> é reduzida suavemente
     ao passar o mouse sobre ela, graças à transição configurada.
    
    */
}


div::before {
    content: "";
    display: block;
    width: 100px;
    height: 100px;
    background-color: blue;
    opacity: 0.8;
}


div {
    backdrop-filter: blur(5px);
    background-color: rgba(255, 255, 255, 0.5); /* Fundo com 50% de opacidade */
}

/* Embaça o próprio elemento - filter: blur(5px): */

.minha-caixa {
  /* Primeiro o prefixo para navegadores antigos/específicos */
  -webkit-backdrop-filter: blur(5px); 
  
  /* Por último a propriedade oficial (que substituirá a de cima se o navegador a suportar) */
  backdrop-filter: blur(5px);
}

```