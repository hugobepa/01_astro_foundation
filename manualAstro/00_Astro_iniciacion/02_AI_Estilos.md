# ESTILOS

(estilos)[https://docs.astro.build/es/guides/styling/]
(ejemploEstilos)[https://gist.github.com/Klerith/6659142852f95466340f79f6d226870b]

## estilo scope

0. estilo en scope o en el mismo componente: ` <style>h1{color: blue;}</style>`
1. estilo en scope o en el mismo componente: ` <style is:global>h1{color: blue;}</style>`
   - (global,inline,raw)[https://docs.astro.build/en/reference/directives-reference/#script--style-directives]

## estilo global

0. crear y rellenar archivo de estilos `src\styles\global.css`.

- (ejemploEstilos)[https://gist.github.com/Klerith/6659142852f95466340f79f6d226870b]

1. buscar el punto mas alto (mainLayout) para llamara lo `src\layouts\MainLayout.astro `: `import '../styles/global.css'; `

### fuentes globales

0. bajar fuentes y colocar fuentes en ` public\fonts\atkinson-bold.woff`
1. llamar fuentes ` src\styles\global.css`:

```
@font-face {
  font-family: "Atkinson";
  src: url("/fonts/atkinson-regular.woff") format("woff");
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}
@font-face {
  font-family: "Atkinson";
  src: url("/fonts/atkinson-bold.woff") format("woff");
  font-weight: 700;
  font-style: normal;
  font-display: swap;
}
```
