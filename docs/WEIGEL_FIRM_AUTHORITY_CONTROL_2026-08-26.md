# Weigel firm authority control — 26 August 2026

This pass separates two Nürnberg Weigel households that library authority data can easily collapse when an imprint says only `Weigel`, `Christoph Weigels Witwe`, or a generic `Weigel` firm name. The distinction matters for the Wappenkalender because current catalogues assign several 1731–1735 issues to Barbara Magdalena Weigel, while other publications in the elder Christoph Weigel succession are securely tied to Magdalena Esther Weigel.

## 1. Christoph Weigel the Elder — the elder art-publishing house

**Christoph Weigel d. Ä.**

- 9 Nov. 1654 – 5 Feb. 1725;
- engraver, art dealer, publisher and bookseller in Nürnberg;
- GND 118630067;
- younger brother: Johann Christoph Weigel (1661–1726).

His wife was **Magdalena Esther Holzmann / Weigel** (1679–1748). Nürnberg church-register reconstruction gives the marriage as 4 May 1698 and records Magdalena Esther's death on 21 June 1748. GND-linked catalogues and digitised imprints identify her as the widow who continued Christoph Weigel the Elder's business.

A 1730 Köhler geography supplies a particularly useful imprint control:

`Nürnberg, Bey Christoph Weigels des Aeltern, Kunsthändlers seel. Wittwe : Gedruckt bey Lorenz Bieling`

The Halle catalogue resolves the publisher as **Weigel, Magdalena Esther**. A c.1742 publication likewise names Magdalena Esther and the `Ältere Weigelische Kunst-Handlung` in institutional metadata.

The elder household's daughter **Barbara Sibylla Weigel** married engraver **Martin Tyroff** in 1729. British Museum authority data state that the elder Christoph Weigel firm was continued after his death by his widow together with Barbara Sibylla and Martin Tyroff; after the widow's death Tyroff continued under `Christoph Weigels Erben`. After Tyroff's death, his sons continued the succession, including the later formula `Johann David Tyroff, ehemals des älteren Christoph Weigels Erben`.

For this corpus, the safest firm chain is therefore:

`Christoph Weigel d. Ä. (1654–1725)`
→ `Magdalena Esther Weigel / elder widow` + family shop
→ `Barbara Sibylla Weigel + Martin Tyroff` within the succession
→ `Christoph Weigels Erben`
→ Tyroff sons / later Tyroff heraldic business.

## 2. Johann Christoph Weigel — the younger/brother's house

**Johann Christoph Weigel**

- 1661–1726;
- engraver and publisher in Nürnberg;
- brother of Christoph Weigel d. Ä.;
- also described in authority resources as `Christoph Weigel junior`, which creates an obvious collision risk with the elder firm's `Christoph Weigel` imprint.

His wife was **Barbara Magdalena** (born Barbara Magdalena Schwab, 1679–1771 according to a Nürnberg register reconstruction). DNB authority record GND 1037508335 states explicitly:

- `Weigel, Barbara Magdalena`;
- alternate/relational form: `Weigel, Johann Christoph, Witwe`;
- active as publisher/bookseller **1726–1734**;
- she continued her husband Johann Christoph Weigel's publishing house from 1726 until 1734, when their son Christoph took over.

This is a distinct widow and a distinct succession from Magdalena Esther's elder Weigel house.

## 3. Why the Wappenkalender attribution is not yet trivial

The current witness census records the 1731 and 1733 Wappenkalender under `Barbara Magdalena Weigel / Weigel constellation`. That attribution should **not** be mechanically replaced with Magdalena Esther.

The Herzog August Bibliothek's Christine-Luise reconstruction, drawing on K10plus records, explicitly assigns Wappenkalender issues for **1731, 1732, 1733 and 1735** to `Weigel, Barbara Magdalena`. The same authority grouping assigns other publications of the younger-house succession to her.

At the same time, series-level DNB/ZDB/BSB records normalize the Wappenkalender simply to `Nürnberg : Weigel`, and historical copy descriptions often say only `C. Weigels Witwe`. Those generic forms do not identify which widow without additional evidence.

The resulting evidentiary state is:

`K10plus/HAB person-level attribution → Barbara Magdalena`

versus

`series-level / many copy descriptions → generic Weigel or C. Weigels Witwe`

This is not enough to infer that the calendar definitely transferred from the elder shop to the younger brother's shop, because the authority assignment itself may have been made from an ambiguous imprint. But it is enough to prohibit silent normalization in either direction.

## 4. Required source-control rule

Every 1725–1748 Wappenkalender publisher field should distinguish four levels:

1. **imprint_literal** — exact wording on the title page/colophon;
2. **catalogue_authority_assignment** — e.g. K10plus/HAB assigns Barbara Magdalena;
3. **resolved_household/firm** — only when person/firm identity is independently secure;
4. **printer** — Lorenz Bieling or another printer must remain separate from publisher/shop identity.

Do not replace a literal `Christoph Weigels Witwe` with a personal name unless the witness or reliable bibliographic authority actually closes the identity.

## 5. Immediate high-value checks

The most informative comparison is now not a generic genealogy search but direct imprint collation across the series:

- 1725 title page / final publisher advertisements;
- 1726–1728 issues;
- 1731–1733, where K10plus assigns Barbara Magdalena;
- 1734–1736 around the younger-house 1734 succession to her son Christoph;
- 1740 BM Clio witness and contemporaneous elder-shop publications securely naming the elder succession.

For each, record the literal form `Christoph Weigel`, `Christoph Weigels Witwe`, `des älteren ... Witwe`, `Erben`, etc. The sequence may reveal whether the calendar's plate stock and publishing responsibility actually moved between the two related Weigel businesses or whether later authority cataloguing has conflated ambiguous widow imprints.

## 6. Current conservative conclusion

There were **two distinct Weigel widow publishers operating in closely overlapping Nürnberg contexts**:

- **Magdalena Esther Weigel**, widow of Christoph Weigel the Elder;
- **Barbara Magdalena Weigel**, widow of his brother Johann Christoph Weigel / `Christoph Weigel junior`.

This distinction is now firm. The Wappenkalender's exact household assignment in individual 1730s issues remains a witness-level question and should be preserved as such until title-page/colophon inspection resolves it.