# CSS Media Queries

## CSS2 Introdução Media Types

 - A ```@media``` regra, introduzida no CSS2, possibilitou definir regras de estilo diferentes para tipos de mídia diferentes.

 - **Exemplos**: Você pode ter um conjunto de regras de estilo para telas de computador, um para impressoras, um para dispositivos portáteis, um para dispositivos do tipo televisão e assim por diante.

 - Infelizmente, esses tipos de mídia nunca tiveram muito suporte por dispositivos, além do tipo de mídia de impressão.

## CSS3 Introdução Media Queries

 - As consultas de mídia em CSS3 estenderam a ideia de tipos de mídia CSS2: em vez de procurar um tipo de dispositivo, eles olham para a capacidade do dispositivo.

 - As consultas de mídia podem ser usadas para verificar muitas coisas, como:

    - Largura```(width)``` e altura```(height)``` da janela de visualização```(viewport)```.

    - Largura```(width)``` e altura```(height)``` do dispositivo```(device)```.

    - orientação (o tablet/telefone está no modo paisagem ou retrato?)

    - resolução

 - O uso de consultas de mídia é uma técnica popular para fornecer uma folha de estilo personalizada para desktops, laptops, tablets e telefones celulares (como telefones iPhone e Android).

## Syntax da media query

 - Uma consulta de mídia consiste em um tipo de mídia e pode conter uma ou mais expressões, que são resolvidas como verdadeiras ou falsas.

 ```
 @media not|only mediatype and (expressions) {
     CSS-Code;
 }
 ```

 - O resultado da consulta é verdadeiro se o tipo de mídia especificado corresponder ao tipo de dispositivo no qual o documento está sendo exibido e todas as expressões na consulta de mídia forem verdadeiras. Quando uma consulta de mídia é verdadeira, a folha de estilo ou as regras de estilo correspondentes são aplicadas, seguindo as regras normais em cascata.

 - A menos que você use os operadores não(not) ou apenas(only), o tipo de mídia é opcional e o alltipo estará implícito.

 - Você também pode ter diferentes folhas de estilo para diferentes mídias:

 ```
 <link rel="stylesheet" media="mediatype and|not|only (expressions)" href="print.css">
 ```
 ### Media Types CSS3
 | Value | Descrição |
 | ----- | --------- |
 |  all  | Usado para todos os dispositivos de tipo de mídia |
 | print(impressora) | Usado para impressoras |
 |screen(tela) | Usado para telas de computador, tablets, smartphones etc. |
 |speech(discurso) | Usado para leitores de tela que "lêem" a página em voz alta |