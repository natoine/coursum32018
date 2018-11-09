# coursum32018
support pour les étudiants de M1 et M2 Miashs à l'UM3 

**intégration de données connectées**

Le but de ce cours est de forger une première culture de ce qu'est le Web et la problématique de l'interopérabilité.
Les étudiants doivent réaliser un premier mashup uniquement en code client.

_Définitions :_

* Web ( http, URI, HTML ) : Le web c'est une application basée sur le réseau internet. Il permet d'échanger des informations via un protocole de communication ( http ) entre un client et un serveur. Les informations ( ou données ) sont représentées dans un format par exemple, originellement le html pour représenter des documents hypertexte, mais d'autres formats sont utilisés ( json, xml, txt, jpg, css, javascript ... ). Chaque Ressource ( dont les pages des documents hypertextes ) est identifiée de manière unique par une URI.
* HTTP : (hypertext transfer protocol) protocole de communication entre client et serveur définissant les méthodes ( GET, PUT, POST, DELETE, HEAD, OPTIONS, TRACE, CONNECT ) que le client peut demander au serveur d'exécuter sur une ressource définie par son URI.  
* REST : c'est une redéfinition des méthodes HTTP qui restreint la portée de chaque méthode et en simplifie la définition / l'utilisation.
* URI / URL : Une URI (Uniform Resource Identifier) est un identifiant d'une ressource, une URL (Uniform Resource Locator) est une adresse vers la ressource. Une adresse est ce qui permet de définir un lien, ou d'accéder à une ressource via le protocole http. 
* un lien : c'est ce qui permet de passer d'une ressource à une autre. Se concrétise par la balise "a" en html et l'attribut "href".
* hypertexte : c'est le système de navigation entre des Ressources par des liens. Un document hypertexte est une collection de Ressources liées entre elles. A comparer à un livre dans lequel la suite d'opération de navigation est de tourner et lire les pages dans l'ordre. Dans un document hypertexte, la suite d'opération de navigation est une collection de liens à parcourir. 
* Ressource : n'importe quoi qui est identifié par une URI.
* interopérabilité : c'est quand des programmes sont capables de communiquer entre eux, ce qui implique la définition d'un protocole de communication et de formats de données connus et partagés par ces programmes.
* mashup : c'est une application qui mélange des données provenant de plusieurs sources.
* client : c'est l'application qui envoie une requête et qui attend une réponse.
* serveur : c'est l'application qui écoute et attend les requêtes et renvoie une réponse à une requête.
* Requête : une requête http est la demande qu'envoie un client à un serveur, l'action de la demande est précisée par la méthode http invoquée.
* Réponse : le retour envoyé par le serveur au client suite à une requête.
<p align="center">
<img src="/schemaS-C.jpg" width="400" margin:>
</p>

* Route http : c'est la définition d'une URL sur laquelle une opération peut être effectuée par le serveur à la demande du client selon une méthode http et aboutissant à une réponse.
* API Web : (Application Programming Interface) Collection de routes http que propose le serveur aux clients. 
* parsing de données : parcourir une donnée pour en extraire ce qui nous intéresse, éventuellement le traduire dans un autre format.
* langage de programmation : c'est un langage qui permet d'écrire un programme (une application), donc de décrire des opérations à faire exécuter par le système. Par exemple, le javascript.
* langage de description : c'est un langage qui permet de mettre en forme des données, de décrire un modèle de données. Par exemple le html est un langage à balises permettant de décrire une page d'un document hypertexte.
* négociation de contenus : c'est l'opération entre le client et le serveur leur permettant de s'accorder sur le format de données renvoyé par le serveur au client.
* web statique : c'est quand un serveur web ne fait que renvoyer des données (principalement des pages web en html) stockées telles quelles dans des fichiers. 
* web dynamique : c'est quand un serveur web fabrique / génére à la volée, par un calcul, les fichiers qu'il renvoie. Le résultat du calcul peut et donc le fichier renvoyé en réponse peut alors varier en fonction du temps. 
* framework : un ensemble d'outils et de pratiques.

_Technologies utilisées :_

* http : le protocole de communication du web. https://www.w3.org/Protocols/rfc2616/rfc2616.html
* html : le format de données des pages web. https://www.w3.org/TR/html/
* URI / URL : le système de nommage et d'adressage des Ressources. https://www.w3.org/Protocols/rfc2616/rfc2616-sec3.html#sec3.2
* git : l'outil de gestion de version utilisé dans le projet. https://git-scm.com/
* github ( et githupage ) : le service en ligne d'hébergement de repository git. https://github.com/
les githubpage sont une façon de rendre accessible une page de votre projet git. Si votre projet n'inclue que du code client, c'est une bonne façon d'héberger et de rendre accessible votre projet. A paramétrer dans chaque projet.
* javascript : un navigateur web est un client http qui interpréte du html. Mais un navigateur est aussi un interpréteur du langage javascript. Ce qui fait de javascript le langage de programmation incontournable du web. https://fr.wikipedia.org/wiki/JavaScript
* fetch : fetch est une fonction pour réaliser des requêtes http asynchrones à partir d'un script javascript client. Cette fonction tend à devenir la référence et remplacer XMLhttprequest dans les bonnes pratiques de développeurs web. Pour une introduction à fetch et mieux comprendre l'histoire de XMLhttprequest et fetch : https://developers.google.com/web/updates/2015/03/introduction-to-fetch
* XML : est un format de données pour représenter des arbres de données. https://www.w3.org/TR/xml/
* RDF : est un framework pour représenter et partager des données et des formats de données. https://www.w3.org/RDF/
* JSON : la façon de représenter des objets javascript. De syntaxe simple mais peu verbeuse, le json est devenu un format de données largement répandu sur le web. https://www.json.org/
* le DOM : ( Document Object Model ) le DOM représente le html interprété par un navigateur et transformé en une collection d'objets dont le navigateur fait notamment un rendu graphique. Le DOM est modifiable par le javascript client et permet de modifier le rendu graphique d'une page html côté client. https://www.w3.org/DOM/

