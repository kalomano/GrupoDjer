# **LAST NIGHTFALL**

## **Dos supervivientes tendrán que enfrentarse a los peligros de la noche. Pasando de nivel y mejorando sus armas o cambiándolas por otras mejores para superar las adversidades**

Jorge Galiano García correo: [j.galiano.2018@alumnos.urjc.es](mailto:j.galiano.2018@alumnos.urjc.es) github: Jorgee-sk

Darío Martín Redondo correo: [d.martinr.2018@alumnos.urjc.es](mailto:d.martinr.2018@alumnos.urjc.es) github: Fyrlian

Pablo Romero Hernández correo: [p.romero.2018@alumnos.urjc.es](mailto:p.romero.2018@alumnos.urjc.es) github: Kalomano

Daniel Romero Hernández correo: [d.romeroh.2018@alumnos.urjc.es](mailto:d.romeroh.2018@alumnos.urjc.es) github: DanielinR



![](RackMultipart20201021-4-3lj6h4_html_768a528ad3a49d0d.png)

## **1.-Cambios**

## **-**

## **2.- Introducción**

Este es el GDD (game design document) del videojuego last nightfall. En este documento se plantea dejar por escrito los principales elementos que conformarán nuestro videojuego en los diferentes ámbitos por los que se compone. Utilizando para su implementación Phaser 3 y buscando ser un videojuego cooperativo.

**2.1 Concepto del juego**

En last nightfall los jugadores comenzarán en un mundo postapocalíptico con armas iniciales (pistolas) y tendrán que abrirse paso por los diferentes &quot;niveles&quot; que conforman el juego, estos niveles son parte de algo global, un mundo por el que los jugadores se deberán mover mientras que se defienden contra las amenazas con las que se irán encontrando

**2.2 Características principales**

Exploración: Los jugadores querrán limpiar las diferentes zonas para acceder a las siguientes con sus mejoras y herramientas que ayudarán al avance del juego, creándose un bucle de avanzar para mejorar.

Frenetismo: Los jugadores han de estar en constante movimiento siempre que no se encuentren en zonas de descanso defendiéndose de los monstruos que los atacan, avanzando en el mapa o cambiando su posición a una más estratégica.

Combate: Este juego pretende generar dinamismo y dopamina a base de matar muchos monstruos en oleadas, no ha de ser táctico ni preciso sino rápido y fluido.

Mejoras: El juego estará muy basado en mejorar nuestras herramientas con el dinero que vayamos recolectando, mejores armas, más visuales, mejorarlas con más munición, cadencia…

**2.3 Género**

Los géneros principales del juego son:

Hacn n slash: Ya mencionado previamente, recompensando al jugador por encadenar combos de bajas, con grandes oleadas y muchos efectos visuales que hagan sentir a este dinamismo y recompensa.

Scroll lateral: Siendo 2D y con diferentes plataformas para colocarse, es un aspecto principal del diseño.

Metroidvania: puesto que el jugador tendrá que retroceder y avanzar a su voluntad utilizando mejoras encontradas más adelante o simplemente para &quot;farmear&quot; dinero o recompensas.

**2.4 Propósito y juego objetivo**

El rango del público objetivo varía desde jugadores casuales hasta jugadores más &quot;tryhard&quot; que pretendan completarlo al 100%, pudiendo ser un juego divertido para pasar el rato pero también con un contenido al que los jugadores más dedicados puedan dedicar horas y horas y al que puedan volver a rejugar. En cuanto a la edad, está claro que no está hecho para los más pequeños, pero no contiene un excesivo uso de violencia explícita como para que solo personas adultas puedan disfrutarlo.

**2.5 Jugabilidad**

Armas: utilizadas para el progreso en el juego, se consiguen abriendo cajas de armas con dinero y serán aleatorias.

Mejoras: Upgrades para las armas que les otorguen más potencias o utilidades, se utilizan abriendo cajas de mejoras y serán aleatorias.

Habilidades: Dashes, doble salto, lanzar granadas… herramientas que ayuden al usuario a la hora del combate y que sirvan para retroceder y desbloquear mejoras a las que no se podían acceder de forma inicial

**2.6 Estilo visual**

Al ser un juego 2D, basaremos nuestro juego en un estilo visual cercano al &quot;pixel art&quot; y cartoon donde es fácil diferenciar los pixeles que componen la escena dando un toque retro y a la vez amigable (consiguiendo rechazar así la violencia explícita). Será llamativo recompensado al usuario con efectos visuales al encadenar combos, matar muchos enemigos o conseguir mejoras.

