# PHLAME — Vente privée (ventes.phlame.fr)

Configurateur de commande pour la vente privée PHLAME (produits test).
Site statique autonome (1 fichier `index.html`), indépendant de la boutique Shopify `phlame.fr`.

## Contenu
- `index.html` — la page (HTML + CSS + JS, sans dépendance, polices Google Playfair Display + Lora).
- `CNAME` — domaine personnalisé GitHub Pages : `ventes.phlame.fr`.

## Fonctionnement
- 4 produits : Bougie, Diffuseur voiture Kheops, Spray, Diffuseur d'huiles essentielles.
- Par produit : ajout/retrait de lignes (« + » / « − »), choix de la senteur ; colorant uniquement
  sur les bougies (s'affiche après le choix de la senteur).
- Disponibilité des senteurs gérée par produit (HE = Coco & Papaye + Monoï uniquement ;
  Brioche au Beurre & Cerise Noire Explosive exclues des bougies).
- Prix avec remise « lot de 2 » automatique ; total calculé en direct.
- Génération d'un e-mail pré-rempli (coordonnées + commande) vers **societe@phlame.fr**
  (bouton « Ouvrir dans ma messagerie » + « Copier l'e-mail »). Aucun serveur requis.

## Mise en ligne (GitHub Pages + OVH)
1. Créer un repo GitHub (ex. `phlame-ventes`), pousser le contenu de ce dossier.
2. Settings → Pages → Source : branche `main`, dossier `/ (root)`.
3. Le fichier `CNAME` configure le domaine `ventes.phlame.fr` ; cocher « Enforce HTTPS ».
4. Chez OVH (zone DNS de `phlame.fr`) : ajouter un enregistrement **CNAME**
   `ventes` → `nebuyr168.github.io.` (point final inclus).

Prix et règles : voir le classeur `Couts de revient PHLAME.xlsx`.
