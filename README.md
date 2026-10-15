# Generador de habilidades de marca

Habilidad de Punilla Digital para convertir un logo, una web, un flyer, una idea o varias fuentes en otra habilidad reutilizable de identidad visual.

## Resultado

Crea una única habilidad «Marca {nombre}», con identificador marca-{slug}, que contiene:

- Colores y funciones, tipografías y alternativas.
- Logo disponible y reglas de composición.
- Temas, iconografía y pautas de imágenes 2D, 3D y fotografía.
- Referencias de procedencia y decisiones confirmadas, aproximadas o propuestas.
- Icono con logo o iniciales y un símbolo discreto de edición.

No genera por defecto una marca de Punilla Digital ni entrega un manual PDF, flyer o presupuesto. Su salida es otra habilidad, que aporta identidad al trabajo realizado por otras habilidades.

## Archivos incluidos

- [SKILL.md](SKILL.md): instrucciones completas.
- [references/contrato-de-salida.md](references/contrato-de-salida.md): estructura y requisitos de la habilidad generada.
- [agents/openai.yaml](agents/openai.yaml): nombre, prompt e iconos.
- [assets/icon.svg](assets/icon.svg) y [assets/icon.png](assets/icon.png): iconos de este generador.

## Uso

Copiar la carpeta completa con el nombre `generador-de-habilidades-de-marca` al directorio de habilidades de un agente compatible. Conservar referencias, metadatos e iconos junto al SKILL.md. Publicar en GitHub no instala automáticamente la habilidad en ChatGPT.

Ejemplo:

> Usá Generador de habilidades de marca para crear Marca Mi Empresa a partir de este logo, mi sitio y este flyer.

Una vez creada la habilidad de marca:

> Usá Marca Mi Empresa y Presupuesto Comercial para preparar esta propuesta.

La habilidad de marca define identidad; la habilidad del trabajo define procedimiento y formato. No se garantiza que todas las plataformas combinen invocaciones automáticamente.

## Requisitos y límites

Necesita inspección de imágenes y archivos, lectura web cuando haya fuentes online, y herramientas para crear y validar habilidades e iconos. Debe seguir el mecanismo de guardado e instalación disponible en el entorno. No incluye credenciales, conectores obligatorios ni habilidades de terceros.

El contenido Markdown y los activos PNG/SVG son portables; los metadatos de interfaz y la instalación dependen del agente. No prometer compatibilidad universal ni afirmar que una habilidad está instalada sin completar el guardado correspondiente.

## Origen

Copia de la habilidad instalada en Complementos, publicada el 15/10/2026 con sus instrucciones, contrato de salida e iconos. Esta publicación no modifica la habilidad instalada.

[Punilla Digital](https://punilladigital.com.ar/) · [Licencia](LICENSE)
