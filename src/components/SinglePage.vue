<template>
<div>
  <v-content>
    <section class="black white--text" id="inicio" @click="$vuetify.goTo('#inscripcion', options)" style="cursor: pointer;">
      <v-layout column wrap class="my-0 pt-0" align-center >
        <v-flex xs12 class="mt-4 mb-0">
          <div class="text-center">
            <img src="@/assets/Carrusel Encuentro 2021.png" alt="Encuentro Internacional REDOC" style="width: 100%;">
          </div>
        </v-flex>
      </v-layout>
    </section>

    <!-- <section class="black" @click="$vuetify.goTo('#inscripcion', options)" style="cursor: pointer;">
      <v-layout column wrap class="my-0 py-0" align-center>
        <v-flex xs12>
          <div class="text-center">
            <h2 class="display-3 my-0 py-0" style="text-decoration: underline;">
              Inscripciones abiertas
            </h2>
          </div>
        </v-flex>
      </v-layout>
    </section> -->

    <!-- <section class="red darken-4">
      <v-layout column wrap class="my-0 py-0" align-center>
        <v-flex xs12>
          <div class="text-center">
            <h2 class="display-3 my-0 py-0">
              Inscripciones cerradas
            </h2>
          </div>
        </v-flex>
      </v-layout>
    </section> -->

    <section id="redoc">
      <v-layout
        column
        wrap
        class="mt-0 mb-12 py-12"
        align-center
      >
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
                    <!-- <v-icon x-large class="red--text">mdi-filmstrip</v-icon> -->
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
                        <v-dialog v-model="dialog.maria" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
                          <v-card>
                            <v-card-title class="headline">Sonia Fritz</v-card-title>
                            <v-card-text class="body-1">
                              <!-- <p>
                                Estudió la licenciatura en Ciencias de la Comunicación en la Universidad Nacional Autónoma de México, y se tituló con la tesis <em>Filmación de un documental sobre la Unión de Mujeres Yalaltecas en Oaxaca</em>. Durante su estancia en la UNAM, Fritz cursó la materia de Taller de guion cinematográfico que impartía Manuel Michel, quien más tarde la invitó a trabajar en un proyecto de filmación. En ese momento Fritz ya se dedicaba al periodismo, profesión que ejercía en medios comerciales y a nivel comunitario en Tepito, pero cuando estuvo en el trabajo de filmación decidió dedicarse al cine. Tras esa experiencia trabajó en el Centro de Producción de Cortometrajes y más tarde en el Cine-Difusión de la Secretaría de Educación Pública (SEP), también trabajo como asistente de producción, asistente de dirección, editora y productora.
                              </p>
                              <p>
                                Se integró al Colectivo Cine Mujer en 1978 porque le interesaba trabajar en cine con un equipo de mujeres sobre temas específicos de la condición de las mujeres. El colectivo trabajaba a partir de la autogestión, metodología participativa con las personas filmadas y exhibición autogestiva con debate final. En ese año se realizó en la Ciudad de México un encuentro de mujeres de grupos autónomos, el registro de ese evento dio resultado al documental <em>Es primera vez</em>, en el que Fritz participó como sonidista y editora.
                              </p>
                              <p>
                                En 1982, la Unión de Mujeres Yalaltecas, después de observar los filmes <em>Es primera vez</em> y <em>Vida de angel</em>, contactó al CCM para ver la posibilidad de que realizara un documental sobre su lucha, su comunidad y organización. Sonia Fritz y otra compañera acudieron al llamado, las autoridades municipales sugirieron que el documental incluyera algunos tópicos, la comunidad también colaboraría con el alojamiento y los alimentos, mientras que el CCM aportaría el trabajo y parte del equipo técnico, con lo que el resultado fue un filme colaborativo, mismo que se exhibió por primera vez en la cancha de la comunidad. <em>Yalaltecas</em> narra la vida cotidiana de las mujeres de la sierra de Oaxaca que decide luchar por sus demandas.
                              </p>
                              <p>
                                Posteriormente ingresó al Archivo Etnográfico Audiovisual del Instituto Nacional Indigenista para editar unas tomas que se habían generado druante la fiesta de la Guelaguetza, en la ciudad de Oaxaca. Para dar sentido a esas imágenes propuso una historia y un guion centradas en los músicos de la comunidad zapoteca Santa Catarina Albarradas, Oaxaca, que habían migrado a Ciudad Nezahualcoyotl, donde reproducían su cultura musical. El resultado fue <em>De bandas, vidas y otros sones</em> (1985).
                              </p>
                              <p>
                                Después de terminar el documental Fritz se mudó a Puerto Rico donde nació su hijo. En 1989 fundó Isla Films, una compañía abocada a la producción de audiovisuales educativos y culturales. En 1993 realizó su primer trabajo histórico, a partir de la adaptación (docudrama) del libro Luisa Capetillo: historia de una mujer proscrita de la periodista Norma Valle Ferrer (1990).
                              </p>
                              <p>
                                Cursó la maestría en Artes Visuales en Vermon Collegue en Norwich University y el doctorado en Literatura del Caribe Inglés en la Universidad de Puerto Rico, recinto Piedras Negras. Es profesora en la Escuela de Comunicación Ferré Rangel de la Universidad del Sagrado Corazón. Es miembro de la National Latino Independent Producers (NALIP).
                              </p> -->

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
                    </v-flex><v-flex xs12 md4>
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
                      Disponible a partir del 1 de junio
                    </div>
                  </v-card-title>
                  <!-- <v-card-text class="body-1 text-center">
                    <p class="font-weight-bold">
                      Lunes 25 de octubre
                    </p>
                    Inauguración
                    <br />
                    Paneles temáticos
                    <br />
                    Conferencia magistral
                  </v-card-text>
                  <v-card-text class="body-1 text-center">
                    <p class="font-weight-bold">
                      Martes 26 de octubre
                    </p>
                    Paneles temáticos
                    <br />
                    Conferencia magistral
                  </v-card-text>
                  <v-card-text class="body-1 text-center">
                    <p class="font-weight-bold">
                      Miércoles 27 de octubre
                    </p>
                    Paneles temáticos
                    <br />
                    Conferencia magistral
                  </v-card-text>
                  <v-card-text class="body-1 text-center">
                    <p class="font-weight-bold">
                      Jueves 28 de octubre
                    </p>
                    Paneles temáticos
                    <br />
                    Sesión plenaria
                    <br />
                    Clausura
                  </v-card-text> -->
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>

        <v-flex xs12 sm8>
          <v-container>
            <v-row>
              <v-col>
                <v-btn color="red" large outlined @click="openDialog(0)">Lunes</v-btn>
              </v-col>
              <v-col>
                <v-btn color="red" large outlined @click="openDialog(1)">Martes</v-btn>
              </v-col>
              <v-col>
                <v-btn color="red" large outlined @click="openDialog(2)">Miércoles</v-btn>
              </v-col>
              <v-col>
                <v-btn color="red" large outlined @click="openDialog(3)">Jueves</v-btn>
              </v-col>
              <v-col>
                <v-btn color="red" large outlined @click="openDialog(4)">Viernes</v-btn>
              </v-col>
            </v-row>
          </v-container>
        </v-flex>
        <!-- <v-btn class="mt-6" color="red" large @click.stop="dialog.programa = true" href="Convocatoria Encuentro REDOC 2020_b.pdf">
          Programa final disponible en junio
        </v-btn> -->

        <v-dialog v-model="dialog.programa" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
          <v-card>
            <v-card-title class="headline justify-center">Mesas Encuentro ReDOC Investigación 2021</v-card-title>
            <v-card-text class="body-1 text-center">

              <v-tabs v-model="indice" background-color="transparent" color="basil" grow slider-size="4">
                <v-tab key="lunes"> Lunes </v-tab>
                <v-tab key="martes"> Martes </v-tab>
                <v-tab key="miercoles"> Miércoles </v-tab>
                <v-tab key="jueves"> Jueves </v-tab>
                <v-tab key="viernes"> Viernes </v-tab>
              </v-tabs>

              <v-tabs-items v-model="indice">
                <v-tab-item key="lunes">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light red--text">
                        Conferencia magistral con Sonia Fritz
                      </h2>
                      <p class="mb-10 text-h6 red--text">
                        11 a 13.30 horas
                      </p>

                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        Investigación colaborativa, experiencias comunitarias y estudios de caso 1ª parte
                      </h3>

                      <p class="text-body-1">
                        <strong>Ana Maria Mauad</strong> <br>
                        História Pública e Memória: sons e imagens da Comunidade Arara de Cachoeira Seca (Pará, Brasil)
                      </p>
                      <p class="text-body-1">
                        <strong>Luis Alejandro García Cervantes</strong> <br>
                        Dialógicas de investigación creación y arte participativo en un espacio totalitario
                      </p>
                      <p class="text-body-1">
                        <strong>Diana Isabel Armenta Ramírez</strong> <br>
                        En busca de perspectivas comunitarias de la realidad a documentar
                      </p>
                      <p class="text-body-1">
                        <strong>Adriana Marcela Moreno Acosta y Esau Salvador Bravo Luis</strong> <br>
                        Comunidades de conocimiento para la Investigación-Creación audiovisual
                      </p>
                      <p class="text-body-1">
                        <strong>Pablo Iván Argüello González</strong> <br>
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
                        Investigación colaborativa, experiencias comunitarias y estudios de caso 2ª parte
                      </h3>

                      <p class="text-body-1">
                        <strong>Ángel Miquel</strong> <br>
                        Revista Semanal México (1919-1920)
                      </p>
                      <p class="text-body-1">
                        <strong>Adriana Estrada Álvarez</strong> <br>
                        Cine y rarámuris: del registro etnográfico al cine experimental (1926-1998)
                      </p>
                      <p class="text-body-1">
                        <strong>Javiera Alejandra Carvallo Fernández</strong> <br>
                        Historia y cine documental; un acercamiento al pasado reciente desde las imágenes de La batalla de Chile; la lucha de un pueblo sin armas
                      </p>
                      <p class="text-body-1">
                        <strong>Jaime Sánchez Macedo</strong> <br>
                        Documental y estudios urbanos: la National Film de Canadá en la ciudad de Monterrey
                      </p>
                      <p class="text-body-1">
                        <strong>Andrea Meza</strong> <br>
                        Prácticas espaciales en los documentales Aquí se construye y En Construcción de José Luis Guerin
                      </p>
                      <p class="text-body-1">
                        <strong>Juliana Muylaert Mager</strong> <br>
                        É Tudo Verdade: um debate sobre trajetórias, sentidos e formas do documentário brasileiro recente a partir dos festivais
                      </p>

                      <h2 class="text-h4 font-weight-light mt-10">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        Metodologías y formación en el campo audiovisual 1ª parte
                      </h3>

                      <p class="text-body-1">
                        <strong>Natalia Bermúdez y Josefina Cordera</strong> <br>
                        Cruces disciplinares y representación de la realidad. Construcción de un documental desde la Antropología Visual
                      </p>
                      <p class="text-body-1">
                        <strong>Vivian Castro</strong> <br>
                        Río desborde: documental de las inundaciones en las ciudades de São Paulo, Brasil y Santiago de Chile
                      </p>
                      <p class="text-body-1">
                        <strong>Lisabete Coradini</strong> <br>
                        Metodologías audiovisuales participativas de investigación en Antropología
                      </p>
                      <p class="text-body-1">
                        <strong>Carlos Y. Flores</strong> <br>
                        Documental, antropología y crisis de representación
                      </p>
                      <p class="text-body-1">
                        <strong>Lourdes Roca</strong> <br>
                        Fuentes para una historia del documental en la región: archivo, metodologías y procesos de enseñanza-aprendizaje
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>

                <v-tab-item key="miercoles">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light red--text">
                        Conferencia magistral con Lynn Novick
                      </h2>
                      <p class="mb-10 text-h6 red--text">
                        11 a 13.30 horas
                      </p>

                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        Metodologías y formación en el campo audiovisual 2ª parte
                      </h3>

                      <p class="text-body-1">
                        <strong>Alfredo Sánchez Carballo</strong> <br>
                        La creación audiovisual documental desde la problematización en ciencias sociales. Una propuesta metodológica
                      </p>
                      <p class="text-body-1">
                        <strong>Gloria Marvic García</strong> <br>
                        Codificación de material audiovisual desde la teoría fundamentada
                      </p>
                      <p class="text-body-1">
                        <strong>Lidia Adriana Álvarez Gómez y Fernando López Martínez</strong> <br>
                        Enseñanaza audiovisual secundaria
                      </p>
                      <p class="text-body-1">
                        <strong>María Paz Peirano</strong> <br>
                        Creación, investigación y documental: Prácticas docentes del Laboratorio de Etnografía Visual de la Universidad de Chile
                      </p>
                      <p class="text-body-1">
                        <strong>Felipe Morales Leal</strong> <br>
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
                        Militancias, márgenes, emergencias y resistencias 1ª parte
                      </h3>

                      <p class="text-body-1">
                        <strong>Darwin Mendoza</strong> <br>
                        Cine ojo en Latinoamerica: hacia un “siempre” nuevo cine latinoamericano
                      </p>
                      <p class="text-body-1">
                        <strong>Itzel Martínez del Cañizo</strong> <br>
                        Extrañamientos familiares: Autoetnografías fílmicas de documentalistas latinoamericanas (2000-2020)
                      </p>
                      <p class="text-body-1">
                        <strong>Luz Estrello, Julio César Gonzales y Gabriela del Pilar Koc</strong> <br>
                        Miradas en Lucha: la producción documental sobre conflictos y movimientos socioambientales en Perú
                      </p>
                      <p class="text-body-1">
                        <strong>Juana Schlenker</strong> <br>
                        Semillero de Cine y Género de la Escuela de Cine y Televisión de la Universidad Nacional
                      </p>
                      <p class="text-body-1">
                        <strong>Liliana Cordero Marines</strong> <br>
                        Alanis Obomsawin y su papel como documentalista en la lucha de las Primeras Naciones
                      </p>
                      <p class="text-body-1">
                        <strong>Juliana Muylaert Mager</strong> <br>
                        É Tudo Verdade: um debate sobre trajetórias, sentidos e formas do documentário brasileiro recente a partir dos festivais
                      </p>

                      <h2 class="text-h4 font-weight-light mt-10">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        Militancias, márgenes, emergencias y resistencias 2ª parte
                      </h3>

                      <p class="text-body-1">
                        <strong>Mitzi Amairani Castellanos Méndez</strong> <br>
                        Narrativas emergentes como respuesta al dolor, la alegría y la rebeldía: el documental en Oaxaca
                      </p>
                      <p class="text-body-1">
                        <strong>Óscar Badillo</strong> <br>
                        Docu-gore: la representación de la violencia y el narcotráfico en tres documentales sobre la frontera México-Estados Unidos
                      </p>
                      <p class="text-body-1">
                        <strong>Omara Corona Ramírez</strong> <br>
                        Figuraciones de lo trans en el audiovisual documental mexicano
                      </p>
                      <p class="text-body-1">
                        <strong>Karen Rivera Rodríguez</strong> <br>
                        Reflexión sobre los colectivos Cine-Mujer (México y Colombia)
                      </p>
                      <p class="text-body-1">
                        <strong>Sarah Shamash</strong> <br>
                        Co-creando espacios de resistencia en las prácticas de investigación documental-creación
                      </p>
                    </v-card-text>
                  </v-card>
                </v-tab-item>

                <v-tab-item key="viernes">
                  <v-card flat >
                    <v-card-text>
                      <h2 class="text-h4 font-weight-light red--text">
                        Conferencia magistral con Tiziana Panizza
                      </h2>
                      <p class="mb-10 text-h6 red--text">
                        11 a 13.30 horas
                      </p>

                      <h2 class="text-h4 font-weight-light">
                        MESA
                      </h2>
                      <p class="text-h6">
                        16 a 18.30 horas
                      </p>
                      <h3 class="mb-6 mt-n2 text-h5">
                        Archivación y memoria
                      </h3>

                      <p class="text-body-1">
                        <strong>Alexis Barbosa Vargas</strong> <br>
                        Las interrelaciones entre el documental y el noticiario fílmico
                      </p>
                      <p class="text-body-1">
                        <strong>Alejandro Gracida Rodríguez</strong> <br>
                        Tras la sombra de los caudillos: Archivo y registros documentales del poder
                      </p>
                      <p class="text-body-1">
                        <strong>Antonio Zirión Pérez</strong> <br>
                        Redescubrir el Archivo Etnográfico Audiovisual del INI
                      </p>
                      <p class="text-body-1">
                        <strong>Celso Castro y Thais Blank</strong> <br>
                        Da entrevista ao documentário: sobre a memória da luta pela liberdade em África na narrativa do Comandante Pedro Pires
                      </p>
                      <p class="text-body-1">
                        <strong>Lilia García Torres</strong> <br>
                        Patrimonio de la subversión; el caso de los audiovisuales generados por la guerrilla salvadoreña
                      </p>
                      <p class="text-body-1">
                        <strong>Anaïs Taracena</strong> <br>
                        El uso creativo de imágenes de archivo en el cine de no ficción: Estudio de caso de la investigación y realización del documental " El Silencio del topo"
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

    <section id="inscripcion">
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
                  <!-- <v-card-text class="text-center white--text body-1">
                    <p>
                      Esta inscripción otorga el derecho al acceso con gafete y paquete de recepción, refrigerios y convivios, así como la acreditación de participación como asistentes al Encuentro.
                    </p>
                  </v-card-text> -->
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

              <!-- <v-flex xs12 md6>
                <v-card flat class="transparent ">
                  <v-card-title primary-title class="layout justify-center">
                    <div class="body-1 text-center">Pago del 1 de marzo al 31 de agosto de 2020</div>
                  </v-card-title>
                  <v-card-text class="body-1 text-center font-weight-bold">
                    $480 MXN / $25 USD
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md6>
                <v-card flat class="transparent ">
                  <v-card-title primary-title class="layout justify-center">
                    <div class="body-1 text-center">Pago del 1 al 21 de septiembre de 2020</div>
                  </v-card-title>
                  <v-card-text class="body-1 text-center font-weight-bold">
                    $675 MXN / $35 USD
                  </v-card-text>
                </v-card>
              </v-flex> -->

              <!-- <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-text class="text-center white--text body-1">
                    <p>
                      Una vez efectuado el pago, favor de remitir el comprobante a: <a href="mailto:redocencuentro2020@mora.edu.mx" style="color: #f44336;">redocencuentro2020@mora.edu.mx</a>
                    </p>
                    <p>
                      <strong>Verificar antes de realizar el pago. En ningún caso habrá reembolso del pago.</strong>
                    </p>
                  </v-card-text>
                </v-card>
              </v-flex> -->

              <v-flex xs12>
                <v-card flat class="transparent">
                  <!-- <v-card-text class="text-center white--text body-1">
                    <p>
                      Las inscripciones otorgan el derecho al acceso con gafete y paquete de recepción, las tres comidas (solo ponentes y conferencistas), refrigerios y convivios, así como la acreditación de participación.
                    </p>
                    <v-simple-table dark>
                      <template v-slot:default>
                        <thead>
                          <tr>
                            <th class="text-left"></th>
                            <th class="text-center subtitle-1 d-xs-table-cell d-sm-none">Pago anticipado</th>
                            <th class="text-center subtitle-1 d-xs-table-cell d-sm-none">Pago en septiembre</th>
                            <th class="text-center subtitle-1 d-none d-sm-table-cell">Pago de marzo a agosto de 2020</th>
                            <th class="text-center subtitle-1 d-none d-sm-table-cell">Pago en septiembre de 2020</th>
                          </tr>
                        </thead>
                        <tbody>
                          <tr>
                            <td class="body-1"> Participantes* </td>
                            <td class="body-1"> 75 USD </td>
                            <td class="body-1"> 100 USD </td>
                          </tr>
                          <tr>
                            <td class="body-1"> Asistentes </td>
                            <td class="body-1"> 25 USD </td>
                            <td class="body-1"> 35 USD </td>
                          </tr>
                        </tbody>
                      </template>
                    </v-simple-table>
                    * <span class="caption"> Estudiantes participantes tendrán 50% de descuento presentando credencia vigente</span>
                  </v-card-text> -->
                  <v-card-actions class="justify-center">
                    <!-- <v-btn class="mt-12" dark large color="red" @click.stop="dialog.infoPago = true">Datos para el pago</v-btn> -->
                  </v-card-actions>
                  <v-dialog v-model="dialog.infoPago" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)" width="70%">
                    <v-card>
                      <v-card-title class="headline">Datos para el pago</v-card-title>
                      <v-card-text class="body-1">
                        <p>
                          Cuenta
                          <br />
                          <strong> BBVA BANCOMER: 0151875221</strong>
                        </p>
                        <p>
                          A nombre de
                          <br />
                          <strong>R38 S91 CONACYT INSTITUTO MORA R.P.5/INSTITUTO DE INVESTIGACIONES DR. JOSÉ MA. LUIS MORA</strong>
                        </p>
                        <p>
                          CLABE INTERBANCARIA
                          <br />
                          <strong>012180001518752210</strong>
                        </p>
                        <p>
                          BIC O SWIFT
                          <br />
                          <strong>BCMRMXMMPYM</strong>
                        </p>
                        <p>
                          Dirección
                          <br />
                          <strong>Av. de la Reforma 510, Col. Juárez, CDMX</strong>
                        </p>
                      </v-card-text>
                    </v-card>
                  </v-dialog>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <section id="fechas" class="black white--text">
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

    <section id="comite">
      <v-layout
        column
        wrap
        class="my-12 py-12"
        align-center
      >
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

    <section id="contacto" class="black white--text">
      <v-container grid-list-xl>
        <v-layout row wrap justify-center class="my-12">
          <v-flex xs12 class="my-4">
            <div class="text-center">
              <h2 class="display-3">Información de contacto</h2>
            </div>
          </v-flex>
          <v-flex xs12> <!-- sm6 -->
            <v-card flat class="transparent justify-center">
              <!-- <v-card-title primary-title class="layout justify-center">
                <div class="headline">Contacto</div>
              </v-card-title> -->
              <v-card-text class="text-center body-1">
                <span class="font-weight-medium">Laboratorio Audiovisual de Investigación Social</span>
                <br />
                <span class="font-weight-light">Instituto Mora</span>
              </v-card-text>
              <p class="text-center">
                <v-icon class="red--text">mdi-map-marker</v-icon> Poussin 45, Mixcoac, 03730, México, CDMX
              </p>

              <p class="text-center">
                <v-icon class="red--text">mdi-email</v-icon> <a href="mailto:redocencuentro2020@mora.edu.mx" style="color: white;">redocencuentro2020@mora.edu.mx</a>
              </p>
            </v-card>
          </v-flex>
          <!-- <v-flex xs12>
            <v-card flat class="transparent">
              <v-card-text>
                <iframe width="100%" height="350" frameborder="0" scrolling="yes" marginheight="0" marginwidth="0" src="https://www.openstreetmap.org/export/embed.html?
                bbox=-99.18746441602708%2C19.37519796836297%2C-99.18298512697223%2C19.37753342382178
                &amp;layer=mapnik
                &amp;marker=19.376365700277347%2C-99.18522477149963" style="border: 1px solid black; width: 100%;"></iframe>
                <br/>
                <small>
                  <a href="https://www.openstreetmap.org/?mlat=19.37607&amp;mlon=-99.18524#map=18/19.37607/-99.18524">Ver mapa completo</a>
                </small>
              </v-card-text>
            </v-card>
          </v-flex> -->
        </v-layout>
      </v-container>
    </section>

    <v-footer color="black darken-2">
      <v-layout row wrap align-center>
        <!-- <v-flex xs12>
          <div class="grey--text text--darken-2 ml-4 text-center">
            ReDOC Investigación – 2020
          </div>
        </v-flex> -->
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
</div>
</template>

