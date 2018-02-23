Esta página/sección recopila es un block de notas colectivo, un *TO-DO* donde cualquiera puede bosquejar la idea de un software 
(o al menos la necesidad) y para que vos mismo u otr@s pueden inspirarse y "agarrar el guante" para implementarlo, por ejemplo, durante un PyCamp_

Algunas observaciones previas
=============================


.. class:: warning

   **Atención**: No es el lugar para que hagan tu trabajo práctico por vos, ni para hacer preguntas, ni para pedir bugfix, soporte o reportar issues de programas ya existentes. 
   
   

- Tratá de no ser muy extenso para expresar la idea. Es más fáctible que no caiga en "letra muerta" si se trata de algo que se entienda en un párrafo. 
- Si ya existe una idea similar pero por algún motivo crees que se puede mejorar (por ejemplo, porque no es software libre, o es un servicio SaaS muy caro y parece simple de reimplementar), no 
  te olvides de poner links
- Tené en cuenta que si expresás acá, aceptás que se trata de un espacio colaborativo (la "wiki" es modificable por cualquier miembro de PyAr) y por lo tanto la idea puede ir mutando sin previo aviso. 
- Si querés mantener tu idea original inalterada, es mejor que la escribás en tu página de usuario o en tu blog 
  y pongas el link. 
- Sé criterioso y respetuoso si vas a modificar una idea preexistente. Una buena idea es intentar contactarte 
  con el autor/a a través de la lista o la sala de chat. 
- En el historial de la página queda el registro de la autoría de cada edición. Si querés sabér quien propuso una idea concreta, revisá el historial de la página. 
- Si una idea te inspiró y empezaste a hacerla, o conocés otro proyecto que es muy parecido al descripto, por 
  favor, linkealo, así otr@s se enteran que ya hay "contra qué comparar". 

Ideas para programar
====================

Agregá acá tus ideas. 


Un acortardor de urls con deeplinking 
-------------------------------------

El servicio `citebite.com <citebite.com>`_ es un generador de `deeplinks <https://en.wikipedia.org/wiki/Deep_linking>`_ a fragmentos de texto específicos que se encuentren en una página
Se ingresa una url y un fragmento de texto contenido en ella, y genera un link cuyo contenido 
es la misma página (o una versión muy parecida) con el texto citado resaltado con un color de fondo.  

No sólo permite hacer citas especificas con fuente en un mismo paso, sino que es una manera 
de archivar versiones de la web en un determinado momento. 

¿El problema? Casi no funciona. Es muy lento. Y no permite cosas como resaltar más de un fragmento de texto del mismo sitio web. 

Podría implementar usando `splash <https://github.com/scrapinghub/splash>`_ para obtener una versión estática de la url solicitada, 
encontrar cada fragmento a resaltar usando `pyquery <http://pythonhosted.org/pyquery/>`_ (y probablemente algun algorimo de scoring 
ya que un texto puede estar "desparramado" en múltiples nodos html)

Un servicio capturador de tweets
--------------------------------
A twitter bot that respond to mentions or follow hashtags, taking an screenshot of the tweet being replied or cited. In addtion, it replies the tweet that trigger the capture with the link/image.
https://github.com/mgaitan/tweetshot

   