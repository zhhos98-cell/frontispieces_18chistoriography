# Evidence and Provenance Policy

This corpus separates **what has been observed** from **what has been reported** and **what is inferred**. The distinction is especially important because a catalogue record for a book, an archival note about an engraver, and direct inspection of a frontispiece support different claims.

## Status vocabulary

### `verified_primary`
The relevant object, page, plate, scan, transcription, advertisement, or review has been inspected directly. Use this for claims that can be checked against the primary item itself.

### `verified_catalogue`
The record is supported by a library catalogue, museum catalogue, finding aid, or comparable institutional metadata, but the relevant physical/digital object has not yet been inspected for this project.

### `reported_correspondence`
An archive, library, museum, curator, or librarian reported the information in research correspondence. Preserve institution and date, but do not publish private email addresses or full correspondence in this public repository.

### `research_inference`
The project draws an analytical connection from evidence. The inference must name its supporting records and must never silently become a bibliographic or material fact.

### `unresolved`
A material identity, personal identity, date, edition, plate-state, relationship, or transcription remains open.

## Claim granularity

A source should be attached to the smallest claim it actually supports. Examples:

- A catalogue entry can verify title, imprint, date, signature, and catalogued contributors.
- A librarian's report that a box contains many Tyroff engravings can verify the existence of that holdings cluster, but not the identity of every plate.
- A cropped image can verify iconographic features, but may be insufficient to establish front-matter placement or binding sequence.
- A full digital copy can support placement, sequence, and copy-specific state, but not automatically establish the chronology of plate alteration across other copies.

## Plate identity

Do not collapse two images into `same_plate_as` merely because they share iconography. Record the strongest justified relation:

- `same_plate_as` — physical plate identity is demonstrated or strongly evidenced;
- `variant_of` — closely related state/design, physical plate identity unresolved;
- `derived_from` — one design demonstrably adapts another;
- `probable_relation` — similarity worth testing;
- `no_relation_established` — co-presence in the corpus only.

Plate identity should eventually be tested through dimensions, line-level details, lettering, damage/wear, re-engraving, plate marks, and copy chronology.

## Person and firm authority control

Do not normalise Weigel-family names prematurely. Nürnberg archival correspondence explicitly warned of confusion among similarly named members of the Weigel family. Store literal source forms alongside provisional authority IDs until identities are resolved.

Publisher succession should be encoded as relationships among people/firms and dated imprint forms rather than treated as spelling variants of one publisher. The currently reported chain includes the continuation of the Weigel business by widow/family, Martin Tyroff's involvement after his 1729 marriage to Barbara Sibylla, later Johann David Tyroff, and subsequent ownership changes. Each step requires source-specific dating and, where relevant, primary verification.

## Correspondence policy

The Gmail-connected research material is used as a discovery and provenance layer. For a public repository:

- retain institution, date, attachment title if useful, and a sanitised factual note;
- omit personal email addresses, Gmail IDs, signatures, and full message text;
- classify information as `reported_correspondence` until independently checked;
- do not redistribute unpublished scans or attachments unless rights and purpose are clear.

## Negative evidence

Negative searches are valuable but bounded. Record them as statements about the search performed, not universal absence. For example, “GNM Historical Archive staff reported no Weigel material located in their search” is preferable to “no Weigel archive exists.”

## Full-sweep rule

Discovery should preserve the complete returned set before thematic selection. Selection, deduplication, and promotion into the analytical core happen in later fields or derivative files, so that apparently peripheral records can be recovered when a new relationship becomes relevant.