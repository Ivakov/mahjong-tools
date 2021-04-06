# mahjong-tools

## 環境構築
### Homebrewのインストール
brew -vでインストールできていることが確認できればスキップでよい

1. /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

1. echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/ユーザ名/.zshrc

1. eval "$(/opt/homebrew/bin/brew shellenv)"

1. brew -v  
バージョンが表示されればok

### Nodebrewのインストール
nodebrew -vでインストールできていることが確認できればスキップでよい
1. mkdir -p ~/.nodebrew/src
   
1. nodebrew compile v15.6.0  
※M1 Macだとbrew install nodebrewが通らないためこちらで対応
   
1. nodebrew use v15.6.0

1. echo 'export PATH=$HOME/.nodebrew/current/bin:$PATH' >> ~/.zshrc

1. source ~/.zshrc
1. node -v  
   バージョンが表示されればok

### git clone
1. git clone https://github.com/Ivakov/mahjong-tools.git

### パッケージのインストール
1. cd mahjong-tools
1. npm install

### 動作確認
1. npm start
1. ブラウザで http://localhost:3000/ にアクセス