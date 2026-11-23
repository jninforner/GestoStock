# GestoStock (inventari de peix i articles)

Respon sempre en català; Joan és principiant, explica pas a pas i una cosa cada vegada.

Llegeix `README.md`: hi ha el funcionament, el flux de treball i la numeració de versions. Resum de les regles:
- App d'un sol fitxer (`index.html`) + `sw.js` + `manifest.webmanifest`; sense compilació.
- Des de la 1.8.6: login amb els comptes de les apps Gesto (Firebase, configuració a `https://gesto-apps.jninforner.workers.dev/auth-config`) i inventari a D1 a través del Worker `gesto-apps` (`/GestoStock/api`, codi al repo privat GestoApps, `stock/api.mjs`). És **l'inventari real del restaurant**: no fer proves contra aquestes dades. Permisos `stock_*` a GestoAdmin.
- Fins a la 8.4 (l’última publicada amb Firebase): Firestore (projecte `control-de-peixos`, document `inventari/dades`). Es manté uns dies com a reserva després del canvi.
- Interpretació d'albarans: Worker de Cloudflare `nexamar-ia` (`nexamar-ia.mjs`, https://nexamar-ia.jninforner.workers.dev).
- Es treballa a `develop`; `main` és producció (GitHub Pages). **No fer commit ni push a `main` sense el vistiplau de Joan.**
- Cada canvi puja la versió (tres números, com les altres apps Gesto; criteri al README) a `index.html`, al README i al nom de la memòria cau de `sw.js`.
- L'app abans es deia NexaMar. Els noms interns (`nexamar-ia`, `window.nexamar*`, projecte `control-de-peixos`) es mantenen.
