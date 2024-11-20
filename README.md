<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center">Multithreaded Concurrent Swimming Race</h3>


---

<p align="center">This project compares the time taken to generate an Abelian sandpile when using a parallel and serial solution. 

    <br> 
</p>

- [About](#about)
- [Prerequisites](#prerequisites)
- [Installing](#installing)
- [Running the Application](#tests)
- [Usage](#usage)
- [built_using](#built_using)
- [Authors](#authors)


## 🧐 About <a name = "about"></a>
In the Abelian Sandpile, each cell contains a certain number of "grains of sand". When the number
of grains in a cell exceeds 4, in the next time step the cell "topples", distributing grains evenly to its
neighboring cells (left, right, up and down) and keeping any remainder. The edge, or border, of the
automaton grid is a “sink” – for cells on the border, their distribution to the border will “disappear”
into the sink. An Abelian Sandpile evolves from a starting configuration (usually something simple
like all cells set to the value 4) until it reaches a stable state, where all cells have fewer than 4 grains.
If this final state is coloured according to the cell values (black for 0, green for 1, blue for 2 and red
for 3) is often revealed to be a beautiful pattern with complex symmetry.

The main objective of the project was to compare the results of the serial and parallel solution and compare the time it takes to generate sandpiles using different values, si at the end we can decide whether it's worth parallizing and if so when is it worth it. The Report.pdf further elaborates the scope of the project and analyses the results with different computer architecture. Also looks at the challenges encountered while conducting the experiment.

## Prerequisites <a name = "prerequisites"></a>

GNU Make:
Linux: Pre-installed on most distributions othrwise install using your package manager if missing.
Windows: Install make on git bash 


## 🔧 Running the application <a name = "tests"></a>

<img width=200px height=200px src="screenshot.png">

Shows you the results and time it takes to generate an image with a 65 by 65 all 4 input


## 🎈 Usage <a name="usage"></a>

1. Go to the project folder
2. execute the command: make run
3. This will execute the code with the default input parameters input/65_by_65_all_4.csv output/65_by_65_all_4.png

OR 

If you would like to run with other parameters, then execute providing the other parameters, e.g:<br>
make run ARGS="input/517_by_517_centre_534578.csv output/517.png"

## ⛏️ Built Using <a name = "built_using"></a>

- Java
- Multithreading (Thread and Runnable)
- ForkJoin Framework

## ✍️ Authors <a name = "authors"></a>

- Blessing Hlongwane
