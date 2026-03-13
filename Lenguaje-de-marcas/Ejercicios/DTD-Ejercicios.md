# Repositorio-VictorF-Estela-Leo
Repositorio para apuntes y prácticas de DAW realizado por Víctor F, Estela y Leonardo 

# Ejercicio1-2

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE letras [
    <!ELEMENT letras (letra)>
    <!ELEMENT letra (#PCDATA)>
]>
<letras>
    <letra>m</letra>
</letras>

# Ejercicio1.4

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE flores [
    <!ELEMENT flores (flor+)>
    <!ELEMENT flor (#PCDATA)>
]>
<flores>
    <flor>Rosa</flor>
</flores>

# Ejercicio1.5

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE animales [
    <!ELEMENT animales (animal*)>
    <!ELEMENT animal (#PCDATA)>
]>
<animales>
    <animal>Perro Caniche</animal>
    <animal>Gato Siamés</animal>
</animales>

# Ejercicio1.6
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE escritores [
    <!ELEMENT escritores (escritor)>
    <!ELEMENT escritor (nombre, nacimiento)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT nacimiento (#PCDATA)>
]>
<escritores>
    <escritor>
        <nombre>Mario Vargas Llosa</nombre>
        <nacimiento>28 de marzo de 1936</nacimiento>
    </escritor>
    <escritor>
        <nombre>Milan Kundera</nombre>
        <nacimiento>1 de abril de 1929</nacimiento>
    </escritor>
</escritores>

# Ejercicio1.7

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE musicos [
    <!ELEMENT musicos (musico*)>
    <!ELEMENT musico ((nombre | apodo), fechaNacimiento)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT apodo (#PCDATA)>
    <!ELEMENT fechaNacimiento (#PCDATA)>
]>
<musicos>
    <musico>
        <apodo>El cura pelirrojo (Antonio Vivaldi)</apodo>
        <fechaNacimiento>4 de marzo de 1678</fechaNacimiento>
    </musico>
    <musico>
        <nombre>Johann Sebastian Bach (El viejo peluca)</nombre>
        <fechaNacimiento>21 de marzo de 1685</fechaNacimiento>
    </musico>
</musicos>

# Ejercicio1.8

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE agenda [
    <!ELEMENT agenda (contacto*)>
    <!ELEMENT contacto (nombre, telefonoFijo*, telefonoMovil+)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT telefonoFijo (#PCDATA)>
    <!ELEMENT telefonoMovil (#PCDATA)>
]>
<agenda>
    <contacto>
        <nombre>Ayuntamiento</nombre>
        <telefonoFijo>010</telefonoFijo>
        <telefonoMovil></telefonoMovil>
    </contacto>
    <contacto>
        <nombre>Emergencias</nombre>
        <telefonoFijo>112 (Unión Europea)</telefonoFijo>
        <telefonoFijo>911 (Estados Unidos)</telefonoFijo>
        <telefonoMovil>Desconocido</telefonoMovil>
    </contacto>
</agenda>

# Ejercicio1.9

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE sistemaSolar [
    <!ELEMENT sistemaSolar (cuerpo*)>
    <!ELEMENT cuerpo (planeta|satelite|asteroide)>
    <!ELEMENT planeta (#PCDATA)>
    <!ELEMENT satelite (#PCDATA)>
    <!ELEMENT asteroide (#PCDATA)>
]>
<sistemaSolar>
    <cuerpo>
        <planeta>Tierra</planeta>
    </cuerpo>
    <cuerpo>
        <satelite>Luna</satelite>
    </cuerpo>
    <cuerpo>
        <asteroide>Ceres</asteroide>
    </cuerpo>
</sistemaSolar>

# Ejercicio2.1

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE marcadores [
    <!ELEMENT marcadores (marcador+)>
    <!ELEMENT marcador (nombre, uri)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT uri (#PCDATA)>
]>
<marcadores>
    <marcador>
        <nombre>W3C</nombre>
        <uri>http://www.w3.org/</uri>
    </marcador>
    <marcador>
        <nombre>Web Hypertext Application Technology Working Group (WHATWG)</nombre>
        <uri>http://www.whatwg.org/</uri>
    </marcador>
</marcadores>

# Ejericio2.2

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE efemerides [
    <!ELEMENT efemerides (efemeride*)>
    <!ELEMENT efemeride (fecha, hecho)>
    <!ELEMENT fecha (#PCDATA)>
    <!ELEMENT hecho (#PCDATA)>
]>
<efemerides>
    <efemeride>
        <fecha>20 de julio de 1969</fecha>
        <hecho>Llegada del hombre a la Luna</hecho>
    </efemeride>
    <efemeride>
        <fecha>12 de octubre de 1492</fecha>
        <hecho>Llegada de Colón a América</hecho>
    </efemeride>
    <efemeride>
        <fecha>6 de abril de 1909</fecha>
        <hecho>Llegada de Robert Peary al Polo Norte</hecho>
    </efemeride>
</efemerides>

# Ejericio2.3

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE aeropuertos [
    <!ELEMENT aeropuertos (aeropuerto*)>
    <!ELEMENT aeropuerto (nombre, cerrado?)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT cerrado (#PCDATA)>
]>
<aeropuertos>
    <aeropuerto>
        <nombre>Berlín Schönefeld (SFX)</nombre>
    </aeropuerto>
    <aeropuerto>
        <nombre>Berlín Tempelhof (THF)</nombre>
        <cerrado />
    </aeropuerto>
</aeropuertos>

# Ejercicio2.4

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE vuelos [
    <!ELEMENT vuelos (vuelo*)>
    <!ELEMENT vuelo ((origen, destino)|(destino, origen))>
    <!ELEMENT origen (#PCDATA)>
    <!ELEMENT destino (#PCDATA)>
]>
<vuelos>
    <vuelo>
        <origen>Valencia (VLC)</origen>
        <destino>Londres Heathrow (LHR)</destino>
    </vuelo>
    <vuelo>
        <destino>Berlin Schönefeld (SFX)</destino>
        <origen>Paris Charles de Gaulle (CDG)</origen>
    </vuelo>
</vuelos>

# Ejercicio2.5

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE reyesEspañoles [
    <!ELEMENT reyesEspañoles ((rey|reina)*)>
    <!ELEMENT rey (nombre, padre, madre)>
    <!ELEMENT reina (nombre, padre, madre)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT padre (#PCDATA)>
    <!ELEMENT madre (#PCDATA)>
]>
<reyesEspañoles>
    <rey>
        <nombre>Felipe III</nombre>
        <padre>Felipe II</padre>
        <madre>Ana de Austria</madre>
    </rey>
    <reina>
        <nombre>Juana la Loca</nombre>
        <padre>Fernando el Católico</padre>
        <madre>Isabel la Católica</madre>
    </reina>
    <rey>
        <nombre>Carlos I</nombre>
        <padre>Felipe el Hermoso</padre>
        <madre>Juana la Loca</madre>
    </rey>
</reyesEspañoles>

# Ejercicio2.6

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE paises [
    <!ELEMENT paises (pais*)>
    <!ELEMENT pais (nombre, unionEuropea?, otan?)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT unionEuropea EMPTY>
    <!ELEMENT otan EMPTY>
]>
<paises>
    <pais>
        <nombre>España</nombre>
        <unionEuropea />
        <otan />
    </pais>
    <pais>
        <nombre>Noruega</nombre>
        <otan />
    </pais>
    <pais>
        <nombre>Austria</nombre>
        <unionEuropea />
    </pais>
</paises>

# Ejercicio2.7

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE colores [
    <!ELEMENT colores (color*)>
    <!ELEMENT color (nombreSvg, codigo)>
    <!ELEMENT nombreSvg (#PCDATA)>
    <!ELEMENT codigo (rgb|cmyk)>
    <!ELEMENT rgb (#PCDATA)>
    <!ELEMENT cmyk (#PCDATA)>
]>
<colores>
    <color>
        <nombreSvg>Purple</nombreSvg>
        <codigo>
            <rgb>#800080</rgb>
        </codigo>
    </color>
    <color>
        <nombreSvg>Purple</nombreSvg>
        <codigo>
            <cmyk>#00FF007F</cmyk>
        </codigo>
    </color>
</colores>

# Ejercicio2.8

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE contabilidad [
    <!ELEMENT contabilidad (apunte*)>
    <!ELEMENT apunte ((ingreso | gasto)*, fecha, cantidad, concepto)>
    <!ELEMENT ingreso EMPTY>
    <!ELEMENT gasto EMPTY>
    <!ELEMENT fecha (#PCDATA)>
    <!ELEMENT cantidad (#PCDATA)>
    <!ELEMENT concepto (#PCDATA)>
]>

# Ejericicio2.9

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE mensajes [
    <!ELEMENT mensajes (mensaje*)>
    <!ELEMENT mensaje (de, para, hora, texto)>
    <!ELEMENT de (#PCDATA)>
    <!ELEMENT para (#PCDATA)>
    <!ELEMENT hora (#PCDATA)>
    <!ELEMENT texto ANY>
    <!ELEMENT strong (#PCDATA)>
]>
<mensajes>
    <mensaje>
        <de>Pepe (pepe@example.com)</de>
        <para>Juan (juan@example.com)</para>
        <hora>28/02/2011 17:48:23,61</hora>
        <texto>¿Hola, Juan, qué haces?</texto>
    </mensaje>
    <mensaje>
        <de>Juan (juan@example.com)</de>
        <para>Pepe (pepe@example.com)</para>
        <hora>28/02/2011 17:54:20,87</hora>
        <texto>Aquí, aprendiendo <strong>XML</strong></texto>
    </mensaje>
</mensajes>

# Ejercicio3.1

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE persona [
    <!ELEMENT persona EMPTY>
    <!ATTLIST persona nombre CDATA #IMPLIED>
]>
<persona />

# Ejercicio3.2

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE película [
    <!ELEMENT película EMPTY>
    <!ATTLIST película título CDATA #IMPLIED>
]>
<película título="La diligencia" />

# Ejercicio3.3

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE cuadros [
    <!ELEMENT cuadros (cuadro*)>
    <!ELEMENT cuadro EMPTY>
    <!ATTLIST cuadro titulo ID #REQUIRED>
    <!ATTLIST cuadro autor CDATA #REQUIRED>
]>
<cuadros>
    <cuadro titulo="Adán_y_Eva_1" autor="Alberto Durero" />
    <cuadro autor="Lucas Cranach, el viejo" titulo="Adán_y_Eva_2" />
</cuadros>

# Ejercicio3.4

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE listaCompra [
    <!ELEMENT listaCompra (item*)>
    <!ELEMENT item EMPTY>
    <!ATTLIST item nombre CDATA #REQUIRED>
    <!ATTLIST item cantidad CDATA #REQUIRED>
]>

# Ejercicio3.5

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE futbol [
    <!ELEMENT futbol (jugador*)>
    <!ELEMENT jugador EMPTY>
    <!ATTLIST jugador nombre NMTOKENS #REQUIRED>
    <!ATTLIST jugador codigo ID #REQUIRED>
]>
<futbol>
    <jugador nombre="Alfredo Di Stéfano" codigo="N1" />
    <jugador nombre="Edson Arantes do Nascimento - Pelé" codigo="N2" />
    <jugador nombre="Diego Armando Maradona" codigo="N3" />
    <jugador nombre="Johan Cruyff" codigo="N4" />
</futbol>

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE futbol [
    <!ELEMENT futbol ((jugador|equipo)*)>
    <!ELEMENT jugador EMPTY>
    <!ATTLIST jugador nombre NMTOKENS #REQUIRED>
    <!ATTLIST jugador codigo ID #REQUIRED>
    <!ELEMENT equipo EMPTY>
    <!ATTLIST equipo nombre CDATA #REQUIRED>
    <!ATTLIST equipo jugadores IDREFS #IMPLIED>
]>
<futbol>
    <jugador nombre="Alfredo Di Stéfano" codigo="ads"/>
    <jugador nombre="Edison Arantes do Nascimento" codigo="ean" />
    <jugador nombre="Diego Armando Maradona" codigo="dam" />
    <jugador nombre="Johan Cruyff" codigo="jc" />
    <equipo nombre="Società Sportiva Calcio Napoli" jugadores="dam" />
    <equipo nombre="Futbol Club Barcelona" jugadores="jc dam" />
</futbol>

# Ejercicio4.1

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE libro [
    <!ELEMENT libro EMPTY>
    <!ATTLIST libro autor NMTOKENS #REQUIRED>
]>
<libro autor="Mario Vargas Llosa" />

# Ejercicio4.2

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE inventores [
    <!ELEMENT inventores (inventor*)>
    <!ELEMENT inventor EMPTY>
    <!ATTLIST inventor invento CDATA #REQUIRED>
    <!ATTLIST inventor nombre CDATA #IMPLIED>
]>
<inventores>
    <inventor nombre="Robert Adler" invento="Mando a distancia" />
    <inventor nombre="Laszlo Josef Biro" invento="Bolígrafo" />
    <inventor nombre="Josephine Garis Cochran" invento="Lavaplatos" />
    <inventor invento="Fuego" />
</inventores>

# Ejercicio4.3

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE cosasPorHacer [
    <!ELEMENT cosasPorHacer (cosa*)>
    <!ELEMENT cosa (#PCDATA)>
    <!ATTLIST cosa fecha CDATA #REQUIRED>
    <!ATTLIST cosa fechaLimite CDATA #REQUIRED>
]>
<cosasPorHacer>
    <cosa fecha="20 de febrero de 2011" fechaLimite="1 de marzo de 2011">
        Preparar ejercicios de DTDs
    </cosa>
    <cosa fecha="21 de febrero de 2011" fechaLimite="5 de marzo de 2011">
        Preparar tema XSLT
    </cosa>
</cosasPorHacer>

# Ejercicio4.4

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE resoluciones [
    <!ELEMENT resoluciones (resolucion*)>
    <!ELEMENT resolucion EMPTY>
    <!ATTLIST resolucion nombre CDATA #REQUIRED>
    <!ATTLIST resolucion alto CDATA #REQUIRED>
    <!ATTLIST resolucion ancho CDATA #REQUIRED>
]>
<resoluciones>
    <resolucion nombre="VGA" alto="480" ancho="640" />
    <resolucion nombre="XGA" alto="1024" ancho="768" />
    <resolucion nombre="HD 1080" alto="1920" ancho="1080" />
</resoluciones>

# Ejercicio4.5

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE albumesMortadelo [
    <!ELEMENT albumesMortadelo (album*)>
    <!ELEMENT album EMPTY>
    <!ATTLIST album nombre CDATA #REQUIRED>
    <!ATTLIST album fecha (1969|1970|1971|1972|1973|1974) #REQUIRED>
]>
<albumesMortadelo>
    <album nombre="El sulfato atómico" fecha="1969"/>
    <album nombre="La caja de diez cerrojos" fecha="1971"/>
    <album nombre="El otro yo del profesor Bacterio" fecha="1973"/>
    <album nombre="Los cacharros majaretas" fecha="1974"/>
</albumesMortadelo>

# Ejercicio5

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE ligaDeFutbol [
    <!ELEMENT ligaDeFutbol (partido*)>
    <!ELEMENT partido (local, visitante)>
    <!ELEMENT local (nombre, goles)>
    <!ELEMENT visitante (nombre, goles)>
    <!ELEMENT nombre (#PCDATA)>
    <!ELEMENT goles (#PCDATA)>
]>
<ligaDeFutbol>
    <partido>
        <local>
            <nombre>Nottingham Presa</nombre>
            <goles>0</goles>
        </local>
        <visitante>
            <nombre>Inter de Miente</nombre>
            <goles>1</goles>
        </visitante>
    </partido>
    <partido>
        <local>
            <nombre>Vodka Juniors</nombre>
            <goles>3</goles>
        </local>
        <visitante>
            <nombre>Sparta da Risa</nombre>
            <goles>3</goles>
            
