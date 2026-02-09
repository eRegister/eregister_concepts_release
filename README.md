# eregister_concept_release

1. ssh into your server with `ssh openmrs@server_ip` and then enter the server the password when prompted
2. Go to the `development_emr` folder with `cd /development_emr`
3. clone the concepts folder by running `sudo git clone https://github.com/eRegister/eregister_concepts_release.git`
4. Get into your container cli with `docker exec -it bahmni_docker_emr-service_1 bash`
5. CD to the `development` folder with `cd /development`
3. Get into your MySQL server by running `mysql -u root -p`
4. Choose your db `use openmrs`
5. Import the latest concepts with `source omrs_concept_dictionary.sql`