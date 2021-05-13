<template>
  <div class="index">
      <div class="topo">
          <div class="frame2 titulo">
              <p>Projeto Final</p>
          </div>
      </div>

      <div class="corpo">
          <div class="Verificacao">
              <corpo :usuario="usuario"/>
          </div>
      </div>
  </div>
</template>

<script>
import corpo from './corpo.vue'
export default {
    components: {
        corpo,
    },
    data() {
        return {
            usuario: [
                {
                    nome: '',
                    sobrenome: '',
                    CEP: '',
                    possuNumero: false,
                    numero: 0,
                    quadra: 1,
                    lote:1
                }
            ]
        }
    }
}
</script>

<style>
.topo {
    /* Barra Superior */
    position: absolute;
    width: 1440px;
    height: 125px;
    left: 0px;
    top: 0px;

    background: #EAEAEA;
    border-bottom: 1px solid black;
    
}
.topo .frame2 {
    position: absolute;
    width: 216px;
    height: 125px;
    left: 0px;
    top: 0px;

}
.topo .titulo {
    position: absolute;
    width: 101px;
    height: 44px;
    left: 58px;
    top: 40px;

    font-family: Montserrat;
    font-style: normal;
    font-weight: 500;
    font-size: 36px;
    line-height: 44px;
    /* identical to box height */

    display: flex;
    align-items: center;
    text-align: center;
    letter-spacing: -0.015em;

    color: #000000;
}

/** Corpo **/
.corpo {
    position: absolute;
    width: 1440px;
    height: 899px;
    left: 0px;
    top: 125px;
}
/* Rectangle 1 */


.Verificacao {
    position: absolute;
    width: 666px;
    height: 462px;
    left: 386px;
    top: 218px;

    border: 1px solid #000000;
    box-sizing: border-box;
}
</style>