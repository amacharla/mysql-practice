# MySQL Practice

**Requirement**: MacOS or Linux


### Download Docker for MacOS:

<https://download.docker.com/mac/stable/Docker.dmg>

### Sandbox Environment

> Run the following commands in your **Terminal**

1. Pull custom built image with test data: 
```bash
docker run -d --name sql amacharla/mysql-practice
```

2. Access mysql container:
```bash
docker exec -it sql /bin/bash
```

3. Onces inside the container here is how you access MySQL:
```
mysql -uroot -proot hbnb_dev_db
```

4. To exit container:
```bash
exit
```

---

### Things to try once you accessed the container :
- `show databases;` <- see all the databases
- `show tables;` <- see all the tables IN the hbnb_dev_db database
- `select * from amenities;` <- see all the columns and rows in the amenities table inside the hbnb_dev_db database



> Note: This mysql instance is running inside your computer in a docker container.
