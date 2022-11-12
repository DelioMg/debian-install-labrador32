#Instalando um sistema na labrador32

Para instalar um novo sistema na sua placa Labrador você vai precisar de  Cartão microSD de pelo menos 4Gb


A instalação deve seguir conforme abaixo:

1. Primeiramente você deve baixar a imagem em Labrador 32 bits no repositorio da caninosloucos ou esse aqui.

2. Depois você deve descompactar os arquivos.

3. Após descompactar deve escrever a imagem em um cartão microSD utilizando o comando dd no Linux ou o software Win32 Disk Imager no Windows.

4. Remova a labrador da fonte de alimentação, insira o cartão SD na Labrador, mantenha o botão de recuperação da Coreboard (no canto superior esquerdo da Coreboard, próximo à etiqueta de número de série) pressionado, conecte a fonte de alimentação, espere próximo de 3 segundos ou até o logo aparecer na tela e solte o botão de recuperação.

5. O sistema será iniciado a partir do cartão. Para conferir utilize o comando $lsblk, o dispositivo em mmcblk0p1 (Cartão SD) deverá estar montado na raiz do sistema, e o dispositivo mmcblk2 (memória interna da labrador) pode estar ou não montada.

6. Para instalar o sistema abra o terminal e execute o comando;

$ cd install

$ sudo ./install32_labrador.sh

8. Aguarde o processo ser finalizado, desligue a Labrador, remova o cartão SD e religue a placa.

9. Após a placa ligada vá em system Tools e entre em Disk Managemt.

10. Selecione SD Card Read(QX63AB) e nas engrenagens selecione Resize...

11. Selecione o tamanho que quer expandir a  partição e aperte em Resize.

Tutoria Base retirado da pagina wiki.caninosloucos.org



