# Infraestrutura

## Componentes

Uma instalação de Specify é composta pelas seguintes componentes:

- __Specify 6__ - software de gestão da colecção, desenvolvido em Java;
- __Java__ (JRE ou JDK versão 8) - framework necessária para executar o Specify 6;
- __MySQL__ ou __MariaDB__ - gestor de base de dados.

Adicionalmente, pode incluir ainda as seguintes componentes:

- __Specify 7__ - gestão da colecção através do browser de internet. Este partilha a base de dados com o Specify 6;
- __Specify Web__ - serviço para consulta pública da colecção através da internet. Os dados são indexados através de Apache Solr;
- __Specify Attachment Server__ - serviço implementado num servidor dedicado para gestão dos anexos em ambiente de rede.

O Sistema Specify pode ser implementado em vários sistemas operativos: Windows, MacOS ou Linux, ou em ambientes mistos, e.g., Specify 6 em desktops Windows, mas base de dados ou outros serviços em Linux.

## Instalação *Stand Alone*

A instalação de __Specify 6__ _Stand Alone_ é adequada para a gestão de colecções de pequena dimensão, geridas apenas por um curador ou gestor de dados.

Neste tipo de infraestrutura, todos os componentes (Specify 6, Java, MySQL e armazenamento de anexos) estão instalados no mesmo computador desktop ou laptop. Uma vez que a instalação é para ser usada apenas por um utilizador, a colecção em Specify pode ser criada com ou sem a segurança activa (no segundo caso, não é necessário fazer login ao abrir o Specify).

Ver mais informação no [Webinar 2 GBIF CESP Specify 6](https://youtu.be/lstA02yTkHI?t=1576).

## Instalação *Cliente-Servidor*

A instalação de __Specify 6__ _Cliente-Servidor_ é adequanda para a gestão de colecções de maior dimensão, com vários curadores e/ou gestores de dados a gerir a base de dados.

Neste  tipo de instalação, a base de dados __MySQL__ ou __MariaDB__ está instalada num servidor dedicado, ao qual se ligam vários computadores desktop ou laptop "clientes", nos quais está instalado o Specify 6 e Java. Neste caso, é possível o acesso simultâneo de vários utilizadores à mesma colecção. Os anexos podem ser armazenados num dos computadores (numa pasta partilhada), ou num servidor onde seja instalado o serviço [_Specify Attachment Server_](https://github.com/specify/web-asset-server).

Ainda neste tipo de instalação, é possível fazer a gestão da colecção através de um servidor de __Specify 7__. O Specify 7 permite realizar a maioria das operações - adição e edição de registos de espécimes, pesquisas, empréstimos, relatórios - que são realizadas com Specify 6 através de um browser. A sua utilização é ideal quando seja necessário fazer a gestão da colecção de modo remoto.

Ver mais informação no [Webinar 2 GBIF CESP Specify 6](https://youtu.be/lstA02yTkHI?t=1615).

### Armazenagem

O espaço global de armazenamento é composto por várias componentes, muito provavelmente distribuidas por vários servidores/computadores. Estas componentes são:

1. __Base de dados__

O armazenamento necessário para a base de dados é composto por:
- instalação do software MySQL (~400 MB)
- base de dados - como exemplo, uma colecção de herbário com 75 mil registos ocupa 488 MB.

2. __Armazenamento de Anexos__

Para o armazenamento de anexos com um servidor [_Specify Attachment Server_](https://github.com/specify/web-asset-server), o espaço necessário depende directamente do total de ficheiros anexados. Para cada registo, o Specify permite a anexação de imagens de espécimes ou documentos em diferentes formatos (pdf, doc), associados ao espécime, ou a componentes e operações de gestão realizadas sobre este (determinações, localização, preparações, empréstimos, etc.). O armazenamento total necessário depende, por isso, do fluxo de trabalho implementado na colecção.

A título de exemplo, para uma __colecção de herbário__, onde foram anexadas apenas as imagens dos espécimes digitalizados, o armazenamento total por espécime é a soma das seguintes parcelas:

| Tipo de ficheiro | Formato | Resolução (dpi) | Dimensão  (px)  | Tamanho |
|------------------|---------|-----------------|-----------------|---------|
| original         | tiff    | 400             | 5574x7370       |  120 MB |
| cópia web*       | jpeg    | 400             | 5574x7370       |   18 MB |
| thumbnail        | png     |                 | 93x123          |   16 KB |
|                  |         |                 |           TOTAL |  138 MB |

*é necessária a criação de uma versão jpeg que facilite a publicação através da web.

3. __Specify 7__

Os requisitos de armazenamento para uma instalação de Specify 7 estão associados à implementação da aplicação web Specify 7, que inclui a instalação de Specify 6. Se a base de dados estiver instalada num servidor dedicado, então o armazenamento não deverá crescer na proporção do número de registos da base de dados. O armazenamento necessário para uma instalação típica é 130 MB.

### Processamento

### Conectividade

