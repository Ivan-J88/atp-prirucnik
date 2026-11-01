# Prvi koraci s Pandocom

Trajanje:20 min 

Provjereno s Pandocom [3.13] na sustavu Windows 11 u terminalu Git Bash.

## Prije početka

- Prije početka morate imati instaliran Visual Studio Cod,instaliran Git Bash,instaliran Pandoc i pripremljenu README.md datoteku

## 1. Instalirajte Pandoc

### Windows

Otvorite službenu stranicu [https://pandoc.org/installing.html],preuzmite `pandoc-…-windows-x86_64.msi` ako koristite Windows.Pokrenite ga i slijedite korake. Nakon instalacije zatvorite i ponovno otvorite VS Code.
### macOS



## 2. Provjerite instalaciju

```bash
pandoc --version
```

**Očekivani rezultat:** Prvi red vam ispisuje pandoc `3.13` ili novija verzija

## 3. Pretvorite Markdown u Word
```bash
mkdir izlaz
pandoc REDAME.md -o izlaz/README.docx
```
**Očekivani rezultat:** U mapi `izlaz` pretvorit ćemo datoteku `README.md` u Word datoteku `README.docx` .Otvorite je u programu Word i trebali bi vidjeti da su naslovi Wordovi stilovi Heading 1 i Heading 2 te da su i ostali elementi pravilno oblikovani.

## 4. Pretvorite Markdown u web-stranicu

```bash
mkdir izlaz
pandoc README.md -s -o izlaz/README-samostalno.html
```
**Očekivani rezultat:**U mapi `izlaz` pretvorit ćemo datoteku `README.md` u web-stranicu HTML,opcija -s(standalone) nam omogućuje da se pri pretvaranju u Markdown datoteke u HTML izradi potpuno nova HTML web stranica.Otvorite je u VS Codeu: desni klik → Reveal in File Explorer , pa dvaput kliknite.

## Ako ne radi

| Poruka | Što znači | Što učiniti |
|---|---|---|
| `command not found` | [ Pandoc nije prepoznao naredbu] | [ Provjerite dali je instaliran pandoc i dodan PATH,zatvorite i ponovo pokrenite VS Code] |

## Što ste napravili

U tutorialu ste naučili instalirati Pandoc i provjeriti njegovu verziju,pretvaranje Markdown datoteke u Word i HTML format te kako napravljene datoteke spremiti u našem slučaju u mapu `izlaz`.Također smo obradili jednu od najčešćih pogrešaka i njeno rješenje.