<template>
  <div id="app">
    <header>
      <section id="header" class="hero hero-header">
        <div class="hero-body hero-body-header">
          <div class="container">
            <div class="columns is-vcentered is-mobile">
              <div class="column is-4">
                <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                  <a href="#networks">Expertises</a>
                </p>
              </div>
              <div class="column is-4">
                <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                  <a href="#maker">Formación</a>
                </p>
              </div>
              <div class="column is-4">
                <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                  <a href="#content">Experiencia</a>
                </p>
              </div>
            </div>  
          </div>
        </div>
      </section>
    </header>
    <div class="box-modal is-marginless">
      <transition name="show">
        <modal
          :modal="targetUrl"
          class="is-active"
          v-show="showModal"
          @clickCloseModal="isClosingModal"
        />
      </transition>
    </div>
    <div class="box-modal-ana is-marginless">
      <transition name="show">
        <modal-ana
          class="is-active"
          v-show="showModalAna"
          @clickCloseModal="isClosingModalAna"
        />
      </transition>
    </div>
    <div class="box-modal-cap is-marginless">
      <transition name="show">
        <modal-cap
          class="is-active"
          v-show="showModalCap"
          @clickCloseModal="isClosingModalCap"
        />
      </transition>
    </div>
    <div class="box-modal-coa is-marginless">
      <transition name="show">
        <modal-coa
          class="is-active"
          v-show="showModalCoa"
          @clickCloseModal="isClosingModalCoa"
        />
      </transition>
    </div>
    <div class="box-modal-ges is-marginless">
      <transition name="show">
        <modal-ges
          class="is-active"
          v-show="showModalGes"
          @clickCloseModal="isClosingModalGes"
        />
      </transition>
    </div>
    <div class="box-modal-web is-marginless">
      <transition name="show">
        <modal-web
          class="is-active"
          v-show="showModalWeb"
          @clickCloseModal="isClosingModalWeb"
        />
      </transition>
    </div>
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <div class="content-tag">
            <a href="#header">
              <span class="tag is-large tag-up">
                <font-awesome-icon icon="arrow-up" />
              </span>    
            </a>
          </div>
          <div class="columns is-marginless">
            <div class="column is-full">
              <figure class="image">
                <img class="img-yo" src="./assets/yo.jpeg">
              </figure>  
            </div>
          </div>
          <div class="columns is-marginless">
            <div class="column is-full is-paddingless">
              <p class="is-size-3-desktop is-size-4-tablet is-size-5-mobile title-text">
                Cristian Castillo Matamoros 
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile subtitle-text">
                Ingeniero Comercial / Máster en Coaching / Desarrollador de Entornos Web
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile subtitle-text">
                <span>
                  <font-awesome-icon icon="envelope" />
                </span>
                ccastim@gmail.com
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile subtitle-text">
                <span>
                  <font-awesome-icon icon="phone" />
                </span>
                +56 9 7778 9116
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile subtitle-text has-text-weight-semibold">
                Disponible para oportunidades inmediatas en tiempo completo, consultoría o proyectos a medida.
              </p>
            </div>
          </div>
        </div>    
      </div>
    </section>
    <section id="networks" class="hero hero-networks">
      <div class="hero-body is-paddingless">
        <div class="container">
          <div class="columns">
            <div class="column is-full is-paddingless">
              <p class="is-size-3-desktop is-size-4-tablet is-size-5-mobile has-text-weight-bold has-text-centered networks-title">
                Expertises
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile has-text-centered networks-subtitle">
                Pulsa los botones amarillos para detalle de expertis.
              </p>
            </div>
          </div>
          <div class="columns is-desktop">
            <div class="column is-4 is-hidden-touch">
              <div class="container">
                <div class="columns">
                  <div class="column is-full">
                    <p class="is-size-5-desktop is-size-5-mobile has-text-weight-bold has-text-centered">
                      Habilidades
                    </p>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Pensamiento Crítico
                    </p>
                    <progress class="progress is-link" value="95" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobiles">
                      Orientación a Resultados
                    </p>
                    <progress class="progress is-link" value="93" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Capacidad de Diagnóstico
                    </p>
                    <progress class="progress is-link" value="100" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Visión Estratégica
                    </p>
                    <progress class="progress is-link" value="85" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Comunicación Efectiva
                    </p>
                    <progress class="progress is-link" value="93" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Trabajo en Equipo
                    </p>
                    <progress class="progress is-link" value="96" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Gestión del Cambio
                    </p>
                    <progress class="progress is-link" value="85" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-6-mobile">
                      Ética Profesional
                    </p>
                    <progress class="progress is-link" value="100" max="100"></progress>
                  </div>
                </div>
              </div>
            </div>
            <div class="column is-4-desktop is-offset-0-desktop is-8-tablet is-offset-2-tablet is-12-mobile">
              <div class="container">
                <div class="border-box-orbe">
                  <div class="box-orbe">
                    <div class="columns is-mobile">
                      <div class="column is-6 is-paddingless centrar">
                        <div class="orbe-up-left">
                          <figure class="image exp-img" @click="clickExp">
                            <img id="111" class="img-exp palpitar" src="./assets/coac.png">
                          </figure>
                        </div>
                      </div>
                      <div class="column is-6 is-paddingless centrar">
                        <div class="orbe-up-rigth">
                          <figure class="image exp-img" @click="clickExp">
                            <img id="112" class="img-exp palpitar" src="./assets/capa.png">
                          </figure>
                        </div>
                      </div>
                    </div>
                    <div class="columns">
                      <div class="column is-12 is-paddingless">
                        <div class="orbe-center">
                          <figure class="image exp-img" @click="clickExp">
                            <img id="113" class="img-exp palpitar" src="./assets/desa.png">
                          </figure>
                        </div>
                      </div>
                    </div>
                    <div class="columns is-mobile">
                      <div class="column is-6 is-paddingless centrar">
                        <div class="orbe-down-left">
                          <figure class="image exp-img" @click="clickExp">
                            <img id="114" class="img-exp palpitar" src="./assets/anal.png">
                          </figure>
                        </div>
                      </div>
                      <div class="column is-6 is-paddingless centrar">
                        <div class="orbe-down-rigth">
                          <figure class="image exp-img" @click="clickExp">
                            <img id="115" class="img-exp palpitar" src="./assets/gest.png">
                          </figure>
                        </div>
                      </div>
                    </div>    
                  </div>
                </div>
              </div>
            </div>
            <div class="column is-4-desktop is-6-tablet is-offset-0-desktop is-offset-3-tablet languages">
              <div class="container">
                <div class="columns">
                  <div class="column is-full">
                    <p class="is-size-5-desktop is-size-4-tablet is-size-5-mobile has-text-weight-bold has-text-centered">
                      Idiomas
                    </p>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Español
                    </p>
                    <progress class="progress is-link" value="100" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Ingles
                    </p>
                    <progress class="progress is-link" value="70" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Italiano
                    </p>
                    <progress class="progress is-link" value="30" max="100"></progress>
                  </div>
                </div>
              </div>
            </div>
            <div class="column is-hidden-desktop is-6-tablet is-offset-3-tablet languages">
              <div class="container">
                <div class="columns">
                  <div class="column is-full">
                    <p class="is-size-4-tablet is-size-5-mobile has-text-weight-bold has-text-centered">
                      Habilidades
                    </p>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Pensamiento Crítico
                    </p>
                    <progress class="progress is-link" value="95" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobiles">
                      Orientación a Resultados
                    </p>
                    <progress class="progress is-link" value="93" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Capacidad de Diagnóstico
                    </p>
                    <progress class="progress is-link" value="100" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Visión Estratégica
                    </p>
                    <progress class="progress is-link" value="85" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Comunicación Efectiva
                    </p>
                    <progress class="progress is-link" value="93" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Trabajo en Equipo
                    </p>
                    <progress class="progress is-link" value="96" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Gestión del Cambio
                    </p>
                    <progress class="progress is-link" value="85" max="100"></progress>
                  </div>
                </div>
                <div class="columns is-mobile">
                  <div class="column is-8 is-offset-2">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Ética Profesional
                    </p>
                    <progress class="progress is-link" value="100" max="100"></progress>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>  
      </div>
    </section>
    <section id="maker" class="hero hero-maker">
      <div class="hero-body hero-body-maker">
        <div class="container">
          <div class="columns">
            <div class="column is-full is-paddingless">
              <p class="is-size-3-desktop is-size-4-tablet is-size-5-mobile has-text-weight-bold prof-title">
                Formación Profesional
              </p>
            </div>
          </div>
          <div class="columns is-vcentered ces is-mobile">
            <div class="column is-paddingless is-2 is-offset-1-desktop">
              <figure class="image">
                <img class="img-logo" src="./assets/ces.png">
              </figure>
            </div>
            <div class="column is-10">
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile formation-text has-text-weight-semibold">
                Máster en Coaching, CES Don Bosco, Madrid.
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile formation-text"  >
                Titulado en el año 2013  
              </p>
            </div>
          </div>
          <div class="columns is-vcentered unap is-mobile">
            <div class="column is-paddingless is-2 is-offset-1-desktop">
              <figure class="image">
                <img class="img-logo" src="./assets/unap.jpg">
              </figure>
            </div>
            <div class="column is-10">
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile formation-text has-text-weight-semibold">
                Ingeniería Comercial, Universidad Arturo Prat.
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile formation-text"  >
                Titulado con distinción en el año 2006  
              </p>
            </div>
          </div>
          <div class="columns is-vcentered aiep is-mobile">
            <div class="column is-paddingless is-2 is-offset-1-desktop">
              <figure class="image">
                <img class="img-logo" src="./assets/aiep.jpg">
              </figure>
            </div>
            <div class="column is-10">
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile formation-text has-text-weight-semibold">
                Ingeniería de Ejecución en Administración de Empresas, AIEP.
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile formation-text"  >
                Titulado con  máxima distinción en el año 2002  
              </p>
            </div>
          </div>
          <div class="columns is-marginless">
            <div class="column is-full is-paddingless">
              <p class="is-size-3-desktop is-size-4-tablet is-size-5-mobile has-text-weight-bold courses-title">
                Cursos Adicionales
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile has-text-centered courses-subtitle">
                Pulsa cada ícono para ver el certificado del curso.
              </p>
            </div>
          </div>
          <div class="columns first-c">
            <div class="column">
              <div class="columns is-mobile">
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="1" class="img-course palpitar" src="./assets/excell.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="2" class="img-course palpitar" src="./assets/bi.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="3" class="img-course palpitar" src="./assets/vue.png">
                  </figure>
                </div>
              </div>
            </div>
            <div class="column">
              <div class="columns is-mobile">
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="4" class="img-course palpitar" src="./assets/vuep.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="5" class="img-course palpitar" src="./assets/prog.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="6" class="img-course palpitar" src="./assets/js.png">
                  </figure>
                </div>
              </div>
            </div>
          </div>
          <div class="columns second-c">
            <div class="column">
              <div class="columns is-mobile">
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="7" class="img-course palpitar" src="./assets/html.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="8" class="img-course palpitar" src="./assets/resp.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="9" class="img-course palpitar" src="./assets/g-suite.png">
                  </figure>
                </div>
              </div>
            </div>
            <div class="column">
              <div class="columns is-mobile">
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="10" class="img-course palpitar" src="./assets/trello.png">
                  </figure>
                </div>
                <div class="column is-one-third">
                  <figure class="image course-img" @click="clickCourse">
                    <img id="11" class="img-course palpitar" src="./assets/trem.png">
                  </figure>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="content" class="hero hero-content">
      <div class="hero-body hero-body-content">
        <div class="container">
          <div class="columns box-content">
            <div class="column is-12-mobile is-10-desktop is-offset-1-desktop">
              <p class="is-size-3-desktop is-size-4-tablet is-size-5-mobile title-content">
                Experiencia Profesional
              </p>
              <p class="is-size-4-desktop is-size-5-tablet is-size-6-mobile has-text-justified">
                Sólida experiencia en gestión de actividades de personas y comerciales, análisis y control financiero de empresas. Óptimo manejo de grupos y equipos de trabajo a través de la aplicación de habilidades relacionales, destacando un estilo de liderazgo de coach, generando relaciones interpersonales potentes y orientadas al cumplimiento de objetivos.<br/>
                Experiencia en el desarrollo y relatoría de Programas de Capacitación. Manejo avanzado de herramientas de Tecnologías de la Información y análisis de datos.<br/><br/>
                Pulsa en cada barra para ver el detalle.
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption1" class="card-header card-header-option">
                  <div class="container">
                    <div class="columns is-mobile is-vcentered">
                      <div class="column is-2">
                        <figure class="image">
                          <img class="img-work" src="./assets/inter.jpg">
                        </figure>
                      </div>
                      <div class="column is-9">
                        <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                          Ejecutivo Comercial
                        </p>
                        <p class="card-header-title is-paddingless is-size-5-desktop is-size-6-tablet is-size-7-mobile">
                          Baninter Factoring S.A.
                        </p>
                      </div>
                      <div class="column is-1 is-paddingless">
                        <a href="" class="card-header-icon" aria-label="more options">
                          <span v-show="!showOption1" class="icon">
                            <font-awesome-icon icon="chevron-down" />
                          </span>
                          <span  v-show="showOption1" class="icon">
                            <font-awesome-icon icon="chevron-up" />
                          </span>
                        </a>
                      </div>
                    </div>
                  </div>
                </header>
                <transition name="expand">
                  <div v-show="showOption1" class="card-content has-text-justified">
                    Diciembre 2024 a Mayo 2025<br/>
                    <strong>Temuco, Chile</strong><br/>
                    <br/>
                    Apertura gestiones comerciales en zona de La Araucanía. Prospección de nuevos clientes en productos de financiamiento de corto plazo, tales como factoring, capitales de trabajo y confirming.
                    <br/>
                    <br/><strong>Referencias</strong>
                    <br/>
                    Daniela Zamorano, Gerente Comercial<br/>
                    dzamorano@baninterfactoring.cl<br/>
                    +56 9 6618 4536<br/><br/>
                    Jorge Ahumada, Jefe Zonal Sur<br/>
                    jahumada@baninterfactoring.cl<br/>
                    +56 9 9533 1481<br/>
                    <br/>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption2" class="card-header card-header-option">
                  <div class="container">
                    <div class="columns is-mobile is-vcentered">
                      <div class="column is-2">
                        <figure class="image">
                          <img class="img-work" src="./assets/mitta.png">
                        </figure>
                      </div>
                      <div class="column is-9">
                        <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                          Jefe de Administración
                        </p>
                        <p class="card-header-title is-paddingless is-size-5-desktop is-size-6-tablet is-size-7-mobile">
                          Autorentas del Pacífico SpA, MITTA
                        </p>
                      </div>
                      <div class="column is-1 is-paddingless">
                        <a href="" class="card-header-icon" aria-label="more options">
                          <span v-show="!showOption2" class="icon">
                            <font-awesome-icon icon="chevron-down" />
                          </span>
                          <span  v-show="showOption2" class="icon">
                            <font-awesome-icon icon="chevron-up" />
                          </span>
                        </a>
                      </div>
                    </div>
                  </div>
                </header>
                <transition name="expand">
                  <div v-show="showOption2" class="card-content has-text-justified">
                    Octubre 2020 a Diciembre 2024<br/>
                    <strong>Temuco, Chile</strong><br/>
                    <br/>
                     Supervisión y control de equipos comerciales y operativos de sucursal, relación con proveedores estratégicos, control presupuestario y financiero<br/>
                     <br/>Desde mi ingreso a la fecha he logrado el óptimo cumplimiento de las obligaciones financieras y legales de la sucursal en tiempo y forma. Mejoramiento de clima organizacional y trabajo en equipo.
                    <br/>
                    <br/><strong>Referencias</strong>
                    <br/>
                    Felipe Mehr, Gerente Sucursal<br/>
                    (Ya no trabaja en Mitta)<br/>
                    +56 9 9680 7517<br/>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption3" class="card-header card-header-option">
                  <div class="container">
                    <div class="columns is-mobile is-vcentered">
                      <div class="column is-2">
                        <figure class="image">
                          <img class="img-work" src="./assets/one.png">
                        </figure>
                      </div>
                      <div class="column is-9">
                        <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                          Agente de Sucursal
                        </p>
                        <p class="card-header-title is-paddingless is-size-5-desktop is-size-6-tablet is-size-7-mobile">
                          Factorone S.A.
                        </p>
                      </div>
                      <div class="column is-1 is-paddingless">
                        <a href="" class="card-header-icon" aria-label="more options">
                          <span v-show="!showOption3" class="icon">
                            <font-awesome-icon icon="chevron-down" />
                          </span>
                          <span  v-show="showOption3" class="icon">
                            <font-awesome-icon icon="chevron-up" />
                          </span>
                        </a>
                      </div>
                    </div>
                  </div>
                </header>
                <transition name="expand">
                  <div v-show="showOption3" class="card-content has-text-justified">
                    Febrero 2016 a Noviembre 2019<br/>
                    <strong>Temuco, Chile</strong><br/>
                    <br/>
                    Evaluación financiera de empresas y confección de informes de riesgo. Gestión y control comercial de sucursal.<br/>
                    <br/>Durante mi período en esta empresa logré un aumento de 150% en colocaciones, mejorando la atomización de la cartera y diversificación de los productos financieros utilizados.
                    <br/>
                    <br/><strong>Referencias</strong>
                    <br/>
                    Felipe Muñoz, Gerente General<br/>
                    fmunoz@factorone.cl<br/>
                    +56 9 9997 1842<br/>
                    <br/>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption4" class="card-header card-header-option">
                  <div class="container">
                    <div class="columns is-mobile is-vcentered">
                      <div class="column is-2">
                        <figure class="image">
                          <img class="img-work" src="./assets/ind.png">
                        </figure>
                      </div>
                      <div class="column is-9">
                        <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                          Asesoría Financiera y Coaching
                        </p>
                        <p class="card-header-title is-paddingless is-size-5-desktop is-size-6-tablet is-size-7-mobile">
                          Independiente
                        </p>
                      </div>
                      <div class="column is-1 is-paddingless">
                        <a href="" class="card-header-icon" aria-label="more options">
                          <span v-show="!showOption4" class="icon">
                            <font-awesome-icon icon="chevron-down" />
                          </span>
                          <span  v-show="showOption4" class="icon">
                            <font-awesome-icon icon="chevron-up" />
                          </span>
                        </a>        
                      </div>
                    </div>
                  </div>
                </header>
                <transition name="expand">
                  <div v-show="showOption4" class="card-content has-text-justified">
                    Mayo 2013 a Enero 2016<br/>
                    <strong>La Serena, Chile</strong><br/>
                    <br/>
                    Asesoría en control financiero, evaluación y seguimiento de proyectos, determinación de posición financiera, análisis de capacidad de pago y estructuras de financiamiento.<br/>
                    <br/>Implementación de modelos de capacitación y entrenamiento organizacional orientado al fortalecimiento de las habilidades de relacionamiento, liderazgo, motivación, técnicas de autocuidado y manejo del estrés. Implementación de Tecnologías de la Información para el Desarrollo Organizacional.
                    <br/>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption5" class="card-header card-header-option">
                  <div class="container">
                    <div class="columns is-mobile is-vcentered">
                      <div class="column is-2">
                        <figure class="image">
                          <img class="img-work" src="./assets/chile.png">
                        </figure>
                      </div>
                      <div class="column is-9">
                        <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                          Ejecutivo Grandes Empresas
                        </p>
                        <p class="card-header-title is-paddingless is-size-5-desktop is-size-6-tablet is-size-7-mobile">
                          Banco Chile
                        </p>
                      </div>
                      <div class="column is-1 is-paddingless">
                        <a href="" class="card-header-icon" aria-label="more options">
                          <span v-show="!showOption4" class="icon">
                            <font-awesome-icon icon="chevron-down" />
                          </span>
                          <span  v-show="showOption4" class="icon">
                            <font-awesome-icon icon="chevron-up" />
                          </span>
                        </a>
                      </div>
                    </div>
                  </div>
                </header>
                <transition name="expand">
                  <div v-show="showOption5" class="card-content has-text-justified">
                    Marzo 2006 a Abril 2013<br/>
                    <strong>Antofagasta, Chile</strong><br/>
                    <br/>
                    - Evaluación financiera y de estructuras de financiamiento, generación de informes de riesgo.<br/>
                    <br/>- Gestión comercial y operativa de productos de crédito, leasing, factoring, boletas de garantía, cartas de crédito exportador, seguros y productos de mesa de dinero (forward y derivados).<br/>
                    <br/>- Gestión comercial y operativa de cartera de clientes PYMES y Grandes Empresas de la Región de Antofagasta, generando anticipo de cuentas por cobrar y saldos de precios en prosucto factoring.<br/>
                    <br/>Durante mi período en este cargo logré un continuo crecimiento de la cartera de colocaciones en todos los productos, llegando el año 2010 a duplicar el stock, premiado a nivel nacional por logros comerciales y habilidad para conjugar la mayor cantidad de productos financieros simples y complejos en la estrategia de financiamiento a empresas.
                    <br/>
                    <br/><strong>Referencias</strong>
                    <br/>
                    Francisco Arancibia, Gerente Zonal Sur<br/>
                    farancibiat@bancochile.cl<br/>
                    +56 9 9219 4025<br/>
                    <br/>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <footer class="footer">
      <div class="content has-text-centered">
        <p>Desarrollado 100% por Cristian Castillo M. - 2025</p>
      </div>
    </footer>
  </div>