**2.7 Alcance**

El juego se planea que esté completo cuando salga de forma oficial (no se añadirán DLCs ni actualizaciones de contenido, solo mejoras de rendimiento o arreglar glitches y bugs)

## **3.- Mecánicas de juego**

En esta sección trataremos con profundidad la jugabilidad del juego, las diferentes mecánicas que se le aplican así como el flujo de dificultad. Además se explicarán los diferentes enemigos y mejoras existentes.

**3.1 Jugabilidad**

Oleadas: El juego está basado en ataques de enemigos en los diferentes niveles, estas oleadas aumentarán en función del nivel en el que estamos, aumentado también la dificultad de los enemigos y no solo el número de estos.

Dificultad: La gráfica de dificultad del juego seguirá un patrón constante de forma que cada nivel será más difícil pero se podrá retroceder para mejorar nuestras habilidades. Si el usuario no es capaz de vencer un nuevo nivel podrá volver a uno ya completado para conseguir recursos que invertir en nuevas armas o en nuevas mejoras.

Aleatoriedad: Las armas y mejoras serán aleatorias dependiendo de unas probabilidades que denotarán lo bueno o malo es. Las cajas tendrán un contenido adecuado para el nivel, existiendo así &quot;piscinas&quot; de objetos.

Dinero: El jugador utilizará el dinero en abrir cajas disponibles en cada nivel, las cajas aumentarán su precio de forma que podrá conseguir unas mejoras antes de pasar de nivel y si quiere más tendrá que rejugarlo.

**3.2 Flujo de juego**

Al iniciar el juego, el usuario se encontrará con un menú de inicio con las opciones de iniciar la partida, una pequeña configuración y un botón para salir.

Al darle a salir el juego se cerrará.

Al darle a configuración el juego abrirá un menú que nos permitirá hacer cambios como poner o quitar el sonido o poner el modo daltónico.

Al darle a iniciar partida, el juego dará comienzo y se encontrará en una casa. Aparecerá un texto que explicará al usuario que para comenzar los ataques de los monstruos tendrá que interactuar con un objeto (diferente cada nivel). Al utilizarlo comenzarán las llegadas de oleadas, al matar monstruos conseguiremos monedas. Al acabar con todos los monstruos se abrirá la puerta al siguiente nivel (atravesándola se accede al anterior) y se podrá gastar el dinero en las diferentes cajas. Si se muere, se perderá 1 vida de 3 existentes. Para perder la partida se deberá morir 3 veces de forma seguida. Al pasar un nivel se restauran todas las vidas. Si se muere en modo co-op, un jugador vivo podrá reanimar al jugador al completar el nivel de forma que no pierde ninguna vida.

**3.3 Armas**

**Leyenda de obtención:**  **Inicial**** , **** común (100%, 70% a partir del segundo nivel), **** épico (30% a partir del segundo nivel, 25% a partir del tercer nivel) **** y **** legendario (5% a partir del tercer nivel)**

Glock: Pistola simple

- Disparo: único (una bala por click)
- Daño a cabeza: 30
- Daño a cuerpo: 15
- Cargador: Infinito

Mangum: Revolver

- Disparo: único (una bala por click)
- Daño a cabeza: 70
- Daño a cuerpo: 20
- Cargador: 15

Escopeta recortada: escopeta

- Disparo: único con dispersión (5 balas por click con poca precisión)
- Daño por bala: 10
- Cargador: 5

Ak-47: fusil

- Disparo: automático (puedes dejar pulsado)
- Daño a cabeza: 90
- Daño a cuerpo: 30
- Cargador: 30

FR4/NK0: francotirador

- Disparo: una bala por click con tiempo de recarga lento
- Daño a cabeza: 300
- Daño a cuerpo: 100
- Cargador: 10

Uz1: subfusil

- Disparo: Automático
- Daño a cabeza: 25
- Daño a cuerpo: 15
- Cargador: 25

S4v2: semiautomática

- Disparo: ráfagas de 2 por click
- Daño a cabeza: 35
- Daño a cuerpo: 25
- Cargador: 30

MG-k7: ametralladora ligera

- Disparo: automático (puedes dejar pulsado)
- Daño a cabeza: 10
- Daño a cuerpo: 5
- Cargador: 300

