# BankManager

Projet de gestion de comptes bancaires conçu avec **Java JDK 21**, mettant en pratique les principes fondamentaux de la Programmation Orientée Objet (POO) : l'**Héritage** et l'**Encapsulation**.

## 🏗️ Architecture du Projet

Le projet est structuré autour d'une classe parente et de trois classes filles spécialisées :

- **`BankAccount`** : Classe parente (superclasse) qui encapsule les attributs communs à tous les comptes : `account` (numéro de compte) et `balance` (solde).
- **`CheckingAccount`** : Classe fille représentant un compte courant, avec un attribut spécifique `limit` (découvert autorisé).
- **`SavingsAccount`** : Classe fille représentant un compte d'épargne, avec un attribut spécifique `interestRate` (taux d'intérêt).
- **`COD` (Certificat de Dépôt)** : Classe fille représentant un compte à terme, avec un attribut spécifique `durationMonths` (durée de blocage).

Toutes les classes filles héritent des attributs `account` et `balance` et permettent d'accéder à ces données en lecture (Getters) et en écriture (Setters).

## 🛠️ Prérequis

- **Java JDK 21** ou version supérieure.
- Un IDE comme IntelliJ IDEA, Eclipse, ou VS Code (ou simplement un terminal).

## 🚀 Importation et Exécution

### Option A : Via IntelliJ IDEA (Recommandé)
1. Clonez ou téléchargez ce dépôt GitHub.
2. Ouvrez IntelliJ IDEA et faites **File > Open**, puis sélectionnez le dossier du projet.
3. Assurez-vous que le SDK du projet est bien configuré sur **Java 21** (*File > Project Structure > Project*).
4. Faites un clic droit sur le fichier `Main.java` dans le dossier `src/com/bankmanager/` et cliquez sur **Run 'Main.main()'**.

### Option B : Via le Terminal
Si vous préférez exécuter le projet sans IDE, placez-vous à la racine du projet dans votre terminal et lancez les commandes suivantes :

```bash
# Compilation des fichiers Java
javac -d bin src/com/bankmanager/*.java

# Exécution de l'application
java -cp bin com.bankmanager.Main
