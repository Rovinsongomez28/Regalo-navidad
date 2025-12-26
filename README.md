[Untitled-1.html](https://github.com/user-attachments/files/24347879/Untitled-1.html)
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>🎁 Regalo Navideño</title>
<style>
    body {
        margin: 0;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        background: black;
        font-family: Arial, sans-serif;
        overflow: hidden;
        color: white;
    }

    .regalo {
        font-size: 100px;
        cursor: pointer;
        animation: parpadeo 1s infinite;
    }

    .contenido {
        display: none;
        text-align: center;
        animation: aparecer 1s ease-in-out;
    }

    .corazon {
        font-size: 60px;
        animation: latido 1s infinite, colores 1s infinite;
    }

    h1 {
        animation: colores 1s infinite;
    }

    @keyframes parpadeo {
        0% { transform: scale(1); }
        50% { transform: scale(1.1); }
        100% { transform: scale(1); }
    }

    @keyframes latido {
        0% { transform: scale(1); }
        50% { transform: scale(1.3); }
        100% { transform: scale(1); }
    }

    @keyframes colores {
        0% { color: red; }
        33% { color: green; }
        66% { color: gold; }
        100% { color: red; }
    }

    @keyframes aparecer {
        from { opacity: 0; transform: scale(0.5); }
        to { opacity: 1; transform: scale(1); }
    }
</style>
</head>
<body>

<div class="regalo" id="regalo">
    🎁
    <p style="font-size:20px;">Haz clic para abrir</p>
</div>

<div class="contenido" id="contenido">
    <div class="corazon">❤️</div>
    <h1>🎄 FELIZ NAVIDAD 🎄</h1>
    <h2 id="nombre"> Milkiani❤️</h2>
</div>

<script>
    const regalo = document.getElementById("regalo");
    const contenido = document.getElementById("contenido");

    regalo.onclick = () => {
        regalo.style.display = "none";
        contenido.style.display = "block";
    }
</script>

</body>
</html>
