# Home_Server
Hey, este é um passo a passo para recriar um servidor assim como tenho em casa.
Criei este github apenas para documentar para não me esquecer dos processos que fiz, mas também para que você se sinta a vontade para refazer e ser feliz com alguns dos benefícios de se ter um servidor :)

Minha ideia original era usar o umbrelOS, mas por algum motivo a iso não se mantinha no computador, após a instalação ao dar reboot, o computador retornava ``No boot device``, então adotei o **Ubuntu Server** junto com **CasaOS**, embora use mais os recursos próprios do Ubuntu Server.

Meu uso do servidor se concentra em **Armazenar arquivos**, **Fazer backups** destes arquivos e também **Hospedar projetos e sites**.

## Requisitos
- 1 Computador que você não se importe em formatá-lo (Desktop ou Laptop)
- 1 unidade de mídia removível (no mínimo 3.0GB)
- Conexão com rede (Ethernet ou Wifi)
- um ou mais nerds disponíveis
  
## Inicio rápido
Conecte a mídia removível em um computador e formate-o como dispositivo Bootável com o Sistema Operacional [Ubuntu Server](https://ubuntu.com/download/server#system-requirements-lts) (se você usar um Flash Drive como eu, recomendo usar [Rufus](https://rufus.ie/pt_BR/) ou [Ventoy](https://www.ventoy.net/) para isso e coloque a iso do Ubuntu no dispositivo), certifique-se que o computador-servidor atenda aos requisitos do Ubuntu Server.

Conecte a mídia bootável no computador que será o servidor e faça a instalação, eu personalizei as partições para maximizar o armazenamento de arquivos, pois pretendia armazenar um volume de dados considerável, mas você pode personalizar como queira ou seguir com o particionamento padrão.

Haverá uma parte na instalação perguntando se você deseja instalar o OpenSSH, eu recomendo que aceite a instalação para se conectar rapidamente no servidor, mas fica a seu critério não instalar ou instalar depois.

Quando terminar a instalação do Sistema Operacional, desligue o computador e remova a mídia bootável.

* Tcharam! Servidor instalado!

Ligue o servidor, aguarde iniciar e faça seu login de usuário.

Faça a instalação do [CasaOS](https://casaos.io/) e aguarde o fim da instalação. O endereço IP será exibido no terminal, digite este endereço IP no seu navegador e crie seu usuário e senha.

Pronto, simples e rápido, você já pode instalar alguns aplicativos na App Store e fazer uso deles.

## Configurações pessoais
Nessa seção conterá algumas configurações que defini no meu servidor, você pode fazer o mesmo ou alterar algum detalhe ou quem sabe fazer sua própria configuração e compartilhar ^-^
### Configuração de SSH
Fiz este com o auxílio do Github
* Abra o Git Bash
* Digite do painel o comando ``ssh-keygen -t ed25519 -C "email_bacanudo@email.bacanudo"``, insira o mesmo email que você tenha uma conta github
* Siga os passos exibidos no painel e insira a sua frase-chave
* Acesse o arquivo gerado, caminhando até o diretório do arquivo, abra-o e copie todo o conteúdo
* Entre na Github Web, acesse a configuração da sua conta e registre a sua chave SSH, no campo ```key``, cole o conteúdo copiado do arquivo.
