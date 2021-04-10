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