# spring-security-jpa
Code for full Spring Security + JPA + MySQL tutorial:  https://youtu.be/TNt3GHuayXs

# Database Scheme
CREATE TABLE users( <br />
  id bigint(20) NOT NULL PRIMARY KEY AUTO_INCREMENT, <br />
  active bit(1) NOT NULL, <br />
  password varchar(50) NOT NULL, <br />
  roles varchar(50) NOT NULL, <br />
  user_name varchar(50) NOT NULL);
  
# Adding Entries to the table
INSERT INTO users(user_name, password, active, roles) VALUES ('user', 'pass', false, 'ROLE_USER');
