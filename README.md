# HibernateTP
Hibernate est un framework open source en Java qui facilite le développement d'applications Java en fournissant un mapping objet-relationnel (ORM). L'ORM est une technique de 
programmation qui lie les objets d'une application à une base de données relationnelle. Hibernate simplifie le processus de stockage et de récupération d'objets Java à partir 
d'une base de données. Il simplifie également la gestion de la base de données en permettant aux développeurs de travailler avec des objets Java au lieu d'écrire des requêtes SQL.

Pour developement de nos compétences on a traité plusieur TPS :

**EXO1:**

**-- Database H1--** 

![h1](https://github.com/ELMOUWAHID-AYOUB/HibernateTP/assets/130571009/6a460799-071e-4250-b43f-fc68e4c371bc)




Base de données : `h1`


![data](https://github.com/simo-laaouibi/hibernate/assets/130571009/687fdd50-d480-40d9-846b-77410f973b50)

**EXO2:**

**-- Database H2:--**

Cette exercice il est déja corrigé:

![h2](https://github.com/simo-laaouibi/hibernate/assets/130571009/f227dab3-76eb-4e30-96bf-6a6c4d821938)

**EXO3:**

**-- Database H3:--**


![H3](https://github.com/ELMOUWAHID-AYOUB/HibernateTP/assets/130571009/4a3332eb-7918-4730-855a-1e116271f816)

cette exercice il passe à déférente étape  :

1.créer Développer les classes entités dans le package « ma.projet.classes ».

2.Créer le fichier de configuration hibernate.cgf.xml dans le package « ma.projet.config ».

3.Créer la classe HibernateUtil dans le package «ma.projet.util ».

4.Créer l’interface générique IDao dans le package « ma.projet.dao ».

5.Créer les classes services : ProjetService, TacheService, EmployeService et
EmployeTacheService qui implémentent l’interface IDao.

6.Créer une méthode permettant d’afficher la liste tâches réalisées par un employé dans la
classe EmployeService.

7.Créer une méthode permettant d’afficher la liste projets gérées par un employé dans la
classe EmployeService.

8.Créer une méthode permettant d’afficher la liste des tâches planifiées pour projet
dans la classe ProjetService.

9.Créer une méthode permettant d’afficher la liste des tâchesréalisées dans un projet 

10.Créer une méthode permettant d’afficher la liste des tâches dont le prix supérieur
à 1000 DH dans la classe TacheService en utilisant une requête nommée.

11.Créer une méthode permettant d’afficher la liste des tâchesréalisées entre deux dates
dans la classe.

12.Créer des programmes permettant de tester les questions 





**TAR:**

**-- Database TAR:--**


![TAR](https://github.com/ELMOUWAHID-AYOUB/HibernateTP/assets/130571009/e8850b23-5274-490a-b0b0-7edcc6f1d6df)


![TAR1](https://github.com/MaskedFezz/tpJDBC/assets/130571009/22f90897-1c84-436c-917b-fc3d49f4d87d)

BASE SQL:

-- phpMyAdmin SQL Dump
-- version 5.2.0
-- https://www.phpmyadmin.net/
--
-- Hôte : 127.0.0.1
-- Généré le : mer. 18 oct. 2023 à 22:00
-- Version du serveur : 10.4.27-MariaDB
-- Version de PHP : 8.2.0

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Base de données : `tar`
--

-- --------------------------------------------------------

--
-- Structure de la table `mariage`
--

CREATE TABLE `mariage` (
  `dateDebut` date NOT NULL,
  `dateFin` date NOT NULL,
  `nbreEnf` int(100) NOT NULL,
  `homme_id` int(100) NOT NULL,
  `femme_id` int(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

-- --------------------------------------------------------

--
-- Structure de la table `personne`
--

CREATE TABLE `personne` (
  `Dtype` varchar(100) NOT NULL,
  `id` int(100) NOT NULL,
  `adrress` varchar(100) NOT NULL,
  `dateNaissance` date NOT NULL,
  `nom` varchar(100) NOT NULL,
  `prenom` varchar(100) NOT NULL,
  `telephone` varchar(199) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Index pour les tables déchargées
--

--
-- Index pour la table `mariage`
--
ALTER TABLE `mariage`
  ADD PRIMARY KEY (`femme_id`);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