M4-A7: Fusil

- Disparo: ráfagas de 3 por click
- Daño a cabeza: 70
- Daño a cuerpo: 25
- Cargador: 30

**3.4 Mejoras**

**Leyenda de obtención:** **común (100%, 60% a partir del segundo nivel),** **épico (40% a partir del segundo nivel, 30% a partir del tercer nivel)**  **y** **legendario (10% a partir del tercer nivel)**

Mejora de daño 1: Aumenta tu daño 5%

Mejora de daño 2: Aumenta tu daño 10%

Mejora de daño 3: Aumenta tu daño 20%

Mejora de cargador 1: Aumenta tu cargador en 5 balas

Mejora de cargador 2: Aumenta tu cargador en 10 balas

Mejora de cargador 3: Aumenta tu cargador en 15 balas

Balas penetrantes: Las balas atraviesan objetivos infligiendo un daño del 25% a los siguientes objetivos.

Balacera: Por cada bala disparas una extra

Mejora de salto: Saltas más alto

Mejora de velocidad: corres más rápido

Mejora de vida: consigues 20 de vida permanente

**3.4 Personajes**

Protagonista:

- Vida: 200

Nivel 1 ---------------------------- 10 oro

**Zombies:**

- Velocidad: Media
- Vida: 100
- Daño: 20

Nivel 2 -------------------------------- 40 oro

**Zombies:**

- Velocidad: Media
- Vida: 150
- Daño: 30

**Murciélagos infectados**

- Velocidad: alta (aéreo)
- Vida: 30
- Daño: 15

Nivel 3--------------------------------------------------- 100 oro

**Zombies:**

- Velocidad: Media
- Vida: 200
- Daño: 40

**Murciélagos infectados:**

- Velocidad: alta (aéreo)
- Vida: 50
- Daño: 20

**Basura andante:**

- Velocidad: lenta
- Vida: 500
- Daño: 10

Nivel 4--------------------------------------------------- 300 oro

**Zombies:**

- Velocidad: Media
- Vida: 300
- Daño: 70

**Murciélagos infectados:**

- Velocidad: alta (aéreo)
- Vida: 100
- Daño: 35

**Basura andante:**

- Velocidad: lenta
- Vida: 2000
- Daño: 15

**Perro enrabietado:**

- Velocidad: alta
- Vida: 70
- Daño: 120

Nivel 5 --------------------------------------------------- ganas

**Zombies:**

- Velocidad: Media
- Vida: 500
- Daño: 100

**Murciélagos infectados:**

- Velocidad: alta (aéreo)
- Vida: 150
- Daño: 50

**Basura andante:**

- Velocidad: lenta
- Vida: 5000
- Daño: 30

**Perro enrabietado:**

- Velocidad: alta
- Vida: 70
- Daño: 200

**Gigante fétido (BOSS FINAL SOLO SPAWNEA 1 AL PASAR LAS OLEADAS)**

- Velocidad: MUY LENTA
- Vida: 15000
- Daño: Depende las habilidades

**3.4 Movimientos y físicas**

En este apartado concretaremos los movimientos existentes, así como las físicas relacionadas al propio videojuego.

Existen dos tipos de físicas en el videojuego, colisiones y gravedad

**Colisiones**

Se darán entre enemigos y personaje, cuando estos impacten reducirán la vida del jugador.

Se darán entre las balas que dispara el jugador y los enemigos infligiendo daño a los mismos.

Obviamos las colisiones con objetos del entorno (paredes etc.)

**Gravedad**

Afectará a los enemigos y los jugadores, sobre todo en los personajes cuando realicen dobles saltos o saltos simples.

**Controles**

**Movimiento:**

- A-\&gt; Desplazamiento a la izquierda.
- D-\&gt;Desplazamiento a la derecha.
- Espacio-\&gt; Salto (doble espacio, doble salto).
- Shift-\&gt;Dash

**Armas:**

- Ratón-\&gt;Apuntar
- R-\&gt;Recargar
- Click izquierdo-\&gt;Disparar

**Extras:**

- Esc-\&gt; Menú de pausa
- E-\&gt;Interactuar

**4. Interfaz**

**4.1 Menú principal**

![](RackMultipart20201021-4-3lj6h4_html_b95acb92579df43d.png)

