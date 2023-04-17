- [Markdown Tutorial](#markdown-tutorial)
  - [1. Destaque e formatação básica](#1-destaque-e-formatação-básica)
    - [1.1. Fonte em itálico:](#11-fonte-em-itálico)
    - [1.2. Fonte em negrito:](#12-fonte-em-negrito)
    - [1.3. Riscar texto:](#13-riscar-texto)
    - [1.4. Pular linha e ignorar caracteres de formatação:](#14-pular-linha-e-ignorar-caracteres-de-formatação)
  - [2. Headers](#2-headers)
- [Header](#header)
  - [Header](#header-1)
    - [Header](#header-2)
      - [Header](#header-3)
        - [Header](#header-4)
          - [Header](#header-5)
  - [3. Links](#3-links)
    - [3.1. Links simples](#31-links-simples)
    - [3.2. Links de referência](#32-links-de-referência)
  - [3.3. Links para headers](#33-links-para-headers)
  - [3.4. Links para arquivos locais](#34-links-para-arquivos-locais)
  - [3.5. Links para headers em outros arquivos .md ou .html](#35-links-para-headers-em-outros-arquivos-md-ou-html)
  - [4. Imagens e Gifs](#4-imagens-e-gifs)
  - [5. Citações de bloco](#5-citações-de-bloco)
  - [6. Formatando Código](#6-formatando-código)
  - [7. Listas](#7-listas)
  - [8. Tabelas](#8-tabelas)
  - [9. Checkboxes](#9-checkboxes)
  - [10. Fórmulas e símbolos](#10-fórmulas-e-símbolos)
  - [11. HTML e CSS no Markdown](#11-html-e-css-no-markdown)
  - [12. Extras](#12-extras)

# Markdown Tutorial

## 1. Destaque e formatação básica

### 1.1. Fonte em itálico:
Envolva a expressão com um underline ou *  
_italico_, *italico*

### 1.2. Fonte em negrito:
Envolva a expressão com dois **  
**negrito**

### 1.3. Riscar texto:
Envolva a expressão em ~  
~~texto riscado~~

### 1.4. Pular linha e ignorar caracteres de formatação:
Para pular linha usamos \ ao fim de uma linha ou simplesmente dois espaços  
Para ignorar caracteres de formatação, usamos \ antes do caractere: \_italico_

## 2. Headers
Para destacar textos como headers, usamos # na frente do texto. Cada # formata o texto para um tamanho, até no máximo 6 #
# Header
## Header
### Header
#### Header
##### Header
###### Header

## 3. Links
### 3.1. Links simples
[Visite o GitHub!](https://www.github.com)

### 3.2. Links de referência
São links que recebem "variáveis" ao invés do endereço:\
Link com o nome da variável [github][] \
Link com nome personalizado [acesse o google][google]

[github]: https://www.github.com
[google]: https://www.google.com.br

A vantagem sobre o link simples é que podemos alterar 
o endereço do link apenas na definição da referência, e
todas as referências não precisarão ser atualizadas.
Note que a definição das referências não aparece na página.

## 3.3. Links para headers
Podemos criar hyperlinks para o próprio documento.
A sintaxe é como de um link normal: \[nomeExibido](#header)
Exemplo:    
[volte ao início](#markdown-tutorial)  
A referência ao header deve ter todas as letras minúsculas e espaços substituídos por -

## 3.4. Links para arquivos locais
[Tutorial de JavaScript](./JavaScript.md)

## 3.5. Links para headers em outros arquivos .md ou .html
[Tutorial de JavaScript](./JavaScript.html#header-name)  
OBS: Para arquivos locais, apenas a versão .html funciona.

## 4. Imagens e Gifs
São como links, mas precisam de um ! na frente do link:  
![imagem](awesome%20face.png)  
![gif](awesome%20face.gif)  
OBS: Se a URL possuir espaços, como no caso do arquivo "awesome face.png", então precisamos substituir os espaços por %20

## 5. Citações de bloco
Para criar uma citação de bloco, escreva um > no início da linha de cada parágrafo ou linha em branco:
> Life is like riding a bicycle. To keep your balance, you must keep moving.
>
> Outra citação

## 6. Formatando Código
Envolva um bloco de texto em ``` ou usa 2 tabs para formatar um bloco de código

```
Um bloco de código
```

    Outro bloco de código

Também é possível especificar a linguagem para adicionar destacamento de sintaxe

```c++
#include <lib>
int fun(){
  return 0;
}
```

Envolva um texto em \` para formatação de código inline \
Destacando um if: `if(condição) {bloco}`

## 7. Listas
Há dois tipos de lista: não-ordenada e ordenada.
Para a lista não-ordenada, usamos * para cada elemento:
* Primeiro item
* Segundo item
* Terceiro item

Para a lista ordenada, usamos apenas números:
1. Primeiro item
2. Segundo item
3. Terceiro item

Em ambos os tipos podemos aninhar listas usando um tab para cada nível:
1. Lista principal
   * Lista secundária
     * Lista terciária

* Um item
  * outro item 

## 8. Tabelas
Definimos tabela com 2 componentes:
1. Um cabeçalho com n colunas
2. Estrutura de alinhamento
3. Corpo com n colunas por m linhas
  
|left|center|right|
|-|-|-|
|elemento|elm 2|elm 3|
|elm 4|elm 5|elm 6|

Por padrão o cabeçalho e todos os elementos são alinhados a esquerda das colunas, mas podemos alinhá-los à direita ou ao centro, usando : no canto direito ou nos dois cantos da estrutura de alinhamento

|left|center|right|
|--:|:--:|--|
|elemento1 a direita|elemento2 ao centro|elm3|
|elemento4|elemento5|elm6|

## 9. Checkboxes
Criamos checkboxes com -[ ] nomeItem ou -[x] nomeItem
 - [ ] item 1
 - [x] item 2

## 10. Fórmulas e símbolos
Todo símbolo ou fórmula usa o sistema de marcação LaTeX e para sua exibição em Markdown deve ser envolto em $.
Alguns exemplos:

$\pi$  
$\alpha$  
$\frac{1}{2}$  
$\sqrt{b^2 - 4ac}$

$
\left(\begin{array}{cc} 
a & b\\
c & d
\end{array}\right)
$

Se a fórmula for envolta em $$, ela fica centralizada
$$E = mc^2$$

## 11. HTML e CSS no Markdown
É possível utilizar qualquer código HTML e CSS num arquivo
Markdown.
Exemplos:
<span style="color:blue">Um texto azul</span>
<br>
<br>
<details>
<summary>Clique para expandir/colapsar o conteúdo</summary>

Um conteúdo qualquer
</details>

## 12. Extras
Podemos usar emojis copiando e colando-os no documento:
🦉