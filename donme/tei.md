* titles of seasons are encoded in heads
* line groupings are made explicit as stanzas

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Season` (hierarchical) | `div@season` (hierarchical) | Automatically translated into named div |
| `Verse` (hierarchical) | `l` (hierarchical) | Single lines |

### Structural overview
```text
text (@xml:lang=olt-Latn)
  body
    div (@data-level=1, @n, @type=season, @xml:id) (multiple)
      head (multiple)
      lg (@n, @type=stanza, @xml:id) (multiple)
        l (@n, @xml:id) (multiple)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="season-1" type="season" data-level="1">
        <head>Pawasario Linksmybės</head>
        <lg type="stanza" n="1" xml:id="season-1-lg-1">
          <l n="1" xml:id="season-1-lg-1-l-1">Iau Sauléle wėl atkópdămă buddı̆nŏ Swieta</l>
          <l n="2" xml:id="season-1-lg-1-l-2">Ir Ʒ́iemôs ſʒaltôs Truſùs pargráudămă jůkės.</l>
          <l n="3" xml:id="season-1-lg-1-l-3">Sʒalcʒû Prámonės ſŭ Lĕdaìs ſugaìſʒtı̆ păgâwo;</l>
          <l n="4" xml:id="season-1-lg-1-l-4">Ir puttódam's Snieg's wiſſùr į Nieką̆ păwirto.</l>
          <l n="5" xml:id="season-1-lg-1-l-5">Tů Laukùs Oraì drungnì gaiwįdămı̆ glóſtė,</l>
          <l n="6" xml:id="season-1-lg-1-l-6">Ir Ʒ́ŏlĕlès wiſſókias ı̆ſʒ Numirrŭſŭ ſʒaùkė.</l>
          <l n="7" xml:id="season-1-lg-1-l-7">Krúmus ſù Sʒillaìs wiſſaìs ı̆ſſı̆buddı̆nŏ kéltı̆ſ'</l>
          <l n="8" xml:id="season-1-lg-1-l-8">O Laukû Kalnaì ſù Klóneis pàmĕtĕ Skrándas.</l>
          <l n="9" xml:id="season-1-lg-1-l-9">Wiſſlâb, kàs Ruddens Biaurybėj' numı̆rĕ wèrkdams;</l>
  ...
```
