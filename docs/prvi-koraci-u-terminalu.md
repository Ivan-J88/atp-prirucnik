# Prvi koraci u terminalu

[U ovom tutorialu naučit ćete kako koristiti terminal u programu Visual Studio Code.Tutorial će trajati 15 min.]

## Prije početka

- [Operacijski sustav koji ćemo koristiti u današnjem tutorijalu je Windows 11 te terminal u Visusal Studio Codu Git Bash.]
- Visual Studio Code je pokrenut, a u njemu je otvorena mapa [NITRO].

## 1. Otvorite terminal

U izborniku **Terminal** odaberite **New Terminal**.

**Očekivani rezultat:** [$/c/Users/NITRO]

## 2. Provjerite gdje se nalazite

```bash
pwd
```

**Očekivani rezultat:** [$/c/Users/NITRO]

## 3. Napravite mapu i uđite u nju

```bash
mkdir proba-terminala
cd proba-terminala
pwd
```

**Očekivani rezultat:** [Putanja završava nazivom mape proba-terminala]

## 4. Napravite datoteku i upišite u nju tekst

```bash
echo "# Moje bilješke" > biljeske.md
cat biljeske.md
```

**Očekivani rezultat:** [Nakon što ste unijeli naredbe očekivani rezultat trebao bi biti # Moje bilješke.]

## 5. Dodajte još jedan redak

```bash
echo "- Naredba pwd ispisuje gdje se nalazim." >> biljeske.md
cat biljeske.md
```

**Očekivani rezultat:** [Očekivani rezultat za unešene naredbe trebao bi biti "# Moje bilješke" te ispod "- Naredba pwd ispisuje gdje se nalazim".Ako ste dobili nesto drugo provjerite dali ste točno unijeli naredbe.]

[Znak `>` u postojećoj dadoteci briše sadržaj i mijenja ga novim ,a Znak `>>` postojeći sadržaj datoteke ostaje a novi se dodaje na kraj datoteke.]

## 6. Kopirajte, preimenujte i izbrišite datoteku

```bash
cp biljeske.md kopija.md
mv kopija.md stara.md
rm stara.md
ls
```

**Očekivani rezultat:** [ls nam ispisuje sadržaj mape nakon unesenih naredbi trebali bi dobiti biljeske.md ]

[Upozorenje: Terminal nema koš za smeće te se prije nardbe `rm` (izbriši) uvjerite u sadržaj mape i što brišete.]

## Ako ne radi


| Poruka | Što znači | Što učiniti |
|---|---|---|
| `No such file or directory` | [poruka  koja nam ukazuje da datoteka ili mapa ne postoje na toj lokaciji.] | [Provjerite naredbom pwd u kojoj se mapi trenutno nalazite te naredbu ls iskoristite da vam prikaže datoteke i mape koje se nalaze u toj mapi.] |
| [bash: pwwd: command not found] | [poruka koja ukazuje da naredba u ovom slučaju "pwwd" ne postoji ili je pogrešno napisana.] | [Upiši naredbu točno te pokušaj ponovo.] |

## Što dalje

[Više o naredbama može se naučiti u priručniku Srca *Uvod u Linux*, poglavlja 2 i 3.]
