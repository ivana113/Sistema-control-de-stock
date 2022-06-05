

<em>Instalamos nuestras dependencias con</em>
<pre><code><b>composer install</b></code></pre>
<em>Realizamos una copia de nuestro archivo .env con el siguiente comando</em>
<pre><code><b>cp .env.example .env</b></code></pre>
<em>Generamos la key para nuestro .env</em>
<pre><code><b>php artisan key:generate</b></code></pre>
<em>Instalamos nuestros paquetes necesarios </em>
<pre><code><b>npm install</b></code></pre>
<em> Compilamos </em>
<pre><code><b>npm run dev</b></code></pre>
<h3>Una vez terminemos con los pasos anteriores, procedemos a configurar nuestro archivo .env</h3>

<h2>IMPORTANTE:</h2>

<p>En el archivo .env creamos 2 variables nuevas llamadas: <b>APP_PATH_LOCAL_VUE && SANCTUM_STATEFUL_DOMAINS</b> </p>	
<ul>
	<li><b>APP_PATH_LOCAL_VUE || VALOR PREDETERMINADO "VACIO" :</b> Esta variable fue creada para entornos donde no contemos con un servidor o donde no podamos ejecutar el comando "<b>php artisan serve</b>" para que levante nuestro servidor, en esta variable podemos colocar la ruta absoluta en donde se encuentro nuestro public, ejemplo: github/visitas/public, de este modo vuejs apuntara hacia esta ruta. Es opcional</li>
	<li><b>SANCTUM_STATEFUL_DOMAINS || VALOR PREDETERMINADO "localhost" :</b> Variable importante para sanctum, paquete que usamos para autenticación, debemos colocar nuestra url sin su protocolo ejemplo: example.com </li>
</ul>

