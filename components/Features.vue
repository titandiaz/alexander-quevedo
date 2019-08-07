<template>
  <div class="features">
    <div class="title title-features">Programa de Gobierno</div>
    <div class="grid">
      <div
        class="feature"
        v-for="item in data"
      >
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">{{item.title}}</div>
          <ul>
            <li v-for="description in item.description">
              <i class="material-icons">check</i>
              <p>{{description}}</p>
            </li>
          </ul>
        </div>
      </div>
      <!-- <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Salud</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Políticas Sociales</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Obras e Infraestructura</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">San José del Guaviare Incluyente</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Productividad y Desarrollo Rural</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div> -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: [
        {
          id: 1,
          title: "Educación",
          description: [
            "Implementación y fortalecimiento de las escuelas de padres.",
            "Actualización de los PEI en articulación con el departamento.",
            "El docente como protagonista en la construcción de sociedad (cualificación, apoyo a redes y bienestar)"
            // "Estímulos e incentivos a iniciativas educativas de impacto para la región.",
            // "Fortalecimiento a los ambientes escolares."
          ],
          icon: ""
        },
        {
          id: 2,
          title: "Salud",
          description: [
            "Competencia municipal en Inspección, Vigilancia y Control efectiva.",
            "Salud familiar como eje de prevención de la enfermedad y promoción de la salud.",
            "Acciones de prevención del consumo de SPA (sustancias psicoactivas) en niños, niña, adolescentes y jóvenes NNAJ y embarazos en adolescentes."
            // "Asesoría y acompañamiento que garantice una prestación de los servicios de salud con oportunidad y calidad (EPS e IPS).",
            // "Garantizar la continuidad y efectividad en la ejecución de los PIC.",
            // "Gestión de la unidad de pago por capitación UPC diferencial."
          ],
          icon: ""
        },
        {
          id: 3,
          title: "Obras e Infraestructura",
          description: [
            "Mejoramiento de la malla vial del municipio a nivel urbano y rural, en articulación con el Departamento.",
            "Mantenimiento y construcción de la red de acueducto y alcantarillado del municipio.",
            "Mejoramiento del parque de la constitución como un referente histórico y turístico del municipio, y la construcción de nuevos parques."
            // "Adecuación y construcción de techos peatonales, en el sector comercial.",
            // "Ampliación de la red de alumbrado público.",
            // "Recuperación de áreas estratégicas ambientales y ecológicas de importancia para el municipio",
            // "Recuperación de la Villa olímpica y otros escenarios deportivos y culturales.",
            // "Guaviare rural. Vías productivas"
          ],
          icon: ""
        },
        {
          id: 4,
          title: "San José del Guaviare Incluyente",
          description: [
            "Garantizar los procesos de restitución de derechos de víctimas.",
            "Articulación de las políticas y programas sociales con la población en procesos de reintegración.",
            "Inclusión de la población en situación de discapacidad"
            // "Atención a población indígena con enfoque diferencial.",
            // "San José pacto por la equidad de genero",
            // "Mujeres como agentes de transformación de paz"
          ],
          icon: ""
        },
        {
          id: 5,
          title: "Productividad y Desarrollo Rural",
          description: [
            "Fortalecimiento e implementación del modelo de “mercados campesinos”.",
            "Estrategia de compras públicas locales institucionalizada, como herramienta para fortalecer productores y comercializadores municipales.",
            "Asistencia técnica integral para el manejo de los ciclos productivos."
            // "Transformación y valor agregado a productos de la región.",
            // "Reconversión, prácticas ganaderas sostenibles.",
            // "Implementación de modelos de granjas integrales amazónicos.",
            // "Articulación con los Programas de Desarrollo con Enfoque Territorial (PDET) como base fundamental para desarrollo del campo."
          ],
          icon: ""
        },
        {
          id: 6,
          title: "Turismo",
          description: [
            "Diseño e implementación del Plan Municipal de Turismo ",
            "Oficina con puntos de orientación e información turística, con articulación departamental. ",
            "Educación en promoción y mercadeo turística."
            // "Vías para el desarrollo de la industria turística.",
            // "Rutas turísticas étnicas."
          ],
          icon: ""
        }
      ]
    };
  }
};
</script>

<style scoped>
.features {
  width: 100%;
  padding: 40px 10px;
  box-sizing: border-box;
}
.grid {
  margin: 0 auto;
  max-width: 1344px;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(340px, 5fr));
  grid-gap: 40px;
}
.title-features {
  text-align: center;
  margin-bottom: 50px;
  color: #2a2f53;
  letter-spacing: -0.4px;
}
.feature {
  display: flex;
}
.icon-description {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: var(--orange);
  color: #fff;
  margin: 5px 10px 0 0;
}
.icon-description i {
  line-height: 1;
}
.description {
  flex: 1;
}
.description li {
  color: #2a2f53;
}
.title-description {
  font-weight: 600;
  margin: 0 0 5px 0;
  color: #2a2f53;
}
li > i {
  font-size: 17px;
  margin: 3px 5px 0 0;
}
ul li {
  display: flex;
}
@media (max-width: 1024px) {
  .grid {
    grid-template-columns: repeat(auto-fill, minmax(250px, 5fr));
  }
  .description li {
    font-size: 14px;
  }
}
</style>
