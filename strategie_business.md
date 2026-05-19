# Stratégie Business — App de gestion d'EDT multi-écosystèmes

> Document de travail interne — v1, mai 2026

---

## 1. Le problème qu'on résout

Beaucoup de gens vivent simultanément dans **plusieurs écosystèmes de calendrier et d'email** qui ne se parlent pas : Google Workspace (école, perso), Microsoft Outlook (entreprise), Apple iCloud (perso). Aucun outil grand public ne fait la sync intelligente des trois en gardant le contexte de chaque "monde".

Les outils existants (Motion, Reclaim, Sunsama, Akiflow, Amie) visent les pros B2B et ignorent cette douleur "multi-vies".

---

## 2. Notre positionnement

> **Le calendrier qui suit la transition école → vie pro.**
> On accompagne les jeunes actifs depuis leur alternance jusqu'à leur premier poste, dans tous leurs écosystèmes (Google, Microsoft, Apple).

**Pourquoi c'est défendable :**
- Motion ne fera pas ça (trop B2B pur).
- Notion non plus (pas un calendrier).
- Personne ne cible la jonction école/pro avec une vraie continuité produit.

**Vision long terme (3 ans) :** étendre aux populations qui vivent dans plusieurs calendriers subis — soignants, ouvriers postés, parents en double activité.

---

## 3. Personas cibles

### Persona principal — Léo, 22 ans, alternant

- Master 1 école d'ingé, alternance dans une scale-up.
- 3 écosystèmes : Google Workspace école, Outlook entreprise, iCloud perso.
- Douleur : double-booking entre cours et réunions, oubli de deadlines, stress de jonglage.
- **Ne paie pas.** Sert d'acquisition virale et de top of funnel.

### Persona secondaire monétisable — Camille, 24 ans, jeune diplômée

- Sortie d'alternance, première vraie job (Data Analyst, Product, etc.).
- 38–45k€/an, premiers revenus stables.
- Paie déjà pour Notion, Spotify, ChatGPT, Headspace.
- Douleur : transition école→pro mal gérée, FOMO d'optimisation, veut "être organisée comme une adulte".
- **Paie 9–12€/mois sans hésiter.**

### Logique de funnel

```
Alternants (gratuit, viral) ──► Jeunes diplômés (Pro 9€/mois)
   acquisition                      monétisation
```

Un seul produit, deux étages du funnel. Même stack technique, même UX, même backend.

---

## 4. Offres

| Offre | Cible | Prix | Contenu |
|---|---|---|---|
| **Free / Student** | Alternants, étudiants | 0€ | 1–2 calendriers connectés, sync basique, mobile + web |
| **Pro** | Jeunes diplômés, freelances | ~9€/mois | Multi-comptes illimités, suggestions IA, deep-work blocks, intégration emails (parsing → events) |
| **Team / Business** *(plus tard)* | Petites équipes | ~15–20€/user/mois | Partage de dispos, scheduling de groupe, analytics, SSO |

**Règle :** on ne lance pas les 3 d'un coup. **Pro en premier**, Free dès qu'on a de la traction, Team uniquement sur demandes entrantes.

---

## 5. Différenciation produit

Le wedge à valider en MVP — il faut que **une chose soit excellente**, pas tout au niveau moyen :

- **Sync multi-écosystèmes fluide** (Google + Microsoft + Apple). C'est notre socle technique différenciant.
- **Contexte préservé** : un événement "Cours" ne se mélange pas visuellement avec un événement "Réunion client".
- **Migration douce école→pro** : quand l'alternant devient jeune diplômé, on déplace proprement ses habitudes vers son nouveau compte pro.

À écarter du MVP pour rester focus : scheduling de groupe, time tracking, intégrations Notion/Slack, etc.

---

## 6. Modèle économique

- **Politique "no income no investment"** — uniquement des outils gratuits tant qu'il n'y a pas de revenu.
- Pas de levée prévue à court terme.
- Monétisation différée : on accepte de ne rien gagner pendant 12–18 mois pour construire la base alternants, puis on convertit à la sortie d'études.
- Objectif de conversion alternant → Pro : **8–12 %** à la sortie d'études.

**Risque à surveiller** : runway personnel des fondateurs. Si on ne peut pas tenir 18 mois sans revenus, il faut un wedge payant plus rapide (freelances ou jeunes pros directement).

---

## 7. Go-to-Market

