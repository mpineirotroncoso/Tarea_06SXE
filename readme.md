en la ruta de nuestro docker-compose.yml ejecutamos
```sh
sudo docker compose up -d
```
para crear las instancias de prestashop y la base de datos

![](img/compose1.png)

Luego desde el navegador ya podemos acceder a la configuracion del prestashop

![](img/compose2.png)

![](img/compose3.png)

Configuramos la conexion a la base de datos y comporbamos que funcione

![](img/compose4.png)

Esperamos a que la instalacion finalize

![](img/compose5.png)

Ahora tenemos que eliminar la carpeta install y renombrar la carpeta admin

![](img/compose6.png)

Entramos en el container
```sh
sudo docker compose exec ps bash
```

![](img/compose7.png)

Eliminamos la carpeta install
```sh
rm -r install/
```

Renombramos la carpeta admin
```sh
mv admin/ admin449arzmyo29zbrujmi0/
```

![](img/compose8.png)

Ahora accedemos a la carpeta admin desde el navegador

![](img/compose9.png)

![](img/compose10.png)

Ya podemos acceder al dashboard

![](img/compose11.png)
