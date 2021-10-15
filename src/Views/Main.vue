<template>
  <div>
    <Select/>
    <!-- 
      <Header/> 
    -->
    <div class="main">
      <div class="box-container">
        <div class="rune-box">
          <h2>Runes</h2>
          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(0,0)" v-bind:style="{'background-color':calcSelectionColor(0,0)}">
              <span>El</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/el_rune.png">
              
            </div>
            <div class="box-item" v-on:click="updateRune(0,1)" v-bind:style="{'background-color':calcSelectionColor(0,1)}">
              <span>Eld</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/eld_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(0,2)" v-bind:style="{'background-color':calcSelectionColor(0,2)}">
              <span>Tir</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/tir_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(0,3)" v-bind:style="{'background-color':calcSelectionColor(0,3)}">
              <span>Nef</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/nef_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(0,4)" v-bind:style="{'background-color':calcSelectionColor(0,4)}">
              <span>Eth</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/eth_rune.png">
            </div>
          </div>

          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(1,0)" v-bind:style="{'background-color':calcSelectionColor(1,0)}">
              <span>Ith</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ith_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(1,1)" v-bind:style="{'background-color':calcSelectionColor(1,1)}">
              <span>Tal</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/tal_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(1,2)" v-bind:style="{'background-color':calcSelectionColor(1,2)}">
              <span>Ral</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ral_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(1,3)" v-bind:style="{'background-color':calcSelectionColor(1,3)}">
              <span>Ort</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ort_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(1,4)" v-bind:style="{'background-color':calcSelectionColor(1,4)}">
              <span>Thul</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/thul_rune.png">
            </div>
          </div>

          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(2,0)" v-bind:style="{'background-color':calcSelectionColor(2,0)}">
              <span>Amn</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/amn_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(2,1)" v-bind:style="{'background-color':calcSelectionColor(2,1)}">
              <span>Sol</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/sol_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(2,2)" v-bind:style="{'background-color':calcSelectionColor(2,2)}">
              <span>Shael</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/shael_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(2,3)" v-bind:style="{'background-color':calcSelectionColor(2,3)}">
              <span>Dol</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/dol_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(2,4)" v-bind:style="{'background-color':calcSelectionColor(2,4)}">
              <span>Hel</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/hel_rune.png">
            </div>
          </div>

          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(3,0)" v-bind:style="{'background-color':calcSelectionColor(3,0)}">
              <span>Io</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/io_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(3,1)" v-bind:style="{'background-color':calcSelectionColor(3,1)}">
              <span>Lum</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/lum_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(3,2)" v-bind:style="{'background-color':calcSelectionColor(3,2)}">
              <span>Ko</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ko_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(3,3)" v-bind:style="{'background-color':calcSelectionColor(3,3)}">
              <span>Fal</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/fal_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(3,4)" v-bind:style="{'background-color':calcSelectionColor(3,4)}">
              <span>Lem</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/lem_rune.png">
            </div>
          </div>

          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(4,0)" v-bind:style="{'background-color':calcSelectionColor(4,0)}">
              <span>Pul</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/pul_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(4,1)" v-bind:style="{'background-color':calcSelectionColor(4,1)}">
              <span>Um</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/um_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(4,2)" v-bind:style="{'background-color':calcSelectionColor(4,2)}">
              <span>Mal</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/mal_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(4,3)" v-bind:style="{'background-color':calcSelectionColor(4,3)}">
              <span>Ist</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ist_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(4,4)" v-bind:style="{'background-color':calcSelectionColor(4,4)}">
              <span>Gul</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/gul_rune.png">
            </div>
          </div>

          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(5,0)" v-bind:style="{'background-color':calcSelectionColor(5,0)}">
              <span>Vex</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/vex_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(5,1)" v-bind:style="{'background-color':calcSelectionColor(5,1)}">
              <span>Ohm</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ohm_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(5,2)" v-bind:style="{'background-color':calcSelectionColor(5,2)}">
              <span>Lo</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/lo_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(5,3)" v-bind:style="{'background-color':calcSelectionColor(5,3)}">
              <span>Sur</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/sur_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(5,4)" v-bind:style="{'background-color':calcSelectionColor(5,4)}">
              <span>Ber</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/ber_rune.png">
            </div>
          </div>

          <div class="box-row">
            <div class="box-item" v-on:click="updateRune(6,0)" v-bind:style="{'background-color':calcSelectionColor(6,0)}">
              <span>Jah</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/jah_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(6,1)" v-bind:style="{'background-color':calcSelectionColor(6,1)}">
              <span>Cham</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/cham_rune.png">
            </div>
            <div class="box-item" v-on:click="updateRune(6,2)" v-bind:style="{'background-color':calcSelectionColor(6,2)}">
              <span>Zod</span>
              <img class="icon" alt="Background" src="../assets/icons/runes/zod_rune.png">
            </div>

            <div class="box-item" v-on:click="resetRunes()">
              <span>Toggle</span>
              <img class="icon" alt="Background" src="../assets/icons/reset.png">
            </div>
            <div class="box-item" v-on:click="confirmRunes()">
              <span>Start</span>
              <img class="icon" alt="Background" src="../assets/icons/check.png">
            </div>


          </div>
        </div>

        <div class="runeword-box">
          <h2>Runewords</h2>
          <div class="item-frame" v-for="item in viableRunewords" :key="item.id">

            <div class="box-column left">
              <span class="i-name">{{item.name}}</span>
              <span class="i-runes">{{item.runename}}</span>
              <div class="box-column">
                <span class="i-bases" v-for="base in item.bases" :key="base.index">{{base}}</span>
              </div>
              <span class="i-clvl">Clvl: {{item.Clvl}}</span>
            </div>

            <div class="box-column right">
              <span class="i-stats" v-for="stat in item.Stats" :key="stat.index">{{stat}}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from '../components/Header.vue'
