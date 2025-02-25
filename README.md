# .github

🎯 Objectif du Microservice
Le microservice subscription-service permet de :
✅ Récupérer la liste des abonnements d'un utilisateur.
✅ Afficher les détails de chaque abonnement (nom du service, coût, date de renouvellement, statut, etc.).


🏗 Architecture et Fonctionnement
Le service fonctionne via une API REST qui interagit avec :

user-service 🔗 pour associer les abonnements à un utilisateur.
auth-service 🔗 pour connecter les utilisateurs.
subscription-service 🔗 pour associer les subscription à un utilisateur.


📌 Endpoints principaux
Méthode	Endpoint	Description
GET	/subscriptions/{user_id}	Récupère la liste des abonnements d’un utilisateur
POST	/subscriptions	Ajoute un nouvel abonnement
PUT	/subscriptions/{subscription_id}	Met à jour un abonnement existant
DELETE	/subscriptions/{subscription_id}	Supprime un abonnement



🚀 Cas d’usage
Un utilisateur connecte son compte et accède à la liste de ses abonnements.
Il visualise ses abonnements actifs et expirés avec leurs coûts.
Il peut annuler ou modifier ses abonnements directement depuis l’application.
