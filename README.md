# spring-security-jpa
Code for full Spring Security + JPA + MySQL tutorial:  https://youtu.be/TNt3GHuayXs

# Database Scheme
CREATE TABLE users( <br />
  &nbsp;&nbsp;&nbsp;&nbsp;id bigint(20) NOT NULL PRIMARY KEY AUTO_INCREMENT, <br />
  &nbsp;&nbsp;&nbsp;&nbsp;active bit(1) NOT NULL, <br />
  &nbsp;&nbsp;&nbsp;&nbsp;password varchar(50) NOT NULL, <br />
  &nbsp;&nbsp;&nbsp;&nbsp;roles varchar(50) NOT NULL, <br />
  &nbsp;&nbsp;&nbsp;&nbsp;user_name varchar(50) NOT NULL);
  
# Adding Entries to the table
INSERT INTO users(user_name, password, active, roles) VALUES ('user', 'pass', false, 'ROLE_USER');
