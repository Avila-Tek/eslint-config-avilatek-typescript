# Eslint Config Avila Tek Typescript

![Avila Tek Logo](https://avilatek.dev/assets/images/logo_white.png)

Este repositorio contiene la configuración de eslint que se utiliza en [Avila Tek](https://avilatek.dev) tiene una fuerte inspiración en la configuración de [wesbos](https://github.com/wesbos/eslint-config-wesbos) la version de [JavaScript](https://github.com/Avila-Tek/eslint-config-avilatek) puedes encontrarla [aquí](https://github.com/Avila-Tek/eslint-config-avilatek).

## Install

Para instalar esta configuración lo que debes hacer es ejecutar este comando dentro de la carpeta de tu proyecto, se instalara como una dependencia de desarrollo, por lo cual las reglas solamente se ejecutaran el proyecto en que lo hayas instalado. **Nótese que es npx no es npm**

```shell
npx install-peerdeps --dev eslint-config-avilatek-typescript
```

Luego deberás crear un archivo de config `.eslintrc.js` es el root del proyecto y copiar lo siguiente.

```javascript
module.exports = {
  extends: ['avilatek-typescript'],
};
```

## Para usar con VS Code

> Requisitos: Debes tener instalado [vscode](https://code.visualstudio.com) y la extension de [eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint).

Luego deberás abrir el archivo de `settings.json` (preferiblemente el global) y agregar las siguientes instrucciones al archivo.

```json
{
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false
  },
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "prettier.disableLanguages": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact"
  ]
}
```

## Licencia

Este proyecto, cuenta con la Licencia MIT.

---

Elaborado por [@zoomelectrico](https://github.com/zoomelectrico)
