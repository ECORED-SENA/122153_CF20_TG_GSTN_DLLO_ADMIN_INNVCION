<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    p.mb-4 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center
      .col-lg-11.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="A continuación, se presenta la síntesis del componente formativo: La acción de mejora basada en big data consta de: - Herramientas colaborativas como lo son las videoconferencias, pantallas interactivas, proyectores y uso compartido a través de dispositivos móviles. - Ciencia de datos: inferencia estadística, técnicas de transformación (mapeo de datos, generación de código, transformación de datos), modelos neuronales, internet de las cosas, inteligencia artificial (aprendizaje automático). - Normativa: características, seguridad y salud en el trabajo, propiedad intelectual, derechos de autor y patrimoniales y por último acciones preventivas, correctivas y no conformidad.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
