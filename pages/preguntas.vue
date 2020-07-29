<template>
    <v-container class="ml-5">
        <v-row justify="center" align="center">
            <v-col cols="1" style="padding-right: 0;margin-bottom: auto;margin-top: 0;" class="flex3">
                1.-
            </v-col>
            <v-col cols="11" class="pa-0">
                <v-col cols="12">
                    <div>
                        Un balón de futbol lleva una velocidad inicial de 2\(m \over segs\), sigue una trayectoria en
                        línea
                        recta, cuando lo recibe un jugador, lo patea a una velocidad final de 6\(m \over segs\)
                        y tarda 3 segundos en detenerse. Con la siguiente expresión, calcula la distancia que
                        recorre el balón. \[d = ({vf-vi \over 2})t.\]
                    </div>
                    <div style="display: flex;justify-content: center;">
                        <img src="http://localhost:3000/mapa.jpeg"/>
                    </div>

                    <div>
                        <div  class="fichaDomino">
                            <table>
                                <tbody>
                                <tr style="height: 100px;">
                                    <td class="parteTop">\(2a^2+2ab–b^2\)
                                    </td>
                                </tr>
                                <tr style="height: 100px;">
                                    <td class="parteBottom"></td>
                                </tr>
                                </tbody>
                            </table>
                            <div class="centroFicha">
                            </div>
                        </div>
                    </div>
                </v-col>

                <v-col cols="12" xs12 sm12 md12>
                    <v-radio-group v-model="radioGroup">
                        <v-radio>
                            <template v-slot:label>B. d= 6\(m\)</template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>C. d= 12\(m\)</template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>D. d= 12\(m \over segs\)</template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>
                                D. \(\begin{pmatrix}
                                a & b \\
                                c & d
                                \end{pmatrix}\)
                            </template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>
                                <div  class="fichaDomino">
                                    <table>
                                        <tbody>
                                        <tr style="height: 90px;">
                                            <td class="parteTop">\(2a^2+2ab–b^2\)
                                            </td>
                                        </tr>
                                        <tr style="height: 90px;">
                                            <td class="parteBottom"></td>
                                        </tr>
                                        </tbody>
                                    </table>
                                    <div class="centroFicha">
                                    </div>
                                </div>
                            </template>
                        </v-radio>
                    </v-radio-group>
                </v-col>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col cols="1" style="padding-right: 0;margin-bottom: auto;margin-top: 0;flex: 0 0 3%;max-width: 3%;">
                2.-
            </v-col>
            <v-col cols="11" class="pa-0">
                <v-col cols="12" xs12 sm12 md12>
                    <div>
                        Luis trabaja en una bodega donde se vende arroz. Por la mañana, le surten 1 750 kg y
                        durante el día tiene las siguientes ventas.
                    </div>
                    <div style="display: flex;justify-content: center;">
                        <table class="tg">
                            <thead>
                            <tr>
                                <th class="tg">Ventas</th>
                                <th class="tg">Kilogramos</th>
                            </tr>
                            </thead>
                            <tbody>
                            <tr>
                                <td class="tg">1</td>
                                <td class="tg">270</td>
                            </tr>
                            <tr>
                                <td class="tg">2</td>
                                <td class="tg">30</td>
                            </tr>
                            <tr>
                                <td class="tg">3</td>
                                <td class="tg">87</td>
                            </tr>
                            <tr>
                                <td class="tg">4</td>
                                <td class="tg">105</td>
                            </tr>
                            <tr>
                                <td class="tg">5</td>
                                <td class="tg">9</td>
                            </tr>
                            <tr>
                                <td class="tg">6</td>
                                <td class="tg">347</td>
                            </tr>
                            <tr>
                                <td class="tg">7</td>
                                <td class="tg">175</td>
                            </tr>
                            </tbody>
                        </table>
                    </div>

                </v-col>
                <v-col cols="12 py-0" xs12 sm12 md12>

                </v-col>
                <v-col cols="12 py-0" xs12 sm12 md12>
                    <v-radio-group v-model="radioGroup">
                        <v-radio>
                            <template v-slot:label>
                                <v-row align="start"
                                       justify="center">
                                    <v-col cols="1" class=" flex5">A.</v-col>
                                    <v-col cols="11" class="pa-0">
                                        <table>
                                            <tbody>
                                            <tr>
                                                <td>
                                                    Vendió 1 021 kg
                                                </td>
                                            </tr>
                                            <tr>
                                                <td>
                                                    Sobró 729 kg
                                                </td>
                                            </tr>
                                            </tbody>
                                        </table>
                                    </v-col>
                                </v-row>
                            </template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>
                                <v-row align="start"
                                       justify="center">
                                    <v-col cols="1" class=" flex5">B.</v-col>
                                    <v-col cols="11" class="pa-0">
                                        <table>
                                            <tbody>
                                            <tr>
                                                <td>
                                                    Vendió 1 022 kg
                                                </td>
                                            </tr>
                                            <tr>
                                                <td>
                                                    Sobró 728 kg
                                                </td>
                                            </tr>
                                            </tbody>
                                        </table>
                                    </v-col>
                                </v-row>
                            </template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>
                                {{variableTabla}}
                            </template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>
                                <div v-html="variableTabla2"></div>
                            </template>
                        </v-radio>
                    </v-radio-group>
                </v-col>
            </v-col>
        </v-row>
    </v-container>
