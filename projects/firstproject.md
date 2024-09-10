---
layout: project
type: project
image: https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRNggEtagHz85kQ5Y2FQPwNAFOY93sAVu7B_w&s
title: "Pokemon Pokedex"
date: 2022
published: false
labels:
  - C++
summary: "During my ICS 212 class, we were assignemnt a homework to create a functional Pokemon Pokedex in C++."
---

<div class="text-center p-4">
  <img src= "https://assets.pokemon.com/assets/cms2/img/pokedex/full//390.png">
  <img src= "https://assets.pokemon.com/assets/cms2/img/pokedex/full//393.png">
  <img src= "https://assets.pokemon.com/assets/cms2/img/pokedex/full//387.png">
</div>

This homework introduces the use of vectors and maps.

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```
