# TOTEM Español ISO para BOOX

Aplicación mínima de distribución física para usar en Android/BOOX el mismo firmware del TOTEM diseñado para **Español ISO de macOS**.

## Qué corrige

macOS y el mapa español estándar de Android interpretan de manera diferente dos posiciones ISO. Por eso el mismo código que en la Mac produce `<` y `>` puede producir `º` y `ª` en el BOOX.

Este diseño intercambia solamente esas asignaciones:

- `GRAVE`: `<` y `>`;
- tecla ISO adicional: `º`, `ª` y `\\` con Alt derecho.

El resto parte del mapa oficial **Spanish (Spain)** de Android: letras, `ñ`, acentos y símbolos conservan la disposición española.

## Privacidad

La aplicación no contiene una interfaz, no funciona como teclado virtual y no solicita permisos. Únicamente registra un archivo de distribución física (`.kcm`) para que Android pueda seleccionarlo.

## Instalación

1. Abrí la pestaña **Actions** de este repositorio.
2. Entrá en la última ejecución correcta de **Build Android layout APK**.
3. Descargá el artefacto `TOTEM-Espanol-ISO-Boox` y descomprimilo.
4. Instalá `TOTEM-Espanol-ISO-Boox.apk` en el BOOX.
5. Con el TOTEM conectado, abrí **Teclado físico → TOTEM → Configurar diseños**.
6. Elegí solamente **TOTEM Español ISO (macOS)**.

No es necesario modificar ni volver a flashear el TOTEM.

## Prueba recomendada

Comprobá: `ñ`, `á`, `é`, `í`, `ó`, `ú`, `ü`, `<`, `>`, `º`, `ª`, `¿`, `¡`, `@`, `#`, `{`, `}` y `\\`.

## Base técnica

El mapa se basa en `keyboard_layout_spanish.kcm` del Android Open Source Project, licenciado bajo Apache License 2.0. Las modificaciones propias de este repositorio se publican bajo la misma licencia.
