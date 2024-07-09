<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplicativo de Música</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .player-container {
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            text-align: center;
            width: 300px;
        }
        .album-cover {
            width: 100%;
            border-radius: 10px;
        }
        .controls {
            display: flex;
            justify-content: space-around;
            margin-top: 20px;
        }
        .control-button {
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 50%;
            width: 50px;
            height: 50px;
            font-size: 20px;
            cursor: pointer;
            box-shadow: 0 3px 5px rgba(0, 0, 0, 0.2);
            transition: background-color 0.3s;
        }
        .control-button:hover {
            background-color: #0056b3;
        }
        .song-info {
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <div class="player-container">
        <img src="album-cover.jpg" alt="Capa do Álbum" class="album-cover">
        <div class="song-info">
            <h3>Nome da Música</h3>
            <p>Artista</p>
        </div>
        <div class="controls">
            <button class="control-button">⏮</button>
            <button class="control-button">⏯</button>
            <button class="control-button">⏭</button>
        </div>
    </div>
    <script>
        // Adicione a funcionalidade do player aqui
        document.querySelector('.control-button:nth-child(1)').addEventListener('click', () => {
            console.log('Anterior');
        });
        document.querySelector('.control-button:nth-child(2)').addEventListener('click', () => {
            console.log('Play/Pause');
        });
        document.querySelector('.control-button:nth-child(3)').addEventListener('click', () => {
            console.log('Próxima');
        });
    </script>
</body>
</html>
