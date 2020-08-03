<template>
  <v-row justify="center" align="center" class="pa-2">
    <v-col cols="12">
      <div style="text-align: justify; margin-bottom: 1.5em;">
        <strong>INSTRUCCIÓN</strong>: Lee detenidamente el texto y contesta las siguientes preguntas:
      </div>
      <div style="text-align: center;">
        <strong>CRÓNICA DE UNA MUERTE ANUNCIADA</strong>
        <p>(Fragmento)</p>
      </div>
      <div style="text-align: right; margin: 1em 0 2em 0;">
        Gabriel García Márquez
      </div>
      <div style="text-align: justify;">
        <p><strong>El acto formal terminó a las seis de la tarde cuando se despidieron los invitados de honor. El buque se fue con las luces encendidas y dejando un reguero de valses de pianola, y por un instante quedamos a la deriva sobre un abismo de incertidumbre,
          hasta que volvimos a reconocernos unos a otros y nos hundimos en el manglar de la parranda.</strong> Los recién casados aparecieron poco después en el automóvil descubierto, abriéndose paso a duras penas en el tumulto. Bayardo San Román reventó cohetes,
          tomó aguardiente de las botellas que le tendía la muchedumbre, y se bajó del coche con Ángela Vicario para meterse en la rueda de la cumbiamba.
          Por último, ordenó que siguiéramos bailando por cuenta suya hasta donde nos alcanzara la vida, y se llevó a la esposa aterrorizada para la casa de sus sueños donde el viudo de Xius había sido feliz.</p>
        <p>La parranda pública se dispersó en fragmentos hacia la media noche, y sólo quedó abierto el negocio de Clotilde Armenta a un costado de la plaza. Santiago Nasar y yo, con mi hermano Luis Enrique y Cristo Bedoya, nos fuimos para la casa de misericordias de
          María Alejandrina Cervantes. Por allí pasaron entre muchos otros los hermanos Vicario, y estuvieron bebiendo con nosotros y cantando con Santiago Nasar cinco horas antes de matarlo. Debían quedar aún algunos rescoldos desperdigados de la fiesta original,
          pues de todos lados nos llegaban ráfagas de música. y pleitos remotos, y nos siguieron llegando, cada vez más tristes, hasta muy poco antes de que bramara el buque del obispo.</p>
        <p>Pura Vicario le contó a mi madre que se había acostado a las once de la noche después de que las hijas mayores la ayudaron a poner un poco de orden en los estragos de la boda. Como a las diez, cuando todavía quedaban algunos borrachos cantando en el patio,
          Ángela Vicario había mandado a pedir una maletita de cosas personales que estaba en el ropero de su dormitorio, y ella quiso mandarle también una maleta con ropa de diario, pero el recadero estaba de prisa. Se había dormido a fondo cuando tocaron a la puerta.
          «Fueron tres toques muy despacio -le contó a mi madre-, pero tenían esa cosa rara de las malas noticias.» Le contó que había abierto la puerta sin encender la luz para no despertar a nadie, y vio a Bayardo San Román en el resplandor del farol público, con la camisa de seda sin abotonar
          y los pantalones de fantasía sostenidos con tirantes elásticos. «Tenía ese color verde de los sueños», le dijo Pura Vicario a mi madre. Ángela Vicario estaba en la sombra, de modo que sólo la vio cuando Bayardo San Román la agarró por el brazo y la puso en la luz. Llevaba el traje de raso en piltrafas y
          estaba envuelta con una toalla hasta la cintura. Pura Vicario creyó que se habían desbarrancado con el automóvil y estaban muertos en el fondo del precipicio.</p>
      </div>
      <div style="font-size: small; text-align: right;">
        Márquez, G. Crónica de una muerte anunciada. Recuperado de http://biblio3.url.edu.gt/Libros/cromuerte.pdf
      </div>
    </v-col>
    <v-footer absolute class="mt-6" color="#ffffff">
      <v-btn  block to="preguntasNext">Contestar Preguntas</v-btn>
    </v-footer>
  </v-row>
</template>
<style>
  .imagenPregunta img{
    max-width: 75vw;
  }
  .imagenPregunta div{
    display: flex;
    justify-content: center;
  }
  .fichaDomino {
    display: flex;
    justify-content: center;
  }

  .fichaDomino table {
    border-spacing: 0;
  }

  .fichaDomino p {
    margin-bottom: -6px !important
  }

  .fichaDomino .parteTop {
    border-style: solid;
    border-top-right-radius: 30px;
    width: 120px;
    text-align: center;
    border-top-left-radius: 30px;
    border-spacing: 0;
  }

  .fichaDomino .parteBottom {
    border-style: solid;
    border-top-style: none;
    border-bottom-right-radius: 30px;
    width: 120px;
    text-align: center;
    border-bottom-left-radius: 30px;
    border-spacing: 0;
  }

  .centroFicha {
    border-radius: 7.5px;
    border-style: solid;
    width: 15px;
    height: 15px;
    background-color: black;
    align-self: center;
    position: absolute;
  }

  .fichaDomino table {
    border-spacing: 0;
  }

  .flex3 {
    flex: 0 0 3%;
    max-width: 3%;
    padding-right: 0;
    margin-bottom: auto;
    margin-top: 0;
  }

  .flex5 {
    padding-top: 2px !important;
    flex: 0 0 5%;
    max-width: 5%;
  }

  .tg {
    border-collapse: collapse;
    border-spacing: 0;
  }

  .tg td {
    border-color: black;
    border-style: solid;
    border-width: 1px;
    overflow: hidden;
    padding: 10px 5px;
    word-break: normal;
  }

  .tg th {
    border-color: black;
    border-style: solid;
    border-width: 1px;
    overflow: hidden;
    padding: 10px 5px;
    word-break: normal;
  }

  .tg {
    border-color: inherit;
    text-align: center;
    vertical-align: top
  }
</style>
<script>
  import katex from "katex";
  import renderMathInElement from "katex/dist/contrib/auto-render.js";
  import "katex/dist/katex.min.css";

  export default {
    data() {
      return {

      };

    },
    methods: {
      ref() {
        renderMathInElement(document.body);
      }
    },
    mounted() {
      renderMathInElement(document.body);
      window.vm = this;
    },
  };
</script>
