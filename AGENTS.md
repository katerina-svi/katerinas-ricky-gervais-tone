# AGENTS.md

Pokyny pro AI agenty (Claude Code, Codex apod.) pracující v tomto repozitáři.

## Co tento repozitář je

Přenositelný agent skill implementovaný čistě v Markdownu. Runtime artefakt je `SKILL.md`: YAML frontmatter (metadata) následovaný přepisovacím promptem. Žádný build, žádný kód.

## Klíčové soubory

- `SKILL.md` — skill samotný, zdroj pravdy. Striktní pravidla, persona, komediální motor, techniky, úrovně ostrosti, workflow a ilustrační příklad transformace.
- `README.md` — pro lidi: instalace, použití, mantinely, ukázka, historie verzí.
- `.claude-plugin/` — manifesty pro Claude Code plugin a single-repo marketplace.

## Kontrakt údržby

- `SKILL.md` a `README.md` musí zůstat v synchronu: při změně technik, úrovní ostrosti nebo pravidel aktualizuj i README a historii verzí.
- Verze se udržuje v `.claude-plugin/plugin.json` a v README (frontmatter `SKILL.md` pole `version` záměrně NEMÁ — validátor skillů v Claude.ai ho nepovoluje).
- **Sekce „Striktní pravidla" je jádro bezpečnosti tohoto skillu.** Žádná úprava nesmí oslabit ani obejít: zachování významu vstupu, zákaz kopírování konkrétních vtipů a formulací Rickyho Gervaise, pravidlo punch up (terčem je moc a pokrytectví, nikdy oběti či menšiny) a zákaz vtipů na konkrétní reálné soukromé osoby.
- Příklady v `SKILL.md` i `README.md` musí být původní — nikdy nevkládej skutečné hlášky Rickyho Gervaise ani jiného komika jako ukázku. Vždy vymysli nový příklad, který demonstruje mechaniku.
- Příklady musí samy splňovat pravidla skillu: punch up, žádný terč v podobě konkrétní reálné osoby, česká typografie dle IJP („ " uvozovky).
- Default úroveň ostrosti je 2. Pokud se mění, musí se změnit současně v `SKILL.md` (tabulka i workflow) a v README.
