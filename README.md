# alta-rock-art

## Wikidata

Collection: https://www.wikidata.org/wiki/Q82688025

### Objects + Features

* Hjemmeluft, Bergbukten 1: https://www.wikidata.org/wiki/Q82685468
  * G-169: https://www.wikidata.org/wiki/Q82688469
  * D-195: https://www.wikidata.org/wiki/Q82690112

*https://w.wiki/Fey*

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
