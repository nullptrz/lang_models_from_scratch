### Setting up Portainer

```Shell
docker volume create portainer_data
```

```Shell
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:2.21.0
```

```Username
admin
```


```Password
admin123456%
```

### Setting up PgAdmin 4

```Docker
version: "3.8"  
services:  
	pgadmin:  
		image: dpage/pgadmin4  
		container_name: pgadmin4_container  
		restart: always  
		ports:  
			- "5050:80"  
		environment:  
		PGADMIN_DEFAULT_EMAIL: admin@localhost.com 
		PGADMIN_DEFAULT_PASSWORD: admin@123456%
		volumes:  
			- pgadmin-data:/var/lib/pgadmin  
  
volumes:  
	pgadmin-data:
```

```Username
admin@localhost.com 
```

```Password
admin@123456%
```


### PostgresDB Credentials

```Username
admin
```

```Password
admin123!
```

