# **CONFIGURAÇÕES DO SISTEMA**

## **MAC**

### **ADICIONAR COR AO TERMINAL**
```BASH
    export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]\$ "
    export CLICOLOR=1
    export LSCOLORS=ExFxBxDxCxegedabagacad
    alias ls='ls -GFh'
```

### **INSTALAR HOMEBREW**
```BASH
    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    export PATH=/usr/local/bin:$PATH
```

### **INSTALAR VIM**
```BASH
brew update
brew install vim && brew install macvim
brew link macvim
```