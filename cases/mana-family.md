# Cas fondateur — Mana Family

*Mana Family est le produit dont cette Constitution est née : un système de cercles familiaux vivants (transmissions de soin entre proches, mémoire familiale durable). Ce document montre comment chaque grand article est implémenté — pas déclaré, implémenté — jusque dans le schéma de données. Conformément à l'article 15, il documente aussi les écarts restants.*

## Article 8 — l'asymétrie de l'attention, dans la structure même de la base

La table qui enregistre les gestes de veille (`transmission_lueurs`) est **insert-only** et ne contient que des gestes *posés*. Il n'existe ni colonne, ni vue, ni compteur permettant d'exprimer « qui n'a pas veillé » : l'asymétrie n'est pas une consigne d'interface, c'est une **impossibilité structurelle** du modèle de données. Dans l'interface, la lueur apparaît quand quelqu'un a veillé ; son absence est invisible.

## Article 10 — l'inaliénabilité, gardée par des triggers

Les transmissions n'ont **pas de colonne `deleted_at`**. Des triggers SQL rejettent tout `DELETE` et tout `UPDATE` sur la mémoire, y compris pour les rôles d'administration, avec ce message d'erreur : *« la mémoire ne s'efface pas, elle se voile »*. Un développeur pressé, dans deux ans, recevra la loi en exception.

## Article 3 — la souveraineté, native dans le graphe

Le voile est une table de première classe (`veils`) : une personne peut masquer sa continuité à un cercle **sans détruire sa propre archive**, et refuser de figurer dans un objet collectif même déjà payé par un tiers (« le droit de l'astre l'emporte sur le droit du portefeuille »). Le graphe est centré sur les personnes : un enfant de parents séparés appartient à deux cercles et conserve une continuité unique.

## Article 7 — le droit au repos, dans le langage de l'interface

Aucune notification de relance n'existe. Quand la famille n'a rien transmis depuis trois jours, l'écran d'accueil affiche : *« La constellation se repose. »* — un état nommé positivement, jamais un manque. Les animations ralentissent au repos (respiration 24 s contre 12 s en présence). Aucun rouge, aucun badge, aucun compteur de non-lus dans toute l'application.

## Article 9 — le refus du regret, comme valeur d'entreprise

Règle interne écrite : *« Nous n'utiliserons jamais le regret comme moteur de croissance. »* Aucune communication ne dira « avant qu'il soit trop tard ». Le backlog conserve un **cimetière des idées rejetées** avec leurs motifs (barre de complétude, nudges de photothèque, reconnaissance faciale d'enfants, étoiles qui s'assombrissent après inactivité) pour qu'aucune ne revienne sous un déguisement neuf.

## Article 5 — les vulnérables, par l'infrastructure

Les données de la famille vivent dans une **base dédiée**, séparée de tout autre produit, hébergée en Europe. Les enfants n'ont pas de compte : l'accès passe par des adultes dont la garde est modélisée comme une relation bornée dans le temps et en périmètre (`guardianships`), jamais comme un pouvoir permanent. À la majorité, l'enfant reçoit la propriété pleine de sa continuité.

## Article 12 — l'économie légitime

La structure familiale complète et la mémoire brute sont gratuites, sans limite de durée. La monétisation porte exclusivement sur l'artisanat (récits, rituels, objets physiques) et chaque offre payante peut être offerte — l'argent circule comme la mémoire, d'une génération vers la suivante.

## Écarts documentés (article 15)

- **Chiffrement de bout en bout** : pas encore construit. Engagement, pas fait accompli.
- **Droit au départ (article 4)** : l'export complet en format ouvert n'est pas encore livré ; prévu avant toute ouverture publique.
- **Transparence algorithmique (article 13)** : sans objet à ce jour — aucun algorithme de tri ou de recommandation n'existe dans le produit, et c'est volontaire.

*Dernière mise à jour : juillet 2026, pendant la mer d'essai du produit dans une famille réelle.*
