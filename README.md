# spring-security-jpa
Code for full Spring Security + JPA + MySQL tutorial:  https://youtu.be/TNt3GHuayXs

# Database Scheme
CREATE TABLE users( 
  id bigint(20) NOT NULL PRIMARY KEY AUTO_INCREMENT, 
  active bit(1) NOT NULL, 
  password varchar(50) NOT NULL, 
  roles varchar(50) NOT NULL, 
  user_name varchar(50) NOT NULL);
  
# Adding Entries to the table
INSERT INTO users(user_name, password, active, roles) VALUES ('user', 'pass', false, 'ROLE_USER');
