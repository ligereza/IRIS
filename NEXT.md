# NEXT — open work, observations, suggestions

Snapshot checked by `LIBELULA` on 2026-09-14. Not a contract and not a
replacement for the operator's decisions.

## Current boundary

This checkout is the IRIS proposal, documentation and transfer surface. It
contains the FONDART dossier, its internal evidence ledger, annexes and the
candidate submission capsule. It has no executable application source or
runtime test suite of its own.

The product boundary described by `README.md` remains intentional: the
working IRIS ordering system is implemented and operated inside MAK. Its
canonical definition is `/home/mak/docs/IRIS_CANONICAL.md`; that file belongs
to MAK and is not a relative file in this checkout. This repository does not
create a second IRIS engine, database, corpus or public portfolio.

## Names that must stay separate

- `IRIS / Atlas Campo del Orden`: the internal MAK system for ordering an
  archive and preparing defensible outputs.
- `IRIS: Mesa de Montaje`: the artistic project and FONDART proposal title.
- `/home/mak/IRIS`: this Git checkout of the proposal and transfer material,
  not the live MAK runtime.
- `iskvw.cl`: the separate public portfolio output described by MAK's
  canonical definition.

PUPILA and VIZZ remain optional capabilities. They are not implicitly embedded
in this checkout or promoted into the IRIS runtime by the proposal documents.

## Current deliverable state

- Active branch: `postulacion/fondart-regional-2027`.
- Upstream relation: `0/0` against
  `origin/postulacion/fondart-regional-2027`.
- Published head: `e4cafd9887fffd17eb1e47ad684548cdb5bd4d41`.
- Transfer instructions: `postulaciones/fondart-regional-2027/TRANSFERENCIA_TECNICA.md`.
- The package is prepared but not submitted. Personal data, signed letters,
  real quotations, final title and the public asset subset remain human
  decisions, as stated by the transfer note and submission checklist.

## Before any implementation extraction

Re-read MAK's canonical definition, source, dependency and rights boundaries;
name the exact consumer and evidence path; and preserve the rule that local
media and artist decisions produce proposals while only artist-approved views
and exports leave. Do not copy MAK artwork, archives, credentials or private
declarations into this checkout.