import Select from '../components/Select.vue'
import Runes from '../../public/json/runewordsByRank.json'

export default {
  name: 'Main',
  components: {
    Header,
    Select
  },
  created () {
    this.runewords = Runes
  },
  data () {
    return {
      runewords: Runes,
      selRune: [
        [false,false,false,false,false],
        [false,false,false,false,false],
        [false,false,false,false,false],
        [false,false,false,false,false],
        [false,false,false,false,false],
        [false,false,false,false,false],
        [false,false,false]
      ],
      viableRunewords: []
    }
  },
  methods: {
    updateRune(c,n){
      this.selRune[c][n] = !this.selRune[c][n]
    },
    calcSelectionColor(c,n){
      if(this.selRune[c][n]) return "#12750E"
      else return "#222"
    },

    resetRunes(){
        var s = this.selRune.every(function (e) {
          return e.reduce((partial_sum, a) => partial_sum + a,0) == 0
        })
        
      if(s) {
        this.selRune = [
          [true,true,true,true,true],
          [true,true,true,true,true],
          [true,true,true,true,true],
          [true,true,true,true,true],
          [true,true,true,true,true],
          [true,true,true,true,true],
          [true,true,true]
        ]
      } else {
        this.selRune = [
          [false,false,false,false,false],
          [false,false,false,false,false],
          [false,false,false,false,false],
          [false,false,false,false,false],
          [false,false,false,false,false],
          [false,false,false,false,false],
          [false,false,false]
        ]
      }
    },
    confirmRunes(){
      var r = []
      this.viableRunewords = []
      if(this.selRune[0][0]) {r.push("El")}
      if(this.selRune[0][1]) {r.push("Eld")}
      if(this.selRune[0][2]) {r.push("Tir")}
      if(this.selRune[0][3]) {r.push("Nef")}
      if(this.selRune[0][4]) {r.push("Eth")}

      if(this.selRune[1][0]) {r.push("Ith")}
      if(this.selRune[1][1]) {r.push("Tal")}
      if(this.selRune[1][2]) {r.push("Ral")}
      if(this.selRune[1][3]) {r.push("Ort")}
      if(this.selRune[1][4]) {r.push("Thul")}

      if(this.selRune[2][0]) {r.push("Amn")}
      if(this.selRune[2][1]) {r.push("Sol")}
      if(this.selRune[2][2]) {r.push("Shael")}
      if(this.selRune[2][3]) {r.push("Dol")}
      if(this.selRune[2][4]) {r.push("Hel")}

      if(this.selRune[3][0]) {r.push("Io")}
      if(this.selRune[3][1]) {r.push("Lum")}
      if(this.selRune[3][2]) {r.push("Ko")}
      if(this.selRune[3][3]) {r.push("Fal")}
      if(this.selRune[3][4]) {r.push("Lem")}

      if(this.selRune[4][0]) {r.push("Pul")}
      if(this.selRune[4][1]) {r.push("Um")}
      if(this.selRune[4][2]) {r.push("Mal")}
      if(this.selRune[4][3]) {r.push("Ist")}
      if(this.selRune[4][4]) {r.push("Gul")}

      if(this.selRune[5][0]) {r.push("Vex")}
      if(this.selRune[5][1]) {r.push("Ohm")}
      if(this.selRune[5][2]) {r.push("Lo")}
      if(this.selRune[5][3]) {r.push("Sur")}
      if(this.selRune[5][4]) {r.push("Ber")}
      
      if(this.selRune[6][0]) {r.push("Jah")}
      if(this.selRune[6][1]) {r.push("Cham")}
      if(this.selRune[6][2]) {r.push("Zod")}

      for(var i=0; i<this.runewords.length; i++){
        var t = this.runewords[i].runeword.every(function (element) {
          return r.includes(element);
        })
        if(t) this.viableRunewords.push(this.runewords[i])
      }

      console.log(this.viableRunewords.length + " hits...")
    }
  }
}
</script>

