# NEXT — open work, observations, suggestions

Written from memory at the end of the 2026-09-07 session, without re-reading
the tree. Not a contract.

Nothing here was modified, and there was nothing to audit. The repository is
`LICENSE` and `README.md`: an empty product boundary, which the README says is
deliberate until MAK is ordered and the source, algorithm, dependencies and
rights are audited.

That is a stated position, not a gap. This file exists so the next agent does
not read the emptiness as neglect and start filling it.

## The one thing worth resolving before code arrives

**The name means three different things.** From memory: MAK's nomenclature
calls IRIS the internal system of ordering and relation; another note records
that IRIS is the name of the FONDART application the system is presented
under, and that it "is not the name of a component and renames nothing in the
tree"; and this repository's README describes IRIS as a local-first interactive
portfolio application.

Three referents for one word, in a system whose own documents already had to
fix what "MAK" meant for the same reason. Deciding which one IRIS is -- and
what the other two are called instead -- is cheaper now, with two files in the
repository, than after a portfolio graph exists.

`DECISIONES.md` in MAK records that separating the system into its own
repositories is the next step and that `ligereza/MAK`, `ligereza/flujo` and
`ligereza/IRIS` were left reserved and empty on purpose. This one is no longer
empty, so that entry has partly happened.

## When implementation starts

The README's own architecture is the useful constraint: local media and artist
decisions produce a portfolio graph, optional agent suggestions sit beside it,
and only artist-approved views and exports leave. It also says PUPILA and VIZZ
may provide optional capabilities but are not embedded implicitly. Worth
keeping literal: "optional" and "not implicit" are the parts an agent building
quickly will quietly drop.

No MAK artwork, archive, credential or declaration has been copied here, and
the README commits to that. Verify it still holds before the first import.
