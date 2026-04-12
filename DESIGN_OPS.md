# Minimal Design Sync — Guía de Uso

Esta demo muestra cómo conectar **Figma** a tu código de forma simple.

## Paso 1: Configura GitHub
En tu repositorio de GitHub, añade dos **Secrets** (Configuración -> Secrets -> Actions):
1. `FIGMA_PAT`: Tu Personal Access Token de Figma.
2. `FIGMA_FILE_ID`: El ID de tu archivo de Figma.

## Paso 2: En Figma
1.  **Estilos Locales:** Crea colores y tipografías como Estilos de Figma (Local Styles).
2.  **Plugin:** Abre el plugin **"Continuous Design"**.
3.  **Sincronización:** Selecciona "Tokens" y dale a exportar si quieres verificar. Pero el CI se encarga de todo.

## Paso 3: Disparar la Sincronización
1.  Ve a la pestaña **"Actions"** de tu repositorio.
2.  Selecciona el workflow **"Design Sync"**.
3.  Dale a **"Run Workflow"**.

El resultado se verá reflejado automáticamente en `css/tokens.css`.

---
*Nota: El script limpia nombres. Ej: "Color Principal" -> "--color-principal".*
