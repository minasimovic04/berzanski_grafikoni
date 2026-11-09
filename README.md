#Generisanje grafikona

Python skripta koja preuzima istorijske berzanske podatke sa Yahoo Finance-a za spisak kompanija iz `tickers.txt` fajla i automatski generise grafikone.
Sta kod radi:
- Čita berzanske simbole iz tekstualnog fajla
- Preuzima podatke za poslednjih 6 meseci preko `yfinance` biblioteke
- Racuna 20-dnevni i 50-dnevni pokretni prosek (MA20 / MA50)
- Čuva grafikone u folderu `izvestaji/`
- Koristi `try-except` blokove kako greska na jednom ticker-u ne bi prekinula izvrsavanje

