# alta-rock-art

## Wikidata

Collection: https://www.wikidata.org/wiki/Q82688025

### Objects + Features

* Hjemmeluft, Bergbukten 1: https://www.wikidata.org/wiki/Q82685468
  * G-169: https://www.wikidata.org/wiki/Q82688469
  * D-195: https://www.wikidata.org/wiki/Q82690112

*https://w.wiki/Fey*

*https://query.wikidata.org/embed.html#%23defaultView%3AMap%0ASELECT%20%2a%20WHERE%20%7B%0A%20%20%3Fitem%20wdt%3AP31%20wd%3AQ220659%3B%0A%20%20%20%20wdt%3AP361%20wd%3AQ82685468.%0A%20%20OPTIONAL%20%7B%0A%20%20%20%20%3Fitem%20rdfs%3Alabel%20%3Flabel.%0A%20%20%20%20FILTER%28%28LANG%28%3Flabel%29%29%20%3D%20%22en%22%29%0A%20%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP625%20%3Fgeo.%20%7D%0A%7D%0AORDER%20BY%20%28%3Flabel%29*

```sql
SELECT * WHERE {
  ?item wdt:P31 wd:Q220659;
    wdt:P361 wd:Q82685468.
  OPTIONAL {
    ?item rdfs:label ?label.
    FILTER((LANG(?label)) = "en")
  }
  OPTIONAL { ?item wdt:P625 ?geo. }
}
ORDER BY (?label)
```
