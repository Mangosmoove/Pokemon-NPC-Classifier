For our project, we decided to explore the various NPC trainers found in Pokemon games. In the games, a player can battle with their pokemon team (containing up to 6 pokemon) against an NPC’s pokemon team (also containing up to 6 pokemon), and there are some patterns in which pokemon an NPC may have based on their title or class. For instance, for an NPC named ‘Sailor Andrew’, the class is Sailor, and Sailors often have more water-based pokemon than any other element. Our project is to discover hidden patterns in NPC trainers players can encounter from Generation 1 through 4 games. Based on our model, we will then allow for a user to enter up to a team of 6 pokemon they would have on their own team, and predict what NPC trainer class they would belong to.
When we first got together as a group, we searched for an online database that contained NPC classes and their pokemon. However, we could not find such a database that would cover all generations. Therefore, we had to implement our own database that consists of nearly 4000 rows of data that we manually input based on this website. We did find a kaggle website that contained information on all pokemon, including their statistics, weaknesses, strengths, elemental type, and etc. We used this database as a helper database to find even deeper patterns in our database to create an accurate model.

The Trainers database contains the following fields: Class, Pkmn1, Pkmn2, Pkmn3, Pkmn4, Pkmn5, Pkmn6. The ‘Class’ field represents the trainer class of a given NPC as a string. Pkmn1 through Pkmn6 represent an individual pokemon as a string and together one row represents one team. Some rows may contain ‘nan’ values because many NPCs do not have 6 pokemon. 

The Pokemon database contains the following fields after cleaning:

--abilities: the abilities a pokemon can possess, stored as a list

--against_?: an integer value that represents if the given pokemon is super effective against, weak against, or has no effect on specified type pokemon. There are 18 fields that represent this for various types

--attack: the base attack stat of the given pokemon

--base total: the sum of all the stats of a given pokemon

--capture_rate: represents the capture rate of a pokemon

--hp: the base HP stat of the pokemon

--defense: the base Defense stat of the pokemon

--sp_attack: the base special attack stat of the pokemon

--sp_defense: the base special defense stat of the pokemon

--speed: the base speed of the pokemon

--is_legendary: a binary representation indicating if a pokemon is of legendary status or not

--height_m: the height of a pokemon in meters

--weight_kg: the weight of a pokemon in kilograms

--type1: the primary type of the pokemon

--type2: the secondary type of the pokemon

--name: the English name of the pokemon

--pokedex_number: the entry number of the pokemon in the national Pokedex

For more information about the project, feel free to check out the report!