<style scoped>
.main {
  margin-top: 25px;
}
.box-container {
  width: 100%;
  display: flex;
  justify-content: center;
}

.rune-box {
  margin: 20px 20px 20px 30px;
  height: 565px;
  padding: 12px;
  background-color: #181818;
  border-radius: 10px;
  box-shadow: 0 0 6px rgb(0 0 0 / 45%);

  display: flex;
  flex-direction: column;

  position: sticky;
  top: 85px;
}
.box-row{
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.box-item {
  display: flex;
  flex-direction: column;
  background-color: #222;
  margin: 2px;
  padding: 3px;
  border-radius: 10px;
  cursor:pointer;
}
.box-item:hover {
  box-shadow: inset 0px 0px 0px 3px #2c3e50;
}

.runeword-box{
  margin: 20px 30px 20px 20px;
  min-height: 565px;
  height: fit-content;
  max-width: 800px;
  width: 70%;
  padding: 12px;
  background-color: #181818;
  border-radius: 10px;
  box-shadow: 0 0 6px rgb(0 0 0 / 45%);
}
.item-frame {
  width: 100%;
  height: fit-content;
  background-color: #222;
  border-radius: 10px;
  margin-top: 10px;
  padding: 8px 0;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.box-column {
  display: flex;
  flex-direction: column;
}



.icon {
  width: 50px;
  height: 50px;
  user-select: none;
}
span {
  color: #FFF;
  font-family: 'Roboto';
  margin: 0 0 -4px 0;
  user-select: none;
}
p {
  color: #FFF;
  font-family: 'Roboto', sans-serif;
}
h2 {
  color: #FFF;
  font-family: 'Roboto', sans-serif;
  margin: 5px 0;
}

.i-name {
  margin-top: 10px;
  font-size: 20pt;
  color: #057af0;
}
.i-runes {
  font-size: 12pt;
  color: #3B7F94;
}
.i-bases {
  font-size: 13pt;
  margin-top: 2px;
}
.i-clvl {
  font-size: 13pt;
  color: #3B7F94;
  margin-top: 2px;
}
.i-stats {
  font-size: 12pt;
  margin: 1px 0;
}


.left {
  display: flex;
  width: 40%;
}
.right{
  width: 60%;
  display: flex;
  justify-content: flex-end;
}
</style>
