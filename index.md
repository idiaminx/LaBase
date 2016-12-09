---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---
# Base de Datos para Analizar y Facilitar Información

Es reiterativo el proceso de probar una lista con canales de televisión, muchas de esas listas ofrecen entre 2000 y 3000 canales de televisión. Aparte muchos de esos canales dejan de andar después de unas horas
de publicada las listas por eso es de interés general tener una base de datos creada y mantenida de forma automática a través de scripts que mantenga actualizada las direcciones de los streams de
los canales de televisión.

# Origen de Nuestros Datos: Listas m3u

El origen de nuestros datos son listas de canales en formato m3u con más de 2000 nombres de canales y sus respectiva dirección del stream (el espacio del ancho de banda de mi conección a internet con el video, luego
codificado, de la transmición del canal deseado de ver). Estos tienen direcciones de internet al cual uno se puede conectar y establecer una comunicación entre el servidor y nuestro ordenador.

La base de datos se va a crear y a mantener de forma automática a través de scripts de linux bash, es entonces de desear que los scripts sean efectivos a la hora de determinar la información
contenida en las listas m3u con 2000+ canales. El problema es que los canales a veces vienen denominados de forma diferente, si comparamos una lista con otra, sin embargo se trata del mismo canal
y nuestros scripts deben aprender a diferenciarlos de manera exacta. Salvado ése problema la base de datos funciona perfectamente dado un canal de televisión devuelve un enlace de emisión del canal
que a mi me gusta.

# Tema 1 a la Hora de Obtener Base de Datos que Funcione

El primer tema a la hora de obtener una base de datos que funcione es analizar de manera efectiva y no fortuíta la información de las listas que aparecen en los foros mencionados en el blog y
en la sección acerca de. Para esto serviría de mucho utilizar la `base de datos` para analizar y obtener información realmente feaciente y exacta sobre el contenido de éstas listas. Por ejemplo
ir obteniendo de forma manual la extracción de los nombres de los canales de varias listas e ir documentando que tipos de comandos y que tipos de opciones fueron utilizados cuando procesamos
las listas de forma `individual`.

Llegaría un momento en que los comandos con sus respectivas opciones quedarían determinados por un número finito de `ellos` y enumerados en la `base de datos`. Puesto que esto todo quedaría documentado
en la `base de datos No 1`, la primera parte de construír un algoritmo inteligente habría concluído de manera efectiva. Entonces nos podemos dedicar ahora a través de una `base de datos No 2`, de
procesar de forma efectiva y administrar manteniendo actualizada esta información de nuestra `base de datos No 2` con los streams que funcionen.

<center> o0o0o - o0o0o - o0o0o </center><br><br>
