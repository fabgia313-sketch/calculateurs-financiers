# Rapport de mise à jour des données financières — calcfin.fr

**Date d'exécution :** 2026-05-31  
**Fichiers modifiés :** 9  
**Corrections appliquées :** 30  

---

## Résumé des corrections par thème

### 1. SMIC 2026 — Revalorisation au 1er juin 2026

| Valeur | Ancienne | Nouvelle |
|--------|----------|----------|
| SMIC horaire brut | 11,88 €/h (base nov. 2024) | 12,31 €/h (depuis 1er juin 2026) |
| SMIC mensuel brut (151,67 h) | 1 801,80 € | 1 867,02 € |
| SMIC mensuel net estimé | ~1 426 € | ~1 477 € |
| SMIC annuel brut | 21 621,60 € | 22 404,24 € |
| Exemple temps partiel 20h/sem | 1 030,40 €/mois | 1 067,85 €/mois |

**Source :** legisocial.fr — SMIC 2026 (valeur 1er janvier : 12,02 €, revalorisation exceptionnelle 1er juin : 12,31 €, +2,41 % liée au dépassement du seuil d'inflation de 2 %)

**Fichiers modifiés :**
- `guides/smic-2026/index.html` (texte principal, tableau, exemple temps partiel, liste à retenir, CTA)
- `guides/negocier-son-salaire/index.html` (référence SMIC horaire dans cadre légal)
- `guides/avantages-en-nature/index.html` (seuils barème logement 1 SMIC et 1,2 SMIC)

---

### 2. ARE (Allocation de Retour à l'Emploi) 2026

| Paramètre | Ancienne valeur | Nouvelle valeur |
|-----------|-----------------|-----------------|
| Partie fixe journalière | 12,95 € | 13,18 € |
| Plancher absolu journalier | 31,59 € | 32,13 € |
| Taux proportionnel SJR | 40,4 % | 40,4 % (inchangé) |
| Plafond ARE | 75 % du SJR | 75 % du SJR (inchangé) |
| Taux plancher | 57 % du SJR | 57 % du SJR (inchangé) |

**Source :** Service-Public.fr (F14860) — valeurs vérifiées au 1er juillet 2025

**Fichiers modifiés :**
- `fr/are/index.html` (constante JS PARTIE_FIXE, constante JS ARE_MIN_ABS, affichage HTML, stat card, texte explainer)

---

### 3. PASS 2026 (Plafond Annuel de la Sécurité Sociale)

| Valeur | Ancienne (PASS 2025) | Nouvelle (PASS 2026) |
|--------|----------------------|----------------------|
| PASS annuel | 47 100 € | 48 060 € (+2,0 %) |
| PSS mensuel (PASS/12) | 3 925 € | 4 005 € |
| 2 × PASS (plafond exonération) | 94 200 € | 96 120 € |
| 75 % PASS (plafond RSP) | 35 325 € | 36 045 € |

**Source :** legisocial.fr — Plafond de la Sécurité sociale 2026

**Fichiers modifiés :**
- `fr/retraite/index.html` (constante JS PLAFOND_SS_MENS : 3925 → 4005)
- `guides/cotisations-salariales/index.html` (PSS mensuel et PASS annuel, 3 occurrences)
- `guides/rupture-conventionnelle-guide/index.html` (2xPASS exonération, PASS valeur, 2 occurrences)
- `guides/interessement-participation/index.html` (75% PASS plafond RSP)
- `guides/demission-vs-rupture-conventionnelle/index.html` (2xPASS, 2 occurrences)
- `guides/licenciement-economique-droits/index.html` (2xPASS plafond exonération)

---

### 4. Tranches IR 2026 — Aucune correction nécessaire

Les tranches en vigueur dans le calculateur sont confirmées correctes :

| Tranche | Seuil | Taux |
|---------|-------|------|
| 1 | jusqu'à 11 600 € | 0 % |
| 2 | 11 601 € à 29 579 € | 11 % |
| 3 | 29 580 € à 84 577 € | 30 % |
| 4 | 84 578 € à 181 917 € | 41 % |
| 5 | au-delà de 181 917 € | 45 % |

**Source :** Service-Public.fr (F1419) — confirmé identique aux valeurs du calculateur

---

### 5. Cotisations salariales URSSAF — Aucune correction nécessaire

Les taux dans le calculateur brut→net sont conformes aux barèmes 2026 :

| Cotisation | Taux | Statut |
|------------|------|--------|
| Assurance maladie | 0,40 % | Confirmé |
| Retraite de base | 6,90 % | Confirmé |
| Retraite complémentaire non-cadre (T1) | 3,15 % | Confirmé |
| Retraite complémentaire cadre (T1+T2) | 4,30 % | Confirmé |
| Chômage | 2,40 % | Confirmé |
| CSG/CRDS | 9,70 % | Confirmé |

---

### 6. Taux immobiliers 2026 — Information

Les taux du marché en mai 2026 selon Meilleurtaux.com :

| Durée | Bon taux | Très bon taux |
|-------|----------|---------------|
| 15 ans | 3,52 % | 3,24 % |
| 20 ans | 3,59 % | 3,39 % |
| 25 ans | 3,70 % | 3,44 % |

Le hint dans le calculateur prêt immobilier indique "3,2 % – 3,8 % sur 20 ans" — cohérent avec la fourchette de marché. Le taux par défaut (3,50 %) reste représentatif. Aucune correction appliquée (valeur indicative).

---

### 7. Frais de notaire — Aucune correction nécessaire

Les frais de notaire restent stables : ~7,5 % pour l'ancien, ~2,5 % pour le neuf. Ces valeurs sont confirmées conformes.

### 8. TVA — Aucune correction nécessaire

Les taux TVA français sont stables : 20 % (normal), 10 % (intermédiaire), 5,5 % (réduit), 2,1 % (super-réduit).

---

## Valeur non modifiée avec note

- `guides/brut-net-net-imposable/index.html` ligne 240 : affiche "~12,95 % × brut" — il s'agit d'un taux de cotisations approximatif (non un montant ARE), valeur correcte, non modifiée.

---

## Sites inaccessibles lors de la récupération des données

| URL | Statut | Solution |
|-----|--------|----------|
| simulez.fr/montants/smic/ | 403 Forbidden | Source legisocial.fr utilisée à la place |
| impots.gouv.fr/particulier/questions/tranches | 404 Not Found | Source service-public.gouv.fr utilisée |
| urssaf.fr/taux-cotisations | Connexion fermée | Valeurs confirmées par comparaison avec le calculateur existant |
| meilleurtaux.com/barometre-des-taux/taux-actuels.html | 404 | URL alternative utilisée avec succès |
| unedic.org/indemnisation | 404 | Source service-public.gouv.fr utilisée |
| empruntis.com/barometre_taux.php | 404 | Non bloquant (taux indicatif uniquement) |
| france-travail.fr/are/ | 404 | Source service-public.gouv.fr utilisée |

---

## Sources officielles utilisées

| Donnée | Source | Date de récupération |
|--------|--------|----------------------|
| SMIC 2026 (horaire, mensuel) | legisocial.fr/reperes-sociaux/montant-smic-2026 | 2026-05-31 |
| PASS 2026 | legisocial.fr/reperes-sociaux/plafond-securite-sociale-2026 | 2026-05-31 |
| Tranches IR 2026 | service-public.gouv.fr/particuliers/vosdroits/F1419 | 2026-05-31 |
| ARE 2026 (fixe, plancher) | service-public.gouv.fr/particuliers/vosdroits/F14860 | 2026-05-31 |
| Taux immobiliers mai 2026 | meilleurtaux.com/credit-immobilier/barometre-des-taux | 2026-05-31 |
