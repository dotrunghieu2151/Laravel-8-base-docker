
```
[/***/doc-sys-api]
$ cp .env-example .env
```

```
[/***/doc-sys-api/src]
$ cd src
$ cp .env.example .env
```

```
[/***/doc-sys-api]
$ cd ..
$ docker-compose up -d --build
```

```
$ docker-compose exec doc-management-app ash
```

```
[/***/doc-sys-api]
$ docker-compose exec doc-management-app composer install
```


URL：http://127.0.0.1:10080


* doc-sys-api container
```
[/***/doc-sys-api]
$ docker-compose up -d
```

```
[/***/doc-sys-api]
$ docker-compose down
```

```
[/***/doc-sys-api]
$ docker-compose down --volumes --rmi all
```

#### DB

* MySQL Workbench

| --- | --- |
| Host | 127.0.0.1 |
| Port | 13308 |
| User | admin-doc |
| Pass | secret |

#### php artisan

```
[/***/doc-sys-api]
$ docker-compose exec doc-management-app php artisan config:cache
```


```
[/***/doc-sys-api]
$ docker-compose exec doc-management-app ash
[/work/doc-management]
$ php artisan migrate
```
