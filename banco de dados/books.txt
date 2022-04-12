-- MySQL Workbench Forward Engineering

SET @OLD_UNIQUE_CHECKS=@@UNIQUE_CHECKS, UNIQUE_CHECKS=0;
SET @OLD_FOREIGN_KEY_CHECKS=@@FOREIGN_KEY_CHECKS, FOREIGN_KEY_CHECKS=0;
SET @OLD_SQL_MODE=@@SQL_MODE, SQL_MODE='ONLY_FULL_GROUP_BY,STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_ENGINE_SUBSTITUTION';

-- -----------------------------------------------------
-- Schema books_controll
-- -----------------------------------------------------

-- -----------------------------------------------------
-- Schema books_controll
-- -----------------------------------------------------
CREATE SCHEMA IF NOT EXISTS `books_controll` DEFAULT CHARACTER SET utf8 ;
USE `books_controll` ;

-- -----------------------------------------------------
-- Table `books_controll`.`books`
-- -----------------------------------------------------
CREATE TABLE IF NOT EXISTS `books_controll`.`books` (
  `ID` INT NOT NULL AUTO_INCREMENT,
  `name_b` VARCHAR(100) NOT NULL,
  `author_b` VARCHAR(100) NOT NULL,
  `number_pages` INT NOT NULL,
  `theme_b` VARCHAR(100) NOT NULL,
  `language_b` VARCHAR(45) NOT NULL,
  PRIMARY KEY (`ID`))
ENGINE = InnoDB;


SET SQL_MODE=@OLD_SQL_MODE;
SET FOREIGN_KEY_CHECKS=@OLD_FOREIGN_KEY_CHECKS;
SET UNIQUE_CHECKS=@OLD_UNIQUE_CHECKS;
