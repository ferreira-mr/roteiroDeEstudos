# **VIM**

## **REFERÊNCIAS**

http://vimcasts.org/

## **LIVROS**

- [ ] Learn Vimscript the Hard Way - Steve Losh
- [ ] Painless Vim - Nate Dickson


Identificar diretório onde está localizdo o arquivo ***.vimrc*** (arquivdo de configuração do VIM) 
```bash
:echo $HOME
```

## **MODOS**

### **NORMAL**

#### **Movimentação**

- **H** - Esqueda 
- **L** - Direita
- **J** - Baixo 
- **K** - Cima

- **/** 					- Inicia busca
- **N** 					- Próximo ocorrencia do termo buscado
- **Shift + N** 	- Ocorrência anterior do termo buscado 
- **X**						- Recorta
- **Y**						- Copia
- **P**						- Cola
- **U**						- Desfazer
- **CTRL + R**		- Refazer
- **O** - Move o cursos para a linha abaixo e altera para o Modo Inserção

#### **Localizar e Substituir**

```bash
`%s/textoL/textoS/g/c
```

- **%s** - Inicia o modo busca
- **/textoL**	: texto a ser localizado
- **/textoS**	: testo a ser substituido
- **/g**			: realiza a busca globalmente no arquivo 
- **/c**			: realiza as substituições interativamente, solicitando confimação

#### **Corrgir identeção**

- **=** - Sobre a linha que necessita ser corrigida

### **INSERT (i)**

- **O** - Move o cursos para a linha abaixo e altera para o Modo Inserção

### **COMANDOS (:)**

- Salvar            :w
- Sair              :q
- Salvar e sair     :wq
- Sair sem salvar   :!q

### **VISUAL (v)**

- **SHIFT + V**	: Modo seleção por linha
- **CTRL + V**	: Modo seleção por bloco


**[Vim_RC](https://github.com/amix/vimrc)**

- [Vim-Bootstrap](https://vim-bootstrap.com/)
- [NeoVim](https://neovim.io/doc/)

# Atalhos
- J (baixo)
- K (cima)
- H (esquerda)
- L (direita)
- /*text* localiza texto.  n (next) - shift n (anterior- u (desfazer)
- CTRL r (refazer)a caracter
- SHIFT V (selecionar linha)
- y copiar
- P colar
- CTRL v (modo seleção por block)
- = altera identação
- o (modo insersão linha abaixo identado)
- :%s/ul/nav/gc
- x delet
- :vs *outro_arquivo* (divide tela)
- CTRL ww (troca de lado)
- SHIFT g
- gg
- SHIFT a

> pressionar um número ***n*** antes de um atalho faz com que o atalho seja executao ***n*** vezes


Pathogen
NerdTree

Vim HARDd
http://ohmyz.sh/
https://github.com/tpope


```vim
execute pathogen#infect()
set tabstop=2
syntax on
set shiftwidth=2
filetype plugin indent on
set backspace=2
colorscheme dracula
set number

```

## **THEMAS**

- Tomorrow Night Eighties
