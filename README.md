# 🍳 Reseptit

Kokoelma arkiruokareseptejä [Cooklang](https://cooklang.org/)-muodossa.

## Mikä Cooklang?

Cooklang on merkintäkieli reseptien kirjoittamiseen. Se erottaa automaattisesti raaka-aineet, välineet ja ajat tavallisesta tekstistä erityisten merkkien avulla.

### Syntaksi

| Merkki | Tarkoitus | Esimerkki |
|--------|-----------|-----------|
| `@` | Raaka-aine | `@voi{1 nokare}` |
| `#` | Väline/osio | `#kattila{}` |
| `~` | Aika | `~{15 minuuttia}` |
| `>>` | Reseptin nimi | `>> Lasagne` |

### Esimerkki

```
>> Lohikeitto

Kuumenna @vesi{7 dl}.
Lisää @peruna{6 kpl} ja @porkkana{2 kpl} kuutioina.
Lisää @kirjolohi{500 g} paloina.
Lisää @kuohukerma{2.5 dl}.
Mausta @suola{} ja @tilli{}.
```
