const productos = [
{
    nombre:"Playera Negra",
    precio:250,
    imagen:"https://via.placeholder.com/250"
},
{
    nombre:"Tenis",
    precio:900,
    imagen:"https://via.placeholder.com/250"
},
{
    nombre:"Mochila",
    precio:600,
    imagen:"https://via.placeholder.com/250"
}
];

const contenedor = document.getElementById("productos");

productos.forEach(producto=>{

contenedor.innerHTML += `
<div class="tarjeta">

<img src="${producto.imagen}">

<h2>${producto.nombre}</h2>

<p>$${producto.precio}</p>

<button>Comprar</button>

</div>
`;

});