_La consigne du Projet :_
Faire un mashup qui récupére des données de plusieurs API ( au moins 2 ) uniquement en code client, en utilisant fetch ( et éventuellement XMLhttprequest ) hébergé en githubpage. Vous serez amenés à modifier le DOM en fonction des données récupérées.

**OpenData**

Le but de ce cours est d'approfondir la culture de ce qu'est le Web en abordant les notions de Web de données, de Web Sémantique et d'OpenData. En s'inspirant des one page application, le code client devra faire des fetch vers l'API développée.
Les étudiants doivent réaliser un deuxième mashup cette fois-ci en code serveur avec node.js.

_Définitions :_

* Web de données : c'est une vision dans laquelle le web est un moyen d'accès à des données les rendant réutilisables. C'est voir le web comme une grande base de données.
* OpenData : démarche d'ouverture des données sur le web. L'opendata par rapport au web des données en utilise ses mécaniques et ajoute des libertés de réutilisation. C'est une démarche notamment adoptée par les administrations publiques ou collectivités territoriales afin de garantir la transparence des administrations aux citoyens. La réutilisabilité des données permet la mise en place de nouveaux services ou nouvelles applications.
* Web Sémantique : c'est une vision du web de données où les relations entre les ressources sont typées et ont une sémantique explicitée. Ce qui définit des formats de données très verbeux (au sens accessible à tout le monde car très fourni) par exemple RDF. 
* one page application : une seule ressource composée de html et de javascript est chargée dans le navigateur. Le contenu de la page évolue en résultat à des requêtes émises par le javascript.
* requête asynchrone : quand on fait une requête, on est dépendant du délai de réponse du serveur. En mode synchrone tout l'exécution du code est en attente de la réponse. En mode asynchrone, on définit un code à traiter au moment de la réponse ( on parle de fonction callback ). Du coup, le reste du code est exécuté. La fonction callback sera quand à elle exécutée au moment de la réponse.

_La consigne du Projet :_
Faire un mashup qui récupére des données de plusieurs API ( au moins 2 ) en code client-serveur, en utilisant fetch et request hébergé sur heroku.
Développer sa propre API avec au moins une route en GET et une route en POST.

_Technologies utilisées :_

* node.js : est une application logicielle libre permettant de développer des applicatifs réseaux et notamment des serveurs http. https://nodejs.org/en/
* npm : dans l'univers javascript on parle de modules pour réutiliser du code fait par d'autres. NPM (initialement Node Package Manager) est l'outil de gestion des modules javacript. C'est ce qui va vous permettre de télécharger et installer les modules que vous allez utiliser dans node. https://www.npmjs.com/
* mongodb : une base de données orientée documents stockant les objets en JSON binaire. L'utilisation de Mongodb avec nodejs est largement documentée et le fait que les documents soient stockés en JSON en font une solution fréquemment utilisée. https://www.mongodb.com/
* mongolab : un service d'hébergement de bases mongodb offrant un hébergement limité gratuit. Largement suffisant pour le projet. https://mlab.com/home
* heroku : qui dit serveur http, dit hébergement du serveur. Heroku est un service proposant un hébergement limité mais gratuit de serveurs http. Largement suffisant pour le projet et bien adapté à un projet nodejs dont les versions du code sont stockées sur github. https://dashboard.heroku.com
* SPARQL : (SPARQL Protocol and RDF Query Language) est le langage de requêtes pour RDF basé sur un principe de matching de graphe. https://www.w3.org/TR/rdf-sparql-query/
* templating ejs : ejs est un outil de templating que vous pouvez utiliser avec nodejs pour générer des pages html. Le templating ejs permet d'écrire un fichier .ejs dont la syntaxe est celle du html plus une balise permettant d'injecter des variables javascript. Le fichier .ejs permet au serveur de renvoyer du html en réponse après avoir interprété les variables présentes dans le .ejs. Cette technologie n'est pas obligatoire pour le projet. https://ejs.co/
* request ( node.js ) : request est un module npm permettant de faire des requêtes http. Cette technologie n'est pas obligatoire pour le projet. https://www.npmjs.com/package/request
* markdown : est un langage simple et léger permettant d'écrire des documents. Il est notamment directement interprété par l'interface de github. Pratique pour écrire et mettre en page simplement des documents comme celui que vous lisez. https://daringfireball.net/projects/markdown/
