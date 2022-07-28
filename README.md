# Instalando o Ruby e o Jekyl 

## Instalando o Ruby 2.7.5 (+ devkit package)

1. Acesse o site https://rubyinstaller.org/ e clique em download.  
2. Procure a versão mais nova WITH DEVKIT.  
3. Inicie o instalador e avance até o final.  
4. Após a instalação, um terminal será aberto para instalar o MSYS2 e MINGW  
	<details> 
		<summary>Caso não apareça...</summary>   
		<br>
    <p>Aperte Windows + R para abrir o Executar.</p>
		<p>Digite "cmd" e confirme.</p>
		<p>Execute o comando: ridk install</p>
	</details> 

5. Instale MSYS2 base installation e MINGW developement development toolchain.  
Basta apertar enter quando ele perguntar: "Which components shall be installed? If unsure press ENTER [1,3]"

Para ter certeza que ele foi instalado, digite:

```
ruby -v
```

Se aparecer a versão, significa que está tudo certo.  

## Instalando o Jekyll:

1. Digite no terminal:

```
gem install jekyll bundler
```

Para ter certeza que ele foi instalado, digite:

```
jekyll -v
```

Se aparecer a versão, significa que está tudo certo.


# Iniciando o servidor

```
bundle exec jekyll serve --livereload
```

<details> 
	<summary>Se o comando não mostrar o porta para acessar o site...</summary> 
	<p>verifique se no log apareceu o seguinte erro: "cannot load such file -- webrick (LoadError)"</p>
	<p>Se sim, digite "bundle add webrick" e tente novamente</p>
</details> 
