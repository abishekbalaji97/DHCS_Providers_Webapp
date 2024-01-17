## DHCS_Providers_Webapp
This project provides an example of how one can build an RShiny app that processes data stored in your local MySQL database instance(localhost) and acts as a service locator app one can use to find where they can avail a particular service near their current location. This project uses various datasets provided by the DHCS(https://data.chhs.ca.gov/dataset) portal to create a database with various tables modeled in 3NF form and insert sample records for each of them. This project is only intended to show other avenues the DHCS can consider to set up their data platforms and create reports on top of that and demonstrates the service location functionality with the FFS providers data to allow one to find which FFS(fee for service) medical providers that are enrolled in the Medi-Cal program are nearby one's current location.

#### Commands to use to create a new user in MySQL workbench to connect to the database that is being built in this example
CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';

GRANT ALL PRIVILEGES ON dhcs_medical_programs.* TO 'abishekbalaji97'@'localhost';

#### Steps to follow to set the MySQL user credentials created above as environment variables

1) Use the Sys.getenv("R_USER") command to get your current working directory. In the current working directory, create a .Renviron file with the following commands inside to store the environment variables for your user credentials
user  = username
password = password

## Issues that persist with this app and other components that are planned to be developed are summarized with GitHub Issues
