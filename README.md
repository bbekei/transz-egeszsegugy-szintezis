# Felnőtt transznemű egészségügyi ellátás — bizonyíték-alapú szintézis és forráskritikai audit

Magyar nyelvű, akadémiai színvonalú, forráskritikai szintézis a **felnőtt (18+) transznemű egészségügyi ellátás** bizonyíték-bázisáról. A tanulmány 63 tudományos forrást dolgoz fel (ebből 62 aktív, 1 kizárt az audit során), három lektorálási körrel (Gemini, Grok, Copilot), és dokumentált verziótörténettel (v1 → v6).

**🌐 Olvasd online:** [tanulmany.html](https://bbekei.github.io/transz-egeszsegugy-szintezis/tanulmany.html) *(interaktív formátum, kereshető forrás-adatbázissal)*

**📋 Aktuális verzió:** v6 (2026. április 24.)

**✍️ Szerző:** Békei Balázs

---

## Miért készült ez a tanulmány

Fiatal felnőttek és kamaszok életében szinte elkerülhetetlen, hogy találkozzanak a transzneműség kérdésével — akár a közvetlen környezetükben, akár az interneten, akár az iskolában. Kérdéseik természetes módon merülnek fel, és az őszinte válasz fontos számukra. A közösségi médiában és a hírközlésben elérhető tartalom azonban **erősen polarizált**: a „gender-affirming care" feltétel nélküli elfogadását hirdető és az ellenoldali, részben politikailag motivált tartalmak rendre egymás ellenében fogalmazódnak meg, és a tárgyszerű, forrás-alapú áttekintés ritkábban jut el a nagyközönséghez, mint a véleménycikkek.

**Szülőként úgy érzem, felelősségem ebben a kérdésben tájékozottnak lenni**, és a gyermekeim számára pártatlan, tárgyszerű, tudományos információt nyújtani — olyat, amely segít őket **tények, és nem vélemények alapján** képet alkotni a jelenségről. Ez a célja a tanulmánynak: felkészülten tudjak beszélni velük, és szükség esetén olyan anyagot átadni nekik, amely a legjobb elérhető evidenciát összegzi, kiegyensúlyozottan és a vitákat is őszintén bemutatva.

A tanulmány **a 2026 áprilisában elérhető, tudományos igényességű információk szintézise**, amelyet néhány hét munkával és Claude (Anthropic), Gemini (Google), Copilot (Microsoft) és Grok (xAI) AI-eszközök használatával állítottam össze. Az AI-eszközök szerepe elsősorban a forráskeresésben, a szövegszerkesztésben és a lektorálásban volt jelentős; a munkafolyamat egyes részeinek pontos dokumentációja a §3 (Módszertan) és §8 (Külső AI-lektori vélemények) fejezetekben olvasható.

Nem klinikus vagyok és nem szakember a területen — érdeklődő szülő és olvasó, aki a saját legjobb tudása szerint igyekezett kiegyensúlyozott és forrás-alapú anyagot összeállítani. Minden érdemi szakmai visszajelzést, javítási javaslatot és további forrás-ajánlást köszönettel fogadok (ld. [Kapcsolat és visszajelzés](#kapcsolat-és-visszajelzés)).

---

## Mit tartalmaz ez a repository

| Fájl | Leírás | Méret |
|---|---|---|
| [`tanulmany.html`](./tanulmany.html) | A tanulmány interaktív HTML-formátuma, beépített szűrhető/kereshető forrás-adatbázissal | ~163 KB |
| [`tanulmany.md`](./tanulmany.md) | A tanulmány teljes szövege Markdown-formátumban (letölthető, idézhető, szerkeszthető) | ~138 KB |
| [`forrasok.csv`](./forrasok.csv) | A 63 forrás strukturált adatbázisa 18 oszloppal (szerző, év, folyóirat, DOI, bizonyíték-réteg, kulcs-állítás, audit-státusz stb.) | ~35 KB |
| `index.html` | Egyszerű landing page a projekthez | ~6 KB |
| `LICENSE` | CC BY 4.0 licenc | — |
| `README.md` | Ez a fájl | — |

---

## Miről szól a tanulmány

A tanulmány **nyolc** fő fejezetben tárgyalja a témát:

1. **Executive summary és köznyelvi kérdés-felelet** — rövid áttekintés + 10 gyakori kérdés közérthető válasszal
2. **Fogalomtár és magyarázó jegyzetek** — ~65 szakkifejezés 10 tematikus csoportban (diagnosztikai entitások, irányelvek, hormonkezelés/sebészet, epidemiológiai mérőszámok, klinikai állapotok, sebészeti komplikációk, vizsgálat-típusok, módszertani keretek, kutatói kohorszok, audit-specifikus fogalmak)
3. **Módszertan** — forrásgyűjtés, kizárási folyamat (1212 → 63), rétegzett bizonyíték-értékelés, háromszakaszos audit
4. **A revideált bizonyíték-alapú szintézis** — diagnosztika, hormonkezelés, sebészet, pszichés kimenetel, detranzíció, nemzeti felülvizsgálatok; abszolút kockázat-kommunikáció és LTFU% áttekintő táblázatokkal
5. **Audit-eredmények** — teljeskörű, 63-forrásos háromszakaszos ellenőrzés dokumentációja
6. **Limitációk** — időbeli, földrajzi, módszertani vakfoltok őszinte elismerése
7. **Záró értékelés**
8. **Külső AI-lektori vélemények és módszertani megfigyelések** — a Gemini, Grok és Copilot lektorálás részletes dokumentációja, beleértve egy Gemini hallucinációs epizódot és a három lektor eltérő megbízhatósági profiljának elemzését

---

## Módszertani kulcspontok

- **AI-asszisztált narratív szintézis** — nem előre regisztrált szisztematikus review; a transzparencia érdekében a módszertan részletesen dokumentált (§3).
- **Háromszakaszos forrás-audit** — a 63 forrás mindegyikét bibliográfiai és tartalmi szinten ellenőriztük (a „nem ellenőrizhető" kategória felszámolva). Az audit-hibák (pl. Manrique 2018 hibás DOI, Thornton 2024 kizárása azonosíthatatlanság miatt) dokumentáltan javítva.
- **Három külső AI-lektor** — Gemini 3 Thinking, xAI Grok, Microsoft Copilot. A lektorok eltérő teljesítménye (konfabuláció, plauzibilitási rábólintás, kalibrált bizonytalanság) önmagában is módszertani tanulság.
- **Abszolút és relatív kockázat-kommunikáció** — a szokásos SIR/SMR/HR mutatókat abszolút többletkockázatra (/1000 personyear) is átszámítottuk a klinikai értelmezhetőség érdekében.
- **Nyílt verziótörténet** — minden verzió (v1 → v6) változásai dokumentáltak, a hibák javításai nyomon követhetők.

---

## Hogyan használd

**Ha átfogó képet akarsz kapni:** olvasd az `tanulmany.html`-t a böngészőben (§1 Executive summary → §4 Szintézis → §8 Lektorálás).

**Ha egy konkrét forrást keresel:** a `forrasok.csv` nyitható Excelben/LibreOffice-ban, vagy használd az `tanulmany.html` §5 fejezetében található interaktív forrás-keresőt.

**Ha a saját kutatásodhoz idézni szeretnéd:** a javasolt hivatkozási formátum a tanulmány legvégén található. A repo GitHub-releases funkciójával konkrét verzió-címkét (pl. `v6.0`) lehet hivatkozni.

**Ha módszertani kérdésed van az AI-asszisztált tudományos munkára vonatkozóan:** a §8 fejezet részletesen dokumentálja a lektori epizódokat, beleértve egy Gemini hallucinációs esetet és annak módszertani tanulságait.

---

## Fontos figyelmeztetések

⚠️ **Ez nem klinikai tanács.** A tanulmány tudományos szintézis és forráskritikai elemzés. Klinikai döntésekhez mindig konzultálj szakorvossal.

⚠️ **A téma erősen polarizált.** A tanulmány kiegyensúlyozott forrás-mixet választott (WPATH SOC-8 + nemzeti felülvizsgálatok, mint Cass/SBU/COHERE + BMJ kritikai újraelemzések), és a vitákat mind tudományos, mind orvoslás-filozófiai szempontból bemutatja.

⚠️ **AI-asszisztált munka.** A tanulmányt Claude (Anthropic) AI-asszisztens állította össze a szerző iránymutatása szerint. Az AI-lektori körök hibáit (pl. Gemini hallucinációs epizód) nyíltan dokumentáljuk (§8). A végső szakmai validálás a szerző felelőssége.

---

## Licenc

A tanulmány a **Creative Commons Attribution 4.0 International (CC BY 4.0)** licenc alatt áll. Ez azt jelenti, hogy szabadon megoszthatod, másolhatod, módosíthatod és felhasználhatod (akár kereskedelmi célra is), feltéve, hogy megadod a megfelelő hivatkozást.

Részletek: https://creativecommons.org/licenses/by/4.0/deed.hu

---

## Hivatkozási javaslat

Ha tudományos vagy publicisztikai munkában idézed:

```
Békei Balázs. (2026). Felnőtt transznemű egészségügyi ellátás: 
bizonyíték-alapú szintézis és forráskritikai audit. v6. 
GitHub: https://github.com/bbekei/transz-egeszsegugy-szintezis/
```

Ha Zenodo DOI-t is regisztrálsz a projekthez, az idézési forma kiegészül a DOI-val.

---

## Verziótörténet (rövid)

| Verzió | Dátum | Fő változások |
|---|---|---|
| **v1** | 2026.04.19 | Eredeti szintézis, 63 forrás |
| **v2** | 2026.04.20 | Belső audit + revízió a 18 rétegzett mintán |
| **v3** | 2026.04.20 | Gemini 3 Thinking lektorálás, hallucinációs epizód dokumentálása |
| **v4** | 2026.04.20 | Teljeskörű audit (63/63 forrás) + „nem ellenőrizhető" kategória felszámolása (63 → 62 aktív forrás) |
| **v5** | 2026.04.20 | Fogalomtár + forrásgyűjtési folyamat dokumentálása |
| **v6** | 2026.04.21 | Grok + Copilot lektorálás, abszolút kockázat + LTFU táblázatok, §4.4 alfejezet-tézisek, §8-§9 egyesítés |

Részletes verziótörténet a `tanulmany.html` végén található.

---

## Kapcsolat és visszajelzés

- **Hibajelzés, javítási javaslat:** GitHub Issues
- **Tudományos lektori megjegyzés:** Pull Request, vagy GitHub Discussions (ha engedélyezett)
- **Adathiány / újabb releváns forrás:** GitHub Issue a forrás javasolt DOI-jával és kulcs-állításával

Minden érdemi visszajelzést köszönettel fogadok és dokumentálok a következő verzióban.
