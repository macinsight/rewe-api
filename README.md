# rewe-api
Documenting the REWE APIs one request at a time.


## REWE Mobile API

### Return EAN, ArticleID, ProductID, Name, Description and Categories

Link: `https://mobile-api.rewe.de/products/ean/$GTIN`
Schema:
```json
{
  "items": [
    {
      "ean": "9011111035264",
      "articleId": "9011111035264",
      "productId": "5001285",
      "name": "Danke Toilettenpapier 3-lagig 8x150 Blatt",
      "description": "• Das DANKE WC Papier besteht zu 100% aus Recyclingfasern und ist besonders umwelt- und hautfreundlich\n• Das 3-lagige Klopapier enthält weder Farbzusätze noch Bleichmittel und ist damit auch ideal für Allergiker geeignet\n• Das weiche Klopapier ist mit dem Umweltzeichen \"Blauer Engel\" für besondere Sicherheit und Unbedenklichkeit ausgezeichnet \n• Umweltfreundliches DANKE Toilettenpapier mit weicher Struktur bietet Qualität und Komfort für jeden Tag und die gesamte Familie\n• Lieferumfang: 1 x 8 Rollen DANKE Toilettenpapier, 100% recyceltes Toilettenpapier 3 lagig im praktischen Vorteilspack",
      "categoryIds": [
        "1072",
        "1067",
        "1066"
      ]
    },

```

**Note:** Returns the same item multiple times, each in its own json dict