- Título: Donde aparecerá el nombre de nuestro videojuego.
- Inicio: Botón para comenzar el juego
- Configuración: Botón para acceder a la configuración de nuestro videojuego donde podremos ajustar los diferentes settings.
- Salir: Botón para cerrar el juego
- Créditos: Aparecen los nombres de los desarrolladores del juego
- Fondo e imagen: La decoración del propio interfaz

**4.2 NIVEL**

![](RackMultipart20201021-4-3lj6h4_html_b503c7309cf449e.png)

- Nivel y oleada: Podremos observar en el interfaz el nivel en el que nos encontramos de todo el juego y las oleadas que han pasado.
- Intentos: Cuantos intentos llevamos en la misma partida (se resetean al acabar el juego o al cerrarlo).
- Armas: Observamos que armas hemos obtenido a lo largo del juego y cuales podemos utilizar.
- Balas: Cuantas balas nos quedan en el cargador.
- Vida: Vida de los personajes que están en la partida.

**4.3 CONFIGURACION**

![](RackMultipart20201021-4-3lj6h4_html_b549d054ed592436.png)

- Sonido: Botón que nos permite ajustarlo a nuestro gusto, tanto sonidos del juego como música.
- Modo daltónico: Botón que cambia la disposición de los colores del juego para ajustarlo en caso de problemas visuales con los colores
- Volver: Botón para retroceder al menú principal
- Fondo: Imagen de fondo del propio menú

**4.4 MENU DE PAUSA**

![](RackMultipart20201021-4-3lj6h4_html_31ef41548610d274.png)

- Vida: Vida de los jugadores.
- Armas: Armas que hayan recogido y estén disponibles para cada jugador en el momento de pausa del juego.
- Balas: Número de balas de cada jugador restantes.
- Nivel y oleada: Podremos observar en el interfaz el nivel en el que nos encontramos de todo el juego y las oleadas que han pasado.
- Sonido: Botón que nos permite ajustarlo a nuestro gusto, tanto sonidos del juego como música.
- Modo daltónico: Botón que cambia la disposición de los colores del juego para ajustarlo en caso de problemas visuales con los colores
- Salir al juego: Botón para reanudar el juego.
- Salir al menú principal: Botón para finalizar la partida y volver al menú principal.
- Mejoras: Para ver las mejoras disponibles que tienen los jugadores en activo.

**5.- Arte**

**5.1 Arte 2D**

Last Nightfall estará repleto de monstruos y enemigos, pero estos no darán tanto miedo debido a la estética semejante al cartoon y al pixel art, el estilo es amigable a la vista e invita a los jugadores a divertirse luchando contra monstruos horribles.

Todas las imágenes serán guardadas tanto en formato .png como en formato .psd para poder modificarlas posteriormente.

- **Logo:** Imagen con el texto &quot;Last Nightfall&quot;, estilo retro.
- **Armas:**

  - Icono Glock: Imagen cuadrada con un dibujo pixel art simple de una Glock.
  - Icono Magnum: Imagen cuadrada con un dibujo pixel art simple de un revolver Magnum.
  - Icono Escopeta recortada: Imagen cuadrada con un dibujo pixel art simple de una escopeta recortada.
  - Icono Uz1: Imagen cuadrada con un dibujo pixel art simple de una Uz1.
  - Icono S4v2: Imagen cuadrada con un dibujo pixel art simple de un fusil semi-automático S4v2.
  - Icono FR4/NK0: Imagen cuadrada con un dibujo pixel art simple de un francotirador FR4/NK0.
  - Icono Ak-47: Imagen cuadrada con un dibujo pixel art simple de una Ak-47.
  - Icono MG-k7: Imagen cuadrada con un dibujo pixel art simple de una ametralladora MG-k7.
  - Icono M4-A7: Imagen cuadrada con un dibujo pixel art simple de un fusil M4-A7.

- **Niveles:**

  - Nivel 1: Pequeña casa de madera acompañada de una fogata que aporte calidez a la escena además de muebles y pertenencias que conviertan el lugar en algo hogareño.
  - Nivel 2: Parque con sus respectivas máquinas de diversión
  - Nivel 3: Colegio con diferentes clases y pasillos en los que haya elementos característicos como taquillas, mesas, sillas etc.
  - Nivel 4: Bosque lúgubre con elementos que acompañen a una escena sombría.
  - Nivel 5: Pequeño templo en las entrañas del bosque.

