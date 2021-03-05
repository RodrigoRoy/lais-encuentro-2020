<template>
<div>
  <v-content>
    <section class="black white--text" id="inicio" @click="$vuetify.goTo('#inscripcion', options)" style="cursor: pointer;">
      <v-layout column wrap class="my-0 pt-0" align-center >
        <v-flex xs12 class="mt-4 mb-0">
          <div class="text-center">
            <img src="@/assets/Carrusel Encuentro 20201.png" alt="Encuentro Internacional REDOC" style="width: 100%;">
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
                    ReDOC Investigación constituye una red de investigación sobre documentales concebida como un espacio que reúne a investigadores, docentes, archivistas, estudiantes y realizadores interesados en los estudios de estos documentos audiovisuales desde las diversas disciplinas involucradas en ellos.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>

    <!-- <section id="magistrales" class="black white--text">
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
                        <v-img class="white--text align-end" height="200px" contain position="top center" src="@/assets/Foto_Aimaretti_2.jpg">
                        </v-img>
                        <v-card-title class="justify-center">María Aimaretti</v-card-title>
                        <v-card-subtitle>Universidad de Buenos Aires</v-card-subtitle>
                        <v-card-text class="text-center white--text body-1">
                          Es investigadora en los institutos Gino Germani y Artes del Espectáculo, ambos de la UBA. Sus áreas de reflexión se vinculan, por un lado, con las relaciones entre arte y política en América Latina, a propósito de las representaciones de la violencia, la historia y la memoria, con un extenso trabajo de investigación sobre cine, teatro y video boliviano.
                        </v-card-text>
                        <v-card-actions class="justify-center">
                          <v-btn text color="red" @click.stop="dialog.maria = true">Leer más...</v-btn>
                        </v-card-actions>
                        <v-dialog v-model="dialog.maria" overlay-opacity="6" overlay-color="rgba(0,0,0,0.9)">
                          <v-card>
                            <v-card-title class="headline">María Aimaretti</v-card-title>
                            <v-card-text class="body-1">
                              <p>
                                Doctora en Historia y Teoría de las Artes por la Universidad de Buenos Aires (2015). Licenciada y profesora en Artes Combinadas, diploma de honor 2009, Facultad de Filosofía y Letras (UBA).
                                Actualmente realiza su posdoctorado en Humanidades en la Facultad de Filosofía y Letras de la UBA.
                              </p>
                              <p>
                                Becaria doctoral del CONICET entre 2010 y 2014 y becaria postdoctoral entre 2015 y 2017. Actualmente es investigadora asistente por el mismo organismo.
                              </p>
                              <p>
                                Adscripta a la cátedra de Historia del Cine Latinoamericano y Argentino (2010-2012), se desempeña como docente concursada en dicha materia desde 2013 a la actualidad.
                              </p>
                              <p>
                                Integrante del grupo de investigación CIyNE (2007-2014), investigadora invitada en UNTREF (2011-2014) y miembro desde 2010 a 2016 del comité editorial de la Revista Cine Documental.
                                Actualmente participa del grupo de estudios “Arte, cultura y política en la Argentina reciente” coordinado por Ana Longoni y Cora Gamarnik en el Instituto Gino Germani de la UBA.
                              </p>
                              <p>
                                Miembro de la Asociación Argentina de Estudios sobre Cine y Audiovisual, de la Red de Investigadores sobre Cine Latinoamericano y de la Asociación Argentina para la Investigación en Historia de las Mujeres y Estudios de Género.
                              </p>
                              <p>
                                Ganadora del primer premio en el Concurso de Ensayos sobre Cine Argentino “Domingo Di Núbila” (2016) auspiciado por el INCAA y AsAECA.
                              </p>
                              <p>
                                Fue distinguida con el diploma y medalla como docente universitaria a la Excelencia Académica, otorgado por el Rectorado de la Universidad de Buenos Aires, en diciembre de 2017.
                              </p>
                              <p>
                                Es investigadora en los institutos Gino Germani y Artes del Espectáculo, ambos de la UBA. Sus áreas de reflexión se vinculan, por un lado, con las relaciones entre arte y política en América Latina, a propósito de las representaciones de la violencia, la historia y la memoria, con un extenso trabajo de investigación sobre cine, teatro y video boliviano. Y por otro, con las vinculaciones entre cultura popular y cultura masiva en el cine argentino, atendiendo especialmente a las figuraciones de lo femenino. Publicó artículos en revistas académicas indexadas de Argentina y el exterior, y capítulos de libros sobre cine argentino y latinoamericano.
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
    </section> -->

    <section id="ejes" class="black white--text">
      <v-layout column wrap class="my-12 py-12" align-center >
        <v-flex xs12 sm4 class="my-4">
          <div class="text-center">
            <h2 class="display-3">Ejes temáticos</h2>
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

    <section id="programa">
      <v-layout
        column
        wrap
        class="my-12 py-12"
        align-center
      >
        <!-- <v-flex xs12>
          <v-card flat class="transparent">
            <v-card-text class="text-center">
              <v-icon x-large class="red--text">mdi-bullhorn</v-icon>
            </v-card-text>
          </v-card>
        </v-flex> -->
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
                      Programa preliminar
                    </div>
                  </v-card-title>
                  <v-card-text class="body-1 text-center">
                    <p class="font-weight-bold">
                      Lunes 25 de octubre
                    </p>
                    Inauguración
                    <br />
                    Paneles temáticos
                  </v-card-text>
                  <v-card-text class="body-1 text-center">
                    <p class="font-weight-bold">
                      Martes 26 de octubre
                    </p>
                    Paneles temáticos
                    <br />
                    Conferencia magistral:
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
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
        <v-btn class="mt-12" color="red" dark large href="Convocatoria Encuentro REDOC 2020_b.pdf" disabled>
          Programa final disponible en junio
        </v-btn>
      </v-layout>
    </section>

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
                  <!-- <v-card-text class="text-center white--text body-1">
                    <p>
                      Esta inscripción otorga el derecho al acceso con gafete y paquete de recepción, refrigerios y convivios, así como la acreditación de participación como asistentes al Encuentro.
                    </p>
                  </v-card-text> -->
                  <v-card-text class="text-center white--text body-1 text-uppercase">
                    <p>
                      Inscripciones abiertas para ingresar al evento a partir del 1 de mayo
                    </p>
                  </v-card-text>
                  <v-card-text class="text-center white--text body-1 font-weight-black" style="text-decoration: underline;">
                    <p>
                      Solo habrá acceso al Encuentro con previa inscripción.
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

              <v-flex xs12>
                <v-card flat class="transparent">
                  <v-card-text class="text-center white--text body-1">
                    <!-- <p>
                      Una vez efectuado el pago, favor de remitir el comprobante a: <a href="mailto:redocencuentro2020@mora.edu.mx" style="color: #f44336;">redocencuentro2020@mora.edu.mx</a>
                    </p> -->
                    <p>
                      <strong>Si el cupo se llena será indicado en la página electrónica del Encuentro de forma muy visible.</strong>
                    </p>
                    <!-- <p>
                      <strong>Verificar antes de realizar el pago. En ningún caso habrá reembolso del pago.</strong>
                    </p> -->
                  </v-card-text>
                </v-card>
              </v-flex>

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

    <section id="comite" class="black white--text">
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

    <section id="contacto">
      <v-container grid-list-xl>
        <v-layout row wrap justify-center class="my-12">
          <v-flex xs12 class="my-4">
            <div class="text-center">
              <h2 class="display-3">Información de contacto</h2>
            </div>
          </v-flex>
          <v-flex xs12 sm6>
            <v-card flat class="transparent">
              <!-- <v-card-title primary-title class="layout justify-center">
                <div class="headline">Contacto</div>
              </v-card-title> -->
              <v-card-text class="text-center body-1">
                <span class="font-weight-medium">Laboratorio Audiovisual de Investigación Social</span>
                <br />
                <span class="font-weight-light">Instituto Mora</span>
              </v-card-text>
              <v-list class="transparent">
                <v-list-item>
                  <v-list-item-action>
                    <v-icon class="red--text">mdi-phone</v-icon>
                  </v-list-item-action>
                  <v-list-item-content>
                    <v-list-item-title>(+52) 5598-3415 ext. 3114 y 3123</v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-list-item>
                  <v-list-item-action>
                    <v-icon class="red--text">mdi-map-marker</v-icon>
                  </v-list-item-action>
                  <v-list-item-content>
                    <v-list-item-title>
                      Poussin 45, Mixcoac,
                      <br />
                      03730, México, CDMX
                    </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-list-item>
                  <v-list-item-action>
                    <v-icon class="red--text">mdi-email</v-icon>
                  </v-list-item-action>
                  <v-list-item-content>
                    <v-list-item-title><a href="mailto:redoc.investigacion@gmail.com" style="color: white;">redoc.investigacion@gmail.com</a></v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list>
            </v-card>
          </v-flex>
          <v-flex xs12 sm6>
            <v-card flat class="transparent">
              <!-- <v-card-title primary-title class="layout justify-center">
                <div class="headline">Company info</div>
              </v-card-title> -->
              <v-card-text>
                <!-- <iframe width="100%" height="350" frameborder="0" scrolling="yes" marginheight="0" marginwidth="0" src="https://www.openstreetmap.org/export/embed.html?
                bbox=-99.18746441602708%2C19.37519796836297%2C-99.18298512697223%2C19.37753342382178
                &amp;layer=mapnik
                &amp;marker=19.376365700277347%2C-99.18522477149963" style="border: 1px solid black; width: 100%;"></iframe>
                <br/>
                <small>
                  <a href="https://www.openstreetmap.org/?mlat=19.37607&amp;mlon=-99.18524#map=18/19.37607/-99.18524">Ver mapa completo</a>
                </small> -->
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d940.9605054617934!2d-99.18540790627482!3d19.375991927909794!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85d1ff8699ba2825%3A0x965fcbf67f5dbba7!2sInstituto%20Mora!5e0!3m2!1sen!2smx!4v1582825728361!5m2!1sen!2smx" width="100%" height="350" frameborder="0" style="border:0;" allowfullscreen=""></iframe>
              </v-card-text>
            </v-card>
          </v-flex>
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
        date: '1 de mayo de 2021',
        date2: '31 de septiembre de 2021',
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
        date: '25 al 28 de octubre de 2021',
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
      {name: 'Liliana Cordero', title: 'Dra.', from: 'CISAN - UNAM'},
      {name: 'Felipe Morales Leal', title: 'Mtro.', from: 'Instituto Mora'},
      {name: 'Lilia García Torres', title: 'Mtra.', from: 'CIALC - UNAM'},
      // {name: 'José Luis Mariño', title: 'Dr.', from: 'Investigador independiente'},
      {name: 'Rodrigo Colín Rivera', title: 'Lic.', from: 'Instituto Mora'},
      {name: 'Gloria Marvic García', title: 'Dra.', from: 'Investigadora independiente'},
      {name: 'Jaime Sánchez', title: 'Mtro.', from: 'ENCRYM - INAH'},
      {name: 'Karen Rivera', title: 'Lic.', from: 'Investigadora independiente'},
    ],
    dialog: {
      lynn: false,
      maria: false,
      tiziana: false,
      infoPago: false,
    },
    options: {
      duration: 900,
      offset: 0,
      easing: 'easeInOutCubic',
    },
  }),
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
