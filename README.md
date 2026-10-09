# KontaktnaStran

Kontaktna stran Borisa Potočnika z logotipom BP, povezavami za telefon, Gmail,
spletno stran in LinkedIn ter gumbom za shranjevanje kontakta.

Stran je napisana v HTML in CSS. Ne potrebuje nameščanja paketov, sestavljanja
ali strežnika za aplikacijo.

## Objava na Vercelu

1. V Vercelu izberi **Add New → Project**.
2. Uvozi GitHub repozitorij **Borci1417/KontaktnaStran**.
3. Root Directory naj ostane koren repozitorija (`./`).
4. Klikni **Deploy**.

Datoteka `vercel.json` že nastavi **Framework Preset: Other**, prazna ukaza
Build Command in Install Command ter **Output Directory: dist**.
Okoljske spremenljivke niso potrebne.

Po objavi naj QR-koda na vizitki vodi na končni javni naslov te kontaktne strani.

## Datoteke

- `dist/index.html` — kontaktna stran in njeno oblikovanje.
- `dist/bp.svg` — logotip BP.
- `dist/kontakt.vcf` — kontakt za prenos v imenik, vključno s spletno stranjo in LinkedInom.
- `dist/robots.txt` — navodilo iskalnikom, naj strani ne indeksirajo.
- `vercel.json` — nastavitve objave in prenosa kontakta.

## Urejanje

Besedilo in povezave uredi v `dist/index.html`. Ob spremembi kontaktnih podatkov
posodobi tudi `dist/kontakt.vcf`.

Povezava do predstavitvene strani se konča z `/en`:
https://boris-potocnik-predstavitvena.vercel.app/en

## Lokalni predogled

V korenu repozitorija zaženi:

```sh
python3 -m http.server 8000 --directory dist
```

Odpri http://localhost:8000.
