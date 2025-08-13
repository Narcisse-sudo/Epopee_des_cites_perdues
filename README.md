# Thème du projet : "L’Épopée des Cités Perdues"

Le projet est un jeu textuel où le joueur incarne un explorateur chargé de redonner vie à des cités perdues. Il devra gérer des ressources, explorer des lieux, interagir avec des personnages (alliés ou ennemis) et relever des défis. Les données de base (personnages, lieux, ressources, etc.) sont fournies dans un fichier JSON, et le joueur interagit via la console.

---

##  Objectif du projet

- Créer une version simple du jeu où le joueur explore une cité, gère des ressources et interagit avec des personnages via des choix textuels.
- Manipuler des **fichiers JSON** (lecture/écriture).
- Structurer un **programme Python** conforme **PEP8** avec des fonctions documentées.
- Gérer un **état de jeu** (inventaire, points de vie, progression) et le **sauvegarder**.
- Implémenter des **mécaniques simples** d’exploration, d’interaction et de combat.

---

## Fichier JSON fourni : Un fichier data.json contient :

Une liste de lieux (par exemple, "Temple Oublié", "Forêt Maudite") avec des caractéristiques (nom, description, ressources disponibles, ennemis présents).
Une liste de personnages (nom, type [allié/ennemi], force, dialogue).
Une liste de ressources (nom, quantité initiale, utilité).
Exemple de data.json :

```json
{
    "lieux": [
        {"nom": "Temple Oublié", "description": "Un temple envahi par la végétation", "ressources": ["or", "pierres"], "ennemis": ["serpent géant"]},
        {"nom": "Forêt Maudite", "description": "Une forêt sombre et mystérieuse", "ressources": ["bois", "herbes"], "ennemis": ["loup spectral"]}
    ],
    "personnages": [
        {"nom": "Arwen", "type": "allié", "force": 5, "dialogue": "Je peux t'aider à explorer, mais il me faut 10 unités d'or."},
        {"nom": "Serpent Géant", "type": "ennemi", "force": 8, "dialogue": "Sssss... Tu ne passeras pas !"}
    ],
    "ressources": [
        {"nom": "or", "quantite": 20, "utilite": "Acheter de l'aide"},
        {"nom": "bois", "quantite": 10, "utilite": "Construire des abris"}
    ]
}
```

## Mécaniques du jeu :

Le joueur commence avec un inventaire vide et un certain nombre de points de vie (par exemple, 100).
Le joueur peut :
Explorer un lieu (afficher sa description, récupérer des ressources, affronter un ennemi via un système de "combat" simple basé sur des comparaisons de force).
Interagir avec un personnage (dialoguer, payer un allié pour obtenir de l’aide, fuir un ennemi).
Gérer son inventaire (ajouter des ressources, vérifier les quantités).
Les choix du joueur sont faits via des entrées textuelles (par exemple, "1 pour explorer, 2 pour parler à un personnage, 3 pour quitter").
Les données du jeu (inventaire, points de vie, etc.) sont sauvegardées dans un fichier JSON à la fin de chaque session.


##  Données d’entrée (`data.json`)

Le jeu lit un fichier `data.json` contenant les **lieux**, **personnages** et **ressources**.



Pour la coloration dans le terminal, il faudra installer `colorama` avec la commande suivante :

```bash
pip install colorama
```
# Epopee_des_cites_perdues
