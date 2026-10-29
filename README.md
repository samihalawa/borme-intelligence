<p><img src="assets/icon.png" width="72" height="72" alt="Icono de BORME Intelligence"></p>

# BORME Intelligence

## Los cambios de una empresa, con su fuente delante.

Consulta actos de una sociedad en el BORME por provincia y fecha, con rangos de hasta siete días y fuentes verificables.

**Para:** Consultoras y equipos B2B que comprueban actos societarios.

**Fuente:** BORME · **Sin cuenta adicional ni API key** · **Python 3.11+** · **MIT**

### Qué obtienes

- Una empresa, una provincia y un periodo explícito.
- Hasta siete días por consulta, con incidencias por día.
- Actos publicados y enlaces, sin una puntuación de riesgo inventada.

### Pruébalo con una pregunta

> Busca actos de LINGUASERVE en Madrid entre el 19 y el 20 de octubre de 2026.

También: “Resume estos anuncios y distingue fecha de publicación, acto e inscripción.”

[Ver el informe de ejemplo](examples/demo.md) · [Código de la página del producto](docs/index.html) · [Flujo completo](skills/borme-intelligence/references/workflow.md)

La demostración es una **captura guardada de fuentes oficiales**, no una consulta actual. Conserva fecha, enlaces y alcance.

## Instalar en Claude Code

```text
/plugin install borme-intelligence --marketplace samihalawa/borme-intelligence
```

O desde terminal:

```bash
claude plugin marketplace add samihalawa/borme-intelligence
claude plugin install borme-intelligence@borme-intelligence
```

Después, pregunta en lenguaje natural o invoca `/borme-intelligence:borme-intelligence`.

## Ver un resultado sin conexión

Desde una copia de este repositorio:

```bash
python3 skills/borme-intelligence/scripts/run.py demo
python3 skills/borme-intelligence/scripts/run.py demo --format html --output ejemplo.html
```

## Consultar y guardar un informe

```bash
python3 skills/borme-intelligence/scripts/run.py report borme_events --json '{"company": "LINGUASERVE", "start_date": "2026-10-19", "end_date": "2026-10-20", "province": "MADRID", "limit": 5}'
```

Añade `--format html --output informe.html` o `--format json`. No se sobrescriben archivos por defecto. `doctor` comprueba el entorno local sin consultar proveedores.

## Dónde funciona

| Entorno | Comportamiento |
|---|---|
| Claude Code / Codex con Python y red autorizada | Adaptadores e informes ejecutables. |
| ChatGPT con navegación/archivos | Flujo con herramientas nativas disponibles; no es un MCP alojado. |
| Sin red | Demo guardada o documentos aportados; no datos actuales inventados. |

## Alcance real

No es un historial completo, monitor continuo, certificado registral ni evaluación crediticia. Una coincidencia de nombre no prueba identidad. No crea perfiles de personas.

## Verificación

```bash
python3 -m unittest discover -s tests -v
python3 scripts/check_package.py
claude plugin validate --strict .claude-plugin/plugin.json
claude plugin validate --strict .
```

[Mejoras y crítica](CHANGELOG.md) · [Evidencia versionada](evidence/) · [Revisión de Claude](SUBMISSION.md). Los tests no equivalen a adopción. `ci/validate.yml` es una plantilla inactiva.

**English:** An independent workflow for Spanish official data, with a self-contained Python adapter, offline example and readable reports. Answer language follows the user.

**Sami Halawa** · Software independiente; sin afiliación oficial. [Privacidad](PRIVACY.md) · [Condiciones](TERMS.md) · [Soporte](SUPPORT.md) · [Seguridad](SECURITY.md).

## Datos enviados a servicios externos

Las consultas en vivo envían únicamente los parámetros públicos necesarios de la consulta a los servicios oficiales identificados en [Fuentes y endpoints](skills/borme-intelligence/references/sources.md). El proveedor recibe esos parámetros y la dirección de red del entorno que ejecuta la consulta. No se envían credenciales, adjuntos, perfiles personales ni el historial de conversación. Estos accesos se realizan desde las herramientas autorizadas del anfitrión o los adaptadores Python locales; este paquete no declara un conector MCP alojado.

Las respuestas oficiales pueden contener nombres, direcciones u otros datos personales públicos. La caché local es solo de memoria, durante un máximo de cinco minutos mientras se ejecuta el proceso. Los resultados pueden permanecer en la conversación o en informes guardados explícitamente por el usuario; su conservación depende del anfitrión y del usuario. El editor no opera un servicio que reciba o almacene estos datos. Consulta [Privacidad](PRIVACY.md) para los detalles y los límites de reutilización.