</template>

<script>

import Modal from './shared/Modal.vue'
import ModalAna from './shared/ModalAna.vue'
import ModalCap from './shared/ModalCap.vue'
import ModalCoa from './shared/ModalCoa.vue'
import ModalGes from './shared/ModalGes.vue'
import ModalWeb from './shared/ModalWeb.vue'

export default { 

  name: 'MyWeb',

  components: { 
    Modal,
    ModalAna,
    ModalCap,
    ModalCoa,
    ModalGes,
    ModalWeb
  },
  
  data () {
    return {

      showModal: false,
      showModalAna: false,
      showModalCap: false,
      showModalCoa: false,
      showModalGes: false,
      showModalWeb: false,
      showOption1: false,
      showOption2: false,
      showOption3: false,
      showOption4: false,
      showOption5: false,

      targetUrl: '',

      courses: [
        {
          id: '1',
          url: './img/texc.f62587d7.png'
        },
        {
          id: '2',
          url: './img/tbi.8ac2e955.png'
        },
        {
          id: '3',
          url: './img/tvue.01271b9e.png'
        },
        {
          id: '4',
          url: './img/tvuep.01271b9e.png'
        },
        {
          id: '5',
          url: './img/tprog.f24e0844.png'
        },
        {
          id: '6',
          url: './img/tjs.12f3f42b.png'
        },
        {
          id: '7',
          url: './img/thtml.07887b14.png'
        },
        {
          id: '8',
          url: './img/tresp.4098ee4c.png'
        },
        {
          id: '9',
          url: './img/tg-suite.f1469bf6.png'
        },
        {
          id: '10',
          url: './img/ttrello.4eefa493.png'
        },
        {
          id: '11',
          url: './img/ttrem.38acfb1a.png'
        }
      ]
      
    }
  },


  methods: {

    isClosingModal () { this.showModal = false },

    isClosingModalAna () { this.showModalAna = false },

    isClosingModalCap () { this.showModalCap = false },

    isClosingModalCoa () { this.showModalCoa = false },

    isClosingModalGes () { this.showModalGes = false},

    isClosingModalWeb () { this.showModalWeb = false },

    clickExp (ev) {
      ev.preventDefault()
      let target = ev.target.id
      const imagen = document.getElementById(target)
      imagen.classList.remove('palpitar')
      
      if (target == 111) {
        this.showModalCoa = true  
      }
      if (target == 112) {
        this.showModalCap = true  
      }
      if (target == 113) {
        this.showModalWeb = true  
      }
      if (target == 114) {
        this.showModalAna = true  
      }
      if (target == 115) {
        this.showModalGes = true  
      }
    },

    clickCourse (ev) {
      ev.preventDefault()
      let target = ev.target.id 
      
      for (var i in this.courses) {
        if (this.courses[i].id == target) {
          console.log(this.courses[i])
          this.targetUrl = this.courses[i].url
          this.showModal = true
          const imagen = document.getElementById(target)
          console.log(imagen)
          imagen.classList.remove('palpitar')
        }
      }
    },
   
    toggleOption1 (ev) {
      ev.preventDefault()
      if (this.showOption1) {
        this.showOption1 = false
      } else {
        this.showOption1 = true
      }
    },

    toggleOption2 (ev) {
      ev.preventDefault()
      if (this.showOption2) {
        this.showOption2 = false
      } else {
        this.showOption2 = true
      }
    },

    toggleOption3 (ev) {
      ev.preventDefault()
      if (this.showOption3) {
        this.showOption3 = false
      } else {
        this.showOption3 = true
      }
    },

    toggleOption4 (ev) {
      ev.preventDefault()
      if (this.showOption4) {
        this.showOption4 = false
      } else {
        this.showOption4 = true
      }
    },

    toggleOption5 (ev) {
      ev.preventDefault()
      if (this.showOption5) {
        this.showOption5 = false
      } else {
        this.showOption5 = true
      }
    }

  }

}

