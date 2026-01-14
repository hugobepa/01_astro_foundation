https://docs.astro.build/en/basics/project-structure/
https://docs.astro.build/en/reference/cli-reference/#astro-preferences

0. crear carpeta, con nombre de proyecto.
1. instalar astro, T: npm create astro@latest .
   - empty
   * typersctipt -- yes
   * typescript strict -- yes
   * install depedencies -- yes
   * git repository -- yes
2. desabilitar barra astro, T: npm run astro preferences disable devToolbar
   - se crea en ".astro\settings.json":
   ```
   "devToolbar": {
   	"enabled": false
   }
   ```
   - pra volver a ver eliminar esta orden o ponerla en `true`
