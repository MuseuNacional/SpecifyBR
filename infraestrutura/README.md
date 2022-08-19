# Infraestrutura

## Instalação *Stand Alone*

## Instalação *cliente-servidor*

### Armazenagem

O armazenamento global é composto por várias componentes, muito provavelmente distribuido por vários servidores/computadores. Estas componentes são:

1. __Base de dados__

O armazenamento necessário para a base de dados é composto por:
- instalação do software MySQL (~400 MB)
- base de dados - como exemplo, uma colecção de herbário com 75 mil registos ocupa 488 MB.

2. __Armazenamento de Anexos__

Para o armanezamento de anexos com um servidor [_Specify Attachment Server_](https://github.com/specify/web-asset-server), o espaço necessário depende directamente do total de ficheiros anexados. Para cada registo, o Specify permite a anexação de imagens de espécimes ou documentos em diferentes formatos (pdf, doc), associados ao espécime, ou a componentes e operações de gestão realizadas sobre este (determinações, localização, preparações, empréstimos, etc.). O armazenamento total necessário depende, por isso, do fluxo de trabalho implementado na colecção.

A título de exemplo, para uma __colecção de herbário__, onde são anexadas apenas as imagens dos espécimes digitalizados, o armazenamento total por espécime é a soma das seguintes parcelas:

| Tipo de ficheiro | Formato | Resolução (dpi) | Dimensão  (px)  | Tamanho |
|------------------|---------|-----------------|-----------------|---------|
| original         | tiff    | 400             | 5574x7370       |  120 MB |
| cópia web*       | jpeg    | 400             | 5574x7370       |   18 MB |
| thumbnail        | png     |                 | 93x123          |   16 KB |
|                  |         |                 |           TOTAL |  138 MB |

*é necessária a criação de uma versão jpeg que facilite a publicação através da web.

### Processamento

### Conectividade

