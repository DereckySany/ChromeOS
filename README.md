# ChromeOS
Scripts para instalação fácil do Chrome OS:
1) É o mesmo que Neverware Cloudready, Flint OS, Bliss OS ou FydeOS?
Não, não é, é o Chrome OS oficial completo, incluindo aplicativos Android, Linux, Google Assistant, Chrome Sync, que geralmente não está disponível nestas versões.

2) Estou preso no logotipo do Google.
Seu arquivo de imagem de recuperação pode estar corrompido. Portanto, baixe-o novamente e siga o procedimento novamente.

3) Meu disco rígido tem um nome diferente de sda.
Você pode editar o script install.sh e substituir "sda" pelo nome do seu disco rígido.
ou digite os seguintes comandos linha por linha no terminal e substitua o nome do seu hdd por "sdX"
sudo apt update
sudo apt install pv
sudo apt install cgpt
sudo chromeos-install.sh -src rammus_recovery.bin -dst /dev/sdX   

4) Não consigo inicializar.
Verifique as configurações do BIOS e desative a inicialização segura, CSM, modo Legecy e ative a opção de inicialização UEFI

5) Quero fazer um boot duplo do Chrome OS com o Windows 10.
Informe nos comentários abaixo para que eu possa fazer um vídeo separado para inicialização dupla do sistema operacional Chrome com Windows 10.

6) ERRO "cgpt precisa ser instalado primeiro"
Certifique-se de estar conectado à Internet antes de executar o script de instalação.

7) Os aplicativos Linux (crostini) não estão funcionando, como faço para corrigir isso?
Verifique se você habilitou todas as opções relacionadas à virtualização em seu BIOS (Ex: "Intel Virtualization", "VT-x", "VT-e" etc ...) (você deve)

8) Preciso instalar o android no pc separadamente?
Nenhum Chrome OS oficial vem com o Android x86, então você não precisa mais de nenhum software de emulação do Android.

9) Tenho CPU não baseada em Intel. Posso instalar?
Não, a partir de agora, CPUs não baseadas em Intel não são suportadas
