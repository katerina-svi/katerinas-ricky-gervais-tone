# Katerinas Ricky Gervais Tone

Agent skill, který přepíše libovolný text do komediálního stylu inspirovaného Rickym Gervaisem — suchá ironie, morální inverze, hyper-logická eskalace do absurdna a ostré pointy. Primárně v češtině, na vyžádání v jiném jazyce.

Není to překladač vtipů. Skill přebírá **mechaniku** humoru — setup, twist, eskalaci, pointu — a aplikuje ji na váš obsah. Konkrétní vtipy, hlášky ani formulace Rickyho Gervaise nikdy nekopíruje. Celý skill je čistý Markdown (`SKILL.md`), takže běží v jakémkoli prostředí, které podporuje skill-style instrukce.

## Jak to funguje

Základní stavební jednotka se opakuje v celém textu:

1. **Setup** — začni známou, rozumnou nebo ušlechtile znějící myšlenkou.
2. **Twist** — otoč ji v nepohodlnou pravdu, kterou všichni znají, ale neříkají.
3. **Eskalace** — dotáhni logiku do absurdního, ale vnitřně konzistentního závěru. Absurdita vyplývá z logiky, ne z náhodné ujetosti.
4. **Pointa** — krátká, ostrá, nečekaná věta. Ideálně kratší než setup.

Každé 2–4 věty musí obsahovat twist nebo komediální posun. Delší vysvětlující pasáž bez pointy je selhání.

## Techniky

Morální inverze (ukázat „dobrou věc" jako pokryteckou), hyper-literální logika (chladná doslovnost na emotivní téma), falešná omluva („Promiňte. Měl jsem říct…" a následuje horší verze), přerušení sebe sama, náhlé tonální skoky, eskalace řadou, odmítnutí publika („Slyším vás. Nesouhlasím.") a tvrdá konkrétnost místo obecných frází.

## Mantinely

Tohle není skill na urážení. Platí čtyři tvrdá pravidla:

- **Zachovej význam vstupu.** Fakta, čísla, termíny a klíčová sdělení zůstávají — mění se jen podání.
- **Punch up, ne dolů.** Terčem je pokrytectví, instituce, moc, ego a absurdita systémů. Nikdy oběti, menšiny, nemoc nebo neštěstí samotné.
- **Žádné vtipy na konkrétní reálné soukromé osoby.** Veřejné instituce a role jsou fér hra.
- **Žádné převzaté vtipy.** Přebírá se struktura, ne materiál.

## Úrovně ostrosti

| Úroveň | Popis |
|---|---|
| 1 — Jemná ironie | Suchý sarkasmus, žádné vulgarismy, vhodné i pro klientský text. |
| 2 — Standard (default) | Plný komediální motor, 1–2 ostřejší výrazy, černý humor s mantinely. |
| 3 — Plný Ricky | Maximální drzost a eskalace, vulgarismy dle potřeby, stále platí punch up. |

Bez upřesnění se použije úroveň 2. U zjevně klientského nebo veřejného textu se skill nejdřív zeptá, jestli chcete 1, nebo 2.

## Instalace

### Claude.ai (web a aplikace)

Stáhni [`SKILL.md`](SKILL.md), v Claude.ai otevři **Settings → Capabilities → Skills** a nahraj ho jako nový skill.

### Claude Code — plugin

```
/plugin marketplace add katerina-svi/katerinas-ricky-gervais-tone
/plugin install ricky-gervais-tone@katerinas-ricky-gervais-tone
```

### Skills CLI (cross-agent)

```
npx skills add katerina-svi/katerinas-ricky-gervais-tone
```

### Ručně

```
git clone https://github.com/katerina-svi/katerinas-ricky-gervais-tone.git /cesta/ke/skillum/ricky-gervais-tone
```

## Použití

```
/ricky

[vlož text k přepsání]
```

Nebo prostě: „Přepiš to jako Ricky Gervais." / „Udělej z toho stand-up." / „Chci to ostřejší."

Úroveň si můžeš vynutit: „/ricky úroveň 1" nebo „/ricky plný Ricky".

## Ukázka

**Vstup:**

> Zveme vás na firemní školení o kybernetické bezpečnosti. Dozvíte se, jak si vytvořit silné heslo a jak rozpoznat phishingový e-mail. Účast je povinná.

**Výstup (úroveň 2):**

> Přijďte na školení o kybernetické bezpečnosti. Já vím. Já vím. Taky bych radši umřel. Naučíte se vytvořit silné heslo — tedy jiné než „Heslo123", které teď máte vy, váš šéf i celé IT oddělení, co tohle školení pořádá. A naučíte se poznat phishingový e-mail. Poznávací znamení: slibuje vám něco hezkého. Takže cokoliv, co vám za posledních pět let přišlo z HR, je v pohodě. Účast je povinná. Stejně jako každý rok. A stejně jako každý rok na to v prosinci někdo klikne. Uvidíme se tam. Nebo na dark webu.

## Jazyk

Default je čeština — hovorová, mluvená, s rytmem člověka na pódiu. Anglosaské reference se nahrazují českými ekvivalenty: nepřekládá se humor doslova, ale mechanika, a hledá se lokální terč. Typografie a pravopis se řídí [Internetovou jazykovou příručkou ÚJČ](https://prirucka.ujc.cas.cz/) — humor není omluva pro chyby.

Pro jiný cílový jazyk stačí říct, který; adaptace referencí na danou kulturu platí stejně.

## Historie verzí

- **1.0.0** — první veřejná verze. Komediální motor (setup–twist–eskalace–pointa), 8 technik, 3 úrovně ostrosti, pravidla punch up a zákaz převzatých vtipů, česká kulturní adaptace.

## Autorka

[Kateřina Švidrnochová](https://svidrnochova.cz) — konzultantka, learning designerka a lektorka AI vzdělávání.

## Poznámka

Skill je *inspirovaný* veřejně známým komediálním stylem, není nijak spojený s Rickym Gervaisem ani jím schválený. Nekopíruje jeho materiál — pracuje se strukturou humoru, která je obecná a nechráněná.

## Licence

MIT
