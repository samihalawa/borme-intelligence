![Icono de BORME Intelligence](assets/icon.png)

# BORME Intelligence

Consulta actos publicados de una sociedad en el BORME por provincia y un periodo de hasta siete días, conservando fuente y límites.

**Versión 0.6.3 · Conector MCP alojado e instrucciones complementarias · Sami Halawa · MIT**

## Instalación y uso

```bash
/plugin install borme-intelligence --marketplace samihalawa/2026-MASTER-Marketplace-Plugins-Connectors-etc
```


Instala el paquete en un anfitrión compatible con plugins y MCP remoto. La configuración incluida conecta `https://aiplugins.megawebs.com/mcp/borme-intelligence` mediante Streamable HTTP y expone `review_spanish_company_events`. No necesitas Python local, instalar dependencias ni proporcionar una clave del editor. La disponibilidad de la conexión depende del anfitrión y de la fuente pública.

> Consulta actos de TELEFONICA en MADRID del 2026-10-26 al 2026-10-30.

- Revisa TELEFONICA en MADRID el 2026-10-30 y conserva los enlaces oficiales.
- Busca hasta cinco actos de IBERDROLA en BIZKAIA del 2026-10-26 al 2026-10-30.

Lee [la habilidad](skills/borme-intelligence/SKILL.md) para el procedimiento, [las fuentes](skills/borme-intelligence/references/sources.md) y [el contrato de acceso](skills/borme-intelligence/references/runtime.md). La herramienta realiza la consulta acotada descrita; la lectura de documentos, interpretación y creación de archivos usan capacidades adicionales del anfitrión. Conserva los identificadores, enlaces, fechas y límites realmente devueltos.

## Alcance

No presenta solicitudes u ofertas, no firma, no compra, no consulta datos protegidos ni activa vigilancia. Una respuesta parcial o fallida no prueba ausencia de registros. No se garantiza elegibilidad, resultado jurídico, titularidad ni financiación.

Los [ejemplos guardados](examples/demo.md) son capturas históricas de versiones anteriores, no consultas actuales. El historial de 0.5.0 conserva la edición de instrucciones; 0.6.0 añade una conexión remota explícita y no reetiqueta esas capturas. La aprobación en un directorio se verifica por separado.

[Producto e instalación](https://aiplugins.megawebs.com/plugins/borme-intelligence) · [Privacidad](https://aiplugins.megawebs.com/plugins/borme-intelligence/privacy) · [Condiciones](https://aiplugins.megawebs.com/plugins/borme-intelligence/terms) · [Soporte](https://aiplugins.megawebs.com/plugins/borme-intelligence/support)
