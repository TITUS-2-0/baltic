

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Part | `div@part` | Automatically translated into named div |
| Page | `pb` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=olt-Latn)
  body (@xml:lang=olt-Latn)
    div (@data-level=1, @n, @type=part, @xml:id) (multiple)
      p (@xml:id, @xml:lang=deu-Latn-x-enhg)
        [pb (@n)]
        [lb (@n) (multiple)]
        [foreign (@xml:lang=deu-Latn-x-enhg) (multiple)]
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
        [lb (@n, @xml:lang=lat-Latn)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="Intr." xml:id="part-1" type="part" data-level="1">
				<p xml:id="part-1-p-1" xml:lang="deu-Latn-x-enhg">
					<pb n="2"/>
					<lb n="1"/>
					<foreign xml:lang="deu-Latn-x-enhg">Der kleine</foreign>
					<lb n="2"/>Catechiſmus<lb n="3"/>D.  Martin <foreign xml:lang="deu-Latn-x-enhg">Luthers/</foreign>
					<lb n="4"/>
					<foreign xml:lang="deu-Latn-x-enhg">Deutſch und Litthauiſch/</foreign>
					<lb n="5"/>
					<foreign xml:lang="deu-Latn-x-enhg">Auf</foreign>
					<lb n="6"/>Allergnädigſten Befehl Sr. Kő=<lb n="7"/>
					<foreign xml:lang="deu-Latn-x-enhg">nigl.</foreign>
  ...
```
