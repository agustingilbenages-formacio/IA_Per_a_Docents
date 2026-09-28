# Intel·ligència Artificial aplicada a la docència — web de la formació

Web estàtica (sense dependències, sense cookies, sense serveis de tercers) de la formació
**«Intel·ligència Artificial aplicada a la docència — De la IA generativa als agents i nous fluxos de treball»**, d'Agustín Gil Benages.

- `index.html` — pàgina principal (5 blocs, metodologia, avaluació, ponent, FAQ, contacte). Imprimible a PDF sencera o per bloc.
- `questionari.html` — test «Quin és el meu nivell en IA?» (12 preguntes, 5 nivells, resultat imprimible). Tot es calcula al navegador.
- `descarregues/` — PPTX de cada bloc + PPTX i PDF de la formació completa.
- `img/` — il·lustracions (les pàgines ja les porten incrustades).
- `_build/` — plantilles i scripts Python per a regenerar `index.html`, `questionari.html` i les PPTX
  (`python3 _build/build_index.py`, `python3 _build/build_quiz.py`, `python3 _build/build_pptx.py`; cal `python-pptx`).

## Publicar amb GitHub Pages
1. Crea un repositori a GitHub (p. ex. `ia-docencia`).
2. Puja este contingut: `git remote add origin https://github.com/USUARI/ia-docencia.git && git push -u origin main`
3. A GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. En un minut la web estarà a `https://USUARI.github.io/ia-docencia/`.

## Privacitat
No s'usa cap cookie, analítica ni font externa; el qüestionari no envia dades. El correu de contacte està ofuscat al codi.
