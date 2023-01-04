---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Sudoku"
date: 2022-04-15
published: true
labels:
  - Python
  - Programming
  - Problem Solving
summary: "I wrote a program that could solve a medium difficulty Sudoku puzzle without using Brute Froce."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

Sudoku is a logic-based combinatorial number placement puzzle.

For this project, I chose to not use a Brute Froce approach in solving this puzzle. I wanted my program to mimic a systematic, box-by-box, row-by-row, column-by-column approach to solve the puzzle.

Here is some code that illustrates how we read values from the line sensors:

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

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
