NexaMar PWA
1. Puja tots els fitxers a l’arrel del repositori GitHub.
2. Settings > Pages > Deploy from a branch > main / (root).
3. Firebase Authentication > Settings > Authorized domains: afegeix USUARI.github.io.
4. Firestore Rules: limita l’accés al teu usuari, ruta inventari/dades.
5. Obre https://USUARI.github.io/NexaMar/ i inicia sessió.
IMPORTANT: no es migren automàticament les dades de l’HTML Viewer. Conserva l’original i exporta’n les dades abans de canviar.
La PWA requereix internet per carregar el SDK de Firebase el primer cop; el funcionament offline posterior depèn de la memòria cau del navegador.
