# Taller 7
[Inicio](/README.md)
- [GEneración de texto](/gen-ai/Taller%207%20Generacion%20de%20Texto.ipynb)

Para la construccion de los codigos de Algoritmo Genetico se emplearon las siguientes librerias:

os: Permite realizar operaciones relacionadas con el sistema operativo, como el manejo de archivos y directorios.
getpass: Proporciona una forma segura de solicitar contraseñas o entradas sin que se muestren en pantalla.
transformers (de Hugging Face):
pipeline: Facilita la carga de modelos preentrenados para tareas de PLN (Procesamiento del Lenguaje Natural).
AutoModelForCausalLM: Carga un modelo de lenguaje causal, como GPT-Neo, optimizado para generación de texto.
AutoTokenizer: Carga el tokenizador adecuado para el modelo, necesario para convertir texto en tokens y viceversa.

Tomando como referencia las siguientes paginas para comprender mejor las librerias y adaptarlas al codigo deseado: 

- Hugging Face. Uso de modelos preentrenados. Recuperado de https://huggingface.co/docs/transformers/main_classes/pipelines

- Hugging Face. GPT-Neo 1.3B - Modelo de generación de texto. Recuperado de https://huggingface.co/EleutherAI/gpt-neo-1.3B

- DataCamp. Generación de texto con modelos de Hugging Face. Recuperado de https://www.datacamp.com/tutorial/text-generation-transformers