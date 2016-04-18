# visual-TSP
Visual-TSP - a web application for travelling salesman problem visualization and solving.

![Screenshot](screenshot.jpg)

##Client Installation

Edit *build.sh* Bash script and set TARGET_DIR as you wish.

*Visual-tsp.js* file is a result of compilation from *visual-tsp-jsx.js* file.  
For compiling *visual-tsp-jsx.js* by yourself, a compiler such as Babel JS is needed for React JSX compiling.  
To start experimenting with TSP, open *visual-tsp.html* in your browser.  
Make sure your browser is up-to-date enough to be able to handle ES6.

##Server Installation

Client side application contains a TSP solver, but server side calculation is recommended for smoother UX.  
'servers' directory contains TSP solver implementations for Python and Node.js.

Python application is based on Tornado server, see http://www.tornadoweb.org/en/stable/ for installation instructions.  
Once you have Tornado installed, start the server with command **python3 tsp-solver.py**

Node.js application is based on express, express-ws and permutation-engine.  
Install tsp-solver.js with command **npm install**  
Start the server with command **node tsp-solver.js**

##3rd party libraries

This project includes a permutation-engine.js file from https://github.com/eriksank/permutation-engine

Following libraries are utilized via CDN:

oCanvas - Canvas drawing made easy http://ocanvas.org/  
Redux - Application state container http://redux.js.org/  
React - For listing the coordinates etc. https://facebook.github.io/react/  
jQuery - For generic DOM manipulation etc. http://jquery.com/


