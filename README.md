# MySQL Practice

**Requirement**: MacOS or Linux


1. Download Docker for MacOS:

<https://download.docker.com/mac/stable/Docker.dmg>

> Run the following commands in your **Terminal**

2. Pull custom built image with test data: 
```bash
docker run -d --name sql amacharla/mysql-practice
```

3. Access mysql container:
```bash
docker exec -it sql /bin/bash
```

4. Onces inside the container here is how you access MySQL:
```
mysql -uroot -proot hbnb_dev_db
```

5. To exit container:
```bash
exit
```
---

### Things to try once you accessed the container :
- `show databases;` <- see all the databases
- `show tables;` <- see all the tables IN the hbnb_dev_db database
- `select * from amenities;` <- see all the columns and rows in the amenities table inside the hbnb_dev_db database



> Note: This mysql instance is running inside your computer in a docker container.
