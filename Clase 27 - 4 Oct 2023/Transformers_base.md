# Transformers

¿Qué son?: Son modelos post-deep learning diseñados para computación en paralelo o supercomputadores que pueden llevar a cabo una gran cantidad de tareas sin fine-tuning

También se llaman **modelos fundacionales (foundational models)** 

**OJO** no siempre estos modelos estan taylorizados y es necesario realizar procesos de ajuste. Esto lo digo porque no podemos pensar que son perfectos.

# Ecosistema de transformers

Estos modelos no fueron creados por la academia sino por la industria. e.g Google invento la arquitectura **transformer** lo cual permitio la creacion de Google BERT. Microsoft  después trabajo en conjunto con Open-AI para crear GPT-3

Estos modelos surgen como necesidad de procesar los petabytes que fluyen en los centros de las grandes tecnologicas

- **Arquitectura**: Industrial, procesamiento paralelo, lo veremos depsues
- **Data**: Zetabytes o mayor
- **Potencial computacional**: GPT-3 fue entrnado en 50 PetaFLOPS/segundo y Google tiene computadoras de hacer 80PataFLOPS/segundo. FLOPS = Floating Point Operations Per Second 
- **Prompt Engineering**: Prompt es el trigger fundamental para hacer que la maquina actue como deseamos

# Modelos fundacionales

Estos modelos tienen dos caracteristicas importantes

1. **Homogenizacion de alto nivel**: lo que permite que un modelo se pueda usar en diferentes tipos de tareas

2. **Emergencia de propiedades creativas**: que aparecen luego del entrenamiento de billones de parametros en supercomputadoras


**¿Nuevo Paradigma de AI?**

- Modelos fundacionales pueden hacer tareas de NLP, CV y mochas mas con un modelo
- Pueden realizar mas de una tarea
- Tareas clasicas de DL de forma suficiente
- Pueden hacer tareas de ML (LR,KNN; MDP)
- Sistemas expertos cuando son necesarios
- Codigo clasico para crear AI pipelines

# Programacion se esta convirtiendo en subdominio de NLP?

Codex (GPT-3 entrenado para convertir NLP en codigo fuente, fue entrnado en cerca de 54 millones de repos de Github Publicos) 

Esto ha traido a colación el tema de **Copilots**

**Github Copilot** esta disponible ahora en Microsoft. Si aprendes el **metalenguage de prompts** reduciras el tiempo de desarrollo en los años que sigan 

# Futuro de especialistas de AI

Prompt engineering será un skill requerido para este rol. Ahora bien **el futuro de esta profesion no está limitada a los transformers**

En mi caso personal he trabajado con modelos clásicos, IoT, DL, ML, entre otros. El rol del **AI specialist** será poder generar conexiones increibles entre bots, robots, servidores y otros dispositovs interconectados

El prompt engineering será in skill deseado pero no es lo único, saber matemáticas, estadística y arquitecturas de datos es fundamental.

# Historia de Transformers

- Principios siglo XX, Andreu Markow introdujo el concepto de valores aleatorios creados a partir de procesos estocasticos (MDP= Markov Deicion Process, Markov Chains, Markov processes)
- 1949 Claude Shannon publico **the Mathematical Theory of Communication**, esto permitio la definicion de encoder, transmisor, receptor y decodificador semántico. **El es el creador de la teoría de información**
- 1950 Alang turing publico **Computing MAchinery and Intelligence**. Además de que creo su máquina que fue capaz de decriptar mensajes alemanes en la segunda guerra mundial
- 1954 GeorgeTown-IBM experiment usaron computadoreas para traducir oraciones en ruso a inglés usando sistemas basados en reglas
- 1956 se introduce el término **AI** por John McCarthy 
- 1980, Yann LeCUn diseó lo que se conoció como **Convolutional Neural Network (CNN)** 
- 1982, John Hopfield introdujo el concepto de RNN conocidas como Hopfield netwroks. El estuvo inspirado en W.A Little quien escribió **The existence of persistent states in the brain in 1974** que trajo los fundamentos teóricos de los procesos de aprendizaje por decádas. Luego de esto aparecieron las LSTM
- 1990, Yann LeCun produjo LeNet-5 lo que introudjo el avance de muchos modelos CNN que conocemos hoy
- 2017, introducción del concepto de **Transformer** con el papar **Attention is all you need**

# Surgimiento de indutria Transformer 4.0 APIs

Hay muchos competidores Microsoft, Google, Amazon IBM entre otros. Estas tecnologicas tienen supercomputadoreas (que valen millones de dolares) junto con datos masivos para entrenar modelos transformer

Hoy en día una compañia pequeña puede acceder a estos modelos a través de la nube por medio de APIs, lo cual reduce el esfuerzo necesario para implementar soluciones. **No se necesita ser un ingeniero o tener un Ph.D para hacer eso**

**Ejemplo** para alguien que quiera usar la API de OpenAI solo tiene que hacer 4 pasos

1. Obtener una API key en pocos clicks
2. Importar OpenAI en un notebook en una línea
3. Entrar una tarea NLO que quieras hacer en un *prompt*
4. Recibirás una respuesta como *completion* en una cantidad de tokens **limitado**

Y eso esto todo!

**Miremos unos ejemplos sencillos**

1. OpenAI API
2. https://demo.allennlp.org/coreference-resolution

Resolvamos un problema de **Coreference** lo cual es basicamente implica encontrar la entidad a la que se refiere una palabra.

Introduzcamos algo como esto: *An user visited the AllenNLP website, tried a transformer model, and found it interesting*

En este caso la palabra **it** se puede referir a la website o al transformer model. En este caso el modelo BERT decidio conectar **it** con **a transformer model**

Hagamos otro ejemplo sencillo pero ahora sobre sentiment analysis:

https://demo.allennlp.org/sentiment-analysis/glove-sentiment-analysis

Introduzcamos un mensaje como **You are a bad person and you are not helping**

Seguramente si ponemos algo ambiguo **The part was break out but I will wait then men, no worries**


# Eligiendo un modelo Transformer

- HuggingFace
- OpenAI
- Google Vertex

Entre otros


# Algunas referencias
- Bommansani et al. 2021, On the Opportunities and Risks of Foundation Models, https://arxiv.org/abs/2108.07258
- Chen et al.,2021, Evaluating Large Language Models Trained on Code, https://arxiv.org/abs/2107.03374
- Microsoft AI: https://innovation.microsoft.com/en-us/ai-at-scale
- OpenAI: https://openai.com/
- Google AI: https://ai.google/
- Google Trax: https://github.com/google/trax
- AllenNLP: https://allennlp.org/
- Hugging Face: https://huggingface.co/