# sublime_user

Pasta com packages necessários para um bom ambiente.

Como usar:

Instalar o Package Control, executando o seguinte comando no console do Sublime (https://packagecontrol.io/installation):
```
import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

Sincronizar esta pasta com as configurações do Usuário criada em `~/.config/sublime-text-3/Packages/User`.
```
$ cd ~/.config/sublime-text-3/Packages/
$ mv User User_bkp
$ git clone https://github.com/GustavoVS/sublime_user.git User
```

And Be Happy.
