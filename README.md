# SpecifyBR
Boas práticas para o uso do [Specify](https://github.com/specify) na organização das informações das coleções zoológicas brasileiras e de língua portuguesa

## Instalação
Para o passo a passo detalhado, acompanhar o vídeo do Rui figueira no canal do Sibbr no YouTube: https://youtu.be/Y78e9PD6RfM

Instalação do MySQL: downloads.mysql.com/archives/installer/ (não pode ser a versão 8; o Rui Figueira ensina usando a versão 5.7.35)

Configurações de instalação (quando não houver observações aqui, apenas ir clicando Next)
"Choosing a setup type": Server only
"Type and Networking": Development computer (computador com mais de um uso, não só para o Specify)
"Accounts and Roles": Criar senha do administrador do SQL (o usuário é sempre root). Anotar a senha, porque vai ser pedida na instalação do Specify

Instalação do Amazon Corretto (Java): 
Para Windows: https://corretto.aws/downloads/latest/amazon-corretto-8-x64-windows-jre.msi
outros SO: https://docs.aws.amazon.com/corretto/latest/corretto-8-ug/downloads-list.html

Não tem mistério. É só ir clicando em Next até terminar.

Instalação do Specify: 
Windows 64 bit: https://update.specifysoftware.org/Specify_windows_64.exe	
macOS 10.7.3+: https://update.specifysoftware.org/Specify_macos.dmg
Linux 64 bit: https://update.specifysoftware.org/Specify_unix_64.sh

Também é bem simples, só ir clicando em Next até concluir.



## Configuração

## Importando Planilhas para o Specify
O Specify aceita a importação de planilhas através do Workbench, até 4000 registros por vez.
