# bash cheatsheet 

Find a file in subdirs with case: `find . -name "foo*"`  

Find a file in subdirs case insensitive: `find . -iname "foo*"`

Install a package without sudo access: 
- `make` returns an executable `a`
- `mv a ~/.local/bin`
- add `~/.local/bin` to `$PATH` by adding `export PATH="~/.local/bin:$PATH"` to `~/.bashrc
- `source ~/.bashrc`
- confirm `a` command



  
