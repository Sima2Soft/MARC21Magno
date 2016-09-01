# MARC21Magno
O MARC21Magno é uma máquina para criar e traduzir registros no formato MARC21

# Introdução

O formato MARC é um conjunto de códigos e designações de conteúdos definido para codificar registros que serão interpretados por máquina. Sua principal finalidade é possibilitar o intercâmbio de dados, ou seja, importar dados de diferentes instituições ou exportar dados de sua instituição para outros sistemas ou redes de bibliotecas através de programas de computador desenvolvidos especificamente para isto.

Um registro MARC é composto por três elementos: estrutura, indicação do conteúdo e conteúdo propriamente dito. A estrutura do registro é uma implementação dos padrões internacionais ANSI Z39.2 e ISO 2709. As indicações de conteúdo são códigos e convenções estabelecidos para identificar e caracterizar os dados dentro do registro e permitir sua manipulação.Os conteúdos dos dados que compõe um registro MARC geralmente são definidos por padrões externos ao formato, como: International Standard Bibliographic Description (ISBD), Anglo-American Cataloguing Rules (AACR2), Library of Congress Subject Headings (LCSH) ou outros códigos usados pela instituição criadora do registro.

O formato MARC 21 para dados bibliográficos inclui informação sobre material textual impresso ou manuscrito, arquivo de computador, mapas, música, recurso contínuo, material visual e material misto; os dados bibliográficos normalmente incluem título, nome, assunto, nota, dado de publicação e descrição física.

Livro (BK) - usado para material textual impresso, eletrônico, manuscritos e microformas, por natureza monográfico, por exemplo: livros, teses, etc.;

Recurso Contínuo (CR) - usado para material textual impresso, eletrônico, manuscritos e microformas, com publicação frequente, por exemplo, periódicos, jornais e anuários. Até 2002 era designado como Publicação Seriada (SE);

Arquivo de Computador (CF) - usado para programas de computador (softwares), dados numéricos, arquivos multimídias desenvolvidos para computador, serviços e sistemas on-line. Outros tipos de recursos eletrônicos são codificados de acordo com seu aspecto mais relevante;

Mapas (MP) - usado para todos os tipos de material cartográfico - impresso, eletrônico, manuscritos e microformas, incluindo mapas planos e globos;

Música (MU) - usado para música impressa, eletrônica, manuscritas e microformas, registros sonoros musicais e não-musicais;

Material Visual (VM) - usado para mídias projetáveis e não projetáveis, gráficos bi-dimensionais, artefatos tri-dimensionais ou objetos naturais e kits;

Material Misto (MX) - usado para documentos com formas mistas principalmente para coleções de arquivos e manuscritos. Até 1994, Material Misto (MX) era designado como Material de Arquivo e Manuscrito (AM).

Todos estes materiais, podem ser monográficos ou seriados, dependendo da sua característica.

# Tipos de registros bibliográficos

Os tipos de registro e de material são especifícados através de códigos, indicados no Líder 06 (Tipo de material), que identificam os seguintes tipos de registro bibliográfico:

Material textual
Material manuscrito
Arquivo de computador
Material cartográfico impresso
Material cartográfico manuscrito
Música impressa
Música manuscrita
Gravação de som não musical
Gravação de som musical 
Mídia projetável
Material gráfico não projetável
Artefatos tridimensionais e objetos da natureza
Kit
Material misto

Microformas, sejam elas originais ou reproduções, não são identificadas como um tipo especial de registro. A microforma é um aspecto secundário do material original, por exemplo a microforma de um livro. O mesmo se aplica para Arquivo de computador.

# Componentes do Registro Bibliográfico

Um registro bibliográfico em formato MARC é composto de três elementos principais: o Líder, o Diretório e os Campos Variáveis.

Líder - contém informações que possibilitam o processamento do registro; apresenta números e códigos que são identificáveis pela sua posição; compreende as 24 primeiras posições de um registro.

Diretório - apresenta uma série de entradas de tamanho fixo, uma para cada campo variável do registro. Cada entrada possui 12 posições e apresenta três partes: a tag ou etiqueta do campo, o tamanho docampo e a posição inicial do campo. O Diretório vem em seguida ao Líder e está localizado na posição 24 do registro, sendo gerado automaticamente.

