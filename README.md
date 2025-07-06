# Buscador de Facturas de Agua

Este proyecto contiene dos scripts de Python diseñados para encontrar y centralizar facturas de agua en formato PDF.

## Scripts

### `AGUA ALL SYSTEM.PY`

Este script escanea **todas las unidades de disco** del sistema en busca de archivos PDF que coincidan con el patrón de nomenclatura de facturas `D<9 dígitos>.pdf`. Los archivos encontrados se copian a una carpeta de destino predefinida.

**Características:**

- Búsqueda exhaustiva en todo el sistema.
- Copia los archivos a una ubicación centralizada.
- Registra los errores de copia en un archivo `errores_copia.txt`.
- Muestra un resumen final con estadísticas de la operación.

### `BUSCAR_COPIAR_FACTURAS_AGUA.PY`

Este script realiza una función similar al anterior, pero en lugar de escanear todo el sistema, busca los archivos en una **ruta de origen específica** (configurable en el propio script).

**Características:**

- Búsqueda focalizada en un directorio o unidad concreta.
- Copia los archivos a una ubicación centralizada.
- Registra los errores de copia.
- Muestra un resumen de la operación.

## Uso

1.  **Configurar las rutas:** Antes de ejecutar los scripts, asegúrate de que la variable `ruta_destino` (y `ruta_origen` en el caso de `BUSCAR_COPIAR_FACTURAS_AGUA.PY`) apunte a las carpetas correctas en tu sistema.
2.  **Ejecutar el script:** Abre una terminal o línea de comandos y ejecuta el script que desees utilizar con Python:

    ```bash
    python "AGUA ALL SYSTEM.PY"
    ```

    o

    ```bash
    python "BUSCAR_COPIAR_FACTURAS_AGUA.PY"
    ```

## Requisitos

- Python 3.x
