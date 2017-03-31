# Qrious

First of all create these Tables in your local databse :

CREATE TABLE user (
  userid int(10) NOT NULL AUTO_INCREMENT,
  fname varchar(50) NOT NULL,
  lname varchar(50) NOT NULL,
  uname varchar(50) NOT NULL,
  mobile varchar(12) NOT NULL,
  email varchar(255) NOT NULL,
  dob varchar(15) NOT NULL,
  password varchar(100) NOT NULL,
  PRIMARY KEY (userid)
);


CREATE TABLE qsn(
	qsnid int(5) NOT NULL AUTO_INCREMENT,
	qsn varchar(2500) NOT NULL,
	Category varchar(50) NOT NULL,
	userid int(10)	NOT NULL,
	PRIMARY KEY(qsnid)
);


CREATE TABLE ans(
	ansid int(5) NOT NULL AUTO_INCREMENT,
	qsn varchar(5000) NOT NULL,
	qsnid int(5) NOT NULL,
	userid int(10)	NOT NULL,
	PRIMARY KEY(ansid)
);
