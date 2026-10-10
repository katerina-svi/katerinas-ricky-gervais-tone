# Dramaturgie: SummiD (12. 10.) a Od UČO k IČO (13. 10.)

Pracovní podklad pro Kateřinu. Stav: **KOSTRA KE SCHVÁLENÍ** (dál nestavím, dokud ji neodsouhlasíš).
Značky: `[DOPLNIT]` = chybí údaj, `[OVĚŘIT]` = předpoklad nebo fakt, který je třeba potvrdit před natáčením.

---

## 0. Co jsem ověřila v kalendáři a poště

| | SummiD (pondělí) | Od UČO k IČO (úterý) |
|---|---|---|
| Kdy a kde | 12. 10., 8:00–11:00, natáčení v Galerii Mánes v Praze | 13. 10., 16:00–17:40, online přes Zoom (Honza Valtr prosí o připojení 5–10 min předem) |
| Formát | předtočená přednáška, **ideál 45 min, max. 60**. Obrazovka a ty se nahrávají zvlášť, postprodukce je spojí. Prezentace jen v šabloně SummiD. Natáčí se i krátký rozhovor. | 5–10 min tvůj příběh, 40–50 min téma, 30 min dotazy přes Slido |
| Název | „AI backoffice: Přestaňte měnit jen nástroje. Začněte stavět procesy.“ (článek pořadatele „SummiD – Firemní operativa“) | téma „profesionální IT“, ENTRE01, 7. běh kurzu |
| Publikum | freelanceři a malé firmy. Loni přes 5 000 účastníků (podle Renaty), festival je zdarma. | asi 100 studentů napříč fakultami a obory |
| Co slibuje pořadatel | „jak si AI backoffice postavit krok za krokem na reálném příkladu“, „konkrétní postup, který můžete ve firmě použít hned“ | — |
| Povinnosti | pozvat na **živý webinář 4. 11. odpoledne** (registrace na stránce s přednáškou) a připomenout **hodnocení pod videem**. Obojí jsi Renatě slíbila. | — |

**Anotace a osnova, kterou jsi 11. 5. vložila, jsou v Notionu SummiD. Tam se nedostanu.** Proto jsem nemohla zkontrolovat, jestli kostra plní zadání slovo od slova. Pošli mi prosím jejich text. `[DOPLNIT]`

### Na co si dát pozor
1. **Překryv s ostatními přednáškami bloku Digitální provoz** (podle článku pořadatele):
   - Markéta Ubíková má Google Workspace, Gemini v práci a Gemini Notebook. → Gemini a NotebookLM u tebe jen zmínit, neukazovat do hloubky.
   - Daria Hvížďalová (Make) má „kde začít s AI transformací“. Mluví o výběru jedné agendy, testu na vzorku a měření. → Netlač na kroky „jak začít“, drž úhel „jak postavit systém, který přežije výměnu nástrojů“.
   - Vibecoding mají Hrubešová, Raková a Fáborský. → Claude Code a dashboardy u tebe nanejvýš jako krátká zmínka.
   - Kyberbezpečnost má Martin Konečný. → Tvoje guardrails ukaž jako *pravidla procesu*, ne jako přednášku o bezpečnosti.
2. **Úterní kolize:** podle Honzova posledního mailu Od UČO k IČO končí v **17:40**. KISKED20 („AI, LLM a osobní tech stack“) začíná v **17:45**. Máš na přepnutí 5 minut. Ráno máš navíc MP Dims fyzicky (10:00–11:30) a odpoledne MP Dims online (13:00–15:00). `[OVĚŘIT]`, jestli je to průchozí.
3. **Natáčí se a uvidí to tisíce lidí, natrvalo.** Na obrazovce nesmí být jména klientů, obsah mailů ani finance. Navrhuju demo profil prohlížeče a ukázkovou kopii složek (víc v části 4).

---

## 1. Analýza: tvoje procesy a vzorce organizovanosti

Zdroje:
- newslettery „Uklidila jsem si život. I ten digitální.“ (31. 8.), „Speciál: Jak vypadá druhý mozek, když ho spravuje AI agent“ (13. 9.) a „Asistenti končí, postupy zůstávají“ (4. 10.);
- kapitoly KISKED20 a CORE100 (druhý mozek, osobní techstack);
- checklist pro Signal;
- Plaud přepisy: Signal 21. 8., Claude skills 1. 7., Barlička 2. 10.;
- struktura štítků v Gmailu (jen názvy).

