# Proposta de definição sobre formatos de imagens

## Recomendações de aquisição de imagem

* Camera RAW é o formato preferido para gravar imagens da câmera.
* As imagens do scanner devem ser gravadas em 24 bits ou superior a 300-600 ppi no formato TIFF.
* Grave na resolução nativa mais alta disponível para o dispositivo de imagem.
* Ajuste as configurações de balanço de branco para corresponder à fonte de luz.
* Um verificador de cor visível e uma escala são recomendados, conforme apropriado.
* Adobe RGB ou sRGB são os espaços de cores preferidos e devem ser declarados nos metadados.
  * O espaço de cores CMYK deve ser evitado.
* Os nomes dos arquivos de imagem devem ser restritos a caracteres alfanuméricos, sem espaços ou outros caracteres especiais, sublinhado (_) e hífen (–) exceto.

## Recomendações de arquivamento de imagens

* O arquivamento de imagens é fortemente recomendado e visto como uma responsabilidade institucional, regido pela política institucional.
  * Os arquivos de imagem arquivados devem ser mantidos permanentemente em um ambiente seguro e redundante na infraestrutura institucional ou em serviços comerciais de backup.
* DNG não compactado é o formato de arquivamento preferido.
  * As imagens capturadas no formato RAW da câmera proprietária (por exemplo, CR2, NEF, PEF, etc.) devem ser convertidas para o formato Negativo Digital (DNG).
  * A conversão para DNG pode ser realizada via Adobe DNG Converter, disponível gratuitamente em Adobe.com, ou via Adobe Photoshop ou Adobe Photoshop Lightroom.
* TIFF compactado sem compressão ou sem perdas, não modificado em 24 bits ou superior é uma alternativa formato de arquivo.

## Recomendações derivadas de imagem

* As imagens JPEG e JPEG 2000 devem ser salvas em suas dimensões nativas (resolução espacial).
  * Aumentar manualmente a resolução (por exemplo, alterações no tamanho da imagem ou configurações de ppi ou dpi) além da registrada pela câmera pode inserir dados derivados ou artefatos visuais indesejados em um arquivo de imagem e não é recomendado.
* EXIF, IPTC e outros metadados de imagem (incluindo dados JPEG 2000 XML), incluindo aqueles adicionados no momento do processamento, devem ser preservados perpetuamente e distribuídos com todas as cópias derivadas e distribuídas de imagens.
* O processamento de imagem deve ser realizado apenas em arquivos DNG ou outros arquivos RAW para evitar perdas de dados acumuladas e potencial degradação da imagem pelo processamento repetido de arquivos de imagem JPEG e TIFF.
* Manipulação ou composição excessiva de imagens, incluindo nitidez, aumento da saturação de cores ou equilíbrio, e o ajuste do contraste deve ser evitado.

## Recomendações de distribuição de imagens

* As imagens carregadas em agregadores e portais devem ser adequadas para exibição.
  * Imagens de qualidade inferior devem ser distribuídas para agregadores e portais somente quando não houver imagem de qualidade superior acessível.
  * Quando uma imagem de baixa qualidade é carregada ou distribuída, os metadados dessa imagem devem indicar que é a única imagem disponível para esse espécime.

## Recomendações e padrões de formato de arquivo de imagem

* O formato JPEG em resolução nativa e compactação mínima é o preferido para distribuição viaInternet.
  * A compressão sem perdas é preferida.
  * Quando a compactação sem perdas não é uma opção, é preferível a compactação com perdas no nível mais baixo.

>Baseado em: https://www.idigbio.org/content/idigbio-image-file-format-requirements-and-recommendations-1