</script>

<style lang="scss">

@import "./scss/main.scss";

html {
  scroll-behavior: smooth;
}

#app {
  font-family: Montserrat, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

header {
  box-shadow: 0px 9px 9px 0px #000033;
}

.hero-header, {
  background-color: #003366;
}

.hero-header p {
  text-align: center;
}

.hero-header a {
  color: #fff !important;
}

.hero-header a:hover {
  text-shadow: 0 0 3px #38b6ff,
  0 0 6px #38b6ff,
  0 0 9px #38b6ff,
  0 0 12px #38b6ff;  
}

.hero-body-header {
  padding: 0.9rem 1.5rem;
}

.hero-body-maker {
  padding: 0 1.5rem;
}

.hero-body-content {
  padding: 1.5rem 1.5rem 4.5rem 1.5rem;
}

.content-tag {
  position: fixed;
  bottom: 3rem;
  right: 3rem;
  z-index: 1;
}

.tag-up {
  background-color: #003366 !important;
  padding-top: 1.8rem;
  padding-bottom: 1.8rem;
  border-radius: 1rem !important;
  box-shadow: 0px 3px 3px 0px #000033;
  color: #fff !important;
  cursor: pointer;
}

.tag-up:hover {
  box-shadow: 0px 6px 6px 0px #000033;
}

