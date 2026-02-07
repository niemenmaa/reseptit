# 🍳 Reseptit

Kokoelma arkiruokareseptejä JSON-muodossa.

## Rakenne

Jokainen resepti on oma `.json`-tiedosto, joka sisältää:

- **`title`** – Reseptin nimi
- **`ingredients`** – Lista raaka-aineista, joilla kullakin on `name` ja `amount` (lista: `[määrä, yksikkö]` tai tyhjä)
- **`phases`** – Valmistusvaiheet, joissa `description` kuvaa vaiheen ja `ingredients` viittaa raaka-aineisiin indekseillä

### Esimerkki

```json
{
  "title": "Lohikeitto",
  "ingredients": [
    { "name": "vesi", "amount": ["7", "dl"] },
    { "name": "peruna", "amount": ["6", "kpl"] },
    { "name": "porkkana", "amount": ["2", "kpl"] },
    { "name": "kirjolohi", "amount": ["500", "g"] },
    { "name": "kuohukerma", "amount": ["2.5", "dl"] },
    { "name": "suola", "amount": [] },
    { "name": "tilli", "amount": [] }
  ],
  "phases": [
    { "description": "Kuumenna vesi.", "ingredients": [0] },
    { "description": "Lisää peruna ja porkkana kuutioina.", "ingredients": [1, 2] },
    { "description": "Lisää kirjolohi paloina.", "ingredients": [3] },
    { "description": "Lisää kuohukerma.", "ingredients": [4] },
    { "description": "Mausta suola ja tilli.", "ingredients": [5, 6] }
  ]
}
```
