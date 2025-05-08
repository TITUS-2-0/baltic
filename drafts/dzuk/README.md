# Dataset 'Dzukian Prayers'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/balt/lit/dzuk/dzuk.htm).

* URL: https://github.com/TITUS-2-0/baltic/tree/main/drafts/dzuk/
* version: unreleased
* date: 2025-03-10

## Citation
```text
Digital version of Dzukian Prayers (draft version). By: Jolanta Gelumbeckaitė, Jost Gippert, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/baltic/tree/main/drafts/dzuk/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Prayer | `div@prayer` | Automatically translated into named div |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=olt-Latn)
  body
    div (@data-level=1, @n, @type=prayer, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [foreign (@xml:lang=lat-Latn)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="prayer-1" type="prayer" data-level="1">
				<p xml:id="prayer-1-p-1">
					<lb n="1"/>Teve mvſu kuriſ eſi /aſi/ dangwaſu ſʒvijſkiſi vardaſ tava /tavo/<lb n="2"/>athaijki tava karaliſtija buki thava vala kaijp dvn=<lb n="3"/>gvij theijp ſʒamijaij . dvanv mvſu viſu dʒenv dvaki<lb n="4"/>mvmvſ nv ijr athlaijſki mvmvſ mvſu kaltheſ<lb n="5"/>kaijp ijr meſ athlyaijdʒame mvſu kalcʒijemvſ<lb n="6"/>nijevijaſki mvſu ſʒalanv ale mvſ gijalbijak nvagi<lb n="7"/>viſa piktha amen.</p>
			</div>
```