<script>
export default {
  name: 'SinglePage',

  data: () => ({
    lineasDeParticipacion: [
      'Documentales como fuentes de investigación: del documento a la fuente',
      'Estudios sobre difusión, puesta en acceso y recepción',
      'Fuentes de investigación en el documental: usos y tratamientos',
      'Recursos narrativos y expresivos en el documental: tratamiento y estudio',
      'Metodologías de investigación-realización de documental',
      'Metodologías de análisis de documentales',
      'Temporalidades y espacialidades en el quehacer documental',
      'Periodos y coyunturas en estudio sobre el documental',
      'Militancia a través del documental',
      'El documental desde la sociedad civil organizada',
      'Enfoques y prácticas interdisciplinarias en la investigación sobre documental',
      'Enseñanza del documental, experiencias y prácticas docentes con documentales',
      'Archivo, patrimonio y memoria en el documental',
    ],
    fechas: [
      // {
      //   date: '30 de enero de 2020',
      //   title: 'Cierre de convocatoria para ponentes',
      //   text: '',
      // },
      // {
      //   date: '1 de marzo al 30 de mayo de 2020',
      //   // date2: '31 de agosto de 2020',
      //   title: 'Inscripciones para ponentes',
      //   text: '',
      // },
      {
        date: '15 de agosto de 2021',
        date2: '30 de septiembre de 2021',
        title: 'Inscripciones para asistentes',
        text: '',
      },
      // {
      //   date: '1 al 21 de septiembre de 2020',
      //   // date2: '24 de septiembre de 2020',
      //   title: 'Inscripciones sin descuento',
      //   text: '',
      // },
      // {
      //   date: '14 al 18 de septiembre de 2020',
      //   title: 'Proyección de documentales',
      //   text: '',
      // },
      {
        date: '25 al 30 de octubre de 2021',
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
      {name: 'Jaime Sánchez', title: 'Mtro.', from: 'ENCRYM - INAH'},
      {name: 'Alejandro Gracida', title: 'Dr.', from: 'Filmoteca UNAM'},
    ],
    dialog: {
      lynn: false,
      maria: false,
      tiziana: false,
      infoPago: false,
      programa: false,
    },
    indice: null,
    options: {
      duration: 900,
      offset: 0,
      easing: 'easeInOutCubic',
    },
  }),
  methods: {
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

/* section{
  background-color: rgba(0, 0, 0, 0.3) !important;
} */

/* .x-large {
  font-size: 58px !important;
} */
</style>
