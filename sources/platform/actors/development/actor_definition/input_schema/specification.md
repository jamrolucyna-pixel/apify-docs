{
  "title": "Contacts config",
  "type": "object",
  "properties": {
    "categories": {
      "title": "Kategorie",
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": { "type": "string" },
          "gmapsQuery": { "type": "string" },
          "panoramaPath": { "type": "string" }
        },
        "required": ["name"]
      }
    },
    "cities": {
      "title": "Miasta",
      "type": "array",
      "items": { "type": "string" }
    },
    "country": { "type": "string", "default": "Polska" },
    "region": { "type": "string", "default": "Zachodniopomorskie" },
    "maxResultsPerQuery": { "type": "integer", "default": 300, "minimum": 1 },
    "usePanorama": { "type": "boolean", "default": true },
    "useGoogleMaps": { "type": "boolean", "default": true }
  },
  "required": ["categories", "cities"]
}
