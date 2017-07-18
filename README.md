# Chatbots

Framework de Spring para el procesamiento de datos.

## Índice
  1. **[historia](#historia)**
  2. descripción
  3. estado del arte
  4. modelo conceptual
  5. comparativa de productos
  6. casos de uso
  7. conclusiones y recomendaciones
  8. referencias

## historia

[`Spring Batch`] es un framework ligero enfocado específicamente en la creación de procesos batch. 
### La Máquina de Turing (1950) 

Entre 1950 y 1960, Alan Turing y Joseph Weizenbaum contemplaron la posibilidad de que los ordenadores se comunicasen como humanos mediante experimentos como el test de Turing y que fue el inicio del concepto de los chatbots.

El test de Turing se desarrollo por Alan Turing en 1950 para verificar la abilidad de un ordenador de mostrar un comportamiento inteligente equivalente al realizado por un humano.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_La_Maquina_de_Turing_1950.png"></p>

### ELIZA La Terapeuta (1966)

ELIZA fue el primer chatbot construido. Inventado en 1966 por Joseph Weizenbaum en el MIT que con apenas 200 lneas de código permitió imitar el lenguaje de una terapeuta.

El funcionamiento de ELIZA se basaba en la búsqueda de palabras clave en las frases introducidas por el usuario repondiendo con frases previamente entrenadas en su base de conocimiento. Tras utilizar el bot, acababa volviéndose intuitivo y repetitivo, convirtiendo las conversaciones con sus usuarios incoherentes.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Eliza_La_terapeuta_1966.png"></p>

### PARRY El Paranoico (1972)

En los 70s, ELIZA conoció a su primer paciente no humano: PARRY, un chatbot que imitaba a una persona con esquizofrenia y paranoia.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Parry_El_Paranoico_1972.png"></p>

### PARRY met ELIZA (1973)

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Parry_Met_Eliza_1973.png"></p>

### DR. SBAITSO (1992)

Un programa de síntesis del habla creado por computadoras basadas en MS DOS. Fue diseñado para mostrar una voz digitalizada, el Doc estaba lejos de asumir un rol de de psicólogo interactuando con usuarios humanos.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Dr.Sbaitso_1992.png"></p>

### A.L.I.C.E (2000)

“Artificial Linguistic Internet Computer Entity” era un bot con procesamiento natural del lenguaje (PNL). Podía aplicar patrones heurísticos uniendo reglas de lo que los humanos le decían, es decir, tenia una conversación.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_ALICE_2000.png"></p>

### EUGENE (2001)

Un bot inteligente distribuido en redes SMS. Con características como acceso veloz a la data y personalizaciones conversacionales, era considerado el precursor de SIRI y Samsung’s Voice.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Eugene_2001.png"></p>

### SIRI Apple (2010)

Un asistente inteligente virtual, parte del sistema operativo iOS de Apple, el cual tiene características como interfaz natural del lenguaje, preguntas y respuestas, y puede generar solicitudes al Internet.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_SIRI_Apple_2010.png"></p>

### IBM Watson (2011)

Watson fue diseñado para competir en Jeopardy!, el cual lo gano en el 2011 ante dos de los más grandes campeones del juego. Ahora Watson ocupa procesamiento natural del lenguaje (PNL) y Machine Learning para revelar características de grandes cantidades de datos.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_IBM_Watson_2011.png"></p>

### Google NOW - Google HOME (2012)

Desarrollado por Google para la aplicación móvil Google Search, empleando una interfaz de usuario natural del lenguaje para responder preguntas, hacer recomendaciones, y realizar acciones como delegar una solicitud a una serie de servicios web.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Google_Now_2012.png"></p>

### Amazon ALLO - Amazon ALEXA (2015) 

Un servicio de voz habitado en el dispositivo de Amazon, Echo. Alexa es capaz de interactuar por medio de la voz, utiliza procesamiento natural del lenguaje para recibir, reconocer y responder comandos de voz.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_ALEXA_Amazon_ALLO_2015.png"></p>

### CORTANA - Microsoft (2015)

Un asistente inteligente personal desarrollado por Microsoft, Cortana te envía recordatorios, reconoce comandos natural de voz, y responde preguntas usando el motor de búsquedas de Bing.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Cortana_Microsoft_2015.png"></p>

### TAY.ai - Microsoft (2016)

Diseñado para simular el habla y los hábitos de una joven americana. Tay rápidamente desarrollo paranoia viciosa y tubo que ser apagado a tan solo 6 horas dado que empezo a dar comentarios ofensivos a la gente.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Tay.ai_Microsoft_2016.png"></p>

### Bots For Messenger - Facebook (2016)

En Abril, Facebook lanzo una plataforma que permite a los desarrolladores crear bots que pueden interactuar con los usuarios de FB. Hasta Junio, 11.000 bots estaban disponibles.

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_Bots_for_Messenger_2016.png"></p>

### VIV (2017)

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_VIV_2017.png"></p>

### BIXBY - Samsung (2017)

<p align="center"><img src="https://raw.githubusercontent.com/maldiny/Chatbots-en-Castellano/bfa29d8c89f1eea74bb6ab3e087b911d831962b8/imagenes/%5BMaldiny%5D_BIXBY_Samsung_2017.png"></p>

**[Ir al índice](#Índice)**

## Referencias

* [Chatbots Magazine](https://chatbotsmagazine.com/)
* [Introducing the Bots Landscape](http://venturebeat.com/2016/08/11/introducing-the-bots-landscape-170-companies-4-billion-in-funding-thousands-of-bots/)
* [MyClever - ChatBots A Consumer Research Study](http://www.mycleveragency.com/media/download/0c44f0c083879818a0d2347ab948752b)
* [Microsoft Channel Inspector](https://docs.botframework.com/en-us/channel-inspector/channels/Telegram)
* [12+ Frameworks to Build ChatOps Bots](http://nordicapis.com/12-frameworks-to-build-chatops-bots/)
* [Así era ELIZA, el primer bot conversacional de la historia](https://www.xataka.com/historia-tecnologica/asi-era-eliza-el-primer-bot-conversacional-de-la-historia)
* [How to build yout own AI Assistant Using API.ai](https://www.sitepoint.com/how-to-build-your-own-ai-assistant-using-api-ai)
* [Gartner's 2016 Hype Cycle for Emerging Technologies](http://www.gartner.com/newsroom/id/3412017)
* [Home Automation devices](https://www.youtube.com/channel/UCXn_loz0TlUKarhS6sUoKVw)
* [War of Bot Platforms](https://chatbotbook.com/war-of-bot-platforms-22e02cfa0a99?gi=cfba6c7b93c1#.q8s3487ay)

**[Ir al índice](#Índice)**
