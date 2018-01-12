---
author_name: Rosa Sala
author_bio: Rosa Sala es CEO y co-fundadora de Nubart
author_location: Berlín / Barcelona
author_image: /blog/images/rosa-sala.jpg
author_url: https://www.linkedin.com/in/rosasalarose/
layout: post
comments: true
published: true
title:  "Las audiorutas Nubart también funcionan sin wifi y sin cobertura de datos"
description: "Aquí te contamos qué nos llevó a desarrollar el modo offline en nuestra primera audioruta por paisajes sin cobertura"
slug: "audioruta-nubart-offline"
date:   2018-01-03
banner_image: audioruta-nexo-nubart-maestrazgo.jpg
tags: [offline, audioruta]
---

A veces un problema acaba siendo una gran oportunidad. Eso es lo que tuvimos ocasión de comprobar con la audioruta por los monumentos naturales del Maestrazgo (Teruel) que produjimos para Nexo Turismo y Cultura y que fue el origen de nuestra primera audioguía digital offline para smartphones que funciona sin wifi y sin cobertura. Aquí te contamos la historia. 

<!--more-->

## No solo audioguías, también hacemos audiorutas

Nuestras audioguías en forma de tarjeta Nubart no solo son útiles para los museos. También pueden ofrecerse en puntos de venta alternativos, como oficinas de información turística, y adaptarse para realizar visitas guiadas a territorios más extensos, como ciudades o espacios naturales. Así lo reconoció Noelia Porrúa cuando tras establecerse en la maravillosa comarca del Maestrazgo decidió fundar la empresa [Nexo Turismo y Cultura.](https://www.facebook.com/Nexo-Turismo-y-Cultura-484623901869492/){:target="_blank"}

Noelia nos contactó porque, además de las visitas guiadas que está preparando, deseaba poder ofrecer la posibilidad de conocer el territorio a los senderistas que prefirieran ir a su aire, sin ir acompañados de un guía, o a los visitantes extranjeros que quisieran hacer la visita en su propio idioma. 

También quería impulsar la economía local mediante la venta de nuestras tarjetas en los establecimientos de la zona. Hace poco que la espectacular belleza de los parajes naturales de El Maestrazgo se está dando a conocer y el turismo todavía es incipiente. "Hay muchas webs que dan información -nos cuenta Noelia- pero tienes que ir visitándolas todas una por una. Yo buscaba que el visitante tuviera toda la información en su móvil, pero también que los establecimientos de la zona pudieran ofrecer sus servicios en este nuevo formato tangible que ofrecéis". 

## El problema de los parajes naturales sin cobertura de datos

Hacía tiempo que en Nubart queríamos producir una ruta turística, así que nos animamos mucho con el proyecto. Noelia preparó un guión estupendo que nosotros revisamos y tradujimos al inglés y al francés. Preparamos la locución en estos dos idiomas y en castellano y reelaboramos los mapas para adaptarlos al contenido de la audioruta. También diseñamos la tarjeta empleando las fotos de Noelia. 

![Audioruta Nubart por los monumentos naturales de El Maestrazgo - Nexo Turismo y Cultura]({{site.baseurl}}/images/posts/audioruta-nexo-nubart-maestrazgo.jpg){: .center-image }

Todo iba viento en popa hasta que le preguntamos por los tuits.

Nuestras audioguías disponen de [la opción "tuitea sobre esta pieza"](/blog/2016/12/12/difusion-visitantes-twitter-audioguia-nubart/){:target="_blank"} que permite que el mismo usuario genere contenido difundiendo la exposición o la excursión desde su propia cuenta en la red social. "Puede que no sea buena idea colocar este botón en tu ruta -le dijimos a Noelia- porque aunque nuestros contenidos están adaptados para consumir el mínimo de datos y cargar con rapidez, la app de Twitter funciona con lentitud cuando la cobertura no es muy buena". "En efecto -nos contestó- mejor lo quitamos. En El Maestrazgo no hay cobertura".

Ups... 

¿Que no hay cobertura en El Maestrazgo? 

En Nubart nos quedamos helados. Nuestras tarjetas funcionan en *streaming*, de modo que a falta de wifi la cobertura de datos, por mala que sea, es necesaria. El contenido estaba producido, la audioruta montada y las tarjetas impresas. Solo que sin datos o sin wifi resultaban inservibles. Se había producido un malentendido. 

Pero ¿es posible que en pleno siglo XXI y en plena UE queden todavía zonas sin cobertura de datos? ¿Qué sucede si un escalador se accidenta y necesita el móvil para pedir ayuda? No nos lo podíamos creer, pero [Internet le dio la razón a Noelia.](https://www.lacomarca.net/dga-atendera-las-quejas-por-la-falta-de-cobertura-en-el-maestrazgo/){:target="_blank"}  ¿Recuerdan el dicho de que "Teruel no existe"? 

Pues bien, el caso es que teníamos un serio problema. Todos habíamos empleado muchas horas e ilusión en este proyecto. Y ahora, o le devolvíamos el dinero a nuestro cliente y aprovechábamos las tarjetas para hacer un mosaico decorativo en el despacho o para fabricar un salvaplatos, o buscábamos una solución técnica. 

## El problema de la descarga offline de contenidos sin instalar una app

Estaba claro que la solución pasaba por permitir la descarga completa del contenido de la audioruta en un lugar que disponga de cobertura para más tarde poder acceder a él desde el móvil, pero sin conexión, en modo offline. En teoría esta capacidad solo está reservada a las apps móviles. Pero en Nubart no desarrollamos apps ni somos partidarios de hacerlo. Había que dar con el modo de utilizar nuestras audioguías Nubart en modo offline desde el mismo navegador y de forma inmediata, sin necesidad de pasar por el engorroso trámite de buscar una app, descargarla, instalarla, abrirla y dar permisos. Tampoco queríamos consumir la memoria del móvil del usuario, como hacen las apps al instalarse. 

Si eres un poco *teckie*, sabrás que en html existe el atributo "preload" aplicable a los archivos en audio y que teóricamente permite su descarga automática. Pero la realidad es que cada navegador decide a su gusto si seguir o no esa indicación, y prácticamente ninguno de los navegadores para teléfono móvil la sigue. Como las audioguías y audiorutas Nubart están especialmente concebidas para su uso desde un smartphone, la etiqueta *preload* no resultaba una solución viable. 

En definitiva: el 99 % de las empresas de software a las que consultáramos nos dirían que, sin una app, nuestro problema no tiene solución.

## Cómo funcionan nuestras audioguías o audiorutas en modo offline

Suerte que en Nubart disponemos de un arma secreta llamada Simon Effing, nuestro cofundador y CTO. Mediante un uso inteligente de Javascript de última generación, Simon encontró el modo de hacer que la descarga del contenido completo de la audioruta se produzca siempre desde cualquier navegador y se almacene de forma pasajera en la memoria temporal del móvil (también llamada 'memoria de acceso aleatorio' o 'memoria RAM'). Tal como nosotros queríamos, la información contenida en la RAM no consume memoria, ya que desaparece al cerrar la página del navegador o al apagarse el dispositivo. No obstante, eso no significa que se pierda para siempre: el usuario siempre podrá recuperarla al emplear de nuevo el código único de su tarjeta Nubart. Y todo esto de forma inmediata y fácil, sin descargar ninguna app. 

En este vídeo puedes ver todo el proceso en tiempo real:
<video width="720" height="548">
  <source src="{{site.baseurl}}/images/posts/audioruta-offline-nubart.mp4" type="video/mp4">
Tu navegador no permite mostrar este vídeo.
</video>{: .center-image }
Como ves, el proceso para acceder a nuestras audiorutas offline es tan fácil para nuestros usuarios como el de cualquier otra audioguía Nubart en streaming convencional. Tan solo hay que esperar un poquito más a que se produzca la carga del contenido.

Además de la urgencia de resolver el problema de Noelia, vimos que la modalidad de uso offline también podría beneficiar a otros clientes, como los numerosos museos que solo disponen de Wifi en la zona de recepción, pero no en las salas de exposiciones. También solventaba un problema a los turistas extracomunitarios que no desean pagar *roaming* mientras utilizan la audioguía, ya que pueden descargar el contenido con el wifi gratuito del punto de venta o del hotel.

Y así es como el problema de un cliente se convirtió en una nueva oportunidad.

Aprovechamos para desearle mucho éxito a Noelia Porrúa con su fantástica iniciativa, que sin duda contribuirá a que a partir de ahora Teruel *exista*.

#### En Nubart producimos audioguías innovadoras y asequibles.

<form action="http://www.nubart.eu/es/">
    <input type="submit" value="Visita nuestra web" />
</form>