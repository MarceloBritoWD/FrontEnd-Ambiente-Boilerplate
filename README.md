# Getting Started


##Intalação do [nodeJS](https://nodejs.org/en/)

Instale a ultima versão do nodejs pelo seguintes comandos (npm vem junto):

```sh
curl -sL https://deb.nodesource.com/setup | sudo bash -
sudo apt-get install nodejs
```



##Instalação do [SublimeText3](http://www.sublimetext.com/3)

```sh
sudo add-apt-repository ppa:webupd8team/sublime-text-3
sudo apt-get update
sudo apt-get install sublime-text-installer
```

####Preferências de Usuário:

Em [Preferences > Settings - User] Cole o seguinte objeto:

{
	"font_size": 8,
	"tab_size": 2,
	"bold_folder_labels": true,
	"highlight_line": true,
	"ignored_packages":["Vintage"]
}


####[Package Control](https://packagecontrol.io/)

Instale o Gerenciador de pacotes do SublimeText3.

- Va em [View > Show Console]
- Cole o seguinte codigo no console

```sh
import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```
- Para instalar os pacotes pressione [CTRL + SHIFT + P] digite [install package] irá aparecer a opção "Package Control: Install Package", em seguida procure o pacote desejado.


##Instalação do [Git](https://git-scm.com/)
```sh
sudo apt-get install git
```

##Instalação do [Grunt](http://gruntjs.com/) + [Gulp](http://gulpjs.com/) + [Bower](http://bower.io/)
```sh
[sudo] npm install -g grunt-cli gulp-cli bower
```

####Agora é só dar init na aplicação :)