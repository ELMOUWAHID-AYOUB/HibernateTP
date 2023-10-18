# HibernateTP
Hibernate est un framework open source en Java qui facilite le développement d'applications Java en fournissant un mapping objet-relationnel (ORM). L'ORM est une technique de 
programmation qui lie les objets d'une application à une base de données relationnelle. Hibernate simplifie le processus de stockage et de récupération d'objets Java à partir 
d'une base de données. Il simplifie également la gestion de la base de données en permettant aux développeurs de travailler avec des objets Java au lieu d'écrire des requêtes SQL.



Database H1

![h1](https://github.com/ELMOUWAHID-AYOUB/HibernateTP/assets/130571009/6a460799-071e-4250-b43f-fc68e4c371bc)

BASE SQL:

-- phpMyAdmin SQL Dump
-- version 5.2.0
-- https://www.phpmyadmin.net/
--
-- Hôte : 127.0.0.1
-- Généré le : mer. 18 oct. 2023 à 21:37
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
-- Base de données : `h1`
--

-- --------------------------------------------------------

--
-- Structure de la table `produit`
--

CREATE TABLE `produit` (
  `id` int(11) NOT NULL,
  `dateAchat` date DEFAULT NULL,
  `desig` varchar(255) DEFAULT NULL,
  `marque` varchar(255) DEFAULT NULL,
  `prix` double NOT NULL,
  `ref` varchar(255) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Déchargement des données de la table `produit`
--

INSERT INTO `produit` (`id`, `dateAchat`, `desig`, `marque`, `prix`, `ref`) VALUES
(1, '2020-11-06', 'rabat', 'infinx', 90, '373S8HS82'),
(2, '2020-11-06', 'london', 'sumsung', 3745, 'FNFNF8724RR3J'),
(4, '2020-11-06', 'fes', 'appelLe', 5000, 'FJDJ5ADJO4589'),
(5, '2020-11-06', 'casa', 'redmi', 7355, 'F89DF9AEJZ3R8'),
(6, '3920-11-17', 'casa', 'redmi', 7355, 'F89DF9AEJZ3R8'),
(7, '3921-11-17', 'casa', 'redmi', 7000, 'F89DF9AEJZ3R8'),
(8, '3909-11-11', 'casa', 'redmi', 7000, 'F89DF9AEJZ3R8'),
(9, '3909-11-11', 'casa', 'redmi', 7000, 'F89DF9AEJZ3R8'),
(10, '3909-12-11', 'casa', 'redmi', 7000, 'F89DF9AEJZ3R8'),
(11, '1900-10-11', 'casa', 'redmi', 7000, 'F89DF9AEJZ3R8'),
(12, '2023-10-16', 'casa', 'redmi', 7000, 'F89DF9AEJZ3R8');

--
-- Index pour les tables déchargées
--

--
-- Index pour la table `produit`
--
ALTER TABLE `produit`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT pour les tables déchargées
--

--
-- AUTO_INCREMENT pour la table `produit`
--
ALTER TABLE `produit`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=13;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
Database H3:



Database TAR:


![TAR](https://github.com/ELMOUWAHID-AYOUB/HibernateTP/assets/130571009/e8850b23-5274-490a-b0b0-7edcc6f1d6df)



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
