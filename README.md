# Model Viewer Types

[![](https://img.shields.io/npm/v/model-viewer-types?color=CB0000&style=for-the-badge)](https://npmjs.com/package/model-viewer-types)
[![](https://img.shields.io/npm/dt/model-viewer-types?color=CB0000&style=for-the-badge)](https://npmjs.com/package/model-viewer-types)
[![](https://img.shields.io/badge/types-TypeScript-blue?style=for-the-badge)](https://github.com/microsoft/TypeScript)
[![](https://img.shields.io/github/license/edixonalberto/model-viewer-types?style=for-the-badge)](LICENSE)

Una librería de definiciones de tipos para la librería
[@google/model-viewer](https://www.npmjs.com/package/@google/model-viewer), diseñada para proporcionar soporte de tipos
y autocompletado en entornos de desarrollo TypeScript. Esta librería facilita la integración de model-viewer en
proyectos, mejorando la experiencia de desarrollo y reduciendo errores.

## Instalación

```sh
# Instalar la dependencia de par ThreeJS
npm install three

# Instalar el paquete Model Viewer
npm install @google/model-viewer

# Instalar el paquete para las definiciones de tipos
npm install model-viewer-types
```

😎 copia y pega rapido:

```sh
npm install three @google/model-viewer model-viewer-types
```

## Uso

Ejemplo en un proyecto usando react y typescript:

```tsx
// src/main.tsx

import { StrictMode, useRef } from 'react'
import { createRoot } from 'react-dom/client'

import '@google/model-viewer' // Importar la librería de model-viewer
import 'model-viewer-types' // Importar la librería de tipos para model-viewer

function App() {
  const viewer = useRef<ModelViewerRef>(null)
  return (
    <model-viewer
      ref={viewer}
      class="my-model"
      src="https://modelviewer.dev/shared-assets/models/NeilArmstrong.glb"
      camera-controls
    ></model-viewer>
  )
}

createRoot(document.getElementById('root')!).render(
  <StrictMode>
    <App />
  </StrictMode>
)
```

## Resultado

Con esto logramos el siguiente autocompletado en editores de código como vsCode:

![preview](https://github.com/EdixonAlberto/model-viewer-types/blob/main/preview.png?raw=true)

## Licencia

[MIT](LICENSE) &copy; Edixon Piña
