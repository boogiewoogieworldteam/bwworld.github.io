# bwworld.github.io
<!-- FILE: README.md -->
# Boogie Woogie World — Sito statico


Questo progetto è un sito **statico** pronto da distribuire su **GitHub Pages** o **Netlify**. Contiene le pagine richieste: **Home**, **Latest (news)**, **Videos**, **WRRC (start list & risultati)**.


## Come usare (deploy rapido su GitHub Pages)
1. Crea un repository su GitHub (pubblico va bene).
2. Copia i file di questo progetto nella root del repository.
3. Commit & push.
4. Vai su Settings → Pages → Branch: seleziona `main` e `/(root)` → Save.
5. Dopo qualche minuto il sito sarà disponibile su `https://<tuo-username>.github.io/<repo>/`.
6. Per usare il dominio personalizzato, aggiungi un file `CNAME` con `bwworld.tuodominio` nella root e aggiorna i DNS (vedi sotto).


## DNS (collegare dominio acquistato a GitHub Pages)
- Se usi **GitHub Pages con repository user/organization site** (nome repo = `<username>.github.io`):
- Imposta un record **A**: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- Aggiungi file `CNAME` con il tuo dominio.
- Se usi **Netlify**: crea un sito su Netlify e collega il repo; Netlify fornisce record CNAME/ALIAS da impostare.


## Come aggiornare contenuti
- **News (Latest)**: modifica `data/news.json` (opzionale) o apri `latest.html` e aggiungi blocchi `article`.
- **Videos**: incolla embed YouTube o link Instagram; consiglio YouTube/Vimeo per affidabilità.
- **WRRC**: aggiorna `data/wrrc.csv` o modifica `wrrc.html` con le tabelle. Il file `main.js` include una funzione per caricare CSV statici e renderizzarli.


---
