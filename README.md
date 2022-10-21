# SpecifyBR
Boas práticas para o uso do [Specify](https://github.com/specify) na organização das informações das coleções zoológicas brasileiras e de língua portuguesa

## Instalação
Para o passo a passo detalhado, acompanhar o vídeo do Rui figueira no canal do SiBBr no YouTube: https://youtu.be/Y78e9PD6RfM

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

Para criar uma coleção, é preciso rodar o SpWizard_64, que foi instalado junto com o Specify.  
IT Username: root  
IT password: a senha que você criou na instalação do mysql  
Database name: o nome que a pasta da base de dados vai ter no SQL  
Clicar em "Create Specify Database" e aguardar.  

O próximo passo é criar o Master User. Esse é o usuário que vai conectar o Specify com a base de dados no mySQL. Os outros usuários das bases de dados serão criados depois, mas algumas ações no Specify pedem a senha do Master User, por isso é importante anotar essas informações (lembrando que o Master Username não pode ser o mesmo que o UserName)  
Depois de definir o nome e a senha do Master User, o Wizard vai perguntar se você quer usar uma ligação segura. Ao marcar que sim, você pode criar vários usuários e dar permissões diferentes de acesso à base de dados a cada um deles.  
O passo seguinte é criar um usuário comum para a base de dados.  
Em seguida, ele vai pedir os dados da Instituição. Os campos em negrito são obrigatórios. Essas informações podem ser atualizadas posteriormente.  
A próxima pergunta é sobre os registros de entrada. Marcando "manage Globally", eles serão geridos em nível institucional. Deixando desmarcado, a gestão será no nível da Divisão (ou Departamento).  
A seguir, selecionar o formato do registro de entrada.  
Configurar a árvore de armazenamento (pode ser alterada depois).  
Criar instituição.  
Após a criação da instituição, será criada a divisão (ou departamento).  
Dentro da divisão, será selecionada a disciplina (o Specify tem configurações diferentes para cada disciplina) e a árvore taxonômica.  
Alguns grupos têm catálogos disponíveis para serem pré carregados.  
Por fim, configurar a árvore geográfica.  

Agora começa a criação da coleção.  
Após o nome e o código, deve-se definir o formato do número de tombo. Recomenda-se usar o CatalogNumberNumeric auto incrementado.  
Ao final das configurações, o Wizard exibe um sumário das informações da sua coleção. É recomendável salvar um pdf desse sumário para eventuais consultas (esse sumário contém inclusive as senhas, portanto é bom mantê-lo em um lugar seguro).  

O último passo é clicar em "Build Database" e aguardar a conclusão.  


## Configuração

## Importando Planilhas para o Specify
O Specify aceita a importação de planilhas através do Workbench, até 4000 registros por vez.