Samotné soubory vaultu (CLAUDE.md, guardrails, lessons learned, backlog) na Drivu nejsou, žijí zřejmě jen lokálně a v gitu. Vycházím proto z toho, jak je sama popisuješ.

### 1.1 Vzorce, které se opakují napříč vším

| # | Vzorec | Kde je vidět | Slovo pro přednášku |
|---|---|---|---|
| 1 | **Jedno místo pravdy** | Google Drive drží originály, vault na ně jen odkazuje. Finální materiály agent ukládá na Drive. Pro Signal: „Udrží tým DVĚ místa pravdy? Ne. Vyberte jedno.“ | data |
| 2 | **Nejdřív data, pak pravidla, teprve pak AI** | kapitola KISKED20, speciál z 13. 9. | metodika |
| 3 | **Ústava před obsahem** | CLAUDE.md jako „ústava“, persona-kaca.md, guardrails.md. Vznikly dřív než první obsah. | instrukce |
| 4 | **Proces je tvůj, nástroj je vyměnitelný** | CORE100; custom GPT končí 11. 12., Gemy se od 17. 11. převádějí na dovednosti; „Asistent byl zamčený v jedné aplikaci. Skill je váš.“ | proces |
| 5 | **OHIO podle tebe: třetí opakování ruční práce → nový postup (skill)** | první prompt v KISKED20; speciál: „Třetí opakování ruční práce → agent navrhne nový postup.“ | proces |
| 6 | **Chyba → pravidlo (lessons learned)** | 24 poučení za 5 týdnů. Pořadí: nejdřív zapsat poučení, pak opravit výstup. Příklady: mail sobě samé, datované reporty ve wiki, „tři pokusy nejsou tři důkazy, ale jeden důkaz třikrát“, „cenu rozhoduju já“. | metodika |
| 7 | **Autonomie jen v hranicích** | nic nemaže (jen karanténa „ke smazání“), maily neposílá (jen koncepty), finance neopustí počítač, do kalendáře jen bloky [NÁVRH], úkol se odškrtne jen s důkazem | organizovanost |
| 8 | **Neřídím seznam, ptám se systému** | ranní přehled, páteční rekapitulace, „co mi tento týden visí a jaká je priorita“ místo dlouhého seznamu úkolů. Na tebe dlouhé seznamy nefungují (tvoje zadání). | organizovanost |
| 9 | **Třídění na vstupu, ne úklid na výstupu** | Gmail: fronty `agent/odpovez`, `rozhodni`, `vyhrad-cas`, `nezapomen` a další; obchodní štítky `KLIENTI/…`, `SPOLUPRÁCE/…`, `BYZNYS/…`; znalostní `nachytři se` (asi 120 vláken). Inbox zero nepotřebuješ, agent čte jen výsek (hvězdičky a schválené odesílatele). | data |
| 10 | **Analýza dat → vlastní metodika** | tone of voice ze zhruba 50 nejlepších LinkedIn postů za 18 měsíců, 3 newsletterů a webu → profil → skill. „Musíte si to vysedět… není to za 5 minut.“ Skill jsi stavěla několikrát. | data → metodika |
| 11 | **Zachytit hned, zpracovat systémem** | Plaud → večerní zpracování → zápis klientům do 24 h. Zpětně 58 přepisů → 44 zápisů a 93 nesplněných slibů. | proces |
| 12 | **Úsudek si nechávám** | „Systému jsem předala evidenci a pamatování, ne úsudek.“ „Ty kontroly se prostě nezbavíš.“ | — |

### 1.2 Silné příběhy pro natáčení (konkrétní, tvoje, ověřené)
- **Asistenti končí** (custom GPT, Gemy): proč myslet v procesech. Nejlepší háček, protože se to týká skoro každého diváka.
- **Lessons learned v akci**: AI ti v nabídce sama navrhovala ceny → pravidlo „cenu rozhoduju já“. Krátké, lidské, pochopí to každý freelancer.
- **Persona**: „vím o sobě, že mě láká všechno a mám tendenci kývat… drž stranu mé vize, ne momentálního nadšení.“ Ukazuje, že kontext není jen o firmě, ale i o tobě.
- **Mantinel „nikdy nic nesmaž“** a složka „ke smazání“, kterou procházíš ručně.
- **Zpětný zátah 58 přepisů → 93 nesplněných slibů.** Silné číslo. `[OVĚŘIT]`, jestli ho chceš zveřejnit (je ve tvém newsletteru, takže asi ano).
- **Stěhování**: v létě jsi uklízela byt i digitální život zároveň (newsletter z 31. 8.). Může sloužit jako rámec celé přednášky, viz metafora níže. `[OVĚŘIT]`, jestli to chceš na video.

