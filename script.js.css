const grid = document.getElementById("videoGrid");


// Cargar videos

videos.forEach(video => {


    const card = document.createElement("div");

    card.className = "card";


    card.onclick = function(){

        abrirVideo(video.id);

    };



    card.innerHTML = `

    <img src="https://img.youtube.com/vi/${video.id}/hqdefault.jpg">

    <h3>${video.titulo}</h3>

    `;



    grid.appendChild(card);


});





// Abrir video


function abrirVideo(id){


    const player =
    document.getElementById("player");


    const frame =
    document.getElementById("videoFrame");



    frame.src =
    "https://www.youtube.com/embed/"
    + id
    + "?autoplay=1";



    player.style.display="flex";


}





// Cerrar video


function cerrarVideo(){


    const player =
    document.getElementById("player");


    const frame =
    document.getElementById("videoFrame");



    frame.src="";


    player.style.display="none";


}





// Botón explorar


function scrollVideos(){


    document.getElementById("videos")
    .scrollIntoView({

        behavior:"smooth"

    });


}





// Compartir página


function compartirPagina(){


    if(navigator.share){


        navigator.share({

            title:"Atlas Secretos",

            text:"Descubrí los misterios de Misiones en Atlas Secretos",

            url:window.location.href

        });


    }else{


        alert(
        "Compartí este enlace:\n"
        + window.location.href
        );


    }


}





// Contador básico


let visitas =
localStorage.getItem("atlasVisitas");


if(!visitas){

    visitas=1;

}else{

    visitas++;

}



localStorage.setItem(
"atlasVisitas",
visitas
);



document.getElementById("contador").innerHTML =
"👁️ "
+ visitas
+ " visitas";

