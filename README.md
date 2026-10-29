# Plateforme de logement étudiant à Rennes (nom de travail : Passe-Clé)

**Pour qui :** projet personnel (portfolio, puis potentiel projet entrepreneurial)
**État :** prototype de démo en ligne (annonces fictives), phase de test auprès d'étudiants ; **vrai site en construction dans `site/`** depuis le 2026-10-25 (Next.js + Supabase : comptes, publication avec photos, espace administrateur)
**Créé le :** 2026-10-19

## Le concept

Mettre en relation, à Rennes, les étudiants qui quittent leur logement et ceux qui en cherchent un, avec une visite virtuelle photo pièce par pièce et toutes les informations utiles, dont le nom et le contact du bailleur.

## Contenu du dossier

| Fichier | Rôle |
|---------|------|
| `prompt-claude-design.md` | Prompt à coller dans Claude Design pour obtenir les maquettes et le prototype |
| `index.html` | Prototype interactif généré par Claude Design (version du 2026-10-19), nettoyé pour être mis en ligne : en-tête HTML propre, langue française, `noindex` (démo non référencée). Photos ajoutées le 2026-10-21 (accueil, cartes, fiches, visite virtuelle) |
| `prompt-logo-claude-design.md` | Prompt à coller dans Claude Design pour obtenir le logo (3 pistes, déclinaisons, favicon) |
| `site/` | Le vrai site (Next.js + Supabase), avec son propre dépôt Git. Guide : `site/MISE-EN-LIGNE.md` |
| `photos/` | 26 photos d'illustration Unsplash (licence Unsplash), classées par pièce : entrée, pièce principale, séjour, cuisine, salle de bain, vue, immeuble. Crédits dans `photos/CREDITS.md` |

## Liens

- **Site de démo en ligne : https://passe-cle.vercel.app/** (hébergé sur Vercel, mis à jour automatiquement à chaque envoi sur GitHub)
- Code source : https://github.com/CharmesSoglohoun/passe-cle
- Prototype d'origine sur claude.ai (privé) : https://claude.ai/artifact/2xjGY1u4ZFvbFVNkYT7mcS
- Pour tester en local : double-cliquer sur `index.html`

## Prochaines étapes possibles

1. Générer les maquettes avec Claude Design et les ajuster
2. Valider le concept auprès de quelques étudiants (sondage, groupes Facebook étudiants de Rennes)
3. Développer le site (front, base de données, stockage des photos, comptes utilisateurs)
4. Vérifier les obligations RGPD (données des bailleurs et des étudiants) avant toute mise en ligne
