---
title: API REST Kaizala | MicrosoftDocs
description: Cette rubrique fournit du contenu de référence d’API REST pour l’API Kaizala.
ms.date: 05-10-2017
ms.service: kaizala
ms.topic: conceptual
author: ''
ms.author: ''
manager: ''
ms.devlang: https
ms.openlocfilehash: 732aae562aaf823798066952a40526e353072efc
ms.sourcegitcommit: d95e42eaf596f2fd27330bd4bfd6525f356a9f2e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384229"
---
# <a name="kaizala-rest-api"></a>API REST Kaizala

Kaizala permet aux développeurs tiers d’intégrer Kaizala à leurs processus métier en offrant la possibilité d’effectuer un ensemble d’actions organisée dans Kaizala à l’aide d’appels d’API basés sur REST. L’étendue de l’API est destinée aux systèmes externes pour appeler le point de terminaison et effectuer des actions à la demande. Autrement dit, il s’agit d’un modèle d’extraction, où les points de terminaison individuels doivent être appelés pour effectuer des actions spécifiques à l’aide des API Kaizala. Le modèle poussé dans lequel la plateforme Kaizala peut déclencher des actions peut être configuré à l’aide des webhooks.

## <a name="rest-operations"></a>Opérations REST

| Opération | Description                                                        |
|-----------------|--------------------------------------------------------------------|
| Générer un code confidentiel | Génère un code confidentiel à usage unique pour un numéro de téléphone mobile, lorsque l’ID de l’application/connecteur est fourni |
| Obtenir un jeton d’actualisation | Génère un jeton d’actualisation pour l’ID d’application/connecteur donné, lorsque le code confidentiel, le numéro de téléphone mobile & l’ID d’application/connecteur est fourni |
| Générer un jeton d’accès | Génère un jeton d’accès pour accéder aux ressources Kaizala, lorsque le jeton d’actualisation, l’ID d’application/connecteur et la clé secrète application/connecteur sont fournis |
| Créer un groupe | Permet la création d’un groupe, y compris les groupes publics gérés. Il prend un tableau de chaîne comme entrée. Chaque chaîne est numéro de téléphone mobile (avec code pays). Cette API peut prendre jusqu’à 100 numéros de téléphone mobile en tant qu’entrée. \ n \ tGroupType : Group/ConnectGroup. ConnectGroup pour le groupe public géré. |
| Créer un sous-groupe | Créer un sous-groupe  |
| Ajouter des membres | Ajouter des membres à un groupe |
| Ajouter un sous-groupe | Ajouter un groupe en tant que sous-groupe à un autre groupe |
| Ajouter des abonnés | Ajouter des abonnés à un groupe public |
| Extraire les détails du groupe | Extraire les détails d’un groupe |
| Extraire les membres | Renvoie la liste des membres d’un groupe |
| Extraire les abonnés | Récupère la liste des abonnés d’un groupe public géré |
| Extraire un sous-groupe | Extraire des sous-groupes d’un groupe |
| Supprimer un groupe en tant que sous-groupe | Supprimer un groupe en tant que sous-groupe d’un autre groupe |
| Supprimer des membres | Supprime les membres d’un groupe |
| Supprimer des abonnés | Supprimer des abonnés d’un groupe public géré |
| Extraire les groupes directs | Renvoie tous les groupes directs associés à l’utilisateur |
| Envoyer un message | Envoyer un message sur un groupe |
| Envoyer un message à un abonné | Envoyer un message à un ou plusieurs abonnés d’un groupe public |
| Télécharger du contenu multimédia | Télécharge le support (image, document, audio, album ou vidéo) |
| Envoyer un sondage | Vous permet de créer une enquête et de l’envoyer sur un groupe |
| Publier une action personnalisée sur un abonné | Publier une action personnalisée sur un ou plusieurs abonnés d’un groupe public |
| Publier une réponse à une action | Publier une réponse à une action |
| Publier une réponse à une enquête | Publier une réponse à une enquête |
| Récupérer des travaux | Récupérer des travaux dans un groupe |
| Extraire les réponses d’enquête | Extraire des réponses pour une enquête |
| Obtenir tous les webhooks | renvoie tous les webhooks d’un groupe |
| S’abonner à tous les événements | S’abonner à tous les événements au niveau de l’action |
| Annuler l’abonnement à un webhook | Résiliation d’un webhook |
