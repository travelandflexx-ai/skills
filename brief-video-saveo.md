# Brief pour la session vidéo : refaire le format « Saveo »

Source : https://x.com/brainextends/status/2110814597653664113. La vidéo vient du compte Instagram **@saveo.house**, l'app de budget Saveo. Le compte a fait environ 6 M de vues et 54,6 K abonnés en 1 jour avec 2 reels.

## 1. Le sujet

- **Concept** : « Tu viens de voler 10 M$. » La série suit un bonhomme stickman (casquette, hoodie) qui doit blanchir l'argent. C'est un prétexte pour **enseigner l'argent et la finance** (poids des billets, bait money, déclaration au-delà de 10 000 $, *structuring*). Ça colle au produit, une app de budget.
- **Mécanique** : une série interactive. À la fin, « Comment HIDE or SPEND, la majorité écrit la partie 2 ». Un épisode par jour. Bio : « $10M. You decide what happens. »
- **Monétisation** : un *Founder's Pass* Gumroad à 10 $ (nom affiché + accès anticipé).

## 2. Le script (transcription, 87 s)

```
You just stole $10,000,000. It's sitting on a motel bed in four duffel bags.
And the hard part, it starts now, because every dollar leaves a trail.
Problem one, you can't even carry it. A single bill weighs about one gram.
10 million in hundreds is 100,000 bills. That's 100 kilos, 220 pounds.
And if the bank gave you 20s, half a ton.
Problem two, banks keep bait money. Bills with their serial numbers written down
mixed in with the real cash. Spend one in the wrong place and it gets flagged.
You have no idea which ones they are.
Rule one, never spend it near where you took it.
Day two, you need it in a bank. So you walk in with a backpack full of cash.
Here's what you don't know. Any cash deposit over $10,000, the bank reports to
the federal government automatically, every time.
So you get smart, $9,000. A different bank every day, just under the line.
Nine, 18, 27, 36,000. Except that pattern has a name, structuring.
It's a federal crime on its own, even if the money was clean.
And it's exactly what banks are trained to spot. Four deposits in and someone is
already looking at a screen with your name on it.
Day three, you've got $9,964,000 you can't touch. And you're sick of motel noodles.
You can hide it or you can spend it. Comment, hide or spend. Part two follows what you pick.
```

**Structure** : hook choc (0-2 s), puis enjeu (« every dollar leaves a trail »), puis Problème 1, Problème 2 et Règle 1, puis Jour 2 (piège, fausse bonne idée, retournement), puis Jour 3 (bilan), puis le vote en CTA.
Le ton est en 2ᵉ personne (« you »), avec des phrases très courtes, un fait chiffré toutes les 3-5 s et un twist récurrent : « Here's what you don't know » / « Except… ».

## 3. Le montage

- **Format** : 9:16 en 720×1280, environ 87 s. Voix off IA, calme et grave, débit rapide.
- **Deux types de plans en alternance (environ 50/50)** :
  1. **Illustration IA** : stickman tête ronde blanche, style cartoon détaillé. Décors réalistes : motel néon rose, banque, rue en automne, bureau d'un agent avec écran. Cadrage de plain-pied, gros plans du visage pour les émotions (sueur, sourcils froncés). Un léger zoom ou pan sur chaque image fixe (Ken Burns), avec une coupe toutes les 2-3 s.
  2. **Motion design en infographie** : fond crème (#EFE9DF) ou noir. Gros chiffres en sans-serif gras noir, petit sur-titre en monospace (« PROBLEM 1 · THE WEIGHT », « THE $10,000 LINE »). Les billets s'empilent en grille, les compteurs défilent (74 152 puis 100 000 bills, 100 kg), un tampon rose « AUTOMATICALLY » ou « FEDERAL CRIME » apparaît, puis des barres de dépôts à 9 000 $ sous une ligne pointillée rouge.
- **HUD de jeu permanent** en haut des plans illustrés : `CASH $10,000,000 | BANKED $0 | SUSPICION 0%`. Les valeurs évoluent (SUSPICION 0 → 20 → 34 → 35 %, en rose). C'est ce qui donne l'effet « jeu ».
- **Sous-titres** : 2-3 mots à la fois, blancs en bas au centre, le mot clé en couleur. Labels ou étiquettes roses sur les objets (« BAIT MONEY – serial number on file », cercle rose autour d'un billet).
- **Palette** : rose/magenta néon (#E8338A environ) comme seule couleur d'accent, plus du noir, du crème et le vert des billets. C'est la « psychologie des couleurs » : le rose = danger/suspicion.
- **Fin** : gros plan du perso derrière une vitrine (voiture de luxe), deux boutons **HIDE** (blanc) / **SPEND** (rose), puis un carton « PART 2 TOMORROW – Comment HIDE or SPEND. The majority writes Part 2. »

## 4. Pour refaire pareil (pipeline suggéré)

1. **Script** : 180-220 mots, une seule règle : un chiffre ou un twist toutes les 3-5 s, et un vote binaire à la fin. Adapter le thème à notre marque (budget, argent, produit).
2. **Personnage** : définir une fiche perso fixe (prompt + image de référence) pour garder la cohérence entre les plans.
3. **Images** : environ 20 plans illustrés générés en 9:16, dans le même style et le même décor que la référence.
4. **Voix** : TTS (ElevenLabs ou équivalent), voix masculine grave et posée.
5. **Infographies et HUD** : en code (Remotion / React ou After Effects) pour les compteurs animés, les tampons et le HUD de suspicion.
6. **Assemblage** : Ken Burns sur les images, coupes calées sur la voix, sous-titres mot à mot, whoosh ou ding légers sur les chiffres.
7. **Publication** : un épisode par jour. L'épisode suivant suit le vote majoritaire en commentaire.

---

# Article « How to build your own app using REA » : ce qui est intéressant

Source : https://www.aiinpublic.com/p/how-to-build-your-own-app-using-rea

**L'idée** : recréer *une* fonctionnalité d'un outil payant avec Claude, sans coder. L'exemple est le « Magic Switch » de Canva (redimensionner un visuel pour IG, Story, YouTube, X, LinkedIn).

**Méthode A, « Watch from outside » (sans rien installer, la plus utile)** :
1. Décrire la fonction en une phrase. Claude en fait une spec en langage simple avec **10 cas de test**.
2. Dans un nouveau chat, Claude construit l'outil à partir de la spec.
3. **Test de parité** : mêmes entrées dans l'original et dans la copie, puis classement « Match », « Small difference » ou « Broken ».

Leçons : une fonction = un après-midi (une app pro = des mois). Tester tôt. Commencer par une seule fonction, une spec et un test.

**Méthode B, « Look inside » avec REA** (Mac/Linux, seulement pour des apps qu'on possède. Attention aux conditions d'utilisation) :
```bash
# Prérequis : Node.js LTS (node -v)
npx rea-agents setup          # accepter, dire oui à Hopper
mkdir rebuild-X && cd rebuild-X
claude                        # puis /mcp : "rea" doit être connecté
# si erreur :
claude mcp add --scope user rea -- npx -y rea-agents@latest mcp
```
Ensuite, donner le chemin de l'app (ex. `/Applications/flameshot.app`) et demander à Claude d'identifier son type, d'expliquer la fonctionnalité et d'écrire une spec.
Repo : https://github.com/morluto/rea · démo : https://rea.tools/showcase/dx-ball/

Les 6 prompts exacts et le CLAUDE.md complet sont dans le « Rebuild Kit », réservé aux abonnés : je ne les ai pas.
