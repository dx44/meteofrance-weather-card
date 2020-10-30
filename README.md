# Lovelace Météo France weather-card - Icones X 2

Adaptations de la carte https://github.com/hacf-fr/lovelace-meteofrance-weather-card, proposer par ![Home Assistant Communauté Francophone](https://hacf.fr/).

![Weather Card](https://github.com/Axellum/lovelace-meteofrance-weather-card/blob/Meteo-France/fixe-fdnoir.png?raw=true)

Projet reprit de https://github.com/Imbuzi/meteo-france-weather-card, pour une adaptation de la carte https://github.com/bramkragten/weather-card dédié à Météo France.

- Ajout de nouveaux jeux d'icônes (resortent mieux avec un thème sombre), possibilitée de remettre les icones d'origine (complété).
- Différentiation des icônes sur certains arguments (Brouillard, Orage pluvieux, Pluie-neige, venteux), sur tout les jeux d'icônes.

Icônes animées bleus: ```yaml /local/community/lovelace-meteofrance-weather-card/icons/ ```:
![Icons_1](https://github.com/Axellum/lovelace-meteofrance-weather-card/blob/Meteo-France/anime-fdblc-2.png?raw=true)

Icônes fixe: ```yaml /local/community/lovelace-meteofrance-weather-card/icons_1/ ```:
![Weather Card](https://github.com/Axellum/lovelace-meteofrance-weather-card/blob/Meteo-France/carte-icone-fdbl.png?raw=true)

Icônes animées blancs: ```yaml /local/community/lovelace-meteofrance-weather-card/icons_2/ ```:
![Icons](https://github.com/Axellum/lovelace-meteofrance-weather-card/blob/Meteo-France/anime-fdblc-3.png?raw=true)



## Installation:

Ajoutez l'adresse https://github.com/Axellum/lovelace-meteofrance-weather-card dans "Custom repositories" sur HACS, "Category": "Lovelace".

## Configuration:

1/ Ajouter une carte manuel.

2/ Mettre:
```yaml
type: 'custom:meteofrance-weather-card'
```
3/ "Afficher l'éditeur de code" (cela affichera l'éditeur visuel)

4/ Si besoin, vous pouvez renseigner "Icones location" avec l'adresse pointant en locale les icones animées d'origine (par example):
```yaml
/local/community/lovelace-meteofrance-weather-card/icons/
```
5/ Choisir votre weather Météo France en Entity.
Cela renseignera automatique les différents sensor, il vous faudra renseigner Vigilance Météo par le sensor vigilance de votre région.

![reglages_graph](https://github.com/Axellum/lovelace-meteofrance-weather-card/blob/Meteo-France/regl-carte-icone.png?raw=true)

N.B.:
La détection de la pluie sur 1h00 n'est valable que pour certaines régions:

![Regions valide pour pluie sur 1h00](https://www.home-assistant.io/images/integrations/meteo_france/carte-couverture-du-service.png?raw=true)

Les icônes fixe viennent de https://icon-icons.com/fr/pack/The-Weather-is-Nice-Today/1370, création de Laura Reen. J'ai parfois apporté de légère modifications.

Les icônes animés sonr issus de https://www.amcharts.com/free-animated-svg-weather-icons/, avec modifications sur certain pour les compléter.
