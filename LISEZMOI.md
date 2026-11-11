# Carnet d’entraînement — programme Riad 3.0

Web app installable sur iPhone, sans App Store ni compte Apple.

Contenu : index.html (toute l’app), sw.js (hors ligne), manifest.webmanifest et icons/.

## Données et sauvegarde

- Tout est stocké sur l’iPhone.
- Sauvegarde automatique (Réglages) : copie dans un dépôt GitHub **privé**, avec une version à chaque synchro. Il faut un jeton « fine-grained » limité à ce dépôt, permission Contents en lecture et écriture.
- Sauvegarde manuelle : Réglages → Exporter mes données.

## Coach IA (facultatif)

- Réglages → Coach IA : avec une clé API Anthropic, un coach lit ton objectif, ton programme et ton historique, et te conseille avant, pendant et après la séance.
- La clé reste sur l’iPhone : elle n’est ni exportée, ni envoyée sur GitHub.
- À chaque question, l’app envoie ton historique d’entraînement à Anthropic (Claude) pour obtenir la réponse. Rien n’est envoyé tant qu’aucune clé n’est saisie.
- L’usage est payant, à la demande, sur ton compte Anthropic.

## Mise en ligne

Le guide GitHub Pages arrive à l’étape suivante. Après une mise à jour des fichiers, l’app se met à jour d’elle-même en un ou deux lancements. Si tu modifies les icônes, change aussi `CACHE` dans `sw.js`.
