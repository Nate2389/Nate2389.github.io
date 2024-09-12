---
layout: project
type: project
image: img/pokedex.jpeg
title: "Pokemon Pokedex"
date: 2022
published: true
labels:
  - C++
summary: "During my ICS 212 class, we were assignemnt a homework to create a functional Pokemon Pokedex in C++."
---
<div class="text-center p-4">
  <img src="https://assets.pokemon.com/assets/cms2/img/pokedex/full//393.png" width = "25%" height = "25%">
  <img src="https://assets.pokemon.com/assets/cms2/img/pokedex/full//390.png" width = "25%" height = "25%">
  <img src="https://assets.pokemon.com/assets/cms2/img/pokedex/full//387.png" width = "25%" height = "25%">
</div>
<p>
  This assignment introduces the use of Map and Vectors. The object was to create a Pokemon Pokedex of different pokemons with each of them having their own type and size. Once a pokemon has been constructed it will then be push into a vector. Then in the vector it well be added to a map. Once thats all done it'll print out all the pokemon in the pokedex with the typing and the weight. Below is a code to the main function:
</p>



```cpp
int main(int argc, char* argv[])
{
    Pokemon* pokeArray[3];
    pokeArray[0] = new Chimchar();
    pokeArray[1] = new Turtwig();
    pokeArray[2] = new Piplup();
    /* 
     * Chimchar = fireChar
     * Turtwig = grassWig
     * Piplup = waterPulp
     */
    /*Vector container*/
    vector<string> pokeCont;
    pokeCont.push_back("fireChar");
    pokeCont.push_back("grassWig");
    pokeCont.push_back("waterPulp");
    /*Map container*/
    map<string,Pokemon*> pokeMap;
    pokeMap["fireChar"] = pokeArray[0];
    pokeMap["grassWig"] = pokeArray[1];
    pokeMap["waterPulp"] = pokeArray[2]; 
    /*loop checkPokedex to print all existing pokemons8*/
    for (int i = 0; i < 3; i++)
    {
        checkPokedex(pokeMap[pokeCont[i]]);
    }
}
```
<p>
  Note: new Chimchar() is a function corresponds to a different cpp file that constructs the pokemon Chimchar with information like its type and its weight. Same goes with the other(new Piplup() and new Turtwig()). Each cpp file of the pokemon has its own h.file
</p>