### 1.3 Nesrovnalosti, které je dobré vyjasnit před natáčením
- **OHIO:** obvyklý význam zkratky je „Only Handle It Once“ (věc vezmu do ruky jen jednou a hned rozhodnu). Ty jsi psala „One Handle It Once“ a ve vaultu ho používáš ve významu „co dělám podruhé nebo potřetí → postav na to skill“. Obojí dává smysl, ale na videu vyslov jasně, že *tvoje* verze je posun původního principu. Jinak se v komentářích někdo ozve. `[OVĚŘIT]` znění.
- **Štítky `agent/…` × mantinel „agent nesahá na štítky“:** v kalendáři je událost „Návrh z mailové triáže… obě vlákna mají štítek agent/vyhrad-cas“. Kdo štítky přiděluje? Na videu to musí sedět. `[DOPLNIT]`
- **Workflow „nachytři se“:** v podkladech je jen jedna věta („Cowork stahuje newslettery ze štítku nachytři se jako zdroj znalostí“). Pro ukázku potřebuju vědět, kam výstup ukládá a v jaké podobě. `[DOPLNIT]`
- **„Claude designer“ s brand manuálem:** myslíš Claude Design? Co přesně ukážeš (zadání → výstup v brandu)? `[DOPLNIT]`
- **Věta v zadání „TTo tvorbu kontextových dokumentů?“** je useknutá. Chtěla jsi kontextové dokumenty jako samostatné téma, nebo jako součást brand manuálu? `[DOPLNIT]`

---

## 2. Hlavní metafora: jedna, ne tři

V podkladech máš tři různé rámce:
- domeček o pěti patrech (data → nástroje → automatizace → AI parťák → strategie, CORE100),
- tři vrstvy (data → pravidla/kontext → AI),
- tvoje zadání: data → knowledge → metodika → instrukce.

Na 45 minut stačí **jeden obraz**. Návrh, který spojí všechny tři a sedí na název přednášky:

> **Digitální domeček: dům stojí, nábytek se stěhuje.**
> AI nástroje jsou nábytek. Když se změní ceník nebo produkt skončí, vyměníte židli. Dům (data, znalosti, metodika, instrukce) zůstane.

| Patro | Vrstva | Co tam je u tebe | Povinná slova |
|---|---|---|---|
| Základy | **Data** | jedno místo (Google Drive / Workspace), kontextová složka v Markdownu, štítky v Gmailu | data, organizovanost |
| Přízemí | **Knowledge** | kontextové dokumenty (o mně, persona, klienti), brand manuál, „nachytři se“ | data |
| 1. patro | **Metodika** | OHIO, lessons learned, postupy | metodika, proces |
| 2. patro | **Instrukce** | ústava, guardrails, skills | proces |
| Nábytek | **AI nástroje** | ChatGPT (skills, pluginy, Codex), Claude (Projects, Code, Design), Gemini (+ NotebookLM), Copilot (+ notebooks, OneDrive) | — |

Stěhování přitom dává přirozený rámec: „Letos jsem se stěhovala. Nábytek jsem si nesla s sebou, dům jsem si musela postavit znova.“ `[OVĚŘIT]`, jestli chceš.

---

## 3. KOSTRA KE SCHVÁLENÍ: SummiD, 45 min (natáčené, live demo)

**Jedna věta, kterou si divák odnese:** *Nástroje se mění každých pár týdnů. Kdo má data na jednom místě, sepsanou metodiku a instrukce mimo chatbota, vymění nástroj za odpoledne.*

**Emoční oblouk** (zahlcené publikum): klid → já → systém. „Nemusíte stíhat novinky“ → „takhle jsem to postavila já, i s chybami“ → „tady je postup pro vás“.

**Začátečníci i pokročilí:** v každém patře dvě úrovně. Pruh **„Zítra ráno“** je bez kódu (jedna složka, jeden dokument o mně, jeden projekt). Pruh **„Když chcete dál“** je Markdown, skills a agenti. Pokročilí uvidí tvůj skutečný systém, začátečník dostane první krok.

