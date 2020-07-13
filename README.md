# django-sugar

This is a package of syntactic sugar to the parser to make writing in django bearable and productive.

Formal description: you write classes, methods, functions, helpers, and data objects (e.g. files) in one file.
The parser runs through this and creates or adds to the files django is looking for.

Rules are simple.

1. You write everything in a file and name it as you want. 
2. You tell the SugarParser where things go by writing the name of the file and it's location
   `def your_function(arg, arg2):  ~> pool, utils`
   This will find or create a module named pool and add `utils.py` as one of its leaves.
3. You can add submodules by adding commas
   `class SuperDuper:  ~> users, models, ticket`
   
 
