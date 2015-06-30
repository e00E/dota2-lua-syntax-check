# dota2-lua-syntax-check
It is often annoying to only find out about small typos and syntax error after you loaded your game, selected a hero and used an ability and so on. By running a syntax checker you dont waste that time.

I found luajit to be usable for this purpose. Follow the download and install instructions here http://luajit.org/download.html.

When compiling on Windows I got `luajit.exe` and `lua51.dll` in the `src/` folder. These two files and the `src/jit/` folder will be needed to run luajit. You can copy them where you like for example in a directory containing your path.

To syntax check a lua file use `luajit -bl <filenam> 1> nul`
The `1>l nul` hides stdout output which we dont want and only shows stderr. If there is an error in your lua file you will gt an error mesage describing the problem and if there is none you will get no output at all.



# TODO for this tutorial:
* Provide good instructions on how to get it in your path
* Add a way to check all lua files recursively in some folder maybe with a batch file.
