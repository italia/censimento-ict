# Docs Italia Theme
Tema per documentazione di Docs.Italia.IT

## Come utilizzare il tema nella propria documentazione

Le operazioni vanno eseguite dentro la cartella del documento su cui si sta lavorando e il documento deve essere già un repository git inizializzato e configurato (git init... add origin...) 

### Aggiungere il repo del tema e caricarlo
```
git submodule add https://github.com/italia/docs-italia-theme.git themes
git commit -m "add docs italia theme"
git push origin master
```

### Copiare conf.py.sample
```
cp themes/conf.py.sample conf.py
```

### Modificare conf.py
```
# -- PROJECT Variables ----------------------------------------------------
settings_project_name = 'nome documento'
settings_copyright_copyleft = 'copyright o copyleft - pa'
settings_editor_name = 'nome pa esteso'
settings_doc_version = 'versione 1...2...3'
settings_doc_release = 'versione 1...1.1...2.1'
settings_basename = 'nome progetto senza spazi'
settings_file_name = 'nome progetto senza spazi'
settings_project_url = 'https://xxx.xxxxxxxxx.xxx'
```

Il conf.py è già configurato per funzionare nelle cartelle definite in questa guida. Eventuali personalizzazioni e aggiunta funzionalità devono essere riportate nel conf.py

### Aggiornare il tema
```
cd themes
git pull origin master
```



