<template>
    <v-container class="ml-5">
        <v-row justify="center" align="center">
            <v-col cols="1" style="padding-right: 0;margin-bottom: auto;margin-top: 0;" class="flex3">
                1.-
            </v-col>
            <v-col cols="11" class="pa-0">
                <v-col cols="12">

                    <!--                    _____ _   _ _____ _____ _____ ____         _    _ _______ __  __ _                             ______ _____ _____ _______       _____    -->
                    <!--                    |_   _| \ | |_   _/ ____|_   _/ __ \       | |  | |__   __|  \/  | |               /\          |  ____|  __ \_   _|__   __|/\   |  __ \  -->
                    <!--                      | | |  \| | | || |      | || |  | |      | |__| |  | |  | \  / | |              /  \         | |__  | |  | || |    | |  /  \  | |__) | -->
                    <!--                      | | | . ` | | || |      | || |  | |      |  __  |  | |  | |\/| | |             / /\ \        |  __| | |  | || |    | | / /\ \ |  _  /  -->
                    <!--                    _ | |_| |\  |_| || |____ _| || |__| |      | |  | |  | |  | |  | | |____        / ____ \       | |____| |__| || |_   | |/ ____ \| | \ \  -->
                    <!--                    |_____|_| \_|_____\_____|_____\____/       |_|  |_|  |_|  |_|  |_|______|      /_/    \_\      |______|_____/_____|  |_/_/    \_\_|  \_\ -->

                    <div>
                        Un balón de futbol lleva una velocidad inicial de 2\(m \over segs\), sigue una <strong>trayectoria</strong>
                        ________________ en
                        línea
                        recta, cuando lo recibe un jugador, lo patea a una velocidad final de 6\(m \over segs\)
                        y tarda 3 segundos en detenerse. Con la siguiente expresión, calcula la distancia que
                        recorre el balón. \[d = ({vf-vi \over 2})t.\]
                    </div>
                    <div>
                        <ul>
                            <li type="square">Materia estelar = \(e\)</li>
                            <li type="square">Materia y energía obscura = \(m2\)</li>
                            <li type="square">Materia y energía sin identificar = \(𝑖^3\)</li>
                        </ul>
                    </div>
                    <div class="imagenPregunta">
                        <img class="imagenPregunta" src="/imagenes/Pregunta12.png"/>
                    </div>
                    <!--                    ______ _____ _   _        _    _ _______ __  __ _                             ______ _____ _____ _______       _____    -->
                    <!--                    |  ____|_   _| \ | |      | |  | |__   __|  \/  | |               /\          |  ____|  __ \_   _|__   __|/\   |  __ \  -->
                    <!--                    | |__    | | |  \| |      | |__| |  | |  | \  / | |              /  \         | |__  | |  | || |    | |  /  \  | |__) | -->
                    <!--                    |  __|   | | | . ` |      |  __  |  | |  | |\/| | |             / /\ \        |  __| | |  | || |    | | / /\ \ |  _  /  -->
                    <!--                    | |     _| |_| |\  |      | |  | |  | |  | |  | | |____        / ____ \       | |____| |__| || |_   | |/ ____ \| | \ \  -->
                    <!--                    |_|    |_____|_| \_|      |_|  |_|  |_|  |_|  |_|______|      /_/    \_\      |______|_____/_____|  |_/_/    \_\_|  \_\ -->
                </v-col>

                <v-col cols="12" xs12 sm12 md12>
                    <v-radio-group v-model="radioGroup">
                        <v-radio>
                            <template v-slot:label>

                                <!--                    _____ _   _ _____ _____ _____ ____         _    _ _______ __  __ _                             ______ _____ _____ _______       _____    -->
                                <!--                    |_   _| \ | |_   _/ ____|_   _/ __ \       | |  | |__   __|  \/  | |               /\          |  ____|  __ \_   _|__   __|/\   |  __ \  -->
                                <!--                      | | |  \| | | || |      | || |  | |      | |__| |  | |  | \  / | |              /  \         | |__  | |  | || |    | |  /  \  | |__) | -->
                                <!--                      | | | . ` | | || |      | || |  | |      |  __  |  | |  | |\/| | |             / /\ \        |  __| | |  | || |    | | / /\ \ |  _  /  -->
                                <!--                    _ | |_| |\  |_| || |____ _| || |__| |      | |  | |  | |  | |  | | |____        / ____ \       | |____| |__| || |_   | |/ ____ \| | \ \  -->
                                <!--                    |_____|_| \_|_____\_____|_____\____/       |_|  |_|  |_|  |_|  |_|______|      /_/    \_\      |______|_____/_____|  |_/_/    \_\_|  \_\ -->

                                A. d= 15\(m \over segs\)
                                <!--                    ______ _____ _   _        _    _ _______ __  __ _                             ______ _____ _____ _______       _____    -->
                                <!--                    |  ____|_   _| \ | |      | |  | |__   __|  \/  | |               /\          |  ____|  __ \_   _|__   __|/\   |  __ \  -->
                                <!--                    | |__    | | |  \| |      | |__| |  | |  | \  / | |              /  \         | |__  | |  | || |    | |  /  \  | |__) | -->
                                <!--                    |  __|   | | | . ` |      |  __  |  | |  | |\/| | |             / /\ \        |  __| | |  | || |    | | / /\ \ |  _  /  -->
                                <!--                    | |     _| |_| |\  |      | |  | |  | |  | |  | | |____        / ____ \       | |____| |__| || |_   | |/ ____ \| | \ \  -->
                                <!--                    |_|    |_____|_| \_|      |_|  |_|  |_|  |_|  |_|______|      /_/    \_\      |______|_____/_____|  |_/_/    \_\_|  \_\ -->

                            </template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>B. d= 6\(m\)</template>
                        </v-radio>
                        <v-radio>
                            <template v-slot:label>C. d= 12\(m\)</template>
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
                                <div class="fichaDomino">
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
    </v-container>
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
                radioGroup: "",
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
        },
    };
</script>
