
![Logo](https://app-30863.nuvem-brasil-10.absamcloud.com/api/public/images/logo-icon.png)


# Momento de vida NoBeeHouse Plugin

Plugin momento de vida NobeeHouse

[![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)

## Instalação

Instale nobeehouse-momentodevida-plugin com npm:

```bash
  npm install nobeehouse-momentodevida-plugin
```

## Instalação por CDN

```HTML
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/nobeehouse-momentodevida-plugin@^1.0.0/dist/nobeehouse.min.css" />

<script src="https://cdn.jsdelivr.net/npm/nobeehouse-momentodevida-plugin@^1.0.0/dist/nobeehouse.min.js"></script>
```

    
## Uso/Exemplos

```javascript
import NoBeeHouse from 'nobeehouse-momentodevida-plugin';
import 'nobeehouse-momentodevida-plugin/dist/nobeehouse.min.css';

const plugin = new NoBeeHouse({
    el: '#plugin',
    seePlaces: function(places) {
        // função que sera execurata ao clicar no botão "Ver bairros".
    }
});
```

## Typescript

```javascript
import NoBeeHouse from 'nobeehouse-momentodevida-plugin/ts';
```


## Argumento de inicialização

#### el

selector de onde o plugin será instalado.

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `el` | `string` | **Obrigatório** |

#### seePlaces(data)

função que sera execurata ao clicar no botão "Ver bairros".

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `seePlaces`      | `Function` | **Opcional** |

## Métodos

#### open()

Abri o modal do plugin.

```javascript
plugin.open();
```

#### close()

Fecha o modal do plugin.

```javascript
plugin.close();
```
## Stack utilizada

Typescript, ES6, Sass

