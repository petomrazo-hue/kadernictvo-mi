# Súhrn pre Dufeka: kadernictvo-mi (obnov PRED každým draftom, stráži dufek-draft-check kontrola e)

Stav k 26.11.2026, zdroje: project_kadernictvo_mi.md (pamäť), kadernictvo-mi/README.md, DENNIK.md (záznamy [kadernictvo-mi] 22. až 24.7.), dufek-posta-export.json (export 26.11.2026 13:17).

## Čo má Dufek u seba
- Web kadernictvomichalovce.sk (Madame hair & beauty, Umbraco 8) nasadený na produkcii; potvrdil 24.7. 17:59 ("Je to nasadené").
- Posledné odovzdané kolo 9 (commit 500bf27, push 24.7., mail 24.7. 15:39): väčšia fotka kaderníctva, vzorkovník pod logom Wella, Salón s popiskami, Instagram pod Facebookom, pozadie oddychová zóna; databáza v sample-db.sql.
- Recenzie (kolo 7, 1b11fba, mail 22.7. 16:35) a slovenské validačné hlášky (kolo 8, ec77ef9): honeypot, časová pasca, limit na IP, antiforgery token; Dufek to pozná, 6.10. na to odkázal pri zadaní FormGuard.
- Platba 250 € poslaná 21.7. (jeho mail z 22.7.), číslo účtu poslal Peto 22.7.
## Čo máme hotové a on o tom nevie
- nič: všetky odovzdané kolá 1 až 9 sú mailom oznámené a pushnuté, žiadny nepushnutý commit ani rozrobená práca (git: posledný zásah je auto-sync, nie zmena webu)
## Čo musí spraviť on
- Nič konkrétne nečakáme: poslal ďalší zákazky (24.7. avizoval ďalšie weby), tento web čaká len na pripomienky klientky.
## Otvorené
- Nezistené: či klientka po 24.7. poslala ďalšie pripomienky; v exporte pošty žiadny mail k tomuto webu po 24.7. nie je.
- Recenzie na tomto webe stále používajú starý anti-bot (honeypot, časová pasca, IP limit), nie FormGuard z dufeksoft.security; nikto nerozhodol, či ho prepnúť (Dufek 6.10. chcel jednotné riešenie na všetkých weboch, zadal len perfektweb a dufeksoft.com).
- Cena: 250 € zaplatené za pôvodnú zákazku; kolá 7 až 9 (recenzie, validácia, úpravy) bez samostatnej ceny.
