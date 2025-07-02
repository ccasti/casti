<template>
  <div id="app">
    <header>
      <section id="header" class="hero hero-header">
        <div class="hero-body hero-body-header">
          <div class="container">
            <div class="columns is-vcentered is-mobile">
              <div class="column is-3-mobile is-2-desktop">
                <figure class="image">
                  <img class="img-logo" src="./assets/logo-small.png">
                </figure>
              </div>
              <div class="column is-3-mobile is-2-desktop is-offset-1-desktop">
                <p class="is-size-4-desktop is-size-6-mobile">
                  <a href="#maker">Modelo</a>
                </p>
              </div>
              <div class="column is-3-mobile is-2-desktop is-offset-1-desktop">
                <p class="is-size-4-desktop is-size-6-mobile">
                  <a href="#content">Cápsulas</a>
                </p>
              </div>
              <div class="column is-3-mobile is-2-desktop is-offset-1-desktop">
                <p class="is-size-4-desktop is-size-6-mobile">
                  <a href="#networks">Redes</a>
                </p>
              </div>
            </div>  
          </div>
        </div>
      </section>
    </header>
    <div class="box-notification is-marginless">
      <transition name="notification">
        <notification
          v-show="showNotification"
          class="notification"
        />
      </transition>
    </div>
    <section class="hero hero-intro">
      <div class="hero-body hero-body-intro">
        <div class="container">
          <div class="content-tag">
            <a href="#header">
              <span class="tag is-large tag-up">
                <font-awesome-icon icon="arrow-up" />
              </span>    
            </a>
          </div>
          <div class="columns">
            <div class="column is-full">
              <p class="is-size-2-desktop is-size-4-mobile title-text">
                Autoconocimiento y Autogestión
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <p class="is-size-2-desktop is-size-4-mobile subtitle-text">
                Instancias web para el desarrollo personal
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <figure class="image">
                <img class="img-title" src="./assets/people.jpg">
              </figure>  
            </div>
          </div>
        </div>    
      </div>
    </section>
    <section id="maker" class="hero hero-maker">
      <div class="hero-body hero-body-maker">
        <div class="container">
          <div id="maker" class="columns maker is-vcentered">
            <div class="column is-1-desktop is-hidden-mobile is-paddingless"></div>
            <div class="column is-12-mobile is-5-tablet is-offset-1-tablet is-4-desktop is-offset-1-desktop">
              <p class="is-size-3-desktop is-size-4-mobile has-text-weight-bold">Nuestro Modelo</p>
              <p class="is-size-5">
                Nos enfocamos en desarrollar interfaces web con dedicación y cariño, pensando en tu desarrollo personal y profesional. Cada herramienta ha sido amorosamente programada para acompañarte en tu proceso de autoconocimiento, ayudándote a gestionar emociones, tomar mejores decisiones y avanzar con confianza hacia tus metas.<br><br>Sabemos que crecer no siempre es fácil, por eso queremos hacerlo más accesible para ti. Nuestras interfaces están basadas en metodologías de Coaching y te ofrecen un camino claro y práctico para fortalecer tu bienestar, mejorar tu productividad y potenciar tu liderazgo a través del autoconocimiento y herramientas de desarrollo personal.<br><br>Con un diseño intuitivo y amigable, estas herramientas digitales han sido creadas para apoyarte en cada paso, brindándote un espacio de reflexión y acción. Porque tu desarrollo nos importa, hemos puesto el corazón en cada detalle para que encuentres aquí un apoyo real en tu camino de crecimiento.
              </p>
            </div>
            <div class="column is-12-mobile is-5-tablet is-offset-1-tablet is-5-desktop is-offset-1-desktop">
              <figure class="image">
                <img class="img-maker" src="./assets/logo.png">
              </figure>  
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="content" class="hero hero-content">
      <div class="hero-body hero-body-content">
        <div class="container">
          <div class="columns box-content">
            <div class="column is-12-mobile is-10-desktop is-offset-1-desktop title-content">
              <p class="is-size-3-desktop is-size-4-mobile">
                Nuestras Cápsulas
              </p>
              <p class="is-size-5">
                Todas nuestras cápsulas son ejecutadas y administradas a través de Hotmart, una de las principales plataformas mundiales para la venta y distribución de productos digitales.
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption1" class="card-header card-header-option">
                  <p class="card-header-title is-size-4-desktop is-size-5-mobile">
                    Conocimiento
                  </p>
                  <a href="" class="card-header-icon" aria-label="more options">
                    <span v-show="!showOption1" class="icon">
                      <font-awesome-icon icon="chevron-down" />
                    </span>
                    <span  v-show="showOption1" class="icon">
                      <font-awesome-icon icon="chevron-up" />
                    </span>
                  </a>
                </header>
                <transition name="expand">
                  <div v-show="showOption1" class="card-content">
                    <div class="container">
                      <div class="columns">
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/autoc.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Autoconocimiento</p>
                                  <p class="subtitle is-6">Introducción al autoconocimiento</p>
                                </div>
                              </div>
                              <div class="content">
                                <strong>El inicio de la autogestión comienza aquí.</strong><br/>
                                <br/>
                                Explora tu mundo interno con una experiencia interactiva diseñada para abrir las puertas del autoconocimiento.<br/>
                                <br/>Esta es una cápsula de conocimiento que consiste en una aplicación web que te guía suavemente hacia una mayor comprensión acerca de la importancia del autoconocimiento y lo que realmente significa: reconocer tus emociones, entender tus pensamientos y descubrir los patrones que influyen en tu forma de vivir y relacionarte. Todo en un espacio seguro, claro y visualmente atractivo, diseñado para invitarte a reflexionar y conectarte contigo.
                                <br/>
                                <br/>Por apenas <strong>US$9.00.-</strong>
                                <br/>
                                <div class="button-offer">
                                  <button
                                    id="autoc"
                                    class="button is-rounded"
                                    @click="buying">
                                    COMPRAR AHORA</button>    
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/logro.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Logro de Objetivos</p>
                                  <p class="subtitle is-6">Técnica Logro de Objetivos</p>
                                </div>
                              </div>
                              <div class="content">
                                <strong>Una técnica de PNL que te ayudará a cumplir tus metas y más...</strong><br/>
                                <br/>
                                Convierte tus metas en logros reales. Aprende a formular objetivos de forma clara y motivadora, y sigue un paso a paso práctico para alcanzarlos. Esta técnica es aplicable a cualquier área de tu vida y te ayudará a obtener resultados concretos.<br/>
                                <br/>Esta es una cápsula de conocimiento que te acompaña a través de una interfaz web interactiva, diseñada para que aprendas a formular tus objetivos de manera clara, consciente y alineada con lo que realmente deseas. A través de un recorrido guiado y visualmente estimulante, descubrirás una técnica efectiva que, paso a paso, te ayuda a transformar tus metas en logros concretos. Una experiencia creada para motivarte, enfocar tu energía y aumentar significativamente tus posibilidades de éxito.
                                <br/>
                                <br/>Por apenas <strong>US$12.00.-</strong>
                                <br/>
                                <div class="button-offer">
                                  <button
                                    id="logro"
                                    class="button is-rounded"
                                    @click="buying">
                                    COMPRAR AHORA</button>    
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                      </div>
                    </div>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption2" class="card-header card-header-option">
                  <p class="card-header-title is-size-4-desktop is-size-5-mobile">
                    Test
                  </p>
                  <a href="" class="card-header-icon" aria-label="more options">
                    <span v-show="!showOption2" class="icon">
                      <font-awesome-icon icon="chevron-down" />
                    </span>
                    <span  v-show="showOption2" class="icon">
                      <font-awesome-icon icon="chevron-up" />
                    </span>
                  </a>
                </header>
                <transition name="expand">
                  <div v-show="showOption2" class="card-content">
                    <div class="container">
                      <div class="columns">
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/croma.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Test Cromático</p>
                                  <p class="subtitle is-6">Test de composiciones cromáticas</p>
                                </div>
                              </div>
                              <div class="content">
                                <strong>Descubre el significado oculto de tus elecciones.</strong><br/>
                                <br/>
                                Una experiencia de introspección personal que revela rasgos de tu personalidad y emociones profundas. Ideal para el autoconocimiento. ¡Atrévete a descubrirte!<br/>
                                <br/>Todo sucede en una interfaz web sencilla y clara diseñada para facilitar una conexión profunda con tu ser interior. Este test de composiciones cromáticas te acompaña de forma sutil e intuitiva hacia un momento de reflexión e introspección,  facilitando una mayor comprensión de tu mundo interno. Más que un test, es una invitación a detenerte y reflexionar sobre quién eres.
                                <br/>
                                <br/>Por apenas <strong>US$6.00.-</strong>
                                <br/>
                                <div class="button-offer">
                                  <button
                                    id="croma"
                                    class="button is-rounded"
                                    @click="buying">
                                    COMPRAR AHORA</button>    
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/orient.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Orientación Profesional</p>
                                  <p class="subtitle is-6">Test de Orientación Profesional</p>
                                </div>
                              </div>
                              <div class="content">
                                <strong>¡Otra forma de autoconocimiento!</strong><br/>
                                <br/>
                                El propósito de este test es estimularte a pensar sobre tus propias áreas de competencia, tus motivaciones y tus valores. Activará tu pensamiento y te preparará para su análisis y reflexión.<br/>
                                <br/>Esta es una cápsula de conocimiento que ocurre a través de una interfaz web diseñada para activar tu pensamiento y conectar contigo mismo a través de un test interactivo. A medida que avanzas, te invita a reflexionar sobre tus competencias, motivaciones y valores personales. Una experiencia introspectiva que despierta tu conciencia, te prepara para el análisis profundo y te abre la puerta a una comprensión más clara de quién eres y hacia dónde quieres ir.
                                <br/>
                                <br/>Por apenas <strong>US$9.00.-</strong>
                                <br/>
                                <div class="button-offer">
                                  <button
                                    id="orient"
                                    class="button is-rounded"
                                    @click="buying">
                                    COMPRAR AHORA</button>    
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                      </div>
                    </div>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption3" class="card-header card-header-option">
                  <p class="card-header-title is-size-4-desktop is-size-5-mobile">
                    Dinámicas
                  </p>
                  <a href="" class="card-header-icon" aria-label="more options">
                    <span v-show="!showOption3" class="icon">
                      <font-awesome-icon icon="chevron-down" />
                    </span>
                    <span  v-show="showOption3" class="icon">
                      <font-awesome-icon icon="chevron-up" />
                    </span>
                  </a>
                </header>
                <transition name="expand">
                  <div v-show="showOption3" class="card-content">
                    <div class="container">
                      <div class="columns">
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/carta.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Carta a mi niñez</p>
                                  <p class="subtitle is-6">Dinamica: Carta a mi niñez</p>
                                </div>
                              </div>
                              <div class="content">
                                <strong>¡Recuerdos y más…!</strong><br/>
                                <br/>
                                Una poderosa y emotiva instancia de reflexión y autodescubrimiento diseñada para conectarte con todo aquello que define a la persona que eres.<br/>
                                <br/>Esta es una cápsula de conocimiento que te invita a reconectar con tu historia personal a través de una experiencia web íntima y reflexiva. A lo largo del recorrido, explorarás vivencias de tu infancia que han dado forma a la persona que eres hoy. Conectarte con esas experiencias te permitirá comprender mejor tus emociones, creencias y patrones actuales. Una herramienta poderosa de autoconocimiento, diseñada para sanar, resignificar y crecer desde tus raíces.
                                <br/>
                                <br/>Por apenas <strong>US$9.00.-</strong>
                                <br/>
                                <div class="button-offer">
                                  <button
                                    id="carta"
                                    class="button is-rounded"
                                    @click="buying">
                                    COMPRAR AHORA</button>    
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                      </div>
                    </div>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption4" class="card-header card-header-option">
                  <p class="card-header-title is-size-4-desktop is-size-5-mobile">
                    Combos
                  </p>
                  <a href="" class="card-header-icon" aria-label="more options">
                    <span v-show="!showOption4" class="icon">
                      <font-awesome-icon icon="chevron-down" />
                    </span>
                    <span  v-show="showOption4" class="icon">
                      <font-awesome-icon icon="chevron-up" />
                    </span>
                  </a>
                </header>
                <transition name="expand">
                  <div v-show="showOption4" class="card-content">
                    <div class="container">
                      <div class="columns">
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/combo.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Combo Conociéndote</p>
                                  <p class="subtitle is-6">Set de nuestras 5 herramientas</p>
                                </div>
                              </div>
                              <div class="content">
                                <strong>Un viaje completo hacia ti mismo</strong><br/>
                                <br/>
                                 Explora tu mundo interior con esta colección de experiencias digitales diseñadas para acompañarte en un proceso transformador de introspección, reflexión y crecimiento personal. Este combo reúne cinco cápsulas de conocimiento complementarias que, juntas, forman una travesía coherente y profunda hacia el autoconocimiento.
                                 <br/>
                                <br/>Desde la sutileza de los colores que revelan tu mundo emocional en el Test de Composiciones Cromáticas, hasta la emotiva reconexión con tu historia personal en Carta a mi Niñez, cada experiencia te invita a detenerte, mirar hacia dentro y descubrir quién eres en verdad. A través de una interfaz web clara, segura y visualmente atractiva, avanzarás por espacios de exploración emocional, descubrimiento de tus motivaciones, identificación de tus valores y construcción de objetivos alineados con tu esencia.
                                <br/>
                                <br/>Este combo es mucho más que un conjunto de herramientas: es una guía para reencuentros significativos contigo mismo, un espacio para ordenar, comprender y resignificar tu experiencia de vida, y una oportunidad para proyectarte con mayor claridad y propósito hacia el futuro.
                                <br/>
                                <br/>Por apenas <strong>US$30.00.-</strong>
                                <br/>
                                <div class="button-offer">
                                  <button
                                    id="combo"
                                    class="button is-rounded"
                                    @click="buying">
                                    COMPRAR AHORA</button>    
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                      </div>
                    </div>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-10-desktop is-offset-1-desktop is-12-mobile column-content">
              <div class="card-option">
                <header @click="toggleOption5" class="card-header card-header-option">
                  <p class="card-header-title is-size-4-desktop is-size-5-mobile">
                    Próximamente
                  </p>
                  <a href="" class="card-header-icon" aria-label="more options">
                    <span v-show="!showOption4" class="icon">
                      <font-awesome-icon icon="chevron-down" />
                    </span>
                    <span  v-show="showOption4" class="icon">
                      <font-awesome-icon icon="chevron-up" />
                    </span>
                  </a>
                </header>
                <transition name="expand">
                  <div v-show="showOption5" class="card-content">
                    <div class="container">
                      <div class="columns">
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/eneag.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Eneagrama</p>
                                  <p class="subtitle is-6">Test y todo del Eneagrama</p>
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                        <div class="column is-6-desktop is-12-mobile">
                          <div class="card card-boll">
                            <div class="card-image">
                              <figure class="image is-4by3">
                                <img
                                  src="./assets/comport.jpg"
                                  alt="Placeholder image"
                                />
                              </figure>
                            </div>
                            <div class="card-content">
                              <div class="media">
                                <div class="media-content">
                                  <p class="title is-4">Comportamiento</p>
                                  <p class="subtitle is-6">Modelo del comportamiento de las personas</p>
                                </div>
                              </div>
                            </div>
                          </div>      
                        </div>
                      </div>
                    </div>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="container">
      <div class="columns warranty is-vcentered">
        <div class="column is-1-desktop is-hidden-mobile is-paddingless"></div>
        <div class="column is-12-mobile is-5-tablet is-offset-1-tablet is-centered is-4-desktop is-offset-1-desktop">
          <figure class="image box-image-warranty">
            <img class="img-warranty" src="./assets/warranty.png">
          </figure>
        </div>
        <div class="column is-12-mobile is-5-tablet is-offset-1-tablet is-5-desktop is-offset-1-desktop">
          <p class="is-size-3">Garantía de 15 <STRONG>días</STRONG></p>
          <p class="is-size-5">
            Tendrás tu dinero devuelta <STRONG>sin preguntas</STRONG>  hasta 15 días después de la compra.
          </p>
        </div>
      </div>
    </div>
    <section id="maker" class="hero hero-networks">
      <div class="hero-body hero-body-netwoks">
        <div class="container">
          <div id="networks" class="columns">
            <div class="column is-full">
              <p class="is-size-3-desktop is-size-4-mobile has-text-weight-bold">Redes Sociales</p>
              <p class="is-size-5">
                Accede a nuestra redes sociales e interactúa compartiendo comentarios o contenidos, estaremos gratos de saber que te parece nuestra iniciativa. Saludos!!!
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-4-desktop">
              <figure class="image">
                <img id="face" class="img-networks" src="./assets/face.png" @click="socializing">
              </figure>
            </div>
            <div class="column is-4-desktop">
              <figure class="image">
                <img id="insta" class="img-networks" src="./assets/insta.png" @click="socializing">
              </figure>
            </div>
            <div class="column is-4-desktop">
              <figure class="image">
                <img id="hot" class="img-networks" src="./assets/hot.jpg" @click="socializing">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <p class="is-size-3-desktop is-size-4-mobile has-text-weight-bold">Sólo válido en Chile</p>
              <p class="is-size-5">
                Aplicamos también nuestro modelo en el diseño de cursos e-learning asíncronos que son dictados con beneficio de franquicia tributaria. Visita la web de nuestra OTEC.
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <figure class="image">
                <img id="otec" class="img-otec" src="./assets/otec.png" @click="socializing">
              </figure>
            </div>
          </div>
        </div>
      </div>
    </section>
    <footer class="footer">
      <div class="content has-text-centered">
        <p>Copyright © desarrollado por Cristian Castillo - 2025</p>
      </div>
    </footer>
  </div>
