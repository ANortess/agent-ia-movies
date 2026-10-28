# Proyecto final de IA generativa

Estado: estructura inicial, tema pendiente. El agente todavía no está implementado.

## Cómo empezar
1. Descomprimir el ZIP conservando la carpeta completa.
2. Abrir proyecto_asistente_experto.ipynb en Jupyter, VS Code o Google Colab.
3. Consultar TOP_3_DATASETS.md y elegir el tema.
4. Después descargaremos el dataset, seleccionaremos una muestra y la colocaremos en data/.
5. Completaremos las secciones del notebook en orden.

## Contenido
- proyecto_asistente_experto.ipynb: índice navegable, objetivos, tareas pendientes y lista de comprobación.
- data/: carpeta para los archivos del dataset, todavía sin datos.
- TOP_3_DATASETS.md: opciones y propuesta de alcance.

## Dominio elegido
Pendiente de elección. Registrar objetivo, usuarios, límites, fuente, versión y licencia.

## Entorno de trabajo: Python 3.11 + venv
- `.venv/`: entorno aislado donde se instalan las librerías.
- `.env`: configuración privada con tu clave de Gemini.
- `requirements.txt`: dependencias iniciales. No es un lockfile; las versiones exactas se fijarán después de comprobar el proyecto completo.

### Windows (terminal CMD)
py -3.11 -m venv .venv
.venv\Scripts\activate.bat
python -m pip install --upgrade pip
python -m pip install -r requirements.txt

### Clave y notebook
1. Obtén tu clave en https://aistudio.google.com/apikey .
2. Edita `.env` y completa `GEMINI_API_KEY=tu_clave_real`. No la envíes por el chat.
3. Deja los identificadores de modelos vacíos por ahora.
4. Abre el notebook y selecciona el kernel **Python (Proyecto IA)**. En VS Code también puedes seleccionar el intérprete de `.venv`.
5. Ejecuta la sección de entorno: solo comprueba paquetes y carga configuración; no llama a Gemini ni consume API.

Cuando implementemos los clientes, pasaremos `API_KEY` explícitamente con `api_key=API_KEY` para evitar ambigüedad entre variables de credenciales.

**Estado de verificación:** se ha comprobado la estructura y sintaxis de las celdas. La instalación completa de dependencias y la conexión con Gemini todavía no se han probado. Al implementar verificaremos compatibilidad, registraremos versiones y ejecutaremos `python -m pip check`.

## System prompt y justificación
Pendiente. Documentar rol, límites, idioma, uso de fuentes y respuesta cuando falte información.

## Pruebas y memoria
Pendiente. Guardar al menos cinco preguntas con sus respuestas reales y un seguimiento que demuestre memoria.

## Presentación
Obligatoria: 5–10 minutos con demo en vivo. Preparar después de completar el MVP.