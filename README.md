# MODES_v1.0
MODES is a Matlab Toolbox for the solution of initial value problems.

# How to install MODES_v1.0
In order to install it you only need to download the included mlappinstall file and install it within matlab, with  the _Install App_.

# How to use MODES_v1.0
Once you have installed it, there will be a html directory containing all help you need to start using the code. 

If you open the matlab documentation (command _doc_) you will also find a special section for this toolbox.

The package should include the following files:
* main file: modes.m,
* info.xml: auxiliary file, needed to create the toolbox documentation,

and the following directories:
* +common: main MODES functions. 
* +ode: .m files for defining initial value problems.
* +tools: tools designed to study properties of linear multistep methods and initial value problems. You can find more information about the functions here in html/how_to_methods.html.
* examples: contains three m files used to generate the html files.
* html: MODES documentation.
* mexSources: **MODES can run faster if you have a C compiler installed in your computer. If this is case you should run the function _buildMex.m_ in the +tools directory before you start using MODES**.
* scripts: m files to solve all initial value problems in the +ode directory using Modes. The initial value problems in +ode have been solved using explicit (explicit methods), implicitK (implicit k steps methods of order k) or implicitKPlus1 (implicit k steps methods of order k+1),
* tests: Function for testing purposes. It tests whether MODES throws the right exceptions when called with wrong input arguments. To run the tests call: runtests('inputCheckTests.m').
