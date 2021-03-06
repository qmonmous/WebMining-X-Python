# Web Mining *X* Python

*Ce répertoire vise à introduire à la collecte de données web (Web Mining).*

![](img/webmining.png)

## Introduction au Web Mining

Le *Web Mining* est une branche spécifique du Data Mining qui s'intéresse aux données issues du web.

Ces données sont très intéressantes pour des problématiques liées au marketing ou aux sciences humaines. En effet, elles permettent de contourner les biais des méthodes expérimentales (préconçus, orientations des questions...) - ou encore le *paradoxe de Labov* - car contrairement aux données recueillies lors de questionnaires/entretiens, les personnes produisent les contenus spontanément.

En Web Mining, on analyse généralement trois types de données :
- Usages du web (parcours utilisateurs, web analytics...)
- Contenus du web (*Scraping*...)
- Structure du web (*Crawling*...)


## La limite des APIs web

Sur la plupart des gros sites web, des *APIs* sont mises à disposition pour pouvoir en récupérer les données. C'est par exemple le cas pour Twitter, Facebook ou Linkedin. Toutefois, certaines de ces APIs sont largement limitées (contenu innaccessible, rate limit, options payantes...). Autre problème, des sites moins importants, mais tout aussi intéressant à analyser, ne possèdent tout simplement pas d'API.
Pour récolter l'ensemble des données qui nous intéressent, il existe une solution puissante qui s'affranchit de ces limites : le *Scraping*.


## Le Scraping

![](img/scraping.png)

*To scrape*, ou gratter en français, c'est l’art d’extraire des données directement depuis leur représentation visuelle. Lorsqu'on crée une page web, on va structurer son contenu avec du HTML. Du templating va permettre de formater et d'insérer des données dynamiques dans ces structures. Ainsi, dans le cas des pages web, on va scraper le HTML lui-même pour récupérer précisément les données souhaitées. D'une certaine manière, on procède à une rétro-ingénierie du processus de templating.

Pour commencer cette introduction au scraping, assurez-vous d'avoir installer les deux dépendances suivantes :
- `pip install requests`
- `pip install beautifulsoup4`

Maintenant, rendez-vous sur [ce notebook](Introduction%20au%20Scraping.ipynb) pour découvrir le scraping !

## Le Crawling

![](img/crawling.png)

*To crawl*, ou ramper en français, c'est parcourir le web à l’aide d’un programme (bot, spider) en récupérant :
- les pages parcourues
- les liens entre elles

Si vous êtes familiés avec la notion de graphe, il apparaît évident qu'on constitue alors un réseau de pages qu'on va pouvoir analyser ([ici avec NetworkX](https://github.com/qmonmous/DataScience-X-Python/blob/master/10.%20Th%C3%A9orie%20des%20graphes%20et%20Analyse%20de%20r%C3%A9seau.ipynb)).

Pour commencer cette introduction au crawling, assurez-vous d'avoir installer les dépendances suivantes :
- `pip install requests`
- `pip install urllib`
- `pip install beautifulsoup4`
- `pip install networkx`

Maintenant, rendez-vous sur [ce notebook](Introduction%20au%20Crawling.ipynb) pour découvrir le crawling !

---

## Disclaimer juridique

Revendre des données protégées par la propriété intellectuelle est répréhensible.

## Notes annexes

**Deepweb** : pages non indexées (70% des pages web mondiales). Cela comprend les intranets par exemple.

**Queue** : Une queue suit la méthode du premier entré, premier sorti (*FIFO* pour *First In First Out* en anglais).  
exemple : [1, 2, 3] => 1, 2, 3  

**Stack** : Une stack suit la méthode du dernier entré, premier sorti (*LIFO* pour *Last In First Out* en anglais).  
exemple : [1, 2, 3] => 3, 2, 1

## Rappel sur les réseaux : 
- des noeuds
- des liens reliant les noeuds

projetables sur un plan qui pourra être visualisé et analysé.
