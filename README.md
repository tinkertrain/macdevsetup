Mac Dev Setup
=============

Files for setting up a mac just the way I like it.

### Before

- Install xcode and Command Line Tools
- Install the fonts from the fonts directory


##OSX

- Use the .osx included
- [QuickLook plugins](https://github.com/sindresorhus/quick-look-plugins)

##Terminal


###[iTerm 2](http://www.iterm2.com/#/section/home)

- Install it
- Regular Font: Sauce Code Powerline 15pt
- Non ASCII font: Sauce Code Powerline 16pt
- Theme: Solarized Dark

###[oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

- install `curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh`
- Drop `remy.zsh-theme` into the zsh themes folder
- Use the .zshrc in the repository


###[Z](https://github.com/rupa/z)

In the terminal:

`mkdir -p ~/code/z`
`curl https://raw.github.com/rupa/z/master/z.sh > ~/code/z/z.sh`
`chmod +x ~/code/z/z.sh`

###[NVM](https://github.com/creationix/nvm)

- Install nodejs: `curl https://raw.github.com/creationix/nvm/master/install.sh | sh`
- `nvm install 0.10` (whichever version we want)

### [Homebrew](http://brew.sh/)

- Install `ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"`

### Ruby: [rbenv](https://github.com/sstephenson/rbenv)

- Install `brew install rbenv ruby-build`
- `rbenv install 2.0.0-p247`
- `rbenv global 2.0.0-p247`

### Ruby: [rubygems](http://rubygems.org/)

- `gem install sass --pre`
- `gem install compass --pre`
- `gem install compass-sourcemaps`

### [Yeoman](http://yeoman.io/)

- Install `npm install -g yo`
- This installs yeoman, grunt and bower

### [gitsh](https://github.com/thoughtbot/gitsh)

### Tools

- `brew install git`
- `brew install tree`

##Apache, PHP, MySQL

Apache

- Apache configuration file included for guidance

PHP

- `brew tap homebrew/dupes`
- `brew tap josegonzalez/homebrew-php`
- `brew install php55 --with-mysql`
- `brew install php55-intl php55-apc php55-mongo php55-memcache`

MySQL

- `brew install mysql --enable-debug`
- `unset TMPDIR`
- ``mysql_install_db --verbose --user=`whoami` --basedir="$(brew --prefix mysql)" --datadir=/usr/local/var/mysql --tmpdir=/tmp``

##Sublime text 3

- [Settings and Packages, sync with dropbox](https://sublime.wbond.net/docs/syncing#dropbox-osx)
- [Package Control](https://sublime.wbond.net/installation#st3) install: `import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())`
- Packages:
	- emmet
	- sass
	- less
	- html/css/js prettify
	- autoprefixer
	- advancednewfile
	- sidebar enhancements
	- trailing spaces
	- sublimelinter
	- bracket highlighter
	- colour theme: Dracula
	- theme: phoenix
- Sublime keymap: `[ { "keys": ["ctrl+s"], "command": toggle_side_bar" } ]`

##Alfred

- [Workflows](https://github.com/zenorocha/alfred-workflows/)


##Acknowledgements

- [https://github.com/mathiasbynens/dotfiles](https://github.com/mathiasbynens/dotfiles)
- [https://github.com/addyosmani/dotfiles](https://github.com/addyosmani/dotfiles)
- [http://remysharp.com/2013/07/25/my-terminal-setup/](http://remysharp.com/2013/07/25/my-terminal-setup/)
- [https://gist.github.com/niepi/1932534](https://gist.github.com/niepi/1932534)