</template>
<style>
    .fichaDomino {
        display: flex;
        justify-content: center;
    }
    .fichaDomino table {
        border-spacing: 0;
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
    .clase_table {
        border-collapse: separate;
        border-spacing: 10;
        border: 1px solid black;
        border-radius: 15px;
        -moz-border-radius: 20px;
        padding: 2px;
    }

    .flex3 {
        flex: 0 0 3%;
        max-width: 3%;
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

    /*.tg td {*/
    /*    border-color: black;*/
    /*    border-style: solid;*/
    /*    border-width: 1px;*/
    /*    overflow: hidden;*/
    /*    padding: 10px 5px;*/
    /*    word-break: normal;*/
    /*}*/

    /*.tg th {*/
    /*    border-color: black;*/
    /*    border-style: solid;*/
    /*    border-width: 1px;*/
    /*    overflow: hidden;*/
    /*    padding: 10px 5px;*/
    /*    word-break: normal;*/
    /*}*/

    /*.tg {*/
    /*    border-color: inherit;*/
    /*    text-align: center;*/
    /*    vertical-align: top*/
    /*}*/
</style>
<script>
    import katex from "katex";
    import renderMathInElement from "katex/dist/contrib/auto-render.js";
    import "katex/dist/katex.min.css";

    export default {
        data() {
            return {
                radioGroup: "",
                variableTabla: `C. Vendió 1 021 kg y Sobró 729 kg`,
                variableTabla2: `C. Vendió 1 021 kg <br> <div style="padding-left: 20px;">Sobró 729 kg</div>`,
                variableMath: `D. d= 12\(m \over segs\)`,
                variableApi: ``,
                items: [
                    {
                        title: "COMPETENCIA MATEMÁTICA",
                        text: "0-35",
                        to: "matematicas",
                    },
                    {
                        title: "COMPETENCIA LECTORA",
                        text: "0-60",
                        to: "matematicas",
                    },
                    {
                        title: "COMPETENCIA EN CIENCIAS EXPERIMENTALES",
                        text: "0-60",
                        to: "matematicas",
                    },
                ],
                opcionC: '<label for="input-46" class="v-label theme--light" style="left:0px;right:auto;position:relative;"><div class="container pa-0 container--fluid"><div class="row align-start justify-center"><div class="flex5 col col-1">B.</div> <div class="pa-0 col col-11"><table><tbody><tr><td>\n' +
                    '                                                Vendió 1 022 kg\n' +
                    '                                            </td></tr> <tr><td>\n' +
                    '                                                Sobró 728 kg\n' +
                    '                                            </td></tr></tbody></table></div></div></div></label>'
            };

        },
        methods: {
            api() {
                this.$axios.get('http://127.0.0.1:8000/api/apiMath').then((response) => {
                    console.log(response.data)
                    this.variableApi = response.data
                    setTimeout(() => {
                        renderMathInElement(document.body);
                    }, 300);
                })
            },
            ref() {
                renderMathInElement(document.body);
            }
        },
        mounted() {
            renderMathInElement(document.body);
            window.vm = this;
            this.api()
        },
    };
</script>