.tag-up svg {
  margin: 1.2rem;
}

.hero-networks {
  background: #b1d7fd;
  color: #003366 !important;
  margin-top: 4.5rem;
}

.networks-title {
  color: #03203D;
  margin: 4.5rem 0 0 0;
}

.networks-subtitle {
  margin-bottom: 2.7rem;
}

.centrar {
  display: flex;
  justify-content: center;
}

.border-box-orbe {
  background-color: #03203D;
  width: 100%;
  padding: 1.8rem 1.2rem 3.9rem 1.2rem;
  margin-bottom: 6rem;
  height: auto;
  border-radius: 4.5%;
}

.box-orbe {
  background-color: #f1f8fe;
  width: 100%;
  height: auto;
  border-radius: 3%;
}

.img-exp {
  max-width: 120px;
  min-width: 120px;
  max-height: 120px;
  min-height: 120px;
  margin: auto;
  border-radius: 60px;
  box-shadow: 0px 6px 6px 0px black;
  cursor: pointer;
}

.orbe-up-left {
  margin: 3rem 0;
  width: 60%;
}

.orbe-up-rigth {
  margin: 3rem 0;
  width: 60%;
}

.orbe-center {
  margin-left: 35%;
  width: 30%;
}

.orbe-down-left {
  margin: 3rem 0;
  width: 60%;
}

