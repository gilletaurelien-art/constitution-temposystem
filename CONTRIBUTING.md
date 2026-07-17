# Contribuer

Ce dépôt fonctionne comme un logiciel libre appliqué à un texte fondateur.

## Critiquer (le plus précieux)

Ouvrez une **issue**. Ce projet recherche activement la relecture contradictoire : juristes, designers, développeurs, psychologues, chercheurs en interaction humain-machine, spécialistes de la protection des données. Le but n'est pas que le texte plaise — c'est qu'il résiste. Une critique qui fait tomber un article vaut plus qu'un compliment qui le flatte.

## Amender

La Constitution évolue par **amendements numérotés**, jamais par réécriture silencieuse :

1. La discussion commence dans une issue.
2. Si elle aboutit, un fichier `amendments/NNNN-titre-court.md` est proposé en pull request, sur le modèle de [amendments/0000-modele.md](amendments/0000-modele.md) : le texte modifié, **et surtout la motivation** — pourquoi ce principe entre, change ou sort.
3. L'adoption d'un amendement incrémente la version du texte canonique et l'amendement reste archivé à jamais : l'histoire des débats fait partie de la Constitution.

Le texte canonique est [CONSTITUTION.md](CONSTITUTION.md) (français). Les traductions suivent le canonique.

## Traduire

Ajoutez `translations/<code-langue>/CONSTITUTION.md` par pull request, en indiquant la version canonique traduite. Une traduction fidèle vaut mieux qu'une traduction élégante.

## Interpréter — la jurisprudence des cas

Une constitution vivante ne grandit pas seulement par ses amendements : elle grandit par la manière dont on l'applique à des situations nouvelles. Le dossier [/cases](cases/) est sa jurisprudence — chaque cas documente comment les articles s'incarnent (ou échouent à s'incarner) dans un système réel, preuves à l'appui. Proposer un cas vaut autant que proposer un amendement : ajoutez `cases/<nom>.md` par pull request, en n'affirmant que ce que vous pouvez montrer.

## Adopter et signer

Inscrivez votre nom ou votre organisation dans [SIGNATORIES.md](SIGNATORIES.md) par pull request. Conformément à l'**article 15 (honnêteté d'affichage)**, une signature honnête mentionne aussi les articles que vous ne respectez pas encore et votre trajectoire pour y parvenir. Une signature parfaite est suspecte ; une signature datée et documentée est crédible.
