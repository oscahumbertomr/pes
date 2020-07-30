<template>
    <v-container class="ml-5">
        <v-row justify="center" align="center" v-for="pregunta in preguntas">
            <v-col cols="1" class="flex3">
                {{pregunta.id}}.
            </v-col>
            <v-col cols="11" class="pa-0" >
                <v-col cols="12" v-html="pregunta.texto" class="pb-0"></v-col>
                <v-col cols="12" xs12 sm12 md12 class="py-0">
                    <v-radio-group v-model="radioGroup" :row="pregunta.direccion == 2 ? true : false">
                        <v-radio v-for="opcion in pregunta.opcionesRespuesta">
                            <template v-slot:label>
                                <div v-html="opcion.respuesta"></div>
                            </template>
                        </v-radio>
                    </v-radio-group>
                </v-col>
            </v-col>
        </v-row>
    </v-container>
</template>
<style>
    .imagenPregunta{
        display: flex;justify-content: center;
        max-width: 75vw;
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

    .centroFicha{
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

    .tg  {
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
                radioGroup: "",
                preguntas:[]
            };
        },
        methods: {
            api() {
                this.$axios.get('http://127.0.0.1:8000/api/apiMath').then((response) => {
                    console.log(response.data)
                    this.preguntas = response.data
                    setTimeout(() => {
                        renderMathInElement(document.body);
                    }, 300);
                })
            },
        },
        mounted() {
            renderMathInElement(document.body);
            window.vm = this;
            this.api()
        },
    };
</script>
