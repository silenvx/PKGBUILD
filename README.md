このPKGBUILDの使い方
====
このgitのクローンをまず作ってから
```
% git clone https://github.com/silenvx/PKGBUILD.git
```

コンパイルしたいディレクトリにこのように移動して
```
% cd PKGBUILD/fuppes
```

コンパイルと同時にpacmanでインストールを行います
```
% makepkg -i
```
これだけで導入までが可能です

pacman -Syuで更新する時に、あるパッケージを無視するには
----
```
/etc/pacman.conf
```
に
```
IgnorePkg   =xterm tmux
```
こんな感じで書いとけば、対象のパッケージがアップデートの時に無視されます
無視した時は、メッセージが出るのでその都度、各自でPKGBUILDを用意してアップデートすれば良い
