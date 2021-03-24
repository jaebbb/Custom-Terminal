# oh-my-zsh 를 이용한 터미널 꾸미기

### zsh 설치
```bash
$ sudo apt-get install zsh
```
### bash 쉘 -> zsh 쉘 변경  
```bash
$ which zsh
$ chsh -s $(which zsh)
```

### oh-my-zsh 설치
```bash
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### powerlevel10k 설치
```bash
$ git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
$ echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>! ~/.zshrc
```

### 필요한 기능들 설치  
ex)  
- zsh-completions
- zsh-syntax-highlighting
- zsh-autosuggestions

```bash
$ git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
$ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

[plugin 목록에 plugin 추가하기]
```bash
plugins=(
         zsh-autosuggestions
         zsh-syntax-highlighting
         zsh-autosuggestions
         )
```
