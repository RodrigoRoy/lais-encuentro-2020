<!-- Contenido principal del Encuentro, dispuesto en un estilo "Single Page App"
Cada parte principal se divide en una sección (<section>) -->
<template>
  <v-content>
    <!-- Imagen de encabezado -->
    <section class="black white--text" id="inicio" @click="$vuetify.goTo('#inscripcion', options)" style="cursor: pointer;">
      <v-layout column wrap class="my-0 pt-0" align-center >
        <v-flex xs12 class="mt-4 mb-0">
          <div class="text-center">
            <img src="@/assets/Carrusel Encuentro 2021.png" alt="Encuentro Internacional REDOC" style="width: 100%;">
          </div>
        </v-flex>
      </v-layout>
    </section>

    <!-- Acerca de REDOC Investigación -->
    <section id="redoc">
      <v-layout column wrap class="mt-0 mb-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">
              ReDOC
              <v-icon x-large class="red--text">mdi-filmstrip</v-icon>
            </h2>
          </div>
        </v-flex>
        <v-flex xs12 sm4>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-text class="text-center">
                  </v-card-text>
                  <v-card-text class="body-1 text-center white--text">
                    ReDOC Investigación constituye una red de investigación sobre documentales concebida como un espacio que reúne a investigadores, docentes, archivistas, curadores, estudiantes y realizadores con interés en los estudios de estos documentos audiovisuales desde las diversas disciplinas involucradas en ellos.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Conferencias magistrales -->
    <section id="magistrales" class="black white--text">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">
              Conferencistas magistrales
              <v-icon x-large class="red--text">mdi-account</v-icon>
            </h2>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-flex xs12>
              <v-card flat class="transparent">
                <v-card-text class="text-center">
                  <v-layout row wrap align-start justify-space-around fill-height>
                    <v-flex xs12 md4>
                      <v-card flat class="transparent white--text">
                        <v-img max-height="200px" contain position="top center" src="@/assets/Foto_Lynn_2.jpg">
                        </v-img>
                        <v-card-title class="justify-center">Lynn Novick</v-card-title>
                        <v-card-subtitle>Florentine Films</v-card-subtitle>
                        <v-card-text class="text-center white--text body-1">
                          Ha producido y dirigido documentales históricos sobre la cultura, la política, los deportes, el arte y la música de su país durante casi 30 años. Su trabajo de co-realización con Ken Burns ha generado más de 80 horas de programación televisiva, incluyendo algunos de los documentales y series documentales más aclamados por la crítica.
                        </v-card-text>
                        <v-card-actions class="justify-center">
                          <v-btn text color="red" @click.stop="dialog.lynn = true">Leer más...</v-btn>
                        </v-card-actions>

                        <!-- Ventana emergente (dialog) con la información de conferencista -->
                        <v-dialog v-model="dialog.lynn" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
                          <v-card>
                            <v-card-title class="headline">Lynn Novick</v-card-title>
                            <v-card-text class="body-1">
                              <p>
                                La documentalista estadounidense Lynn Novick ha producido y dirigido documentales históricos sobre la cultura, la política, los deportes, el arte y la música de su país durante casi 30 años. Su trabajo de co-realización con Ken Burns ha generado más de 80 horas de programación televisiva, incluyendo algunos de los documentales y series documentales más aclamados por la crítica y con la más alta valoración en la cadena pública de televisión que los produce y primariamente los difunde, el <em>Public Broadcasting Service</em>, PBS; entre esas obras están <em>La guerra de Vietnam</em> y <em>La guerra</em> –actualmente en Netflix México-, <em>Baseball</em>, <em>Jazz</em>, <em>Frank Lloyd Wright</em> y <em>Prohibición</em>. Sus documentales han sido vistos por más de mil millones de espectadores en los EUA y millones más en todo el mundo. Lynn Novick ha recibido importantes distinciones como los premios Emmy, Peabody y Alfred I. duPont Columbia.
                              </p>
                              <p>
                                La serie televisiva que marca el inicio de su carrera individual como directora es <em>College Behind Bars</em> (2019), un documental de cuatro horas hecho en conjunto con Sarah Botstein, su productora y colaboradora creativa por más de 20 años. El tema general es acerca de un pequeño grupo de hombres y mujeres encarcelados que luchan para obtener títulos universitarios y cambiar sus vidas, dentro de la Iniciativa Penitenciaria Bard, uno de los programas más rigurosos y eficaces de este tipo de educación en los Estados Unidos.
                              </p>
                              <p>
                                El Departamento de Correccionales del estado de Nueva York otorgó a Novick y su equipo un acceso sin precedente a prisiones de máxima y mediana seguridad en el estado a lo largo de cuatro años. <em>College Behind Bars</em> expone, por medio de historias profundas, íntimas y personales de rendición de cuentas, de rehabilitación y de toma de conciencia, el enorme potencial humano que languidece en las prisiones de Estados Unidos.
                              </p>
                              <p>
                                Los proyectos que Novick desarrolla actualmente son una serie documental sobre la historia del crimen y su castigo en Estados Unidos, una biografía del escritor Ernest Hemingway en colaboración con Burns, que se concluirá en 2021, un documental de dos partes sobre la respuesta de Estados Unidos al Holocausto, y una serie documental de varios capítulos acerca de la presidencia de Lyndon Johnson.
                              </p>
                              <p>
                                Novick  se graduó magna cum laude en Yale con honores en Estudios Estadunidenses y vive en la ciudad de Nueva York.
                              </p>
                            </v-card-text>
                            <v-card-actions>
                              <v-spacer></v-spacer>
                              <v-btn color="red" text @click="dialog.lynn = false">Cerrar</v-btn>
                            </v-card-actions>
                          </v-card>
                        </v-dialog>
                      </v-card>
                    </v-flex>

                    <v-flex xs12 md4>
                      <v-card flat class="transparent white--text">
                        <v-img class="white--text align-end" height="200px" contain position="top center" src="@/assets/Foto_Sonia_2.jpg">
                        </v-img>
                        <v-card-title class="justify-center">Sonia Fritz</v-card-title>
                        <v-card-subtitle>Universidad del Sagrado Corazón</v-card-subtitle>
                        <v-card-text class="text-center white--text body-1">
                          Estudió Comunicación en la UNAM y trabajó como free lance en películas y documentales, ganando un “Ariel” a mejor documental por “De bandas, vidas y otros sones” en 1986. En 1985 se muda a Puerto Rico y sigue trabajando los temas que le apasionan tales como migración, género, artes visuales y ecología en sus más de 25 documentales y 4 películas de ficción.
                        </v-card-text>
                        <v-card-actions class="justify-center">
                          <v-btn text color="red" @click.stop="dialog.maria = true">Leer más...</v-btn>
                        </v-card-actions>

                        <!-- Ventana emergente (dialog) con la información de conferencista -->
                        <v-dialog v-model="dialog.maria" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
                          <v-card>
                            <v-card-title class="headline">Sonia Fritz</v-card-title>
                            <v-card-text class="body-1">
                              <p>
                                Estudió Comunicación en la Universidad Nacional Autónoma de México, trabajó como free lance en películas y documentales, y fue parte del Colectivo Cine Mujer. En 1986 ganó un “Ariel” a mejor documental por “De bandas, vidas y otros sones” producido por el INI. En 1985 se mudó a Puerto Rico y comenzó a enseñar en la Universidad del Sagrado Corazón. Posteriormente estudió una maestría en Artes Visuales en Vermont College at Norwich University. Ha realizado más de 25 documentales sobre los temas que le apasionan tales como migración, género, artes visuales, temas sociales y ambientales. En el año 2000 dirigió su primera película de ficción y luego realiza tres más. <em>América</em> fue seleccionada por los festivales de Huelva, Montreal, Guadalajara, Rabat, Ankara, San Diego Latino, Chicago Latino, entre otros, ganando un premio a la mejor actriz en el Festival de Marruecos, y un premio del jurado en el Festival FEMI de Guadaloupe, en el Worldfest Houston, que está disponible en Amazon. Las estrellas del estuario es una película infantil que DIVERCINE exhibió en 15 ciudades de América Latina y a través de KidsFirst recorrió 100 ciudades de Estados Unidos. Sus producciones han ganado premios en festivales internacionales y se han exhibido en televisión pública y circuitos universitarios, tales como <em>Pequeños emigrantes</em>, <em>Carnavales del Caribe</em>, <em>Mona, tesoro del Caribe</em> y <em>Mariachis con pantalones</em>. En 2018 co-dirige los cap. 1 y 2 de la serie LatinoAmericans para PBS, serie que gana el Peabody Award y el Imagen Award. En 2019 tuvo una exhibición retrospectiva en la Galería de Arte de la Universidad del Sagrado Corazón, titulada <em>Cartografías de Sonia Fritz, género y migración</em>. Actualmente produce el documental <em>Voces maravillosas</em> que recoge la gesta de cinco cantantes líricos puertorriqueños que destacan en el mundo.
                              </p>
                              <p>
                                Fritz forma parte de la Asociación de Documentalistas de Puerto Rico.
                              </p>
                            </v-card-text>
                            <v-card-actions>
                              <v-spacer></v-spacer>
                              <v-btn color="red" text @click="dialog.maria = false">Cerrar</v-btn>
                            </v-card-actions>
                          </v-card>
                        </v-dialog>
                      </v-card>
                    </v-flex>

                    <v-flex xs12 md4>
                      <v-card flat class="transparent white--text">
                        <v-img class="white--text align-end" height="200px" contain position="top center" src="@/assets/Foto_Tiziana_2.jpg">
                        </v-img>
                        <v-card-title class="justify-center">Tiziana Panizza</v-card-title>
                        <v-card-subtitle>Universidad de Chile</v-card-subtitle>
                        <v-card-text class="text-center white--text body-1">
                          Ha conducido diversas investigaciones en el ámbito de la realización documental en chile y Latinoamérica, formatos televisivos, videoarte y los movimientos contraculturales y el video activismo durante la dictadura. Sus textos han sido publicados en revistas y libros de circulación nacional e internacional.
                        </v-card-text>
                        <v-card-actions class="justify-center">
                          <v-btn text color="red" @click.stop="dialog.tiziana = true">Leer más...</v-btn>
                        </v-card-actions>

                        <!-- Ventana emergente (dialog) con la información de conferencista -->
                        <v-dialog v-model="dialog.tiziana" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
                          <v-card>
                            <v-card-title class="headline">Tiziana Panizza</v-card-title>
                            <v-card-text class="body-1">
                              <p>
                                Documentalista y docente de la Universidad de Chile en la Carrera de Cine y Televisión.
                              </p>
                              <p>
                                Es Magíster en Art and Media Practice de la University of Westminster, Inglaterra (beca Chevening 2002). Estudia Cine Documental en la Escuela Internacional de Cine y Televisión en Cuba (Beca Ibermedia, 2011). Entre sus peliculas están la trilogía <em>Cartas Visuales</em>, compuesta por los cortometrajes <em>Dear Nonna: a film letter</em> (2005), <em>Remitente: una carta visual</em> (2008) y <em>Al Final: la última carta</em> (2012).
                              </p>
                              <p>
                                La trilogía <em>Bitácora Visual</em>, integrada por <em>Tierra en Movimiento</em> (2014), <em>Tierra Sola</em> y <em>Tierra Incógnita</em> (ambas en progreso), y el largometraje <em>74 metros cuadrados</em> (2012).
                                <br />
                                En televisión fue realizadora en series para Discovery Channel y Travel Channel, en programas culturales como <em>El Show de los Libros</em> y <em>Cine Video</em> para Televisión Nacional de Chile y series documentales como <em>Testigo</em> y <em>Un Día</em> para Canal 13.
                              </p>
                              <p>
                                Es autora de las investigaciones <em>Joris Ivens en Chile: el documental entre la poesía y la crítica</em> (Ed. Cuarto Propio) y <em>Recuperación de la historia Fílmica de Isla de Pascua</em> (Ed. Pehuén). Desde 1995 ha conducido diversas investigaciones en el ámbito de la realización documental en chile y Latinoamérica, formatos televisivos, video arte y los movimientos contraculturales y el video activismo durante la dictadura.Sus textos han sido publicados en revistas y libros de circulación nacional e internacional, como <em>Chasqui</em> (ISI), <em>Contracorriente</em> (ISI), <em>100 años de Cine Chileno</em> (Ed. Arcis), <em>Prismas del Cine Latinoamericano</em> (Ed. Cuarto Propio) y <em>Audiovisual y Política en Chile</em> (Ed. Arcis), entre otros.
                              </p>
                              <p>
                                Ha obtenido reconocimientos en el Festival Internacional de Documentales de Santiago, Torino Film Festival, Bienal de Video y Nuevos Medios y el Premio Pedro Sienna, entre otros. Obtuvo la beca de artista residente en la Fundación Rockefeller en el Bellagio Center en Italia y el Proyecto A, residencia para artistas en Antártica del Consejo Regional de la Cultura de Magallanes.
                              </p>
                            </v-card-text>
                            <v-card-actions>
                              <v-spacer></v-spacer>
                              <v-btn color="red" text @click="dialog.tiziana = false">Cerrar</v-btn>
                            </v-card-actions>
                          </v-card>
                        </v-dialog>
                      </v-card>
                    </v-flex>
                  </v-layout>
                </v-card-text>
              </v-card>
            </v-flex>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Lineas de investigación -->
    <section id="ejes">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">Líneas de investigación</h2>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12 md6>
                <v-card flat class="transparent">
                  <v-card-text class="text-center">
                    <v-icon x-large class="red--text">mdi-movie-search</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-center">Investigación sobre documentales</div>
                  </v-card-title>
                  <v-card-text class="body-1 text-center">
                    Metodologías, periodos, escuelas, movimientos, autores, estudios comparativos, historiografía, curaduría, teorías, enseñanza-aprendizaje de investigación sobre documentales.
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md6>
                <v-card flat class="transparent">
                  <v-card-text class="text-center">
                    <v-icon x-large class="red--text">mdi-movie-edit</v-icon>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-center">Investigación para documentales</div>
                  </v-card-title>
                  <v-card-text class="body-1 text-center">
                    Enseñanza-aprendizaje de investigación para documental, equipos de trabajo, procesos metodologías, fuentes, puntos de vista, narrativas, tratamiento, dispositivos, públicos, archivos y acceso.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
        <v-flex xs12>
          <v-card flat class="transparent">
            <v-card-text class="text-center">
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </section>

    <!-- Programa -->
    <section id="programa" class="black white--text">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">
              Programa
              <v-icon x-large class="red--text">mdi-bullhorn</v-icon>
            </h2>
          </div>
        </v-flex>
        <v-flex xs12 sm4>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-center">
                    </div>
                  </v-card-title>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>

        <v-flex xs12>
          <v-container fill-height>
            <v-row align="center" justify="center">
              <v-col class="text-center">
                <v-btn color="red" large outlined @click="openDialog(0)">Lunes <br> 25 octubre </v-btn>
              </v-col>
              <v-col class="text-center">
                <v-btn color="red" large outlined @click="openDialog(1)">Martes <br> 26 octubre </v-btn>
              </v-col>
              <v-col class="text-center">
                <v-btn color="red" large outlined @click="openDialog(2)">Miércoles <br> 27 octubre</v-btn>
              </v-col>
              <v-col class="text-center">
                <v-btn color="red" large outlined @click="openDialog(3)">Jueves <br> 28 octubre</v-btn>
              </v-col>
              <v-col class="text-center">
                <v-btn color="red" large outlined @click="openDialog(4)">Viernes <br> 29 octubre</v-btn>
              </v-col>
            </v-row>
          </v-container>
        </v-flex>

        <v-flex xs12 class="text-center">
          <h3 class="text-h5 font-weight-light text-uppercase text--secondary mb-4 mt-2">Mesas</h3>
          <p>
            <v-icon small color="teal" class="mr-1">mdi-circle</v-icon><a class="red--text text-decoration-underline font-weight-medium body-1" @click="openDialog(0)">Investigación colaborativa, experiencias comunitarias y estudios de caso</a>
          </p>
          <p class="mt-n2">
            <v-icon small color="indigo" class="mr-1">mdi-circle</v-icon><a class="red--text text-decoration-underline font-weight-medium body-1" @click="openDialog(1)">Metodologías y formación en el campo audiovisual</a>
          </p>
          <p class="mt-n2">
            <v-icon small color="purple" class="mr-1">mdi-circle</v-icon><a class="red--text text-decoration-underline font-weight-medium body-1" @click="openDialog(3)">Militancias, márgenes, emergencias y resistencias</a>
          </p>
          <p class="mt-n2">
            <v-icon small color="lime" class="mr-1">mdi-circle</v-icon><a class="red--text text-decoration-underline font-weight-medium body-1" @click="openDialog(4)">Archivación y memoria</a>
          </p>
        </v-flex>

        <!-- Ventana emergente (dialog) con la información específica del programa dividida por días -->
        <v-dialog v-model="dialog.programa" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
          <v-card>
            <v-card-text class="body-1 text-center">

              <v-tabs v-model="indice" background-color="transparent" color="basil" grow slider-size="4">
                <v-tab key="lunes"> Lunes <br> 25 octubre </v-tab>
                <v-tab key="martes"> Martes <br> 26 octubre</v-tab>
                <v-tab key="miercoles"> Miércoles <br> 27 octubre</v-tab>
                <v-tab key="jueves"> Jueves <br> 28 octubre</v-tab>
                <v-tab key="viernes"> Viernes <br> 29 octubre</v-tab>
              </v-tabs>

              <v-tabs-items v-model="indice">
                <v-tab-item key="lunes">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light red--text">
                        Conferencia magistral con Sonia Fritz 🇲🇽
                      </h2>
                      <h3 class="mb-2 mt-2 text-h5 red--text font-weight-medium">
                        <v-icon small color="orange" class="mr-1">mdi-circle</v-icon>Migración, género y ambiente en documentales latino-caribeños
                      </h3>
                      <p class="text-body-1 font-weight-medium red--text">
                        Anfitriona ReDOC: Lilia García Torres
                      </p>
                      <p class="mt-n2 mb-10 text-h6 red--text">
                        11 a 13.30 horas
                      </p>

                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="teal" class="mr-1">mdi-circle</v-icon>Investigación colaborativa, experiencias comunitarias y estudios de caso 1ª parte
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitriona ReDOC: Sarah Samash
                      </p>

                      <p class="text-body-1">
                        <strong>Ana Maria Mauad</strong> 🇧🇷 <br>
                        História Pública e Memória: sons e imagens da Comunidade Arara de Cachoeira Seca (Pará, Brasil)
                      </p>
                      <p class="text-body-1">
                        <strong>Luis Alejandro García Cervantes</strong> 🇲🇽 <br>
                        Dialógicas de investigación creación y arte participativo en un espacio totalitario
                      </p>
                      <p class="text-body-1">
                        <strong>Diana Isabel Armenta Ramírez</strong> 🇲🇽 <br>
                        En busca de perspectivas comunitarias de la realidad a documentar
                      </p>
                      <p class="text-body-1">
                        <strong>Adriana Marcela Moreno Acosta y Esaú Salvador Bravo Luis</strong> 🇲🇽 <br>
                        Comunidades de conocimiento para la Investigación-Creación audiovisual
                      </p>
                      <p class="text-body-1">
                        <strong>Pablo Iván Argüello González</strong> 🇲🇽 <br>
                        Diseños de antropología visual colaborativa con ciegos y débiles visuales: ensayos metodológicos y creatividad artística
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>

                <v-tab-item key="martes">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        11 a 13.30 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="teal" class="mr-1">mdi-circle</v-icon>Investigación colaborativa, experiencias comunitarias y estudios de caso 2ª parte
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitriona ReDOC: Ana Mauad
                      </p>

                      <p class="text-body-1">
                        <strong>Ángel Miquel</strong> 🇲🇽 <br>
                        <em>Revista Semanal México</em> (1919-1920)
                      </p>
                      <p class="text-body-1">
                        <strong>Adriana Estrada Álvarez</strong> 🇲🇽 <br>
                        Cine y rarámuris: del registro etnográfico al cine experimental (1926-1998)
                      </p>
                      <p class="text-body-1">
                        <strong>Javiera Alejandra Carvallo Fernández</strong> 🇨🇱 <br>
                        Historia y cine documental; un acercamiento al pasado reciente desde las imágenes de <em>La batalla de Chile; la lucha de un pueblo sin armas</em>
                      </p>
                      <p class="text-body-1">
                        <strong>Jaime Sánchez Macedo</strong> 🇲🇽 <br>
                        Documental y estudios urbanos: la National Film de Canadá en la ciudad de Monterrey
                      </p>
                      <p class="text-body-1">
                        <strong>Andrea Meza</strong> 🇪🇸 <br>
                        Prácticas espaciales en los documentales <em>Aquí se construye</em> de Ignacio Agüero y <em>En Construcción</em> de José Luis Guerín
                      </p>
                      <p class="text-body-1">
                        <strong>Juliana Muylaert Mager</strong> 🇧🇷 <br>
                        <em>É Tudo Verdade</em>: um debate sobre trajetórias, sentidos e formas do documentário brasileiro recente a partir dos festivais
                      </p>

                      <h2 class="text-h4 font-weight-light mt-10">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="indigo" class="mr-1">mdi-circle</v-icon>Metodologías y formación en el campo audiovisual 1ª parte
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitriona ReDOC: Gloria Marvic
                      </p>

                      <p class="text-body-1">
                        <strong>Natalia Bermúdez y Josefina Cordera</strong> 🇦🇷 <br>
                        Cruces disciplinares y representación de la realidad. Construcción de un documental desde la Antropología Visual
                      </p>
                      <p class="text-body-1">
                        <strong>Vivian Castro</strong> 🇧🇷 <br>
                        <em>Río desborde</em>: documental de las inundaciones en las ciudades de São Paulo, Brasil y Santiago de Chile
                      </p>
                      <p class="text-body-1">
                        <strong>Lisabete Coradini</strong> 🇧🇷 <br>
                        Metodologías audiovisuales participativas de investigación en Antropología
                      </p>
                      <p class="text-body-1">
                        <strong>Carlos Y. Flores</strong> 🇲🇽 <br>
                        Documental, antropología y crisis de representación
                      </p>
                      <p class="text-body-1">
                        <strong>Lourdes Roca</strong> 🇲🇽 <br>
                        Fuentes para una historia del documental en la región: archivo, metodologías y procesos de enseñanza-aprendizaje
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>

                <v-tab-item key="miercoles">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light red--text">
                        Conferencia magistral con Lynn Novick 🇺🇸
                      </h2>
                      <h3 class="mb-2 mt-2 text-h5 red--text font-weight-medium">
                        <v-icon small color="orange" class="mr-1">mdi-circle</v-icon>El oficio de la realización de documentales: encuentros entre arte e investigación
                      </h3>
                      <p class="text-body-1 font-weight-medium red--text">
                        Anfitrión ReDOC: Felipe Morales Leal
                      </p>
                      <p class="mt-n2 mb-10 text-h6 red--text">
                        11 a 13.30 horas
                      </p>

                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="indigo" class="mr-1">mdi-circle</v-icon>Metodologías y formación en el campo audiovisual 2ª parte
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitriona ReDOC: Josefina Cordera
                      </p>

                      <p class="text-body-1">
                        <strong>Alfredo Sánchez Carballo</strong> 🇲🇽 <br>
                        La creación audiovisual documental desde la problematización en ciencias sociales. Una propuesta metodológica
                      </p>
                      <p class="text-body-1">
                        <strong>Gloria Marvic García</strong> 🇲🇽 <br>
                        Codificación de material audiovisual desde la teoría fundamentada
                      </p>
                      <p class="text-body-1">
                        <strong>Lidia Adriana Álvarez Gómez y Fernando López Martínez</strong> 🇲🇽 <br>
                        Enseñanaza audiovisual secundaria
                      </p>
                      <p class="text-body-1">
                        <strong>María Paz Peirano</strong> 🇨🇱 <br>
                        Creación, investigación y documental: Prácticas docentes del Laboratorio de Etnografía Visual de la Universidad de Chile
                      </p>
                      <p class="text-body-1">
                        <strong>Felipe Morales Leal</strong> 🇲🇽 <br>
                        El historiantrocomunicólogo, la ruptura disciplinar en la realización documental
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>

                <v-tab-item key="jueves">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        11 a 13.30 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="purple" class="mr-1">mdi-circle</v-icon>Militancias, márgenes, emergencias y resistencias 1ª parte
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitrión ReDOC: Alejandro Gracida
                      </p>

                      <!-- <p class="text-body-1">
                        <strong>Darwin Mendoza</strong> 🇭🇳 <br>
                        <em>Cine ojo</em> en Latinoamérica: hacia un “siempre” nuevo cine latinoamericano
                      </p> -->
                      <p class="text-body-1">
                        <strong>Itzel Martínez del Cañizo</strong> 🇲🇽 <br>
                        Un cine propio: autoetnografías fílmicas de mujeres documentalistas en México (1994-2020)
                      </p>
                      <p class="text-body-1">
                        <strong>Andrea Ortega Serrano</strong> 🇲🇽 <br>
                        Una tempestad. Nuevos sentidos desde las prácticas de las mujeres documentalistas en el contexto de nuevas formas de guerra en México
                      </p>
                      <p class="text-body-1">
                        <strong>Luz Estrello, Julio César Gonzales y Gabriela del Pilar Koc</strong> 🇵🇪 <br>
                        Miradas en Lucha: la producción documental sobre conflictos y movimientos socioambientales en Perú
                      </p>
                      <p class="text-body-1">
                        <strong>Juana Schlenker</strong> 🇨🇴 <br>
                        Semillero de Cine y Género de la Escuela de Cine y Televisión de la Universidad Nacional
                      </p>
                      <p class="text-body-1">
                        <strong>Liliana Cordero Marines</strong> 🇲🇽 <br>
                        Alanis Obomsawin y su papel como documentalista en la lucha de las Primeras Naciones
                      </p>

                      <h2 class="text-h4 font-weight-light mt-10">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="purple" class="mr-1">mdi-circle</v-icon>Militancias, márgenes, emergencias y resistencias 2ª parte
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitriona ReDOC: Adriana Estrada
                      </p>

                      <!-- <p class="text-body-1">
                        <strong>Mitzi Amairani Castellanos Méndez</strong> 🇲🇽 <br>
                        Narrativas emergentes como respuesta al dolor, la alegría y la rebeldía: el documental en Oaxaca
                      </p> -->
                      <p class="text-body-1">
                        <strong>Óscar Badillo</strong> 🇲🇽 <br>
                        Docu-gore: la representación de la violencia y el narcotráfico en tres documentales sobre la frontera México-Estados Unidos
                      </p>
                      <p class="text-body-1">
                        <strong>Omara Corona Ramírez</strong> 🇲🇽 <br>
                        Figuraciones de lo trans en el audiovisual documental mexicano
                      </p>
                      <p class="text-body-1">
                        <strong>Karen Rivera Rodríguez</strong> 🇲🇽 <br>
                        Reflexión sobre los colectivos Cine-Mujer (México y Colombia)
                      </p>
                      <p class="text-body-1">
                        <strong>Sarah Shamash</strong> 🇨🇦 <br>
                        Co-creando espacios de resistencia en las prácticas de investigación documental-creación
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>

                <v-tab-item key="viernes">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light red--text">
                        Conferencia magistral con Tiziana Panizza 🇨🇱
                      </h2>
                      <h3 class="mb-2 mt-2 text-h5 red--text font-weight-medium">
                        <v-icon small color="orange" class="mr-1">mdi-circle</v-icon>Coleccionar lo que el mar devuelve: digresión y deriva en la investigación documental
                      </h3>
                      <p class="text-body-1 font-weight-medium red--text">
                        Anfitriona ReDOC: Lourdes Roca
                      </p>
                      <p class="mt-n2 mb-10 text-h6 red--text">
                        11 a 13.30 horas
                      </p>

                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18.30 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        <v-icon small color="lime" class="mr-1">mdi-circle</v-icon>Archivación y memoria
                      </h3>
                      <p class="text-body-1 font-weight-medium mt-n4 mb-8 ">
                        Anfitrión ReDOC: Jaime Sánchez
                      </p>

                      <p class="text-body-1">
                        <strong>Alexis Barbosa Vargas</strong> 🇲🇽 <br>
                        Las interrelaciones entre el documental y el noticiario fílmico
                      </p>
                      <p class="text-body-1">
                        <strong>Alejandro Gracida Rodríguez</strong> 🇲🇽 <br>
                        Tras la sombra de los caudillos: Archivo y registros documentales del poder
                      </p>
                      <p class="text-body-1">
                        <strong>Antonio Zirión Pérez</strong> 🇲🇽 <br>
                        Redescubrir el Archivo Etnográfico Audiovisual del INI
                      </p>
                      <p class="text-body-1">
                        <strong>Celso Castro y Thais Blank</strong> 🇧🇷 <br>
                        Da entrevista ao documentário: sobre a memória da luta pela liberdade em África na narrativa do Comandante Pedro Pires
                      </p>
                      <p class="text-body-1">
                        <strong>Lilia García Torres</strong> 🇲🇽 <br>
                        Patrimonio de la subversión; el caso de los audiovisuales generados por la guerrilla salvadoreña
                      </p>
                      <p class="text-body-1">
                        <strong>Anaïs Taracena</strong> 🇬🇹 <br>
                        El uso creativo de imágenes de archivo en el cine de no ficción: Estudio de caso de la investigación y realización del documental <em>El Silencio del topo</em>
                      </p>

                      <h2 class="text-h4 font-weight-light mt-12">
                        CONVIVIO Y CIERRE DEL ENCUENTRO
                      </h2>
                      <p class="text-h6">
                        19 a 20 horas
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>
              </v-tabs-items>
            </v-card-text>
          </v-card>
        </v-dialog>
      </v-layout>
    </section>

    <!-- Sala de proyecciones -->
    <section id="sala">
      <v-layout column wrap class="my-12 py-12" align-center>
        <v-flex xs12 class="text-center">
          <h2 class="display-3 mt-4">
            Sala de Proyecciones
            <v-icon x-large class="red--text">mdi-video-vintage</v-icon>
          </h2>
        </v-flex>
        <v-flex xs12 sm4 class="mb-6">
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-text class="text-center">
                  </v-card-text>
                  <v-card-text class="body-1 text-center white--text">
                    La sala de proyecciones es un espacio que brinda la oportunidad de visionar documentales que las y los ponentes del Encuentro refieren en sus participaciones.<br>
                    Los documentales se podrán ver en línea entre el <strong>20 de octubre y el 3 de noviembre de 2021</strong>, en FilminLatinoMx, Retina Latina, Vimeo y YouTube.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
        <!-- Carrusel con información del documental -->
        <v-flex xs12 class="text-center">
          <v-hover v-slot="{ hover }">
            <v-carousel v-model="carousel" fluid delimiter-icon="mdi-movie" show-arrows-on-hover :cycle="!hover" hide-delimiters :show-arrows="false" interval="10000" class="py-0">
              <v-carousel-item v-for="(documental, i) in documentales" :key="i">
                <!-- Cada elemento del carrusel serán dos columnas con información e imagen -->
                <v-sheet color="rgba(0,0,0,0.7)" height="100%" tile>
                  <v-row class="fill-height" align="center" justify="center">
                    <div>
                      <v-container>
                        <v-row align="center">
                          <v-col sm="12" md="5" offset-md="1">
                            <!-- Información del documental -->
                            <p class="text-h4 font-weight-medium">
                              <!-- <a class="white--text text-decoration-underline" :href="documental.link"> -->
                                {{ documental.name }}
                              <!-- </a> -->
                            </p>
                            <p v-if="documental.altName" class="text-h6 font-weight-light my-n2">
                              {{ documental.altName }}
                            </p>
                            <p class="my-4 text-h6">
                              {{ documental.author }},<span v-if="documental.year"> {{ documental.year }},</span> {{ documental.time }} <span v-if="documental.time">minutos</span>
                            </p>

                            <v-divider class="mx-4 mb-6"></v-divider>

                            <!-- Información relativa al programa -->
                            <div class="mt-4 text-body-1">
                              <a class="white--text text-decoration-underline" @click="openDialog(documental.dialog)">{{ documental.speech }}</a>
                            </div>
                            <v-chip color="secondary" class="ma-2"><v-icon small :color="documental.color" class="mr-1">mdi-circle</v-icon> {{documental.category}}</v-chip>
                            <v-chip color="secondary" class="ma-2"> {{documental.speaker}} </v-chip>
                          </v-col>

                          <!-- Imagen/animación del documental -->
                          <v-col sm="12" md="5" align="center" justify="center">
                            <!-- <a :href="documental.link" target="_blank"> -->
                              <v-img max-height="250" contain :src="require('@/assets/' + documental.image)"></v-img>
                            <!-- </a> -->
                          </v-col>
                        </v-row>
                      </v-container>
                    </div>
                  </v-row>
                </v-sheet>
              </v-carousel-item>
            </v-carousel>
          </v-hover>
        </v-flex>

        <!-- Listado de documentales en formato de v-cards -->
        <v-container xs12>
          <v-row align="center" justify="left">
            <v-col cols="6" md="3" v-for="(documental, i) in documentales" :key="i">
              <v-hover v-slot="{ hover }">
                <v-card outlined shaped color="rgba(0,0,0,0.8)" @click="carousel = i" :class="{ 'on-hover': hover, 'my-selection': i == carousel, 'my-v-card': true }">
                  <v-card-text class="justify-center text-center text-h6 font-weight-bold">
                    <v-icon small :color="documental.color" class="mr-1">mdi-circle</v-icon>{{ documental.name }}
                  </v-card-text>
                </v-card>
              </v-hover>
            </v-col>
          </v-row>
        </v-container>
      </v-layout>
    </section>

    <!-- Inscripciones -->
    <section id="inscripcion" class="black white--text">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">
              Inscripciones
              <v-icon x-large class="red--text">mdi-ticket-confirmation</v-icon>
            </h2>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-text class="text-center white--text body-1 text-uppercase">
                    <p>
                      Inscripciones abiertas para asistir al evento del 15 de agosto al 30 de septiembre
                    </p>
                  </v-card-text>
                  <v-card-text class="text-center white--text body-1 font-weight-black" style="text-decoration: underline;">
                    <p>
                      Acceso al Encuentro con previa inscripción | Evento sin costo | Cupo limitado
                    </p>
                  </v-card-text>
                </v-card>
              </v-flex>

              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-actions class="justify-center">
                    <v-btn disabled class="mt-0" dark large color="red" href="http://lais-interno.mora.edu.mx/convocatorias/index.php/818258?lang=es-MX">Inscripción al Encuentro concluidas</v-btn>
                  </v-card-actions>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Fechas importantes -->
    <section id="fechas">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 class="my-4">
          <div class="text-center">
            <h2 class="display-3">
              Fechas importantes
              <v-icon x-large class="red--text">mdi-calendar</v-icon>
            </h2>
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-text class="text-center">
                    <!-- <v-icon x-large class="red--text">mdi-calendar</v-icon> -->
                  </v-card-text>
                  <v-card-text>
                    <!-- Uso de timeline de Vuetify para manejo de fechas. Los datos se definen en la variable "fechas" -->
                    <v-timeline>
                      <v-timeline-item v-for="(item, index) in fechas" :key="index" right color="red" fill-dot small>
                        <template v-slot:opposite>
                          <span class="headline font-weight-bold" justify="center">
                            {{ item.date }}
                            <span v-if="item.date2">
                              <br />
                              al {{ item.date2 }}
                            </span>
                          </span>
                        </template>
                        <div class="py-6">
                          <h2 class="headline font-weight-light" v-text="item.title"></h2>
                          <div v-text="item.text"></div>
                        </div>
                      </v-timeline-item>
                    </v-timeline>
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Comité organizador -->
    <section id="comite" class="black white--text">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">
              Comité organizador
              <v-icon x-large class="red--text">mdi-account-group</v-icon>
            </h2>
          </div>
        </v-flex>
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <!-- <v-icon x-large class="red--text">mdi-account-group</v-icon> -->
          </div>
        </v-flex>
        <v-flex xs12>
          <v-container fluid>
            <v-row dense align="center" justify="center">
              <!-- Información de los integrantes definida en la variable "comite" -->
              <v-col cols="7" v-for="(person, index) in comite" :key="index">
                <v-card flat class="py-1 my-n2">
                  <v-card-text class="text-center body-1 py-1 my-0">
                    {{ person.name }}
                    <br />
                    <span class="font-weight-thin">
                      <small>{{ person.from }}</small>
                    </span>
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- Información de contacto -->
    <section id="contacto">
      <v-container grid-list-xl>
        <v-layout row wrap justify-center class="my-12">
          <v-flex xs12 class="my-4">
            <div class="text-center">
              <h2 class="display-3">Información de contacto</h2>
            </div>
          </v-flex>
          <v-flex xs12> <!-- sm6 -->
            <v-card flat class="transparent justify-center">
              <v-card-text class="text-center body-1">
                <span class="font-weight-medium">REDOC Investigación</span>
                <br />
                <span class="font-weight-light">Red de investigación sobre documentales</span>
              </v-card-text>
              <p class="text-center">
                <v-icon class="red--text">mdi-email</v-icon> <a href="mailto:redocencuentro2020@mora.edu.mx" style="color: white;">redocencuentro2020@mora.edu.mx</a>
              </p>
              <p class="text-center mt-12">
                <span class="font-weight-light">Laboratorio Audiovisual de Investigación Social</span>
                <br />
                <span class="font-weight-light">Instituto Mora</span>
              </p>
              <p class="text-center">
                <v-icon class="red--text">mdi-map-marker</v-icon> Poussin 45, Mixcoac, 03730, CDMX, México
              </p>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </section>

    <!-- Pie de página con logos -->
    <v-footer color="black darken-2">
      <v-layout row wrap align-center>
        <v-flex xs12 sm3>
          <div class="grey--text text--darken-2 ml-4 text-center justify-center">
          </div>
        </v-flex>
        <v-flex xs12 sm2>
          <div class="grey--text text--darken-2 ml-4 text-center justify-center">
            <a href="http://lais.mora.edu.mx/encuentroREDOC/">
              <v-img src="@/assets/logo_ReDOC.png" height="75" contain class="mx-2 my-2"></v-img>
            </a>
          </div>
        </v-flex>
        <v-flex xs12 sm2>
          <div class="grey--text text--darken-2 ml-4 text-center justify-center">
            <a href="http://lais.mora.edu.mx/" target="_blank">
              <v-img src="@/assets/logo_LAIS.png" height="75" contain class="mx-2 my-2"></v-img>
            </a>
          </div>
        </v-flex>
        <v-flex xs12 sm2>
          <div class="grey--text text--darken-2 ml-4 text-center justify-center">
            <a href="http://mora.edu.mx/" target="_blank">
              <v-img src="@/assets/logo_Mora.png" height="75" contain class="mx-2 my-2"></v-img>
            </a>
          </div>
        </v-flex>
        <!-- <v-flex xs12 sm2>
          <div class="grey--text text--darken-2 ml-4 text-center justify-center">
            <a href="http://www.cisan.unam.mx/" target="_blank">
              <v-img src="@/assets/logo_CISAN.png" height="75" contain class="mx-2 my-2"></v-img>
            </a>
          </div>
        </v-flex>
        <v-flex xs12 sm2>
          <div class="grey--text text--darken-2 ml-4 text-center justify-center">
            <a href="https://www.unam.mx/" target="_blank">
              <v-img src="@/assets/logo_UNAM.png" height="75" contain class="mx-2 my-2"></v-img>
            </a>
          </div>
        </v-flex> -->
      </v-layout>
    </v-footer>
  </v-content>