.orbe-down-rigth {
  margin: 3rem 0;
  width: 6  0%;
}

.hero-maker {
  background: #0080FF;
  color: #fff !important;
}

.hero-content {
  background-color: #003366;
}

.img-yo {
  margin: 1.5rem auto;
  max-width: 240px;
  min-width: 240px;
  max-height: 285px;
  min-height: 285px;
  border-radius: 90px;
  box-shadow: 0px 9px 9px 0px black;
}

.ces {
  margin-top: 3rem;
}

.unap, .aiep {
  margin-top: 1.8rem;
}

.img-logo {
  max-width: 90px;
  min-width: 90px;
  max-height: 90px;
  min-height: 90px;
  margin: auto;
  border-radius: 18px;
  box-shadow: 0px 6px 6px 0px black;
}

.img-work {
  max-width: 75px;
  min-width: 75px;
  max-height: 75px;
  min-height: 75px;
  border-radius: 12px;
  border: 1px solid #003366;
  box-shadow: 0px 6px 6px 0px black;
}

.first-c {
  margin-bottom: 2.4rem !important;
}

.second-c {
  margin-bottom: 4.5rem !important;
}

.img-course {
  max-width: 120px;
  min-width: 120px;
  max-height: 120px;
  min-height: 120px;
  margin: auto;
  border-radius: 60px;
  box-shadow: 0px 6px 6px 0px black;
}

