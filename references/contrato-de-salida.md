# Contrato de la habilidad generada

Estructura mínima:

```
marca-nombre/
  SKILL.md
  agents/openai.yaml
  assets/icon.png
  assets/icon.svg         # solo si corresponde
  assets/logo-original.*  # si existe
  references/identidad.md
```

Añadir `assets/brand.json` solo si ayuda a consumir valores de forma automática; mantenerlo coherente con las instrucciones. No generar carpetas vacías ni recursos ficticios. Los valores deben estar resueltos para la marca, nunca dejar placeholders.

## SKILL.md
Frontmatter YAML con `name: marca-nombre` (ASCII, minúsculas y guiones, menos de 64 caracteres) y descripción orientada a invocación y convivencia. Cuerpo con:

1. Nombre de marca y función: aportar el tema visual.
2. Colores HEX y funciones; combinaciones permitidas.
3. Tipografías, pesos, jerarquías y alternativas.
4. Logos, variantes reales, rutas relativas y reglas de uso.
5. Composición, iconos, fondos e imágenes 2D/3D/fotografía.
6. Temas y parámetros variables por pieza.
7. Convivencia con otras habilidades y prioridad de la petición del usuario.
8. Enlace relativo a `references/identidad.md` para consultar procedencia, decisiones y detalle.

Incluir las reglas frecuentes en SKILL.md; no obligar a leer una larga referencia para encontrar los colores principales. Evitar imponer contenido comercial, precios, forma de pago o procesos de una agencia como si fueran identidad visual.

## agents/openai.yaml
Seguir el esquema de la habilidad de creación instalada y validar sus restricciones. Ejemplo de valores a resolver:

```yaml
interface:
  display_name: "Marca Nombre"
  short_description: "Identidad visual de Nombre para tus proyectos"
  default_prompt: "Usá $marca-nombre para aplicar esta identidad al trabajo solicitado."
  icon_small: "./assets/icon.png"
  icon_large: "./assets/icon.png"
```

No añadir dependencias MCP si no son imprescindibles. La marca debe funcionar una vez cargados sus archivos, sin volver a consultar la web cada vez.

## references/identidad.md
Registrar fuentes y fecha, decisiones confirmadas/estimadas/propuestas, reglas detalladas y restricciones de activos. Si hay varias fuentes, señalar cómo se resolvieron diferencias. Incluir versión inicial 1.0; en actualizaciones conservar identidad de la habilidad y documentar brevemente el cambio cuando sea útil. No incluir secretos, rutas personales o contenido ajeno a la marca.

## Portabilidad
Mantener Markdown, JSON opcional y archivos PNG/SVG estándar. El archivo openai.yaml es metadato de ChatGPT/Codex y puede ser ignorado por otras IA; las reglas visuales deben seguir siendo comprensibles desde SKILL.md. No garantizar que otra plataforma admita importar habilidades ni que dos invocaciones se combinen automáticamente: redactar instrucciones explícitas y comunicar el estado real.
