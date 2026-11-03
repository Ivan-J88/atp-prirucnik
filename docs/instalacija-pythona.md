# Instalacija Pythona i prvi program

## 1. Instalacija Pythona

Python je programski jezik koji možemo koristiti na Windows i macOS sustavima.

### Instalacija Windows
- otvoriste službenu stranicu [https://www.python.org/downloads/]
- preuzmite instalacijsku datoteku za Windows
- pokrenite instalaciju
- označite opciju Add Python to PATH
- Kliknite install now

### instalacija macOS
- otvorite [https://www.python.org/downloads/macOS]
- preuzmite instalacijsku datoteku za macOS
- otvorite preuzetu datoteku
- slijedite korake instalacije

## 2. Razlika između Windowsa i macOS-a

| Windows | macOs |
|---|---|
| Preuzimanje s python.org | Preuzimanje s python.org |
|instalacijska `.exe` datoteka | instalacijska `.pkg` datoteka |
| provjera verzije `python --version` | provjera verzije `python3 --version` |
| Visual Studio Code | Visual Studio Code |

## 3 Provjera instalacije

```bash
python --version   # Windows
python3 --version  # macOS
```

**Očekivani rezultat:** 3.14.7 ili noviji znaci da je pyhon instaliran i da je prepoznat u terminalu

## 4 . Prvi Python program

Nakon instalacije Pythona možemo napisati svoj prvi program.Python kod pišemo u datoteci koja završava s `.py`

Možemo napisati jednostavnu naredbu koja će ispisati poruku:

``` python
print("Volim python!")

kada pokrenemo program terminal će ispisati

Volim python!

