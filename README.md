# CSS-discover

# Introdução

## O que Significa CSS ?

* Cascading Style Sheet
* Código para criar estilos no HTML
* HTML é a estrutura, e o CSS é a beleza
* Não é uma linguagem de prgramação;
* É uma linguagem style sheet


# Anatomia

```css

elemento {
    propriedades: valor da propriedade;
}

* Selector
* Declaration
* Propeties
* Property Value

======================
# Slectors

Conecta um elemento HTML com o CSS

## Tipos

* Global selector `*`
* Element/Type selector `h1, h2, p, div`
* ID Selector `#box, #container`
* Class Selector `.red, .m-4`
* Attribute selector, Pseudo-class, Pseudo-element e outros

=========================================
## Caixas

* Voçê irá perceber que (quase) tudo são caixas do CSS
* Posicionamentos, tamanhos, espaçamentos, bordas, cores
* Caixa pode ficar ao lado uma da outra, ou acima
* Elementos HTML são caixas

==================================================
# Adicionando Class

# inline

* atributo`style`

## <style>

* tag html que irá conter o css

## <link>

* arquivo css externo

## @import

* indicado no google fonts
* arquivo css externo

============================================
# A Cascata (cascading)

A escolha do browser de qual regra aplicar, caso haja regras para o mesmo elemento.

* Seu estilo é lido de cima para baixo.

É levado em consideração 3 fatores

1. Origem do estilo
2. Especificidade
3. Importância

### Origem do estilos

inline > tag style > tag link

### Especificidade

É um cálculo matemático, onde cada tipo de selector e  origem do estilo, possuem valores a serem considerados.

0. Universal selector, combinators e negation pseudo-class (:not())
1. Element type selector e pseudo-elements (::before, ::after)
10. classes e attribute selectors ([type="radio"])
100. ID selector
1000. Inline

==============================
### A regra !important

* cuidado, evite o uso
* não é considerado uma boa prática
* quebra o fluxo natural da cascata

===================================
# At-rules

* Está relacionado ao comportamento do CSS
* começa com sinal de `@` seguido do identificador e valor

## Exemplos comuns

- @import       /* incluir um CSS externo */

- @media        /* regras condicionais para dispositivos */

- @font-face    /* fontes externas */

- @keyframes    /* Animation */


```css

@import url ("http://local.com/style.css");

@media (min-width: 500px) {
    /* rules here */
}

@font-face {
    /* rules here */
}

@keyframes nameofanimation {
    /* rules here */
}

===============================================
# Shorthand

* junção de propriedades
* resumido
* legível

```css
{
     /* background propeties */
     background-color: #000;
     background-image: url(images/bg.gif);
     background-repeat: no-repeat;
     background-position: left top;

    /* background shorthand */
    background: #000 url(images/bg.gif) no-repeat left top;


    /* font properties */
    font-style: italic;
    font-weight: bold;
    font-size: .8em;
    line-height: 1.2;
    font-family: Arial, sans-serif;

    /* font shorthand */
    font: italic bold .8em/1.2 Arial, sans-serif;
}

````
## Detalhes

* não irá considerar propriedades anteriores
* valores não especificados irão assumir o valor padrão
* geralmente, a ordem descrita não importa, mas, se houver muitas propriedades com valores semelhantes, poderemos encontrar problemas

## Propriedades que aceitam shorthand

animation, background, border....

**https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties**

======================================================

# Funções

* nome seguido de abre e fecha parenteses
* recebe argumentos

## Exemplos

```css
@import url("http://urlaqui.com/style.css");

{
    color: rgb(255, 0, 100);
    width: calc(100% - 10px);
}

==========================================
# Vendor Prefixes

Permite que browsers adicionem `fatures` a fim de colocar em uso alguma novidade que vemos no CSS.

# Consultas 

http://ireade.github.io/wich-vendor-prefix/
http://caniuse.com