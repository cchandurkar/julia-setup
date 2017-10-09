# julia-setup
How to setup developer environment for Julia. [Install Julia](https://julialang.org/downloads/platform.html) . Make sure `julia` is on your path. You can later add julia path to julia-client settings in atom.

## STEP 1: Install [ATOM](https://atom.io/) editor

## STEP 2: Run following commands from terminal
Use Atom Package Manager (apm) to install julia specific ATOM packages.

```
apm install language-julia
apm install latex-completions
apm install indent-detective
apm install ink
apm install julia-client
```

## STEP 3: From Julia Terminal Install:
```
Pkg.clone("http://github.com/JunoLab/Atom.jl")
Pkg.clone("http://github.com/JunoLab/CodeTools.jl")
```

## Step 4: Add Key Bindings to ATOM 
Open `keymap.cson`. Preferences Menu => Keybindings => click on "your keymap file" ) and paste the following:
```
'atom-text-editor[data-grammar="source julia"]:not([mini])':
  'tab':       'language-julia:toggle-docstrings'
  'shift-tab': 'language-julia:toggle-all-docstrings'
```


