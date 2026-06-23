# JMC – web

Statický web firmy JMC a.s. (jedna stránka, čisté HTML/CSS/JS).

## Struktura
- `index.html` – celý web (HTML, CSS i JS v jednom souboru)
- `.gitignore` – ignorované soubory

## Nasazení (deploy)
Web hostuje **Netlify** a nasazuje **automaticky z GitHubu**.
Po jakékoli úpravě stačí změnu odeslat na větev `main`:

```bash
git add -A
git commit -m "popis změny"
git push
```

Netlify do ~1 minuty změnu nasadí. Žádný build krok není potřeba
(publish directory = kořen repozitáře, build command = žádný).

- Živý web: https://jmc-web.netlify.app
- GitHub repo: https://github.com/mblazoo/jmc-web

## Poznámky
- Vždy uprav `index.html` a po dokončení proveď commit + push (viz výše),
  jinak se změny na web nepromítnou.
