![Icono de BORME Intelligence](assets/icon.png)

# BORME Intelligence

## Los cambios de una empresa, con su fuente delante.

Revisa actos de una sociedad en el BORME por provincia y periodo explícito, con fuentes verificables y cobertura declarada.

**Edición de instrucciones 0.5.0** · **Fuente: BORME** · **MIT para las instrucciones**

Esta habilidad guía al asistente para leer fuentes oficiales y documentos del usuario. Usa las funciones nativas de navegación y archivos que su anfitrión ya tenga autorizadas. No añade herramientas de consulta propias, procesos ni servicios; no requiere código, dependencias, cuentas ni claves de API del editor.

## Cómo usarla

Carga o comparte [SKILL.md](skills/borme-intelligence/SKILL.md) en un anfitrión que admita instrucciones o habilidades. No hace falta ejecutar ni instalar software adicional. El anfitrión decide cómo cargar instrucciones y qué funciones puede usar. La existencia de un paquete no acredita aceptación en su directorio.

Empieza con una pregunta concreta o aporta los documentos que quieras revisar:

> Busca actos de LINGUASERVE en Madrid entre el 19 y el 20 de octubre de 2026.

> Resume estos anuncios y distingue fecha de publicación, acto e inscripción.

> Muéstrame una ficha de ejemplo con el alcance exacto de la búsqueda.

Si hay navegación autorizada, el asistente abre las [fuentes oficiales](skills/borme-intelligence/references/sources.md). Si no la hay, trabaja con tus documentos y señala lo que no puede verificar actualmente. Nunca debe simular una búsqueda ni utilizar una captura como si fuera actual.

## Qué entrega

Identidad buscada y grado de confirmación; provincia y fechas revisadas, incluidos días no comprobados; tabla con anuncio, sociedad, acto, fecha del acto/inscripción, publicación, referencia registral y enlace. Añade homónimos, lagunas y límites de interpretación.

Consulta el [procedimiento detallado](skills/borme-intelligence/references/workflow.md) y las [reglas de acceso](skills/borme-intelligence/references/runtime.md). Separa hechos documentales e interpretación; incluye enlaces y fechas para las afirmaciones relevantes.

## Alcance

No es un historial completo, monitor continuo, certificado registral ni evaluación crediticia. Un nombre coincidente no prueba identidad. No crea perfiles de personas.

## Ejemplo histórico

La [captura JSON](skills/borme-intelligence/references/demo.json), el [informe guardado](examples/demo.md) y la [vista documental](docs/mcp-preview.html) son material histórico de ediciones anteriores, con captura 2026-10-20T16:59:24.525292+00:00. Son ejemplos de presentación, no consultas actuales. Sus campos técnicos se conservan para procedencia y no describen dependencias de esta habilidad.

## Privacidad y permisos

Las búsquedas nativas pueden comunicar términos públicos mínimos y la dirección de red del anfitrión a los proveedores elegidos. No envíes historiales, documentos privados ni credenciales para una consulta pública. La conservación de respuestas y archivos depende del anfitrión. La habilidad no amplía permisos, tramita solicitudes ni activa seguimiento.

[Privacidad](PRIVACY.md) · [Seguridad](SECURITY.md) · [Condiciones](TERMS.md) · [Soporte](SUPPORT.md) · [Revisión editorial](DEVELOPMENT.md) · [Descripción para directorios](SUBMISSION.md).

**English:** An instruction-only skill for reviewing Spanish official sources and user-provided documents with authorized native browsing and file tools. No custom execution service or programming runtime is required. Historical examples remain explicitly dated.

Un símbolo sencillo identifica la función y una pequeña bandera española marca su borde; no es un sello oficial. Producto independiente de Sami Halawa, sin afiliación con ninguna autoridad pública.