- **Mejoras:**

  - Icono Mejora daño 1: Imagen cuadrada con un dibujo pixel art simple de un bíceps y una flecha apuntando arriba, fondo color amarillo.
  - Icono Mejora daño 2: Imagen cuadrada con un dibujo pixel art simple de un bíceps y dos flechas apuntando arriba, fondo color morado.
  - Icono Mejora daño 3: Imagen cuadrada con un dibujo pixel art simple de un bíceps y tres flechas apuntando arriba, fondo color rojo.
  - Icono Mejora balas penetrantes: Imagen cuadrada con un dibujo pixel art simple de una bala, fondo color morado.
  - Icono Mejora de cargador 1: Imagen cuadrada con un dibujo pixel art simple de un cinturón de balas y una flecha apuntando arriba, fondo color amarillo.
  - Icono Mejora de cargador 2: Imagen cuadrada con un dibujo pixel art simple de un cinturón de balas y dos flechas apuntando arriba, fondo color morado.
  - Icono Mejora de cargador 3: Imagen cuadrada con un dibujo pixel art simple de un cinturón de balas y tres flechas apuntando arriba, fondo color rojo.
  - Icono mejora Balacera: Imagen cuadrada con un dibujo pixel art simple de una bala partida, fondo color rojo.
  - Icono Mejora de cargador 3: Imagen cuadrada con un dibujo pixel art simple de un cinturón de balas y tres flechas apuntando arriba, fondo color rojo.
  - Icono Mejora de salto: Imagen cuadrada con un dibujo pixel art simple de unas botas y una flecha apuntando arriba, fondo color amarillo.
  - Icono Mejora de velocidad: Imagen cuadrada con un dibujo pixel art simple de unas botas con alas y una flecha apuntando a la derecha, fondo color amarillo.
  - Icono Mejora de vida: Imagen cuadrada con un dibujo pixel art simple de un corazón y una flecha apuntando arriba, fondo color morado.

- **Puntero de juego:** Hit marker simple estilo first person shooter.
- **Barra de vida:** Rectángulo el cual tendrá de color verde el porcentaje de vida del personaje y de color rojo el porcentaje de vida perdida.
- **Contador de balas restantes:** Imagen de tres balas a pixel art simple contiguo a un número que muestra el número de balas restante.
- **Cartel de Game Over:** Se muestra cuando ambos jugadores quedan sin vida.
- **Contador de siguiente oleada:** Se muestra para avisar a los jugadores cuando va a venir una nueva oleada.
- **Animaciones:** Todos los personajes contarán con animaciones de movimiento, ataque, recibir daño y morir.

**5.1 Audio**

El audio de Last Nighfall pondrá en tensión a los jugadores en las oleadas más difíciles de superar, mientras que en las primeras oleadas será más relajante.

Los efectos de sonido se guardarán en .wav.

- **Músicas:**

  - Menú principal: Música relajada, de ambiente.
  - Juego: Música generalmente tensa.
  - Game Over: Música ambiente triste.
  - Música de victoria: Música alegre e incluso épica.

- **Efectos:**

  - Ataque de Zombie: Ruido de grito de Zombie cuando ataca al jugador.
  - Ataque de Murciélago infectado: Ruido de grito de murciélago cuando ataca al jugador.

  - Ataque de basura andante: Ruido de golpe físico cuando ataca al jugador.
  - Ataque de perro enrabietado: Ruido de mordisco cuando ataca al jugador.
  - Ataque de gigante fétido: Tiene varios sonidos de ataque como el ruido de un efecto tóxico, golpes físicos o gritos de gigante.
  - Ruido daño a Zombie: Ruido al dañar al zombie.
  - Ruido daño a Murciélago infectado: Ruido al dañar al murciélago.
  - Ruido daño basura andante: Ruido al dañar basura andante.
  - Ruido daño perro enrabietado: Ruido de ladrido al dañar a perro enrabietado.
  - Efecto de coger mejora: al coger una mejora.
  - Efecto de coger arma: al coger un arma.
  - Efecto disparo: al disparar una bala.
  - Efecto colisión de bala contra pared u otro objeto: sonido colisión con el objeto.
  - Efecto de recarga: sonido de recarga de arma.
  - Efecto navegar por el menú: Al mover el ratón por las opciones de los menús.
  - Ruido daño al jugador: sonido sufrimiento de personaje.
