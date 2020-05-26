# angular9phpdatabase
Angular 9 with php and mysql database
npm install -g @angular/cli //Setup Angular9  
ng new angular9php  //Install New Angular App
/**You need to update your Nodejs also for this verison**/
cd angular9php  //Go inside the Angular 9 Project

add this repo to the Project to override the src/app folder

create an employee.php file in ur PHP wamp server in the document root

create database as company
The SQL file for employee table 

-- --------------------------------------------------------

--
-- Table structure for table `employee`
--

DROP TABLE IF EXISTS `employee`;
CREATE TABLE IF NOT EXISTS `employee` (
  `id` int(12) NOT NULL AUTO_INCREMENT,
  `name` varchar(50) NOT NULL,
  `email` varchar(50) NOT NULL,
  `created_date` datetime NOT NULL DEFAULT CURRENT_TIMESTAMP,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=3 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

--
-- Dumping data for table `employee`
--

INSERT INTO `employee` (`id`, `name`, `email`, `created_date`) VALUES
(1, 'David', 'david@example.com', '2020-05-26 10:28:08'),
(2, 'james', 'james@example.com', '2020-05-26 10:28:08');
COMMIT;
