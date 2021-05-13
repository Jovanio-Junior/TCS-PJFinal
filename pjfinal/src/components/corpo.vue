<template>
    <div>
        <h1 class="titulo">Verificar disponibilidades</h1>
        <div class="subTitulo">
            <p class="nomeT">nome</p>
            <p class="sobrenomeT">sobrenome</p>
            <p class="CEPT">CEP</p>
            <p class="possuiNumeroT">Possui Nª</p>
            <p class="NumeroT">Numero</p>
            <p class="QuadraT">Quadra</p>
            <p class="LoteT">Lote</p>
            <p class="op" style="left: 187px; top: 220px;">sim</p>
            <p class="op" style="left: 247px; top: 220px;">não</p>
        </div>
        <div>
            <input type="text" v-model="usuario.nome" class="nome">
            <input type="text" v-model="usuario.sobrenome" class="sobrenome">
            <input type="text" v-model="usuario.CEP" class="CEP">
            <input type="radio" id="true"  value="true" 
            v-model="usuario.possuiNumero" class="pNumero" style="left: 194px; top: 219px;">
            <input type="radio" id="false" value="false" 
            v-model="usuario.possuiNumero" class="pNumero" style="left: 254px; top: 219px;">
            <input type="number" v-model="usuario.quadra" class="quadra">
            <input type="number" v-model="usuario.lote" class="lote">
        </div>
        <button @click.prevent="busca" class="Search">Procurar</button>
    </div>
</template>

<script>
export default {
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
.titulo {
    position: absolute;
    width: 450px;
    height: 44px;
    left: 59px;
    top: 27px;

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
.subTitulo .nomeT {
    position: absolute;
    width: 44px;
    height: 17px;
    left: 59px;
    top: 107px
}
.subTitulo .sobrenomeT{
    position: absolute;
    width: 82px;
    height: 17px;
    left: 284px;
    top: 107px;
}
.subTitulo .CEPT{
    position: absolute;
    width: 30px;
    height: 17px;
    left: 59px;
    top: 174px;
}
.subTitulo .possuiNumeroT{
    position: absolute;
    width: 107px;
    height: 17px;
    left: 177px;
    top: 174px;
}
.subTitulo .NumeroT{
    position: absolute;
    width: 58px;
    height: 17px;
    left: 313px;
    top: 174px;
}
.subTitulo .QuadraT{
    position: absolute;
    width: 53px;
    height: 17px;
    left: 59px;
    top: 244px;
}
.subTitulo .LoteT {
    position: absolute;
    width: 31px;
    height: 17px;
    left: 168px;
    top: 244px;
}
.subTitulo .op {
    position: absolute;
    width: 26px;
    height: 17px;
}
.nome {
    position: absolute;
    width: 177px;
    height: 34px;
    left: 59px;
    top: 148px;

    background: #FFFFFF;
    border: 1px solid #000000;
    box-sizing: border-box;
    border-radius: 3px;
}
.sobrenome {
    position: absolute;
    width: 177px;
    height: 34px;
    left: 284px;
    top: 148px;

    background: #FFFFFF;
    border: 1px solid #000000;
    box-sizing: border-box;
    border-radius: 3px;
}
.CEP {
    position: absolute;
    width: 95px;
    height: 31px;
    left: 59px;
    top: 215px;

    background: #FFFFFF;
    border: 1px solid #000000;
    box-sizing: border-box;
    border-radius: 3px;
}
.pNumero {
    position: absolute;
width: 13px;
height: 13px;


background: #C4C4C4;
border: 1px solid #000000;
}
.quadra {
    /* Rectangle 9 */
    position: absolute;
    width: 68px;
    height: 31px;
    left: 59px;
    top: 290px;
    
    background: #FFFFFF;
    border: 1px solid #000000;
    box-sizing: border-box;
    border-radius: 3px;
}
.lote {
    /* Rectangle 10 */
    position: absolute;
    width: 68px;
    height: 31px;
    left: 168px;
    top: 290px;

    background: #FFFFFF;
    border: 1px solid #000000;
    box-sizing: border-box;
    border-radius: 3px;
}

.Search {
    position: absolute;
    width: 91px;
    height: 27px;
    left: 59px;
    top: 407px;

    background: #0596FF;
    mix-blend-mode: normal;
    border-radius: 6px;
    color: white;

    font-size: 1rem;
}
</style>