---
title: API REST de Kaizala | MicrosoftDocs
description: Cette rubrique fournit le contenu de référence API REST pour l’API Kaizala.
ms.date: 05-10-2017
ms.service: kaizala
ms.topic: conceptual
author: ''
ms.author: ''
manager: ''
ms.devlang: https
ms.openlocfilehash: 732aae562aaf823798066952a40526e353072efc
ms.sourcegitcommit: a9df86259a9029a137346752ff43e135e2db6d14
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19907234"
---
# <a name="kaizala-rest-api"></a>API REST de Kaizala

Kaizala permet aux développeurs tiers 3e Kaizala intégrer leurs processus d’entreprise en fournissant des appels d’API en fonction de la capacité à exécuter un ensemble d’actions curated dans Kaizala à l’aide de REST. L’étendue de l’API est pour les systèmes externes pour le point de terminaison d’appel et effectuer des actions sur la demande. Autrement dit, il s’agit d’un modèle de collecte – où les points de terminaison individuels doivent être appelée pour effectuer des actions spécifiques à l’aide de Kaizala APIs. Le modèle PUSH où plateforme Kaizala peut déclencher des actions permettre être configuré à l’aide de webhooks.

## <a name="rest-operations"></a>Opérations de REST

| Opération | Description                                                        |
|-----------------|--------------------------------------------------------------------|
| Générer du code confidentiel | Génère le code confidentiel unique pour un numéro de téléphone mobile, lors de l’Id de connecteur d’Application est fourni |
| Obtenir le jeton actualisation | Génère le jeton d’actualisation pour l’Id de connecteur d’Application donné, lorsque le code confidentiel, numéro de téléphone mobile et Id de connecteur d’Application est fourni |
| Générer un jeton d’accès | Génère le jeton d’accès pour accéder aux ressources de Kaizala, lorsque le jeton d’actualisation, Id de connecteur d’Application et le Secret de connecteur d’Application est fourni. |
| Créer le groupe | Permet de créer un un groupe, y compris des groupes publics gérées. Il prend un tableau de chaînes comme entrée. Chaque chaîne est le numéro de téléphone mobile (avec le code du pays). Cette API peut prendre au maximum 100 numéros de téléphone portable en tant que input.\n\tGroupType : groupe/ConnectGroup. ConnectGroup pour le groupe public géré. |
| Créer le groupe secondaire | Créer un groupe sub  |
| Ajouter des membres | Ajouter des membres à un groupe |
| Ajouter sous-groupe | Ajouter le groupe comme un groupe secondaire à un autre groupe |
| Ajoutez des abonnés | Ajouter les abonnés à un groupe public |
| Détails de l’extraction d’un groupe | Extraction des détails pour un groupe |
| Extraction des membres | Renvoie la liste des membres d’un groupe |
| Extraction d’abonnés | extrait la liste des abonnés à un groupe public géré |
| Groupe secondaire d’extraction | Extraction des sous-groupes d’un groupe |
| Supprimer un groupe en tant que groupe secondaire | Supprimer le groupe comme un groupe vers un autre groupe secondaire |
| Supprimer des membres | Supprime des membres d’un groupe |
| Supprimer les abonnés | Supprimer les abonnés à partir d’un groupe public géré |
| Extraction des groupes Direct | Renvoie tous les groupes directes attachés à l’utilisateur |
| Envoyer le Message | Envoyer un message sur un groupe |
| Envoyer un Message à un abonné | Envoyer un message aux abonnés dans un groupe public |
| Télécharger des fichiers multimédias | Téléchargements multimédia (image, document, audio, album ou vidéo) |
| Envoyer le sondage | Vous permet de créer une enquête et envoyer un groupe |
| Publier une Action personnalisée pour un abonné | Publier une action personnalisée pour les abonnés dans un groupe public |
| Réponse à une Action | Publier une réponse à une action |
| Réponse à une enquête. | Publier une réponse à une enquête |
| Extraction des travaux | Extraction des travaux dans un groupe |
| Extraction des réponses de l’enquête | Extraction des réponses à une enquête |
| Obtenir tous les Webhooks | Renvoie tous les webhooks sur un groupe |
| S’abonner à tous les événements | S’abonner à tous les événements au niveau de l’action |
| Annuler l’abonnement une Webhook | Annulation d’un webhook |
