# DHCS_Providers_Webapp
This project provides an example of how one can build an RShiny app that processes data stored in your local MySQL database instance(localhost) and acts as a service locator app one can use to find where they can avail a particular service near their current location. This project uses data provided by to implement various and demonstrates the service location functionality with the FFS providers data to allow one to find which FFS(fee for service) medical providers that are enrolled in the Medi-Cal program are nearby one's current location.

## Commands to use to create a new user in MySQL workbench to connect to the database that is being built in this example
CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';

GRANT ALL PRIVILEGES ON dhcs_medical_programs.* TO 'abishekbalaji97'@'localhost';

## Steps to follow set the username and password for the MySQL user created above as environment variables