.palpitar {
  animation: palpitar 1.29s infinite ease-in-out;
  transition: transform 0.2s ease-in-out;
}

@keyframes palpitar {
  0%, 100% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.05);
    box-shadow: 0px 12px 12px 0px black;
  }
}

.img-warranty {
  max-width: 195px;
  min-width: 195px;
  max-height: 195px;
  min-height: 195px;
}

.title-text {
  font-weight: bold;
}

.title-text, .subtitle-text {
  color: #002549;
  display: block;
  text-align: center;
}

.prof-title {
  display: block;
  text-align: center;
  margin-top: 4.5rem;
  margin-bottom: .6rem;
}

.courses-title {
  display: block;
  text-align: center;
  margin-top: 4.5rem;
  margin-bottom: 0;
}

.courses-subtitle {
  margin-bottom: 4.5rem;
}

.course-img img {
  cursor: pointer;
}

.maker, .warranty {
  margin-top: 5.4rem;
  margin-bottom: 5.4rem !important;
}

.box-content {
  margin-top: 2.4rem;
  margin-bottom: 2.4rem !important;
  color: #fff;
}

.title-content {
  display: block;
  text-align: center;
  margin-bottom: 2.4rem;
}

.card-option {
  background-color: #fff;
  border-style: solid;
  border-radius: 9px;
  border-color: #003366;
  margin-bottom: 1.5rem;
}