| Čas | Blok (kapitola pro střih) | Cíl | Demo / slide | Úroveň |
|---|---|---|---|---|
| 0:00–3:00 | **Úvod: asistenti končí** | háček a teze | Slide: data ukončení custom GPT (11. 12.) a Gemů (17. 11.) `[OVĚŘIT k 12. 10. i k premiéře 4. 11.]`. Otázka do kamery: „Kolik hodin práce máte zavřených v jednom chatbotu?“ Teze: dům a nábytek. | všichni |
| 3:00–6:00 | **Kdo jsem a proč mě to pálilo** | důvěra, ztotožnění | Deset profesí najednou (navazuje na úvodní text bloku). Dlouhé seznamy úkolů na mě nefungují. Stěhování a úklid. Prázdný pozemek domečku. | všichni |
| 6:00–13:00 | **Základy: data a jedno místo pravdy** | data, organizovanost | **Demo:** struktura Google Drive (demo kopie) + složka s Markdown kontextem + štítky v Gmailu (jen panel štítků, ne maily). Agent ukládá finální materiál na Drive. Věta: „Rozhodnutí o nástroji je vratné, rozhodnutí o pořádku ne.“ | Zítra: vyberte jedno místo. Dál: Markdown, štítky jako fronty. |
| 13:00–20:00 | **Přízemí: znalosti a kontext** | od dat ke knowledge | **Demo:** jak vznikl brand manuál a tone of voice analýzou (vstupy → profil → skill). Pak rychlý výstup v Claude Design s brandem `[DOPLNIT, co přesně]`. „Nachytři se“: štítek → znalosti `[DOPLNIT]`. | Zítra: jeden dokument „kdo jsem a jak píšu“. Dál: analýza vlastních textů. |
| 20:00–28:00 | **1. patro: metodika a procesy** | proces, metodika | **OHIO** (tvoje verze, viz 1.3). **Lessons learned**: ukázat soubor (anonymizovaný), příběh „cenu rozhoduju já“, „tři pokusy nejsou tři důkazy“. Persona „drž stranu mé vize“. | Zítra: zapište si 3 věci, které děláte opakovaně. Dál: lessons learned jako povinný krok. |
| 28:00–35:00 | **2. patro: instrukce** | instrukce mimo chatbota | Ústava a guardrails (nic nemaže, neposílá, finance zůstávají u mě). Skill = „postup zapsaný jednou, v jednom souboru“. **Demo, které dokazuje název přednášky:** *jeden a tentýž skill* ve dvou nástrojích (Claude + ChatGPT), u Gemini a Copilotu jen screenshot. Jedna věta o placených verzích. | Zítra: zkopírujte instrukce svého asistenta do dokumentu. Dál: knihovna skills s majitelem. |
| 35:00–40:00 | **Bydlíme: jak to vypadá v úterý ráno** | odměna: všechno do sebe zapadne | **Live demo:** „Co mi tento týden visí a jaká je priorita?“ Systém odpoví z mailů, kalendáře a přepisů. Úkoly v Gmailu jako rychlý přehled. Vrchol přednášky: dům odpovídá na jednu otázku. | pokročilí vidí cíl, začátečníci motivaci |
| 40:00–45:00 | **Závěr: 6 kroků + pozvánka** | akce | 6 kroků: jedno místo → ústava před obsahem → popsat sebe → pilot na malé oblasti → automatizovat až proces, který už běží → chyby měnit v pravidla. „Systému jsem předala evidenci a pamatování, ne úsudek.“ **Pozvánka na živý webinář 4. 11. + hodnocení pod videem.** | všichni |

**Co do přednášky záměrně nedávám:**
- přehled nástrojů jeden po druhém (4 chatboty × 5 minut by popřely název přednášky),
- Gemini a NotebookLM do hloubky (Ubíková),
- vibecoding a dashboardy (jiní řečníci),
- noční agenty a 70 agentů z univerzitního projektu (pro tohle publikum moc daleko; jen jako teaser na 4. 11.),
- Claude Code (jen jedna věta „pod kapotou mám Claude Code“).

---

## 4. Moje doporučení a tipy (natáčení a live demo)

