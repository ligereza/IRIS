# Transferencia técnica — FONDART Regional Creación 2027, caso IRIS

Documento breve para que otro operador o agente retome este paquete sin
depender del historial de conversación que lo produjo. No es un anexo de
la postulación: no corresponde adjuntarlo al FUP.

## Commit publicado

- Repositorio: `github.com/ligereza/IRIS` (privado)
- Rama: `postulacion/fondart-regional-2027`
- Commit: `d6bff19266ddd9838826213407b27bed18893615`
- Rama no fusionada a `main` -- el operador decide cuándo/si abrir la PR.
- Esta nota se agrega en el mismo commit que la publica; no modifica ningún archivo de entrega -- los comandos de comprobación de abajo se pueden ejecutar contra este mismo commit sin diferencia.

## Rutas de entrega (dentro de esta rama)

- Dossier principal: `postulaciones/fondart-regional-2027/FONDART_2027_IRIS_POSTULACION.{json,md}`
- Ledger interno de decisión y evidencia: `postulaciones/fondart-regional-2027/FONDART_2027_IRIS_REGIONAL_CREACION.md`
- Checklist de envío (repo/portal): `postulaciones/fondart-regional-2027/anexos/CHECKLIST_ENVIO.md`
- Paquete candidato listo para adjuntar: `postulaciones/fondart-regional-2027/anexos/PAQUETE_CANDIDATO_20260907/`
  (`ANEXO_01_DESCRIPCION_PROPUESTA.{md,html,pdf}` -- 4 páginas -- más `MANIFEST.md`
  con 9 hashes SHA-256 de los 7 archivos del paquete)
- Plantillas sin firmar, **no adjuntar tal cual**: `anexos/ANEXO_02_MODELO_COMPROMISO_ESPACIO.md`, `anexos/ANEXO_03_CARTAS_COMPROMISO_EQUIPO.md`

## Comandos de comprobación reproducibles

```sh
# Clonar exactamente este estado
git clone --branch postulacion/fondart-regional-2027 --single-branch https://github.com/ligereza/IRIS.git
cd IRIS/postulaciones/fondart-regional-2027

# Confirmar el commit publicado
git log -1 --format=%H
# -> d6bff19266ddd9838826213407b27bed18893615

# Paginación del anexo listo para adjuntar
pdfinfo anexos/PAQUETE_CANDIDATO_20260907/ANEXO_01_DESCRIPCION_PROPUESTA.pdf | grep Pages  # -> 4

# Validez del dossier JSON
python3 -c "import json; json.load(open('FONDART_2027_IRIS_POSTULACION.json'))"

# Ausencia de patrón de RUT chileno en todo el árbol de la postulación
grep -RnE '[0-9]{1,2}\.[0-9]{3}\.[0-9]{3}-[0-9kK]' .
# -> sin resultados
```

## Bloqueos que requieren decisión humana

- Identidad y contenido real de Perfil Cultura del responsable.
- Cartas firmadas del equipo declarado y del espacio anfitrión (las
  plantillas en `anexos/ANEXO_02` y `anexos/ANEXO_03` son borradores sin
  firmar, no sustitutos válidos).
- Cotizaciones reales, reemplazando las estimaciones del presupuesto.
- Decisión de título entre las 3 direcciones candidatas descritas en el
  expediente interno.
- Qué activos declarar públicamente elegibles -- hoy 0, según el propio
  piloto ARICA-FONDART-2027 citado en la sección 2-ter del ledger interno.

## Qué no autoriza este documento

No autoriza enviar la postulación, completar datos personales, ni tratar
las plantillas de anexo o las cotizaciones estimativas como documentos ya
válidos. Es una guía de dónde está todo y cómo comprobarlo, no una
ejecución de los pasos pendientes.