.card-option:hover {
  box-shadow: 0px 15px 15px 0px #0080ff;
}

.card-option header {
  cursor: pointer;
  padding: .9rem;
}

.card-header-option p, a {
  color: #003366;
}

.icon {
  color: #003366;
}

.footer {
  background-color: #292C2F;
  color: #fff;
  padding: 2.4rem 1.5rem;
}

@media screen and (min-width: 769px) and (max-width: 1024px) {

  .border-box-orbe {
    margin-bottom: .9rem;
  }

  .languages {
    margin-bottom: 3rem;
  }

}


@media screen and (max-width: 768px) {

  .box-notification {
    margin-top: 3rem;
  }

  .notification {
    max-width: 90%;
  }

  .hero-header a {
    text-shadow: 0 0 3px #38b6ff,
    0 0 6px #38b6ff,
    0 0 9px #38b6ff,
    0 0 12px #38b6ff;  
  }

  .hero-body-header {
    padding: 0.6rem 1.5rem;
  }

  .hero-body-maker {
    padding: 1.5rem;
  }

  .content-tag {
    right: .9rem;
    bottom: 3rem;
  }

  .tag-up {
    padding-top: 1.5rem;
    padding-bottom: 1.5rem;
    box-shadow: 0px 6px 6px 0px #38b6ff;
  }

  .img-yo {
    max-width: 160px;
    min-width: 160px;
    max-height: 190px;
    min-height: 190px;
    border-radius: 24px;
    box-shadow: 0px 6px 6px 0px black;
  }

  .img-logo {
    max-width: 48px;
    min-width: 48px;
    max-height: 48px;
    min-height: 48px;
    border-radius: 6px;
    box-shadow: 0px 3px 3px 0px black;
  }

  .img-work {
    max-width: 48px;
    min-width: 48px;
    max-height: 48px;
    min-height: 48px;
    border-radius: 6px;
    box-shadow: 0px 3px 3px 0px black;
  }

  .img-course {
    max-width: 90px;
    min-width: 90px;
    max-height: 90px;
    min-height: 90px;
    border-radius: 45px;
    box-shadow: 0px 3px 3px 0px black;
  }

  .title-text {
    margin-top: 0;
  }

  .subtitle-text {
    margin-bottom: 0;
  }

  .column-content {
    padding-left: 0;
    padding-right: 0;
  }

  .box-image-warranty {
    display: flex;
    justify-content: center;
  }

  .maker, .warranty {
    margin: 1.5rem 3% .9rem 3% !important;
  }

  .border-box-orbe {
    max-width: 94%;
    padding: 0;
    margin-right: 3%;
    margin-left: 3%;
    margin-bottom: .9rem;
  }

  .box-orbe {
    border: 3px solid #03203D;
  }

  .languages {
    margin-bottom: 3rem;
  }

  .card-option {
    box-shadow: 0px 9px 9px 0px #0080ff;
  }

  .card-option:hover {
    box-shadow: 0px 6px 6px 0px #0080ff;
  }

  .footer {
    padding: 1.5rem;
  }

  .footer p {
    font-size: .81rem;
  }

}

</style>
