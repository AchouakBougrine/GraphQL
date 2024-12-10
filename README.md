# Projet GraphQL - Gestion des Comptes et Transactions
Ce projet implémente une API GraphQL pour la gestion de comptes bancaires et de transactions financières. Il permet aux utilisateurs de créer, consulter et manipuler des comptes, ainsi que d'effectuer des transactions telles que des dépôts et des retraits. L'API fournit également des statistiques sur les transactions et les comptes.

# Fonctionnalités principales
## 1 Gestion des Comptes
Création de comptes : Créez un compte avec un solde initial et un type (courant ou épargne).
Consultation des comptes : Obtenez une liste de tous les comptes ou recherchez un compte spécifique par ID ou par type.
Suppression de comptes : Supprimez un compte en fonction de son ID.
## 2 Gestion des Transactions
Ajout de transactions : Effectuez des transactions de type dépôt ou retrait pour un compte spécifique.
Consultation des transactions : Obtenez les transactions effectuées sur un compte spécifique.
## 3 Statistiques des Transactions
Statistiques globales : Obtenez des statistiques globales sur les transactions (nombre total, somme totale, moyenne des transactions).
Statistiques par type de transaction : Obtenez des statistiques sur les dépôts et les retraits effectués.

# Requêtes et Mutations
Voici quelques requêtes et mutations disponibles via l'API GraphQL :

## Requêtes
allComptes : Liste tous les comptes.
compteById(id: ID!) : Recherche un compte par son ID.
compteByType(type: TypeCompte!) : Recherche des comptes par type (courant ou épargne).
totalSolde : Obtient des statistiques globales sur les soldes des comptes.
compteTransactions(id: ID!) : Recherche les transactions effectuées sur un compte spécifique.
## Mutations
saveCompte(compte: CompteRequest!) : Crée un nouveau compte.
addTransaction(transaction: TransactionRequest!) : Ajoute une nouvelle transaction (dépôt ou retrait).
deleteCompte(id: ID!) : Supprime un compte.