</template>

<script>
export default {
  name: 'SinglePage',

  // Variables principales
  data: () => ({
    fechas: [
      {
        date: '15 de agosto de 2021',
        date2: '30 de septiembre de 2021',
        title: 'Inscripciones para asistentes',
        text: '',
      },
      {
        date: '20 de octubre de 2021',
        date2: '3 de noviembre de 2021',
        title: 'Sala de proyecciones',
        text: '',
      },
      {
        date: '25 al 29 de octubre de 2021',
        title: 'Encuentro Internacional ReDOC 2021',
        text: '',
      },
    ],
    conferencistasMagistrales: [
      {
        image: '@/assets/Foto_Lynn_Novick.jpg',
        name: 'Lynn Novick',
        text: 'Lynn Novick is one of the most renowned and respected documentary filmmakers in America. For more than 30 years she has directed and produced landmark documentary films for PBS about American life and culture, history, politics, sports, art, architecture, literature, and music.'
      },
      {
        image: '@/assets/Foto_Aimaretti.jpg',
        name: 'María Aimaretti',
        text: 'Es investigadora en los institutos Gino Germani y Artes del Espectáculo, ambos de la UBA. Sus áreas de reflexión se vinculan, por un lado, con las relaciones entre arte y política en América Latina, a propósito de las representaciones de la violencia, la historia y la memoria —con un extenso trabajo de investigación sobre cine, teatro y video boliviano.'
      },
      {
        image: '@/assets/Foto_Tiziana_2.png',
        name: 'Tizana Panizza',
        text: 'Ha conducido diversas investigaciones en el ámbito de la realización documental en chile y Latinoamérica, formatos televisivos, video arte y los movimientos contraculturales y el video activismo durante la dictadura.Sus textos han sido publicados en revistas y libros de circulación nacional e internacional.'
      },
    ],
    comite: [
      {name: 'Lourdes Roca', title: 'Dra.', from: 'Instituto Mora'},
      {name: 'Felipe Morales Leal', title: 'Mtro.', from: 'Instituto Mora'},
      {name: 'Lilia García Torres', title: 'Mtra.', from: 'CIALC - UNAM'},
      {name: 'Rodrigo Colín', title: 'Lic.', from: 'Instituto Mora'},
      {name: 'Jaime Sánchez', title: 'Mtro.', from: 'El Colegio de Michoacán'},
      {name: 'Alejandro Gracida', title: 'Dr.', from: 'Filmoteca UNAM'},
    ],
    dialog: { // banderas para visibilizar las diferentes ventanas emergentes
      lynn: false,
      maria: false,
      tiziana: false,
      infoPago: false,
      programa: false,
    },
    indice: null, // parámetro para mostrar programa del evento
    // Configuración adicional para el movimiento de pantalla en imagen de encabezado
    options: {
      duration: 900,
      offset: 0,
      easing: 'easeInOutCubic',
    },
    carousel: 0, // indice del elemento en carrusel que se muestra
    documentales: [ // documentales para sala de proyecciones
      {
        name: 'Pequeños inmigrantes',
        altName: 'Little Immigrants',
        speaker: 'Sonia Fritz',
        speech: 'Migración, género y ambiente en documentales latino-caribeños',
        author: 'Sonia Fritz',
        year: '2008',
        time: '42',
        link: 'https://www.youtube.com/watch?v=DHrGAmzmlDM',
        dialog: 0,
        image: 'PequenosInmigrantes.gif',
        color: 'orange',
        category: 'Conferencia magistral'
      },
      {
        name: 'Luisa Capetillo. Pasión de justicia',
        altName: '',
        speaker: 'Sonia Fritz',
        speech: 'Migración, género y ambiente en documentales latino-caribeños',
        author: 'Sonia Fritz',
        year: '1993',
        time: '41',
        link: 'https://www.youtube.com/watch?v=Bu2bw7TqjRs',
        dialog: 0,
        image: 'LuisaCapetillo.gif',
        color: 'orange',
        category: 'Conferencia magistral'
      },
      {
        name: 'Puerto Rico: arte e identidad',
        altName: '',
        speaker: 'Sonia Fritz',
        speech: 'Migración, género y ambiente en documentales latino-caribeños',
        author: 'Sonia Fritz',
        year: '1991',
        time: '56',
        link: 'https://www.youtube.com/watch?v=u_E8PYUCWAU',
        dialog: 0,
        image: 'PuertoRico.png',
        color: 'orange',
        category: 'Conferencia magistral'
      },
      {
        name: '15 faros de Puerto Rico',
        altName: '',
        speaker: 'Sonia Fritz',
        speech: 'Migración, género y ambiente en documentales latino-caribeños',
        author: 'Sonia Fritz',
        year: '2015',
        time: '72',
        link: 'https://youtu.be/FjwyXxYkyFQ?t=928',
        dialog: 0,
        image: 'FarosDePuertoRico.png',
        color: 'orange',
        category: 'Conferencia magistral'
      },
      {
        name: 'En construcción',
        altName: '',
        speaker: 'Andrea Meza Navarro',
        speech: 'Prácticas espaciales en los documentales Aquí se construye de Ignacio Agüero y En Construcción de José Luis Guerín',
        author: 'José Luis Guerín',
        year: '2000',
        time: '127',
        link: 'https://www.youtube.com/watch?v=puiLV6rWdlE',
        dialog: 1,
        image: 'EnConstruccion.png',
        color: 'teal',
        category: 'Investigación colaborativa'
      },
      {
        name: 'Sensorium',
        altName: '',
        speaker: 'Pablo Iván Argüello González',
        speech: 'Diseños de antropología visual colaborativa con ciegos y débiles visuales: ensayos metodológicos y creatividad artística',
        author: 'Pablo Iván Argüello y Diana Luna',
        year: '2020',
        time: '26',
        link: 'https://vimeo.com/378409110',
        dialog: 0,
        image: 'Sensorium.gif',
        color: 'teal',
        category: 'Investigación colaborativa'
      },
      {
        name: 'Tío Yim',
        altName: 'Uncle Yim',
        speaker: 'Itzel Martínez',
        speech: 'Un cine propio: autoetnografías fílmicas de mujeres documentalistas en México (1994-2020)',
        author: 'Luna Marán',
        year: '2019',
        time: '83',
        link: 'https://www.retinalatina.org/video/tio-yim/',
        dialog: 3,
        image: 'TioYim.png',
        color: 'purple',
        category: 'Militancias'
      },
      {
        name: 'Trans',
        altName: 'Episodio 2. Víctimas de la vanidad',
        speaker: 'Omara Corona Ramírez',
        speech: 'Figuraciones de lo trans en el audiovisual documental mexicano',
        author: 'Flavio Florencio',
        year: '2016',
        time: '19',
        link: 'https://www.youtube.com/watch?v=Z9VflEln_3s',
        dialog: 3,
        image: 'Trans.gif',
        color: 'purple',
        category: 'Militancias'
      },
      {
        name: 'The memory of the struggle for Freedom in Africa',
        altName: 'An interview with Comandante Pedro Pires',
        speaker: 'Celso Castro e Thais Blank',
        speech: 'Da entrevista ao documentário: sobre a memória da luta pela liberdade em África na narrativa do Comandante Pedro Pires',
        author: 'Celso Castro',
        year: '2019',
        time: '11',
        link: 'https://www.youtube.com/watch?v=VQg2fM7hwRs',
        dialog: 4,
        image: 'FreedomInAfrica.gif',
        color: 'lime',
        category: 'Archivación y memoria'
      },
    ],
    tab: null,
  }),
  methods: {
    // Permite abrir la pestaña (tab) correcta
    openDialog: function(numberOfTab){
      // alert(dayOfWeek);
      this.indice = numberOfTab;
      this.dialog.programa = true;
    }
  },
};
</script>

<style scoped>
.v-application .display-3 {
  font-family: AR BONNIE !important;
}

.v-application .body-1 {
  font-size: 1.2rem !important;
  font-family: 'Quicksand', sans-sans-serif !important;
}

.v-application .black {
  background-color: rgba(0, 0, 0, 0.55) !important;
}

/* Efecto de aparición para documentales de sala de proyecciones */
.my-v-card {
  transition: opacity .4s ease-in-out;
}
/* Sin opacidad a documental seleccionado (se emplea en conjunto con evento hover) */
.my-selection {
  opacity: 1.0 !important;
}
/* Transparencia a documentales si no están seleccionados */
.my-v-card:not(.on-hover) {
  opacity: 0.4;
}
</style>
