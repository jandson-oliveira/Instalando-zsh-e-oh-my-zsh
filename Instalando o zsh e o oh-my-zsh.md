# Instalando o zsh e o oh-my-zsh 


[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Estou usando uma distro baseada no arch linux, neste caso estou usando o PACMAN como gerenciador de pacotes
portanto, alguns comandos só irão funcionar em distros arch linux, substitua pelo seu gerenciador de pacotes nos comando  abaixo.

## Comandos
- Instalando o zsh: sudo pacman -S zsh 
- Fazendo um curl do oh-my-zsh: curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh; zsh
- ✨Definina o zsh como padrão: sudo usermod --shell $(which zsh) $USER
- Faça o curl do highlight: git clone https://github.com/zsh-users/zsh-syntax-highlighting.git${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
- Entre no arquivo com algum editor de sua preferência, eu usei o nano: nano ~/.zshrc procure a sessão plugins coloque dentro do () o plugin: zsh-syntax-highlighting 
- Faça um curl do Suggestions:git clone https://github.com/zsh-users/zsh-autosuggestions$ZSH_CUSTOM/plugins/zsh-autosuggestions
Entre no arquivo com lagum editor de sua preferência, eu usei o nano: nano ~/.zshrc procure a sessão plugins coloque dentro do () o plugin: zsh-autosuggestions

- Buscador com CTRL + t faça um curl
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install
quando terminar o curl ele fará algumas perguntas, só confirmar com Y.

- Tema powerlevel10k 
git clone e redirecionamento para o ~/.zshrc
yay -S --noconfirm zsh-theme-powerlevel10k-git
echo 'source /usr/share/zsh-theme-powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc

- Entre no arquivo com algum editor de sua preferência, eu usei o nano: nano ~/.zshrc procure a sessão ZSH_THEME, COLOQUE O # no que está copie ele e cole embaixo dele, e dentro das aspas duplas coloque powerlevel10k/level10
