<h1>PENTALINK</h1>

![alt text](https://github.com/OscarJansana/Pentalink/blob/Im%C3%A1genes/PentaLink%20logo%20update.png)

## índice
  * [Introducción](#introduccion)
  * [Materiales necesarios](#materiales-necesarios-(hardware-y-software))
  * [Red](#red)
  * [Web](#web)
  * [Servicios](#servicios)
  * [Incidencias](#incidencias)
  * [Conclusiones](#conclusiones)
  * [Bibliografía](#bibliografia)

<details>
<summary><h2>Introducción</h2></summary>

Somos un grupo de estudiantes de IFP Innovación en formación profesional Hospitalet del Llobregat, nuestros nombres son Paula Simó, Oscar Jansana y Aleksei Zagrebelnii. Tenemos como idea de proyecto intermodular el crear un portal web donde los usuarios podrían registrarse y compartir contenido multimedia creado por ellos mismos. Esta idea ha sido referenciada por otros 2 portales <a href="https://www.newgrounds.com/">New Grounds</a>, donde hemos cogido como referencia el poder subir diversos distintos tipos de entretenimiento y, posteriormente <a href="https://spacehey.com/">MySpace</a>, actualemte conocido como SpaceHey como formato para la creación de usuarios.<br>
<br>Como nombre del proyecto hemos decidido poner PentaLink, este, referencia a los 5 tipos de archivos que se podrán subir al portal web, que serán Blogs, Imágenes, Música, Vídeos y Videojuegos.


### Objetivo e ideas
Como objetivo principal, queremos crear un portal web funcional donde cada usuario pueda subir el contenido que desee, al igual que visitar el contenido subido por los otoros usuarios con los 5 tipos de archivos mencionados anteriormente (blogs, imágenes, música, vídeos y videojuegos) diferenciados por sus respectivas secciones. Para en el caso de las imágenes, música y vídeos permitiríamos que se pudieran subir archivos con distintas extensiones por cada tipo. Como ejemplo para terminar de entender a qué nos referimos con las distintas extensiones por archivo sería para el caso de las imágenes, que el usuario pudiera subir imágenes jpg, jpeg, pnj (entre otros que también existen), en el caso de música podría ser con formato mp3 o wav y finalmente, en el caso de vídeos mp4 o wmv.<br>

<br>Para el caso de los blogs, nuestra idea es que en cambio de que los usuarios suban un archivo como blog integrarlo dentro del portal, es decir, el usuario crearía un nuevo blog donde lo que le aparecería para publicarlo serian 2 cajas de texto, donde una sería el título/asunto del blog y posteriormente el cuerpo del mismo. Finalmente, en el caso de los videojuegos intentaremos integrar los que sean más simples y ejecutables dentro del mismo navegador.<br>

<br>Una vez tengamos el portal (descrito anteriormente) completamente funcional es cuando nos gustaría hacer las ampliaciones con el objetivo de hacerlo lo más completo posible, donde tenemos pensadas ya ciertas ampliaciones, como pueden ser las siguientes:<br>

<ul>
<br><li> Para el apartado de videojuegos nos gustaría que se pudiera permitir subir videojuegos más complejos y estos poder descargarlos para poder jugarlos
<br><li> Para el perfil del usuario nos gustaría poder agregar la personalización básica, es decir, el poder cambiar la foto de perfil, biografía y banner
<br><li> Agregar la posibilidad de añadir comentarios en las publicaciones de otros usuarios
<br><li> Agregar la opción de poder dar Like, Dislike y poder agregar a favoritos una publicación
<br><li> Poder personalizar lo máximo posible la experiencia del usuario, añadiendo por ejemplo la opción de poder mostrarle un apartado de relevantes o recomendados para él encima de las publicaciones recientes de los usuarios
</ul>


### Público objetivo
El público objetivo de este portal es bastante amplio gracias a su amplio contenido y versatilidad de contenido, algunos ejemplos del público con el que queremos conectar son: <br>
<ul>
<br><li> Jóvenes creativos con ganas de compartir su pasión y arte con otras personas
<br><li> Personas que quieran conectar con otros usuarios que tengan sus mismos intereses
<br><li> Bloggers o escritores que quieran compartir o dar ideas para historias
<br><li> Gente interesada en un tipo de red social o plataforma alternativa
</ul>


### Módulos del ciclo relacionados
Los módulos que consideramos relacionados de nuestro ciclo (Sistemas Microinformáticos y Redes) con el proyecto son los siguientes:
<ul>
<li>Aplicaciones web: Para el diseño y el desarrollo de la página web.</li>
<li>Servidores en red: Para instalar y configurar los servidores que formarán parte de la red de nuestro proyecto.</li>
<li>Seguridad informática: Para reforzar la seguridad de la web y nuestros servidores (firewall, copias de seguridad...)</li>
<li>Sistemas operativos en red: Para instalar y configurar los sistemas operativos y máquinas virtuales que utilizaremos para desarrollar el proyecto.</li>
</ul>
</details>
<details>
<summary><h2>Materiales necesarios (Hardware y software)</h2></summary>
Para la implementación de la infraestructura del proyecto hemos optado por el uso del Docker como parte principal de virtualización y despliegue de servicios, de esta forma, podremos tener en distintos contenedores los servicios de DNS, DHCP y WEB donde tendremos una mayor facilidad de mantenimiento, ya que, de esta forma podremos garantizar un mejor control de los recursos. Aparte de este servidor, implementaremos otro dedicado exclusivamente a las copias de seguridad, de esta forma podremos realizar respaldos automáticos y periódicos de los servicios principales para poder asegurar la disponibilidad y recuperación en caso de fallos o incidentes de seguridad.
 
 <br>** agregar parte del router y firewall ** Aparte, para poder reforzar la seguridad de la WEB, tenemos pensado implementar cloudflare como capa de protección y optimización del tráfico, de esta forma, podremos tener protección frente ataques y amenazas comunes

<br>Por otro lado, para el apartado de los videojuegos hemos pensado en poder abarcar la mayor cantidad de lenguajes de programación que hay (es decir, admitirlos todos) para que, de esta forma, los usuarios tengan la libertad absoulta de subir los juegos que quieran. Para ello, diferenciaremos los lenguajes en 2 grupos, los que incluyen la tecnologia compatible y los que no, para los que sean compatibles los ejecutaremos directamente en el navegador y se jugará de forma completamente online con opción a descargar el juego, en caso de no ser compatible, se deberán descargar para poder ser jugados.

<br>El grupo que se considera compatible serían HTML5, JavaScript (JS), WebAssembly (WASM) y los que puedan ser interpretados a través de JS o WASM como Python, Ruby, Lua, C, C++ o Rust, mientras que los no compatibles son los que se encuentran fuera de esta lista. De esta forma, podemos garantizar que se puedan jugar todos los juegos que suban los usuarios utilizando el lenguaje de programación que quieran. 


### Recursos
Los recursos principales que estamos utilizando son aquellos que estamos subiendo en el <a href="https://trello.com/b/C53JrxYj/amnis-project">Trello</a>, donde estamos añadiendo enlaces de tutoriales y cursos para estudiar sobre los temas que aún no controlados, aparte de ello, también estamos creando documentos aparte con muestros apuntes y explicaciones para poder aprender sobre Docker, MySql, PHP y la implementación del Cloudflare.
</details>
<details>
<summary><h2>Red</h2></summary>
Para la red seguiremos el esquema básico que se nos ha mostrado en clase. Dentro de nuestra red interna, tendremos cuatro servidores:
<ol>
<li><b>Servidor web</b>
 <br>Donde almacenaremos: 
 <br>- Apache
 <br>- PHP
 <br>- Html, Css y JavaScript
<li><b>Base de datos</b>
 <br>Que contendrá:
 <br>- MySQL
 <br>- PHPmyadmin
<li><b>Servidor DNS</b>
<li><b>Backup</b>
 <br>Donde haremos copias de:
 <br>- Apache
 <br>- PHP
 <br>- MySQL (Base de datos)
 <br>- Configuración del DNS
 <br>- Firewall
</ol>

### Diagrama de la red

Este es el esquema de red que utilizaremos; es el mismo que se nos fue proporcionado en clase. 

<img width="2000" height="1400" alt="Red de clase (dhcp) (2)" src="https://github.com/user-attachments/assets/d21bfec3-fcb5-44a0-8266-4405b9c06172" />

### Mapa físico

### Mapa lógico
</details>
<details>
<summary><h2>Web</h2></summary>

### Diseño

### Mockup
Como colores para nuestro portal web hemos elegido un color turquesa oscuro como base, esto se debe a que lo hemos considerado un color muy bonito y sólido con el que poder hacer grandes combinaciones gracias a su versatilidad. Aparte de ello, consideramos que este color puede llegar a transmitir un punto elegante donde evitamos los tonos más comunes y combinables con el blanco o negro para que se haga una vista menos pesada y más suavizada.

<br>Como colores secundarios o llamados complementarios hemos elegido 3 tonos distintos. Como primer tono hemos elegido una escala de grises claros para que puedan dar un toque de claridad. donde pueda tener una legibilidad superior sobre el fondo y a su misma vez, puede reducir el impacto de brillo o contraste excesivo que pudiera fatigar la vista como pudiera pasar con el color blanco.

<br>Como segundo tono, hemos elegido un color gris oscuro, para aportar el toque de oscuridad, profundidad textura y diferenciación, donde lo usaremos para crear capas que no rompan el esquema oscuro que ya tiene la web. La idea sería utilizarlo para la diferenciación de áreas principales y secundarias, para que el contenido se vea en armonía sin que parezcan simples pegotes y pueda dar la sensación underground y retro de los portales Newground y MysPace en los que nos hemos basado, comentados ya anteriormente.

<br>Como tercer y último tono, hemos decidido elegir un tono amarillo, para que de esta forma podamos aportar un contraste a la vista del usuario, de esta forma fomentaremos la interacción. Esta interacción se verá aumentada gracias al gran contraste generado con el fondo oscuro, ya que obligaremos al ojo a mirar primero los elementos amarillos, donde lo usaremos en etiquetas, notificaciones, botones o bien, para otros detalles que consideremos convenientes y necesarios que el usuario vea

<br>A continuación, podemos ver los ejemplos de los tonos elegidos y cómo se verían combinados:
<img width="950" height="350" alt="cp-removebg-preview" src="https://github.com/user-attachments/assets/1173cdba-1bb6-4e22-b0d5-e5763b073be0" />

### Mapa de navegabilidad

</details>
<details>
<summary><h2>Servicios</h2></summary>
 
### DNS

### DHCP

### Apache

### Firewall

### Copias de seguridad

</details>
<details>
<summary><h2>Incidencias</h2></summary>
</details>
<details>
<summary><h2>Conclusiones</h2></summary>
</details>
<details>
<summary><h2>Bibliografía</h2></summary>

### Documentación general
https://github.com/ossu/computer-science

https://www.geeksforgeeks.org/python/how-to-use-css-in-python-flask/

### Documentación sobre MySql
http://youtube.com/watch?v=AJUJ1f9gFm8

https://www.tutorialesprogramacionya.com/mysqlya/

### Documentación sobre Docker
https://www.geeksforgeeks.org/devops/docker-tutorial/ 

</details>
