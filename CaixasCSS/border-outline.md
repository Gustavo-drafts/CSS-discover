## border (e outline)

As bordas da caixa

- value: `<border-style>` |  `<border-width>` | `<border-color>`
- style: solid | dotted | dashed | double | groove | ridge | inset | outset
- width: `<lenght>`
- color: `<color>`

```css
div {
    /* shorthand */
    border: solid 2px; /* top | right | bottom | left */
    
    /* style */
    border: solid;

    /* width <length> | style */
    border: 2px dotted;

    /* style | color */
    border: outset #ff3;

    /* width | style | color */
    border: medium dashed green;
}
```

### outline ?

- difere em 4 sentidos:
    - não modifica o tamanho da caixa, pois não é parte do Box Model
    - Poderá ser diferente de retangular
    - Não permite ajuste individuais
    - Mais usado pelo user agent para acessibilidade
