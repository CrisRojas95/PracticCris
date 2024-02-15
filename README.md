# PracticCris
Practicas individuales
<!DOCTYPE html>
<html> 
    <head>
        <meta charset="utf-8"/>
        <title> Piedra, papel o Tijera</title>
        <script> 
            function aleatorio(min, max){ // accion que se establece y se puede usar en varias variables
                
                return Math.floor(Math.random() * (max - min + 1) + min)
            }
            // 1 es piedra, 2 es papel, 3 es tijera
            let jugador = 0
            let pc = aleatorio(1,3)

            jugador = prompt("Elije: 1 para piedra, 2 para papel y 3 para tijera")
            //alert("Elegiste " + jugador)
            if(jugador == 1){
                alert("Elegiste 🪨🪨🪨")
            } else  if (jugador ==2) {
                alert("Elegiste 🧻🧻🧻")
            } else if (jugador == 3) {
                alert("Elegiste ✂️✂️✂️")
            } else {
                alert("Elegiste perder!!!!")
            }
            if(pc == 1){
                alert("Pc elige 🪨🪨🪨")
            } else  if (pc ==2) {
                alert("Pc elige 🧻🧻🧻")
            } else if (pc == 3) {
                alert("Pc elige ✂️✂️✂️")
            }

            /// combate, codigo de gestion 

            if(pc == jugador){
                alert("Empate")  //&& = dos cosas se comparen al tiempo
            }else if (jugador == 1 && pc == 3) {
                alert("Ganaste!!!")
            }else if (jugador == 2 && pc == 1){
                alert("Ganaste!!!")
            }else if (jugador == 3 && pc == 2){
                alert("Ganaste!!!")
            }else{
                alert("perdiste:c")
            }
        




        </script>

    </head>
   <body>
        <h1>Piedra, Papel o Tijera</h1>
    </body>

</html>