</template>

<script>

import Notification from './shared/Notification.vue'
export default { 

  name: 'Webcoach',

  components: { Notification },
  
  data () {
    return {

      showNotification: false,    
      showOption1: false,
      showOption2: false,
      showOption3: false,
      showOption4: false,
      showOption5: false,

      targetUrl: '',
      targetId: '',

      courses: [
        {
          id: 'autoc',
          url: 'https://pay.hotmart.com/P99585037U'
        },
        {
          id: 'logro',
          url: 'https://pay.hotmart.com/A99180336E'
        },
        {
          id: 'croma',
          url: 'https://pay.hotmart.com/Q98606053K'
        },
        {
          id: 'orient',
          url: 'https://pay.hotmart.com/X99600629R'
        },
        {
          id: 'carta',
          url: 'https://pay.hotmart.com/Y99588589J'
        },
        {
          id: 'combo',
          url: 'https://pay.hotmart.com/A99603316T'
        }
      ],

      networks: [
        {
          id: 'face',
          url: 'https://www.facebook.com/profile.php?id=61575693165438'
        },
        {
          id: 'insta',
          url: 'https://www.instagram.com/autoconocimientoygestion/'
        },
        {
          id: 'otec',
          url: 'https://otec-aurea.cl/'
        },
        {
          id: 'hot',
          url: 'https://hotmart.com/es/club/autoconocimiento-y-autogestion'
        }
      ]

    }
  },

  methods: {

    click (ev) {
      ev.preventDefault()
      this.targetId = ev.target.id
      
      document.getElementById(this.targetId).style.boxShadow = "0px 6px 6px 0px #922D23";
      setTimeout(() => {
        document.getElementById(this.targetId).style.boxShadow = "0px 12px 6px -3px #922D23";
      }, 300)
    },

    redirecting () {
      setTimeout(() => {
        document.getElementById(this.targetId).classList.add('is-loading')
      }, 600);

      setTimeout(() => {
        this.showNotification = true
      }, 900);

      setTimeout(() => {
        location.href = this.targetUrl
      }, 2400);
    },

    buying (ev) {
      this.click(ev)

      for (var i in this.courses) {
        if (this.courses[i].id == this.targetId) {
          this.targetUrl = this.courses[i].url
        }
      }

      this.redirecting()
    },

    socializing (ev) {
      this.click(ev)

      for (var i in this.networks) {
        if (this.networks[i].id == this.targetId) {
          this.targetUrl = this.networks[i].url
        }
      }

      this.redirecting()
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

.box-notification {
  display:flex;
  justify-content: center;
  margin-top: 6rem;
}

.notification {
  margin: 0;
  padding: 0;
  position: fixed;
  z-index: 1;
  max-width: 400px;
  border: 3px solid #CB4335;
  border-radius: 9px;
  box-shadow: 0px 0px 9px 3px #CB4335;
}

header {
  box-shadow: 0px 9px 9px 0px black;
}

.hero-header, {
  background-color: #292C2F;
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

.hero-body-netwoks {
  padding: 4.5rem 1.5rem;
}

.content-tag {
  position: fixed;
  bottom: 3rem;
  right: 3rem;
  z-index: 1;
}

.tag-up {
  background-color: #292C2F !important;
  padding-top: 1.8rem;
  padding-bottom: 1.8rem;
  border-radius: 1rem !important;
  box-shadow: 0px 3px 3px 0px #38b6ff;
  color: #38b6ff !important;
  cursor: pointer;
}

.tag-up:hover {
  box-shadow: 0px 6px 6px 0px #38b6ff;
}

.tag-up svg {
  margin: 1.2rem;
}

.hero-maker, .hero-networks {
  background: #CD564A;
  color: #fff !important;
  margin-top: 4.5rem;
}

.hero-content {
  background-color: #292C2F;
}

.img-logo, {
  max-width: 90px;
  min-width: 90px;
  max-height: 90px;
  min-height: 90px;
  border-radius: 45px;
  box-shadow: 0px 9px 9px 0px black;
}

.img-title {
  margin: 1.5rem auto;
  max-width: 639px;
  min-width: 639px;
  max-height: 426px;
  min-height: 426px;
  border-radius: 60px;
  box-shadow: 0px 9px 9px 0px black;
}

.img-maker {
  max-width: 450px;
  min-width: 450px;
  max-height: 450px;
  min-height: 450px;
  border-radius: 225px;
  box-shadow: 0px 9px 9px 0px black;
}

.img-warranty {
  max-width: 195px;
  min-width: 195px;
  max-height: 195px;
  min-height: 195px;
}

.img-networks {
  margin: 1.5rem auto;
  max-width: 195px;
  min-width: 195px;
  max-height: 195px;
  min-height: 195px;
  border-radius: 48px;
  box-shadow: 0px 9px 9px 0px black;
  cursor: pointer;
  opacity: .81;
}

.img-otec {
  margin: 1.5rem auto;
  max-width: 270px;
  min-width: 270px;
  max-height: 167px;
  min-height: 167px;
  box-shadow: 0px 9px 9px 0px black;
  cursor: pointer;
  opacity: .81;
}

.img-networks:hover, .img-otec:hover {
  opacity: 1;
  box-shadow: 0px 15px 15px 0px black;
}

.title-text {
  font-weight: bold;
  margin-top: 2.4rem;
}

.subtitle-text {
  margin-bottom: 3rem;
}

.title-text, .subtitle-text {
  color: #f1f7fb;
  display: block;
  text-align: center;
  text-shadow: 0 0 6px #38b6ff,
  0 0 12px #38b6ff,
  0 0 15px #38b6ff,
  0 0 18px #38b6ff;  
}

.maker, .warranty {
  margin-top: 5.4rem;
  margin-bottom: 5.4rem !important;
}

.box-content {
  margin-top: 2.4rem;
  margin-bottom: 2.4rem !important;
}

.title-content {
  display: block;
  text-align: center;
  color: #fff;
}

.card-option {
  background-color: #292C2F;
  border-style: solid;
  border-radius: 9px;
  border-color: #38b6ff;
  box-shadow: 0px 3px 3px 0px #38b6ff;
  margin-bottom: 1.5rem;
}

.card-option header {
  cursor: pointer;
}

.card-header-option p, a {
  color: #fff;
}

.icon {
  color: #fff;
}

.card-header-option p:hover {
  text-shadow: 0 0 3px #38b6ff,
  0 0 6px #38b6ff,
  0 0 9px #38b6ff,
  0 0 12px #38b6ff;
}

.card-boll {
  margin: 10%;
}

.footer {
  background-color: #292C2F;
  color: #fff;
  padding: 2.4rem 1.5rem;
}

.button-offer {
  display: flex;
  justify-content: center;
}

.button {
  margin-top: 2.4rem;
  margin-bottom: 1.2rem;
  background-color: #CD564A;
  border-color: #CD564A;
  color: #fff !important;
  box-shadow: 0px 6px 6px 0px #922D23;
  transition: all 300ms;
  -webkit-tap-highlight-color: transparent;
  opacity: .9;
}

.button:hover {
  box-shadow: 0px 12px 6px -3px #922D23;
  opacity: 1;
}

@media screen and (max-width: 768px) {

  .box-notification {
    margin-top: 3 rem;
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

  .img-logo {
    max-width: 48px;
    min-width: 48px;
    max-height: 48px;
    min-height: 48px;
    border-radius: 24px;
    box-shadow: 0px 6px 6px 0px black;
    margin-left: .9rem;
  }

  .img-title {
    margin: 1.5rem 5%;
    max-width: 90%;
    min-width: 90%;
    max-height: 100%;
    min-height: 100%;
    border-radius: 39px;
    box-shadow: 0px 6px 6px 0px black;
  }

  .img-maker {
    margin: 1.5rem 0;
    max-width: 100%;
    min-width: 100%;
    max-height: 100%;
    min-height: 100%;
  }

  .img-networks {
    max-width: 90px;
    min-width: 90px;
    max-height: 90px;
    min-height: 90px;
    border-radius: 21px;
    box-shadow: 0px 15px 15px 0px black;
    opacity: 1;
  }

  .img-otec {
    max-width: 167px;
    min-width: 167px;
    max-height: 111px;
    min-height: 111px;
    box-shadow: 0px 15px 15px 0px black;
    opacity: 1;
  }

  .title-text {
    margin-top: 0;
  }

  .subtitle-text {
    margin-bottom: 0;
  }

  .card-header-option p {
    text-shadow: 0 0 3px #38b6ff,
    0 0 6px #38b6ff,
    0 0 9px #38b6ff,
    0 0 12px #38b6ff;
  }

  .column-content {
    padding-left: 0;
    padding-right: 0;
  }

  .card-boll {
    margin-left: 0;
    margin-right: 0;
  }

  .box-image-warranty {
    display: flex;
    justify-content: center;
  }

  .maker, .warranty {
    margin: 1.5rem 3% .9rem 3% !important;
  }

  .button {
    box-shadow: 0px 12px 6px -3px #922D23;
    transition: all 300ms;
    -webkit-tap-highlight-color: transparent;
    opacity: 1;
  }

  .footer {
    padding: 1.5rem;
  }

  .footer p {
    font-size: .81rem;
  }

}

</style>
