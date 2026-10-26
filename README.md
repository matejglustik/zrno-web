# Zrno – stránka s CMS

## Čo je čo
- `index.html` – samotná stránka (dizajn a animácie). Do nej sa nemusí siahať.
- `content/` – všetok obsah, ktorý sa mení: káva, menu, workshopy, kontakt.
- `admin/` – CMS. Otvorí sa na adrese `vasa-stranka.sk/admin`.

## Ako to nasadiť (raz)
1. Na github.com si vytvorte účet a nový repozitár (napr. `zrno-web`). Nahrajte do neho celý tento priečinok.
2. Otvorte `admin/config.yml` a riadok `repo:` zmeňte na `vaseMeno/zrno-web`.
3. Na netlify.com sa prihláste cez GitHub, zvoľte Add new site, Import from Git a vyberte repozitár. Stránka sa zverejní.
4. V nastaveniach stránky na Netlify povoľte prihlasovanie cez GitHub (OAuth provider GitHub). Presný postup nájdete v dokumentácii Decap CMS pre Netlify, názvy menu sa môžu líšiť.
5. Otvorte `vasa-stranka.sk/admin`, prihláste sa cez GitHub a upravujte.

## Ako upravovať
V `/admin` vyberte Káva, Menu, Workshopy alebo Nastavenia, zmeňte text či cenu a kliknite Publish. Zmena sa uloží do GitHubu a stránka sa sama aktualizuje za minútu až dve.

## Ďalší editori
Editor si založí bezplatný GitHub účet. Vy ho pridáte v repozitári v Settings, Collaborators. Potom sa prihlási do `/admin` rovnako ako vy.

## Poznámky
- Pri otvorení `index.html` priamo z disku sa obsah nenačíta. Stránka musí bežať cez server alebo hosting.
- Košík a objednávky sú ukážka. Na skutočný predaj treba platobnú bránu (napr. Stripe alebo Snipcart).
- Rozhranie CMS je v angličtine, polia a popisy sú po slovensky.
