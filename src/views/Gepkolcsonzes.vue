<template>

  <div class="gepkolcsonzes">

    <h4>Gépkölcsönzés</h4>

    <div class="d-flex justify-content-center">

      <table class="m-5 ">

        <tbody >
        <tr>
          <td class="p-5 ">
            <img src="../assets/machines/gyalu.png" class="img-responsive" height="100"  alt="gyalu"/>
          </td>
          <td class="align-top ">
            <p class="p-1">
              <a href="acsgyalu.html">Ácsgyalu</a>
            </p>
            <p id="description" >
              Teljesítmény: 1 200 W
              Teljes hossz: 525 mm
              Lökésszám: 15 000 / perc
              Gyalulási szélesség: 170 mm
              Vágásvastagság: 2 mm
              Méret (hossz x szélesség x magasság): 530 mm x 240 mm x 150 mm
              Súly: 9 kg
            </p>
          </td>
          <td class="p-4">
            <table >
              <p class="p-1"><a href="acsgyalu.html">Ácsgyalú</a></p>
              <tr class="mx-md-n5">
                <td class="m-4"> <p>1 nap <br>6. naptól<br>21. naptól<br>  </p></td>
                <td class="m-2"> <p>   6.500 Ft <br> 6.100 Ft <br>   5.800 Ft <br>  </p></td>
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
      machine: [
        {
          id: 1,
          name: "Ácsgyalu",
          discription: "Teljesítmény: 1 200 W Teljes hossz: 525 mm Lökésszám: 15 000 / perc Gyalulási szélesség: 170 mm Vágásvastagság: 2 mm Méret (hossz x szélesség x magasság): 530 mm x 240 mm x 150 mm Súly: 9 kg",
          link: "",
          price1: 6500,
          price2: 6100,
          price3: 5800
        },
        {
          id: 2,
          name: "Merülő körfűrész",
          discription: "Teljesítmény: 1 200 W Teljes hossz: 525 mm Lökésszám: 15 000 / perc Gyalulási szélesség: 170 mm Vágásvastagság: 2 mm Méret (hossz x szélesség x magasság): 530 mm x 240 mm x 150 mm Súly: 9 kg",
          link: "",
          price1: 6500,
          price2: 6100,
          price3: 5800
        }
      ]
    }
  }


}

</script>

<style >

@media screen and (max-width: 800px) {
  #description{
    display: none;
  }
  .p{
    text-align: center;
  }

}

</style>