### Acquisition alternants (gratuit)
- BDE et associations étudiantes (écoles d'ingé, écoles de commerce avec alternance).
- Discord serveurs étudiants (42, Epitech, écoles d'ingé).
- Bouche-à-oreille via les promos d'alternance.
- LinkedIn organique (témoignages alternants).
- Partenariats avec écoles (gratuit en échange de visibilité).

### Conversion alternants → Pro
- Trigger automatique à la fin d'alternance détectée (compte école qui se désactive).
- Email de campagne "tu changes de vie, ton calendrier suit".
- Offre de bienvenue "premier mois Pro offert pour les anciens étudiants".

### Acquisition jeunes diplômés directs
- SEO sur les douleurs ("agenda multi-comptes", "Outlook + Google Calendar", etc.).
- Communautés type Welcome to the Jungle, Indie Hackers FR, Twitter/X dev FR.

---

## 8. Recrutement tech (rentrée prochaine)

### Profils cibles

- **Bac+4/5 écoles d'ingé** (Epitech, 42, INSA, Centrale, EPITA, Télécom) en stage de fin d'études ou alternance.
- **Bac+5 master info universitaire** (Paris-Saclay, Sorbonne, Grenoble) — souvent sous-cotés et excellents.
- **Autodidactes 42 / Holberton / O'clock** — affamés, parfaits pour aller vite.
- **1 profil design produit** (Gobelins, Strate, HETIC) — à ne pas négliger.

### Pitch de recrutement

> On construit le calendrier qui suit la transition école → vie pro. On est X founders, on a [traction / waitlist / users].
>
> On ne cherche pas un stagiaire à qui coller des tickets. On cherche un futur co-fondateur tech ou un early employee #1.
>
> **Ce que tu auras :**
> - Vrai impact produit : tu choisis la stack, tu codes du zéro, tu parles aux users.
> - Mentorat business et produit.
> - Equity package si tu rejoins post-stage.
> - Réseau : intros à nos mentors et autres founders.
>
> **Ce qu'on ne t'offre pas :**
> - Un gros salaire (stage min légal, ~600€).
> - Des bureaux à La Défense.
>
> Si t'as envie de construire plutôt que d'exécuter, parle-nous.

**Règle d'or :** transparence totale sur la précarité. Les bons profils détectent le bullshit en 3 minutes.

### Où chercher
- LinkedIn (filtre école + année de promo).
- Forums et Discord des écoles ciblées.
- Hackathons (Hacking Project, Station F events).
- Recommandations du réseau (le plus efficace).

---

## 9. Stack technique (contrainte "no income no investment")

### Choix de stack

| Couche | Outil | Coût | Raison |
|---|---|---|---|
| Frontend web | Next.js sur Vercel hobby | 0€ | Free tier large, déploiement instant |
| Mobile | Expo (React Native) | 0€ | Cross-platform iOS/Android |
| Backend | Node.js + tRPC ou Hono | 0€ | Léger, typesafe end-to-end |
| Hébergement back | Railway ou Fly.io free tier | 0€ | Éviter AWS au début (piège à coûts) |
| Base de données | Supabase ou Neon (Postgres) | 0€ | Free tier généreux |
| Auth | Supabase Auth ou Clerk | 0€ | Clerk gratuit jusqu'à 10k MAU |
| Email transactionnel | Resend | 0€ | 3000 emails/mois gratuits |
| Monitoring | PostHog + Sentry free tier | 0€ | Open source, self-hostable si besoin |
| LLM (features IA) | Claude Haiku ou Gemini Flash | ~quelques € | Pay-per-use, négligeable à notre volume |
| Code & projet | GitHub + Linear free + Figma free | 0€ | — |

### Intégrations calendrier
- **Google Calendar API** — gratuit jusqu'à quotas élevés.
- **Microsoft Graph API** — gratuit jusqu'à quotas élevés.
- **Apple Calendar via CalDAV** — gratuit mais techniquement plus pénible.

### ⚠️ Points d'attention techniques majeurs

1. **Google API verification** — au-delà de 100 users sur des scopes sensibles (Gmail, Calendar full), Google demande un security assessment payant (15–75k$). À anticiper dès maintenant : démarrer la procédure tôt.
2. **CalDAV Apple** — vraie galère technique, faire un spike dédié avant tout le reste.
3. **Sync moteur** — architecturer en système d'événements (queue, jobs async), pas en synchrone. Sinon mort à 100 users.

### Choses concrètes à faire en premier (semaine 1–2)

1. Décider mono-repo vs poly-repo (recommandation : **mono** pour démarrer).
2. CI/CD basique en place (GitHub Actions, gratuit).
3. Spike technique OAuth Google + Microsoft + Apple : c'est là que ça va coincer.
4. Démarrer la procédure de Google API verification.
5. Modéliser le schéma de données "événement multi-source" (un event peut avoir N sources et N représentations).

---

## 10. Roadmap macro (12 mois)

| Phase | Période | Objectif |
|---|---|---|
| **Discovery** | M1 | 20 user interviews alternants + 10 jeunes diplômés |
| **Spike technique** | M1–M2 | Valider sync Google + Microsoft + Apple |
| **MVP** | M2–M4 | Sync 3 écosystèmes + UI mobile/web minimale |
| **Beta alternants** | M4–M6 | 50–200 alternants en usage réel |
| **Itération produit** | M6–M9 | Couches IA + suggestions + deep work |
| **Lancement Pro** | M9–M12 | Premiers payants jeunes diplômés |

---

## 11. Risques identifiés et mitigations

| Risque | Impact | Mitigation |
|---|---|---|
| Marché saturé (Motion, Reclaim, etc.) | Critique | Positionnement vertical alternant→jeune pro, multi-écosystèmes |
| Alternants ne convertissent pas en payants | Critique | Soigner le moment de sortie d'études + offre de transition |
| Google API verification bloque l'échelle | Élevé | Anticiper la procédure dès le MVP |
| Apple CalDAV complexe à intégrer | Moyen | Spike technique en M1 avant d'investir |
| Runway perso des fondateurs trop court | Élevé | Plan B : monétiser direct sur freelances ou jeunes diplômés sans phase gratuite |
| Recrutement tech difficile sans cash | Moyen | Equity, mentorat, mission, transparence |

---

## 12. Prochaines étapes (cette semaine)

1. ✅ Valider ce doc entre cofondateurs.
2. ⏳ Lancer les 20 user interviews alternants (objectif : terminé d'ici 2 semaines).
3. ⏳ Démarrer le spike technique OAuth multi-providers.
4. ⏳ Définir le wedge feature précis du MVP (1 chose qu'on fait mieux que tout le monde).
5. ⏳ Rédiger la fiche de poste tech pour la rentrée prochaine.

---

*Document à itérer après chaque cycle de user interviews et chaque décision stratégique.*
