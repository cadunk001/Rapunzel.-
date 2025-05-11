<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para minha Rapunzel</title>
  <link href="https://fonts.googleapis.com/css2?family=Sacramento&family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background: #000;
      color: #fff;
      text-align: center;
      overflow-x: hidden;
      position: relative;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    /* Efeito de sobreposição roxa/lilás */
    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(135deg, rgba(138, 43, 226, 0.3), rgba(186, 85, 211, 0.2));
      z-index: -1;
      pointer-events: none;
    }
    header {
      padding: 40px 20px;
      position: relative;
      z-index: 1;
    }
    h1 {
      font-family: 'Sacramento', cursive;
      font-size: 4.5em;
      margin: 0;
      color: #fff;
      text-shadow: 2px 2px 6px rgba(0, 0, 0, 0.5);
    }
    p {
      font-size: 1.3em;
      margin: 10px auto;
      max-width: 700px;
      line-height: 1.6;
      color: #000;
      background: rgba(255, 255, 255, 0.9);
      padding: 10px 20px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    }
    .upload-section {
      margin: 30px auto;
      padding: 20px;
      background: rgba(255, 255, 255, 0.95);
      border-radius: 15px;
      max-width: 600px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
      position: relative;
      z-index: 1;
    }
    input[type="file"] {
      margin: 10px;
      padding: 10px;
      font-size: 1em;
      border: 2px solid #8a2be2;
      border-radius: 25px;
      background: #fff;
      color: #000;
      transition: border-color 0.3s;
    }
    input[type="file"]:focus {
      border-color: #ba55d3;
      outline: none;
    }
    button {
      padding: 12px 30px;
      font-size: 1.2em;
      font-family: 'Montserrat', sans-serif;
      background: linear-gradient(45deg, #8a2be2, #ba55d3);
      color: #fff;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
      z-index: 1;
    }
    button:hover {
      transform: scale(1.05);
      box-shadow: 0 6px 15px rgba(138, 43, 226, 0.5);
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
      max-width: 1200px;
      position: relative;
      z-index: 1;
    }
    .gallery img {
      max-width: 100%;
      border-radius: 10px;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .gallery img:hover {
      transform: scale(1.1);
      box-shadow: 0 8px 20px rgba(138, 43, 226, 0.5);
    }
    .proposal {
      margin: 40px auto;
      padding: 20px;
      background: rgba(255, 255, 255, 0.95);
      border-radius: 15px;
      max-width: 600px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
      position: relative;
      z-index: 1;
    }
    #proposal-text {
      display
