# InsuranceCompany-Database
mysql> create database IC;
mysql> use IC;

mysql> create tablE participated(driver_id varchar(10),regno varchar(10),report_no int, damage_amt float(10,2));
mysql> create table person(driver_id char(10),name varchar(20), address varchar(30));
mysql> create table CAR(regno varchar(10), model varchar(30), year int(4));
mysql> create table ACCIDENT(ReportNumber int(10),acc_date date, location varchar(20));
mysql> create table OWNS(driver_id varchar(10), regno varchar(20));

mysql> insert into OWNS values("1","UP36E7");
mysql> insert into OWNS values("2","UP16E7");
mysql> insert into OWNS values("3","DL16E7");
mysql> insert into OWNS values("4","DL00E7");
mysql> insert into OWNS values("5","DL10E7");

mysql> insert into CAR values("Duster", "2",2000);
mysql> insert into CAR values("DC Avanti", "36",2009);
mysql> insert into CAR values("Porsche", "36",2020);
mysql> insert into CAR values("Fortuner", "43",2021);
mysql> insert into CAR values("Creta", "4",2022);

mysql> insert into PERSON values("1","Vanshika","Rajnagar");
mysql> insert into PERSON values("2","Steve","Rajnagar");
mysql> insert into PERSON values("3","Aditya","Noida");
mysql> insert into PERSON values("4","Prakhar","Wave City");
mysql> insert into PERSON values("5","Vanshii","Wave City");

mysql> insert into participated values("1","UP36E7",27,6000);
mysql> insert into participated values("2","UP16E7",17,10000);
mysql> insert into participated values("3","DL16E7",10,11000);
mysql> insert into participated values("4","DL00E7",22,9000);
mysql> insert into participated values("5","DL10E7",40,8500.97);

mysql> alter table PERSON add PRIMARY KEY (driver_id);
mysql> alter table CAR add primary key(regno);
mysql> alter table ACCIDENT add primary key(ReportNumber);
mysql> alter table OWNS add primary key(driver_id);
mysql> alter table PARTICIPATED add primary key(driver_id);

mysql> select * from ACCIDENT;
mysql> select * from CARS;
mysql> select * from OWNS;
mysql> select * from PARTICIPATED;
mysql> select * from PERSON;

mysql> update participated set damage_amt=16000 where regno="UP36E7";
mysql> update accident set location="U.P." where ReportNumber BETWEEN 12 AND 25000;
mysql> insert into accident values(2314,"2021-09-30","Delhi");

