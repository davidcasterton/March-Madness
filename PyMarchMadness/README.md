PyMarchMadness Source Code
=============

####Source Code Documentation:
- http://pymarchmadness.readthedocs.org/

####Source Code Overview:
- **\__init\__.py :** Initialize package.
- **\__main\__.py :** Main program.
  1. Prompts user to choose analysis method.
  2. Generates win probabilities for all possible matchups in each years March Madness tournament.
  3. Generates March Madness Tournament predictions.
- **Analysis/ directory:** Analysis base and derived classes, each derived class implements a distinct analysis method.
  - **Analysis.py :** Analysis base class.
- **Constants.py :** Loads input data files and defines constant values.
- **Basketball.py :** Team, Season, & Tournament classes.
- **Misc.py :** Miscellaneous helper functions.

####How To Add New Analysis To Framework:
- Create an analysis module that inherits from [Analysis.BaseClass] (Analysis/Analysis.py)
- Implement all methods that were not defined in [Analysis.BaseClass] (Analysis/Analysis.py)
- Insert analysis module into [PyMarchMadness/Analysis/] (Analysis/)
- Select new analysis module when prompted at run-time

####How To Add New Input Data:
- Add *\<new_folder\>* into [InputData/] (InputData/)
- Add data files into InputData/*\<new_folder\>*
