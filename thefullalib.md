# CHEAT SHEET
## for ALIB configs

### <cmd>
#### classics: 
`extern:package[store:[], from:[""], name:[""]]` <- this one imports a package from the web

`intern:package[from:[]]` <- this one is for PRE-COMPILED ALANG LIBRARIES 

`auto:compile alang --c --exe --file myfile.alang` <- with this all you have to do is just execute the alib inside of VSCode and the source file referenced will compile to a .exe

`auto:compile alang --c --dll --file myfile.alang` <- same as before, but now instead of a .exe, it will be a .dll

`auto:compile alang --c --lib --file myfile.alang` <- same as before, except we are compiling to a static library (.lib) 

#### core 

`core:source[source_file[""], fpath[], expose? true]` <- this one exposes the constructs inside of your .rs file into alang

`core:source[source_file[""], fpath[], expose? false]` <- one change, `true` -> `false` this is essentially useless 

`core:config --op1` <- this one changes the optimisation level to 1, which is the same as the default 0 (no optimisation) except it handles variables a bit faster, it ranges from 0 to 10 

`core:config --alng_extent --!alang | !alng --h` <- this one changes the file extension of alang, useful for creating your own version 

`core:config --alng_syntax --!func --class | class --reflect func` <- this one deletes the `func` syntax as replaces it with class 

------------

### <package> 
`insert:construct[]` <- this is how you insert macros

`insert:construct:math* []` <- this inserts math macros

`insert:package=""` <- this inserts a module/package globally across the codebase 

`pack:file --myfile.alang` <- this converts it to a .apack (which is basically a non binary static library for this language)

---------------------
