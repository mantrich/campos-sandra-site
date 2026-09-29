# Fontes locais

Arquivos obtidos dos serviços oficiais Google Fonts em 22/09/2026 (UTC).
As fontes são alternativas editoriais de implementação, não tipografias oficiais confirmadas da marca.

## Correção localizada do Hero

`hero-editorial-normal-latin.woff2` é uma derivação local de
`cormorant-garamond-400-normal-latin.woff2`, mantida sob SIL OFL 1.1.
O nome interno é **Hero Editorial Regular**, para distinguir a derivação do original.
Os créditos e a licença original em `cormorant-garamond-OFL.txt` continuam aplicáveis.

O circunflexo do glifo `ecircumflex` (ê, U+00EA) tinha contorno entre y=471 e y=730,
enquanto o topo da letra e está em y=395. Essa proporção produzia a aparência de
um acento alto e separado na headline. Apenas as coordenadas verticais desse
contorno foram ajustadas para y=425..560, pela transformação
`y_novo = round(425 + (y_original - 471) * 135 / 259)`.

O desenho da letra e, as coordenadas horizontais, todos os demais glifos, as
métricas, o kerning e as tabelas de composição foram preservados e comparados
programaticamente com o original. A fonte itálica não foi modificada. O arquivo
original continua disponível sem alterações; não há caracteres separados,
pseudo-elementos ou acentos adicionados por CSS/JavaScript.

## Famílias

- **Cormorant Garamond**: peso 400, estilos normal e itálico, WOFF2.
- **DM Sans**: normal, arquivo variável compartilhado pelos pesos 400 e 500 retornados pelo Google Fonts, WOFF2.

Os arquivos `latin` incluem U+0000–00FF, portanto os caracteres portugueses precompostos como á, à, â, ã, ç, é, ê, í, ó, ô, õ e ú. Os arquivos `latin-ext` complementam a cobertura latina. Para carregamento seletivo, usar o `unicode-range` correspondente.

## Origem

CSS oficial consultado:

https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;1,400&family=DM+Sans:wght@400;500&display=swap

| Arquivo | Origem oficial |
| --- | --- |
| cormorant-garamond-400-normal-latin.woff2 | https://fonts.gstatic.com/s/cormorantgaramond/v21/co3umX5slCNuHLi8bLeY9MK7whWMhyjypVO7abI26QOD_v86KnTOig.woff2 |
| cormorant-garamond-400-normal-latin-ext.woff2 | https://fonts.gstatic.com/s/cormorantgaramond/v21/co3umX5slCNuHLi8bLeY9MK7whWMhyjypVO7abI26QOD_v86KnrOiss4.woff2 |
| cormorant-garamond-400-italic-latin.woff2 | https://fonts.gstatic.com/s/cormorantgaramond/v21/co3smX5slCNuHLi8bLeY9MK7whWMhyjYrGFEsdtdc62E6zd58jD-iNM8.woff2 |
| cormorant-garamond-400-italic-latin-ext.woff2 | https://fonts.gstatic.com/s/cormorantgaramond/v21/co3smX5slCNuHLi8bLeY9MK7whWMhyjYrGFEsdtdc62E6zd58jD-htM8Efs.woff2 |
| dm-sans-variable-latin.woff2 | https://fonts.gstatic.com/s/dmsans/v17/rP2Yp2ywxg089UriI5-g4vlH9VoD8Cmcqbu0-K4.woff2 |
| dm-sans-variable-latin-ext.woff2 | https://fonts.gstatic.com/s/dmsans/v17/rP2Yp2ywxg089UriI5-g4vlH9VoD8Cmcqbu6-K6h9Q.woff2 |

## Licenças preservadas

- `cormorant-garamond-OFL.txt`: https://raw.githubusercontent.com/google/fonts/main/ofl/cormorantgaramond/OFL.txt
- `dm-sans-OFL.txt`: https://raw.githubusercontent.com/google/fonts/main/ofl/dmsans/OFL.txt

Ambas as famílias são distribuídas sob SIL Open Font License 1.1. Os arquivos de licença acompanham os binários sem alteração.

## Unicode ranges fornecidos pelo Google Fonts

```css
/* latin */
unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;

/* latin-ext */
unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;
```
