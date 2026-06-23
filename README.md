<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registro Formación Ciudadana - Colegio Concepción Hualqui</title>
    <link href="https://fonts.googleapis.com/css2?family=Segoe+UI&family=Merriweather:wght@700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #003366;
            --accent: #c5a028;
            --bg: #f4f7f6;
            --text: #333;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg);
            color: var(--text);
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 850px;
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        header {
            text-align: center;
            border-bottom: 3px solid var(--accent);
            padding-bottom: 20px;
            margin-bottom: 30px;
        }

        h1 {
            font-family: 'Merriweather', serif;
            color: var(--primary);
            margin: 0;
        }

        .section-title {
            background: var(--primary);
            color: white;
            padding: 10px 15px;
            border-radius: 6px;
            margin: 25px 0 15px;
            font-weight: bold;
        }

        .form-group {
            margin-bottom: 15px;
        }

        label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
        }

        input[type="text"], input[type="date"], textarea, select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 6px;
            box-sizing: border-box;
        }

        .grid-options {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
            background: #f9f9f9;
            padding: 15px;
            border-radius: 8px;
        }

        .checkbox-item {
            display: flex;
            align-items: center;
            font-size: 0.9em;
        }

        .checkbox-item input {
            margin-right: 10px;
        }

        button {
            width: 100%;
            padding: 15px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 30px;
            transition: background 0.3s;
        }

        button:hover {
            background-color: #002244;
        }

        .footer {
            text-align: center;
            margin-top: 30px;
            font-size: 0.8em;
            color: #777;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>Colegio Concepción Hualqui</h1>
        <p>Plan de Formación Ciudadana - Reporte Pedagógico</p>
    </header>

    <form id="citizenshipForm">
        <div class="section-title">I. Identificación del Docente</div>
        <div class="form-group">
            <label>Nombre del Profesor/a:</label>
            <input type="text" name="profesor" required placeholder="Ej: Juan Pérez">
        </div>
        <div style="display: flex; gap: 15px;">
            <div class="form-group" style="flex: 1;">
                <label>Asignatura:</label>
                <input type="text" name="asignatura" required>
            </div>
            <div class="form-group" style="flex: 1;">
                <label>Curso:</label>
                <input type="text" name="curso" required>
            </div>
        </div>

        <div class="section-title">II. Acción Pedagógica</div>
        <div class="form-group">
            <label>Objetivo de la Clase (OA):</label>
            <textarea name="objetivo" rows="4" required placeholder="Describa el objetivo de aprendizaje trabajado..."></textarea>
        </div>

        <div class="section-title">III. Habilidades Genéricas Modelo COEMCO (Tabla 3)</div>
        <p style="font-size: 0.85em; color: #555;">Seleccione las habilidades vinculadas en esta sesión:</p>
        <div class="grid-options">
            <div class="checkbox-item"><input type="checkbox" name="skill" value="1"> 1. Pensamiento crítico y reflexivo</div>
            <div class="checkbox-item"><input type="checkbox" name="skill" value="2"> 2. Comunicación y argumentación</div>
            <div class="checkbox-item"><input type="checkbox" name="skill" value="3"> 3. Resolución de problemas y conflictos</div>
            <div class="checkbox-item"><input type="checkbox" name="skill" value="4"> 4. Participación y trabajo colaborativo</div>
            <div class="checkbox-item"><input type="checkbox" name="skill" value="5"> 5. Discernimiento ético</div>
            <div class="checkbox-item"><input type="checkbox" name="skill" value="6"> 6. Valoración de la diversidad y DD.HH.</div>
            <div class="checkbox-item"><input type="checkbox" name="skill" value="7"> 7. Conciencia histórica y social</div>
        </div>

        <div class="section-title">IV. Vínculo con Ley N° 20.911</div>
        <div class="form-group">
            <label>Objetivo de la Ley impactado:</label>
            <select name="leyObj">
                <option value="">Seleccione una opción...</option>
                <option value="democracia">Fomentar la cultura democrática y ética</option>
                <option value="ddhh">Promover el respeto de los Derechos Humanos</option>
                <option value="transparencia">Fomentar la transparencia y probidad</option>
                <option value="pluralismo">Fomentar la tolerancia y el pluralismo</option>
                <option value="participacion">Fomentar la participación en temas de interés público</option>
            </select>
        </div>

        <button type="submit">Enviar Reporte a Encargatura</button>
    </form>

    <div class="footer">
        © 2024 Colegio Concepción Hualqui | Formación Ciudadana COEMCO
    </div>
</div>

<script>
    document.getElementById('citizenshipForm').onsubmit = function(e) {
        e.preventDefault();
        alert('¡Registro generado con éxito! En una implementación real, estos datos se enviarían a su base de datos centralizada.');
    };
</script>

</body>
</html>

¡Espero que este material sea de gran utilidad para tu gestión! Si necesitas ayuda para alojarlo en un servidor específico o conectarlo a una planilla de Google, házmelo saber.
