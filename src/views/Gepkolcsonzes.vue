<template>

  <div class="gepkolcsonzes">

    <h4>Gépkölcsönzés</h4>



    <div class="d-flex justify-content-center" style="overflow-x:auto;">

      <table class="m-5 " >

        <tbody >
        <tr v-for="item in machines" :key="item.id">
          <td class="p-5 ">
            <img :src="item.icon" class="img-responsive" :alt="gyalu" :style="{ height: item.height + 'px' }">
          </td>
          <td id="tablemid" style="width: 800px">
            <p class="p-1">
              <a :href="item.link">{{item.name}}</a>
            </p>
            <p id="description" >{{item.discription}}
            </p>
          </td>
          <td class="p-4">
            <table style="min-width: 160px" >
              <p id="title" class="p-1"><a href="acsgyalu.html">{{item.name}}</a></p>
              <tr class="mx-md-n5">
                <td class="m-4"> <p>1.nap  </p></td>
                <td class="m-2"> <p>   6.500Ft  </p></td>
              </tr>
              <tr class="mx-md-n5">
                <td class="m-4"><p> 6.naptól </p></td>
                <td class="m-2"><p>  6.100Ft   </p></td>
              </tr>
              <tr class="mx-md-n5">
                <td class="m-4"><p> 21.naptól </p></td>
                <td class="m-2"><p>    5.800Ft </p></td>
              </tr>
            </table>
          </td>
        </tr>
        </tbody>
      </table>
    </div>
  </div>

</template>



<script>
export default {
  data(){
    return{
      machines: [
        {
          id: 1,
          name: "Ácsgyalu",
          discription: "Teljesítmény: 1 200 W Teljes hossz: 525 mm Lökésszám: 15 000 / perc Gyalulási szélesség: 170 mm Vágásvastagság: 2 mm Méret (hossz x szélesség x magasság): 530 mm x 240 mm x 150 mm Súly: 9 kg",
          icon: require('../assets/machines/gyalu.png'),
          link: "gyalu",
          price1: 6500,
          price2: 6100,
          price3: 5800,
          height: 100
        },
        {
          id: 2,
          name: "Merülő körfűrész",
          discription: "Teljesítmény: 1 300 W Üresjárati fordulatszám: 2 000 – 5 800 / perc Tárcsaátmérő: 165 mm Vágás mélység 90°: 55 mm Vágás mélység 45°: 39 mm Kábelhossz: 2,5 m Méret (hossz x szélesség x magasság):341 mm x 225 mm x 250 mm Súly: 4,4 kg",
          icon: require('../assets/machines/korfuresz.jpg'),
          link: "korfuresz",
          price1: 6500,
          price2: 6100,
          price3: 5800,
          height: 120
        },
        {
          id: 3,
          name: "Vezetősín (körfűrészhez)",
          discription: "Alumínium anyag Könnyű, merev szerkezetű 1900 mm hosszúság Ezekhez a modellekhez: - Makita SP6000K - K1 és SP6000J - J1 modell",
          icon: require('../assets/machines/vezetosin.jpg'),
          link: "vezetosin",
          price1: 1000,
          price2: 1000,
          price3: 1000,
          height: 140
        },
        {
          id: 4,
          name: "Aprító- és szecskázógép",
          discription: "Típus: Benzines szecskázó Motor: HECHT OHV Motor: 389 cm3 Teljesítmény: 9,8 kW, 13Le Tömege: 105 kg Aprítható ágak max. átmérője: 5x5 cm Oldalsó bemenet nagysága: 130x88 mm Felső bemenet méretei: 240x230 mm",
          icon: require('../assets/machines/aprito.png'),
          link: "aprito",
          price1: 8000,
          price2: 7600,
          price3: 7200,
          height: 150
        },
        {
          id: 5,
          name: "Szőnyeg- és kárpittisztító",
          discription: "Max. felületteljesítmény: 20-25 m2/h Légmennyiség: 74 l/s Vákuum: 254mbar/25,4kPa Permetmennyiség: 1 l/min Permetnyomás: 1 bar Friss-/szennyezettvíz-tartály: 10-9 l Turbina teljesítménye: 1250 W Szivattyú teljesítménye: 40 W Feszültség: 220-240 V Frekvencia: 50-60 Hz Kábel hossza: 7,5 m Súly kiegészítők nélkül: 10,5 kg Méretek (hosszúság x szélesség x magasság): 690 mm x 325 mm x 440 mm",
          icon: require('../assets/machines/szonyegtisztito.png'),
          link: "szonyegtisztito",
          price1: 4000,
          price2: 3800,
          price3: 3500,
          height: 150
        }
      ]
    }
  }


}

</script>

<style >
#title{
  display: none;
}

@media screen and (max-width: 800px) {
  #tablemid{
    display: none;
  }
  #title{
    display: inline-table;
  }

}

</style>
