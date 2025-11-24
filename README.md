Desde el fondo de mi corazón
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para África 🩵</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #87CEEB, #B6E6FF);
            color: #333;
            min-height: 100vh;
            line-height: 1.6;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 15px;
            text-align: center;
        }
        
        /* HEADER RESPONSIVE */
        .header {
            background: rgba(255, 255, 255, 0.95);
            padding: 25px 20px;
            border-radius: 15px;
            margin-bottom: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .main-title {
            font-size: clamp(1.8em, 5vw, 2.5em);
            color: #2c3e50;
            margin-bottom: 15px;
            word-wrap: break-word;
        }
        
        .personal-message {
            font-size: clamp(1em, 3vw, 1.3em);
            line-height: 1.6;
            margin-bottom: 20px;
            color: #2c3e50;
            padding: 0 10px;
        }
        
        /* CONTADOR RESPONSIVE */
        .counter-container {
            background: rgba(255, 255, 255, 0.9);
            padding: 20px 15px;
            border-radius: 12px;
            margin: 20px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .counter-title {
            font-size: clamp(1.4em, 4vw, 1.8em);
            color: #2c3e50;
            margin-bottom: 8px;
        }
        
        .counter-subtitle {
            font-size: clamp(0.9em, 2.5vw, 1.1em);
            color: #7f8c8d;
            margin-bottom: 15px;
            font-style: italic;
            padding: 0 10px;
        }
        
        .time-counter {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin: 15px 0;
        }
        
        @media (min-width: 768px) {
            .time-counter {
                grid-template-columns: repeat(4, 1fr);
                gap: 15px;
            }
        }
        
        .time-unit {
            background: linear-gradient(135deg, #4FC3F7, #81D4FA);
            color: white;
            padding: 15px 10px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(79, 195, 247, 0.3);
        }
        
        .time-number {
            font-size: clamp(1.8em, 6vw, 2.5em);
            font-weight: bold;
            display: block;
        }
        
        .time-label {
            font-size: clamp(0.8em, 2vw, 0.9em);
            opacity: 0.9;
        }
        
        .anniversary-date {
            background: #E3F2FD;
            padding: 12px;
            border-radius: 8px;
            margin: 12px 0;
            border: 2px dashed #4FC3F7;
            font-size: clamp(0.9em, 2.5vw, 1.1em);
        }
        
        /* MENSAJES RESPONSIVE */
        .messages-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 12px;
            margin: 20px 0;
        }
        
        @media (min-width: 600px) {
            .messages-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 15px;
            }
        }
        
        .message-card {
            background: white;
            padding: 18px;
            border-radius: 8px;
            border-left: 4px solid #4FC3F7;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            text-align: left;
            font-size: clamp(0.9em, 2.5vw, 1em);
        }
        
        /* RAZONES RESPONSIVE */
        .reasons-section {
            background: white;
            padding: 25px 20px;
            border-radius: 12px;
            margin: 25px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .reasons-list {
            text-align: left;
            display: inline-block;
            margin-top: 15px;
            width: 100%;
        }
        
        .reasons-list li {
            margin: 8px 0;
            font-size: clamp(0.9em, 2.5vw, 1.1em);
            line-height: 1.5;
            padding: 5px 0;
        }
        
        .heart {
            color: #4FC3F7;
            font-size: clamp(1em, 2.5vw, 1.2em);
            margin: 0 5px;
        }
        
        /* NUBE DE PALABRAS RESPONSIVE */
        .wordcloud-section {
            background: white;
            padding: 25px 20px;
            border-radius: 12px;
            margin: 25px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .wordcloud {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
            min-height: 150px;
            align-items: center;
        }
        
        .word {
            padding: 6px 12px;
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
            background: #E3F2FD;
            border: 2px solid #4FC3F7;
            font-size: clamp(0.8em, 2.5vw, 1em);
        }
        
        .word:hover {
            transform: scale(1.1);
            background: #4FC3F7;
            color: white;
        }
        
        .word-size-1 { font-size: clamp(0.8em, 2.5vw, 1em); }
        .word-size-2 { font-size: clamp(0.9em, 3vw, 1.2em); }
        .word-size-3 { font-size: clamp(1em, 3.5vw, 1.4em); }
        .word-size-4 { font-size: clamp(1.1em, 4vw, 1.6em); }
        .word-size-5 { font-size: clamp(1.2em, 4.5vw, 1.8em); }
        
        /* MENSAJES SECRETOS RESPONSIVE */
        .secret-section {
            background: white;
            padding: 25px 20px;
            border-radius: 12px;
            margin: 25px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        .secret-container {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            margin: 20px 0;
        }
        
        @media (min-width: 768px) {
            .secret-container {
                grid-template-columns: repeat(3, 1fr);
                gap: 15px;
            }
        }
        
        .secret-box {
            background: linear-gradient(135deg, #E3F2FD, #B3E5FC);
            padding: 20px 10px;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            border: 2px solid #81D4FA;
            position: relative;
            overflow: hidden;
            min-height: 80px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .secret-box:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(79, 195, 247, 0.3);
        }
        
        .secret-question {
            font-size: clamp(1.5em, 4vw, 2em);
            margin-bottom: 8px;
        }
        
        .secret-message {
            font-size: clamp(0.8em, 2vw, 0.9em);
            opacity: 0;
            max-height: 0;
            transition: all 0.5s ease;
            color: #1565C0;
            font-weight: 500;
            text-align: center;
            padding: 0 5px;
        }
        
        .secret-box.active .secret-message {
            opacity: 1;
            max-height: 80px;
            margin-top: 8px;
        }
        
        .secret-box.active {
            background: linear-gradient(135deg, #B3E5FC, #81D4FA);
        }

        /* CARTA DE AMOR RESPONSIVE */
        .letter-section {
            background: white;
            padding: 25px 20px;
            border-radius: 12px;
            margin: 25px 0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            position: relative;
        }
        
        .letter-envelope {
            background: linear-gradient(135deg, #E3F2FD, #B3E5FC);
            padding: 20px 15px;
            border-radius: 8px;
            border: 2px solid #4FC3F7;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .letter-envelope:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(79, 195, 247, 0.4);
        }
        
        .letter-envelope h3 {
            margin: 0;
            color: #1565C0;
            font-size: clamp(1.2em, 3.5vw, 1.5em);
        }
        
        .letter-envelope p {
            margin: 8px 0 0 0;
            font-size: clamp(0.9em, 2.5vw, 1em);
        }
        
        .letter-content {
            max-height: 0;
            opacity: 0;
            overflow: hidden;
            transition: all 0.8s ease;
            text-align: left;
            line-height: 1.6;
            padding: 0 15px;
            background: #fafafa;
            border-radius: 8px;
            margin-top: 0;
        }
        
        .letter-content.open {
            max-height: 70vh;
            opacity: 1;
            padding: 20px 15px;
            margin-top: 15px;
            overflow-y: auto;
        }
        
        .letter-text {
            font-size: clamp(0.9em, 2.5vw, 1.1em);
            color: #333;
            white-space: pre-line;
        }
        
        .letter-signature {
            text-align: right;
            font-style: italic;
            margin-top: 15px;
            color: #4FC3F7;
            font-weight: bold;
            font-size: clamp(0.9em, 2.5vw, 1em);
        }
        
        /* TÍTULOS DE SECCIÓN RESPONSIVE */
        .section-title {
            font-size: clamp(1.5em, 4vw, 2em);
            color: #2c3e50;
            margin-bottom: 15px;
            padding: 0 10px;
        }
        
        /* CORAZONES FLOTANTES */
        .floating-hearts {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .floating-heart {
            position: absolute;
            font-size: clamp(16px, 4vw, 24px);
            opacity: 0.3;
            animation: float 6s infinite linear;
        }
        
        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
            }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        /* MEJORAS PARA TOCAR EN MÓVIL */
        @media (max-width: 480px) {
            .container {
                padding: 10px;
            }
            
            .header, .counter-container, .messages-section, 
            .reasons-section, .wordcloud-section, .secret-section, 
            .letter-section {
                padding: 20px 15px;
                margin: 15px 0;
            }
            
            .secret-box, .time-unit, .message-card {
                padding: 15px 8px;
            }
            
            /* Tamaños mínimos para botones táctiles */
            .secret-box, .letter-envelope {
                min-height: 60px;
            }
        }

        /* MEJORAS PARA TABLETS */
        @media (min-width: 769px) and (max-width: 1024px) {
            .container {
                max-width: 90%;
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Corazones flotantes de fondo -->
    <div class="floating-hearts" id="heartsContainer"></div>
    
    <div class="container">
        <!-- (Todo el contenido se mantiene igual que antes) -->
        <div class="header">
            <h1 class="main-title">Para África 🩵</h1>
            <div class="personal-message">
                Esto es para ti, así puedes ver siempre cuánto te amo y que eres lo mejor en mi vida.
            </div>
            
            <div class="counter-container">
                <h2 class="counter-title">Nuestro Tiempo Juntos</h2>
                <p class="counter-subtitle">Este tiempo llevas aguantándome y lo que te queda</p>
                
                <div class="anniversary-date">
                    <p>Desde aquel día especial: <strong>9 de Febrero</strong></p>
                </div>
                
                <div class="time-counter">
                    <div class="time-unit">
                        <span class="time-number" id="days">0</span>
                        <span class="time-label">Días</span>
                    </div>
                    <div class="time-unit">
                        <span class="time-number" id="hours">0</span>
                        <span class="time-label">Horas</span>
                    </div>
                    <div class="time-unit">
                        <span class="time-number" id="minutes">0</span>
                        <span class="time-label">Minutos</span>
                    </div>
                    <div class="time-unit">
                        <span class="time-number" id="seconds">0</span>
                        <span class="time-label">Segundos</span>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Resto de las secciones se mantienen igual -->
        <!-- ... -->
    </div>

    <script>
        // El JavaScript se mantiene igual
        // ... (todo el código JavaScript anterior)
    </script>
</body>
</html>
