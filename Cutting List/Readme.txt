To Create DataBase And Table....................

1) CREATE DATABASE `cutting_list`;
2) USE `cutting_list`
3) CREATE TABLE `material` (
  `id_no` varchar(25) NOT NULL,
  `partname` varchar(45) DEFAULT NULL,
  `material` varchar(45) DEFAULT NULL,
  `length` varchar(45) DEFAULT NULL,
  `width` varchar(45) DEFAULT NULL,
  `thickness` varchar(45) DEFAULT NULL,
  `diameter` varchar(45) DEFAULT NULL,
  `quantity` varchar(45) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

4) CREATE TABLE `userinfo` (
  `id_no` varchar(25) NOT NULL,
  `email` varchar(45) DEFAULT NULL,
  `teacher` varchar(45) DEFAULT NULL,
  `batch` varchar(45) DEFAULT NULL,
  `date` varchar(45) DEFAULT NULL,
  `image` mediumblob,
  `lesson` varchar(45) DEFAULT NULL,
  PRIMARY KEY (`id_no`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;


UserId and password for logining as a student:-student Login
				UserId:-101
				Password:student1

UserId and password for logining as a teacher:-teacher Login
				UserId:-110
				Password:teacher1

UserId and password for logining as a student:-student Login
				UserId:-1110
				Password:admin123

*Note:- For Checking or Changing userId and password go to there corresponding servlet pages...


After designing the database make changes in connection url in the following files:---
1)DBConnection.java
2)adminportal.jsp
3)adminnotification.jsp
4)image.jsp
5)Notification.jsp
6)Request.jsp
7)teacherportal.jsp

*Note:- Replace the id,password in existing connection url with your database credentials....
     :-use tomcat8 and mysql-connector-java-5.1 and above......

