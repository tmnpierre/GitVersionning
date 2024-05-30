### 1. Installer Zsh
Si Zsh n'est pas déjà installé :
```bash
sudo apt install zsh -y
```

### 2. Installer Oh My Zsh
Pour installer Oh My Zsh :
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### 3. Changer votre shell par défaut en Zsh
Pour configurer Zsh comme votre shell par défaut :
```bash
chsh -s $(which zsh)
```
Vous devrez peut-être vous déconnecter et vous reconnecter pour que ce changement prenne effet.

### 4. Installer le thème Powerlevel10k
Pour installer Powerlevel10k dans votre répertoire personnalisé Oh My Zsh :
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

### 5. Configurer Oh My Zsh pour utiliser Powerlevel10k
Ouvrez votre fichier de configuration `.zshrc` :
```bash
nano ~/.zshrc
```
Modifiez la ligne contenant `ZSH_THEME` pour y mettre :
```bash
ZSH_THEME="powerlevel10k/powerlevel10k"
```
Enregistrez et fermez le fichier (`Ctrl+O`, `Enter`, puis `Ctrl+X`), puis sourcez le fichier pour appliquer les changements :
```bash
source ~/.zshrc
```

### 6. Configurer Powerlevel10k
Lors du prochain démarrage de votre terminal, Powerlevel10k devrait démarrer l'assistant de configuration pour personnaliser votre prompt.

En suivant ces étapes, vous aurez installé et configuré Oh My Zsh avec Powerlevel10k en utilisant une Nerd Font, sans avoir besoin d'installer à nouveau la police.