Campos Variáveis - os dados ou informação do registro estão organizados em campos variáveis ou de conteúdo variável, cada um identificado por uma tag ou etiqueta composta por três caracteres numéricos. Existem dois tipos de campos variáveis:

campos de controle - que são os campos 00X; não contém indicadores nem sub-campos;

campos de dados - são agrupados em blocos, de acordo com o primeiro caractere da tag; o tipo de informação no campo é identificado pelos caracteres restantes da tag. Apresenta dois tipos de designação de conteúdo: indicadores, as duas primeiras posições no campo de dados variáveis; são representados por um caractere numérico ou alfabético minúsculo; e os códigos de sub-campos, representados por dois caracteres que distinguem as informações dentro do campo; aprsenta um delimitador ($) e um identificador de dados - que pode ser um caractere numérico ou alfabético minúsculo.

# Repetitividade de campos e subcampos

Teoricamente, todos os campos (exceto o 001 - número de controle) e 005 (data e hora da última atualização) e subcampos podem ser repetidos. A natureza do dado, entretanto, não permite a repetitividade. Por exemplo, um registro do formato bibliográfico pode conter somente um título principal, ou seja o campo 245 subcampo $a não é repetitivo.

A repetitividade ou não de um campo ou subcampo está representada pelas abreviaturas R (Repetitivo) e NR (Não Repetitivo), apresentadas ao lado de cada campo e subcampo.

Níveis de Catalogação

O formato MARC21 apresenta dois níveis de catalogação, utilizados nos EUA: nacional e mínimo. Os registros com nível nacional contém informações de catalogação suficientes para permitir o uso por várias agências nacionais e internacionais. Os registros com nível mínimo de catalogação contém apenas informações essenciais, embora informações adicionais possam ser fornecidas.

São utilizados códigos para indicar a exigência ou não de um determinado dado ou informação no registro:

A - Obrigatório, se aplicável: a informação referente aquele campo ou subcampo deve estar presente se a utilização dos mesmos for apropriada ao documento que está sendo descrito e se a informação estiver disponível;

M - Obrigatório: é obrigatória a utilização do campo ou subcampo;

O - Opcional: a utilização do campo ou subcampo é opcional.

Caractere cheio e valores relacionados

Um caractere cheio (ASCII 7C hex), representado neste documento por uma barra vertical (|), pode ser utilizado em um registro quando o formato especifica que deve-se utilizar um código, porém o criador do registro decide não fornecer este código. Este caractere não deve ser utilizado em nenhuma posição do Líder, tags, indicadores ou códigos de subcampos.

O código u - desconhecido ou não especificado - é utilizado para indicar que o criador do registro tentou fornecer um código, porém não foi capaz de determinar o código apropriado.

O código n - não se aplica - é utilizado para indicar que as características definidas pela posição não se aplicam ao tipo específico de documento ou registro.

Convenções Tipográficas

0 – representa o dígito zero nas etiquetas, campos fixos e indicadores e outros lugares numéricos. Não confundir com a letra “O” maiúscula, em exemplos e textos.

"#" - é usado para espaço em branco em campos codificados e em outras situações especiais, onde a existência do espaço em branco poderia ser ambígua.

$ - indicador de subcampo – utilizado como delimitador de código de subcampo. No texto, os códigos de subcampo são indicados como subcampo $a, por exemplo.

/ (barra diagonal) – posições específicas de caracteres do Líder, Diretório, campo 007 e 008, subcampo $7 dos campos de entradas de ligação são expressas utilizando-se uma barra e o número da posição do caractere. Exemplo: Líder/06, 007/00, 008/12.

1 – o símbolo gráfico 1 representa o número 1. Não confundir com a letra i “I” maiúscula e a letra L “l” minúscula.

| (barra vertical) – representa um caractere cheio em exemplos do MARC para casos em que um código pode ser usado mas o criador do registro decide não fornecê-lo. Podemos utilizá-lo nos campos 006, 007 e 008 e subcampo $7 do campo 533 e nas entradas de ligação (760-787). Não utilizamos este símbolo no Líder, nas tags, nos indicadores ou nos códigos de subcampos.

Fonte: http://www.dbd.puc-rio.br/MARC21/conteudo.html
