# Como instalar alguns app linux

## .tar.xz
    Exemplo 1:
        wget https://nodejs.org/dist/vXX.XX.XX/node-vXX.XX.XX-linux-x64.tar.xz
        tar -xf node-vxx.x.x-linux-x64.tar.xz
        sudo mv node-vxx.x.x-linux-x64 /usr/local/node (ou /opt)    
        echo 'export PATH=/usr/local/node/bin:$PATH' >> ~/.bashrc
        source ~/.bashrc

	exemplo 2:

        tar -xf vlc-ide-*.tar.xz
        sudo mv vlc /opt/
        cd /opt/vlc/bin
        ./studio.sh
        echo 'export PATH=$PATH:/opt/vlc/bin' >> ~/.bashrc
        source ~/.bashrc

## .bundle
	acessa o diretorio do arquivo
	chmod +x arquivo_desejado.bundle
	
	ubuntu:
        sudo ./arquivo_desejado.bundle
        sudo apt install build-essential linux-headers-generic
	
	debian:
        sudo apt install perl build-essential gcc make
        para debian: sudo ./nome_arquivo.bundle

## .run
	chmod +x app.run
	./app.run
	
	Criar .desktop
	nano ~/.local/share/applications/nome-do-aplicativo.desktop

        [Desktop Entry]
        Name=Nome do Aplicativo
        Exec=/home/sousa/Documents/apps/genymotion/genymotion
        Icon=/home/sousa/Documents/apps/genymotion/icons/genymotion-logo.png
        Terminal=false
        Type=Application
        Categories=Utility;