1. **Nástroje jako důkaz, ne jako katalog.** Chceš ukázat ChatGPT, Claude, Gemini i Copilot. To je v konfliktu s vlastním názvem přednášky („Přestaňte měnit jen nástroje“) a na 45 minut je to moc. Řešení: ukázat stejný postup ve dvou nástrojích naživo a u zbylých dvou screenshot. Tím názorně předvedeš, že proces přežije výměnu nástroje.
2. **Demo data, ne skutečný provoz.** Udělej si samostatný profil prohlížeče s kopií složek bez klientů. V Gmailu ukazuj jen panel štítků. Je to i konzistentní s tvými guardrails: kdybys na video ukázala klientská data, popřela bys vlastní pravidla.
3. **Předpečené výstupy.** AI odpovídá pokaždé jinak a různě dlouho. Ke každému demu měj připravenou záložku s hotovým výstupem a screenshoty (pravidlo „záloha ke každému demu“). Ticho při čekání se dá vystřihnout, ale říkej nahlas, co se děje.
4. **Kapitoly pro střih.** Každé patro začni stejnou větou („Základy: data“). Postprodukce pak snadno vloží titulky a divák se orientuje.
5. **Bez publika mluv k jednomu konkrétnímu člověku** (třeba freelancerka s deseti profesemi z úvodního textu bloku). Vynech „vidíte mě?“ a dotazy do sálu.
6. **Technika na Macu:** vypnout notifikace, zoom 125–150 %, skrýt lištu záložek, zavřít ostatní okna. Dotaz na Renatu, jestli produkce chce rozlišení obrazovky 1920 × 1080. `[OVĚŘIT]`
7. **Šablona SummiD je povinná** (odkaz je v pozvánce do kalendáře). Slidů měj málo: zhruba 1 slide na patro, metafora domečku jako opakující se obrázek, který se postupně staví.
8. **Materiál ke stažení.** Checklist „Druhý mozek“ a 6 kroků jako PDF by dávaly smysl. `[OVĚŘIT]` u Renaty, jestli lze odkaz dát pod video.
9. **Úvodní háček ověř den předem.** Termíny ukončení GPT a Gemů se mohou posunout a video běží od 4. 11.

---

## 5. Úterý: Od UČO k IČO (návrh úpravy, ke schválení zvlášť)

Jiné publikum: **studenti před IČO**, ne zavedení podnikatelé. Mají méně dat a peněz a nejspíš free verze. Postavit ale můžou správně od prvního dne.

| Čas | Blok |
|---|---|
| 16:00–16:08 | Tvoje cesta k podnikání, kde tě IT a procesy zachránily a kde ne `[DOPLNIT příběh]` |
| 16:08–16:20 | Domeček, stejná metafora. Teze: „Začněte od základů, dokud je dům prázdný.“ Pojem *toolhopper*. |
| 16:20–16:40 | Základy a přízemí v praxi OSVČ, jen nástroje, které prokazatelně používáš: Google Workspace (jedno místo), fakturace ve Fakturoidu napojená na banku jen ke čtení, Plaud na schůzky, štítky v Gmailu, rezervační kalendář `[OVĚŘIT seznam]`. Profesionální minimum: vlastní doména a e-mail, 2FA, zálohy, správce hesel `[DOPLNIT, co používáš]`. |
| 16:40–16:48 | AI patro zkráceně: minimální stack „1 nastavený chatbot, 1 projekt, 1 místo na podklady“ (CORE100) a „asistenti končí, postupy zůstávají“ |
| 16:48–16:50 | 3 kroky na zítřek |
| 16:50–17:20 | Slido (připrav si 5 záložních otázek pro případ ticha) |

**Tip:** v úterý od 17:45 máš KISKED20 „AI, LLM a osobní tech stack“. Jednu sadu slidů (domeček) můžeš použít třikrát (SummiD, UČO, KISKED20) a jen měnit hloubku. To je tvoje OHIO v praxi a dá se to i říct nahlas.

---

## 6. Otázky pro tebe (jedna dávka)

1. Pošli text anotace a osnovy z Notionu SummiD.
2. Smím na video ukázat skutečný Drive a Gmail, nebo chystáme demo kopii? (Doporučuju kopii.)
3. Chceš použít příběh stěhování jako rámec?
4. Kdo přiděluje štítky `agent/…` (kvůli souladu s guardrails)?
5. Workflow „nachytři se“: kam a v jaké podobě ukládá výstup?
6. Co přesně ukážeš v Claude Design s brand manuálem?
7. Useknutá věta „TTo tvorbu kontextových dokumentů?“: samostatné téma, nebo součást brand manuálu?
8. Úterý: platí 17:40, nebo 17:30? Kolize s KISKED20 v 17:45 je pro tebe ok?

Po schválení kostry rozpracuju: přesný scénář vět pro každý blok, seznam záložek a demo souborů k přípravě v prohlížeči, seznam záloh (screenshoty) a zadání slidů do šablony SummiD.
