# GestoStock (inventari de peix i articles)

Respon sempre en català; Joan és principiant, explica pas a pas i una cosa cada vegada.

Llegeix `README.md`: hi ha el funcionament, el flux de treball i la numeració de versions. Resum de les regles:
- App d'un sol fitxer (`index.html`) + `sw.js` + `manifest.webmanifest`; sense compilació.
- Dades a Firestore (projecte Firebase `control-de-peixos`, document `inventari/dades`): és **l'inventari real del restaurant**. No fer proves contra aquestes dades. Login amb Firebase Auth.
- Interpretació d'albarans: Worker de Cloudflare `nexamar-ia` (`nexamar-ia.mjs`, https://nexamar-ia.jninforner.workers.dev).
- Es treballa a `develop`; `main` és producció (GitHub Pages). **No fer commit ni push a `main` sense el vistiplau de Joan.**
- Cada canvi puja la versió (seqüència del README) a `index.html` i al nom de la memòria cau de `sw.js`.
- L'app abans es deia NexaMar. Els noms interns (`nexamar-ia`, `window.nexamar*`, projecte `control-de-peixos`) es mantenen.
