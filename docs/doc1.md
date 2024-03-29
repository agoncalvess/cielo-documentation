---
id: doc1
title: Documentação e Tutoriais Cielo
sidebar_label: Example Page
layout: manuals
---

# Documentação Cielo LIO

Nessa documentação você tem acesso a todas as informações sobre a plataforma Cielo LIO e boas práticas para o desenvolvimento e modelos de integração disponíveis para complementar o negócio de seu cliente.

O objetivo dessa documentação é facilitar o processo de desenvolvimento fornecendo os materiais necessários para realizar a integração com a Cielo LIO e todos os conceitos sobre a Cielo Store, a loja de aplicativos da Cielo disponível na Cielo LIO.

# Visão Geral da Plataforma

### Cielo LIO

É uma plataforma aberta que fornece controle e gestão de negócios indo além de um sistema de pagamentos tradicional. Essa solução suporta aplicativos desenvolvidos para sistema Android, possibilitando que desenvolvedores parceiros possam criar aplicativos especializados para diversos segmentos e qualquer porte de cliente.

A LIO conta com duas opções de hardware, com e sem impressão.

### Cielo LIO+

Solução 2 em 1, a primeira do segmento a oferecer smartphone e maquininha de cartão em um único aparelho, com o objetivo de digitalizar o pequeno negócio.

A Cielo LIO+ oferece mobilidade e praticidade ao vendedor. Isso porque ela é 2 em 1: o mesmo equipamento opera como um smartphone, com todas as suas funções de voz e aplicativos, e uma maquininha de cartão que se conecta de maneira rápida e intuitiva ao celular com um simples snap (encaixe magnético que oferece uma conexão imediata entre o celular e o módulo de pagamento), diferente das soluções que exigem o pareamento via bluetooth, por exemplo.

Ambas contam com a Cielo Store, loja de aplicativos B2B disponível em todos as LIO´s, dando escala e distribuição para qualquer aplicativo integrado a ela.

## Modelos disponíveis da Cielo LIO

Atualmente a Cielo LIO está disponível em 3 modelos: LIO V1, LIO V2 e LIO +

![Comparação - LIO V1 e LIO V2](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/lio_v1_v2.png)
![BLUE](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/blue_lio.png)

Ambos os modelos foram desenvolvidos pela Cielo pensando em atender as necessidades específicas de alguns clientes.

Enquanto a LIO V1 possui um design mais compacto e permite uma maior mobilidade, a LIO V2 foi concebida em um tamanho maior e possui algumas funcionalidades exclusivas e adicionais como por exemplo:

**Impressora térmica**: o cliente poderá ter a 1ª e 2ª via impressa após o pagamento realizado. Além disso, as aplicações parceiras poderão utilizar os métodos disponíveis da impressora para imprimir dados importantes ou necessários para o negócio do cliente.

Especificação da Bobina:
Papel Azul 48 gramas, Comprimento: 12 metros, Diâmetro máximo: 30 milímetros, Largura: 57 milímetros.

**NFC**: tecnologia presente permitindo o pagamento utilizando cartões com tecnologia contactless.

## Arquitetura

### Sobre

A plataforma Cielo LIO é baseada em Android que consiste em:

- Uma loja de aplicativos [Cielo Store](https://developercielo.github.io/manual/cielo-lio#cielo-store) para os desenvolvedores publicarem seus aplicativos e os disponibilizarem para os estabelecimentos comerciais (lojistas).
- Uma plataforma com arquitetura em nuvem e APIs REST que permite a integração com sistemas de automação comercial de parceiros.
  Acesse Documentação da [Integração Remota](https://developercielo.github.io/manual/cielo-lio#integra%C3%A7%C3%A3o-remota)
- Um SDK para desenvolvimento em Android, de forma que aplicativos de parceiros possam se integrar com as funcionalidades de pagamento da Cielo LIO.
  Acesse Documentação da [Integração Local](https://developercielo.github.io/manual/cielo-lio#integra%C3%A7%C3%A3o-local)

### Modelos de integração com a plataforma Cielo LIO

#### Integração Remota | Cielo LIO Order Manager

Conjunto de APIs que permitem que o cliente continue utilizando sua solução de PDV / Automação Comercial com todas as funcionalidades. No momento de realizar o pagamento, ocorre a integração com o gerenciador de pedidos (Order Manager) da Cielo LIO, de forma rápida, simples e segura.
[Ir para integração remota](https://developercielo.github.io/manual/cielo-lio#integração-remota)

#### Integração Local | Cielo LIO Order Manager SDK

A Cielo disponibiliza um SDK com base na Cielo LIO Order Manager API que permite ao desenvolvedor e parceiro Cielo LIO integrar em sua aplicação as funcionalidades da Cielo LIO.
[Ir para integração local](https://developercielo.github.io/manual/cielo-lio#integração-local)

### Serviços periféricos

A Cielo LIO também se integra com os seguintes periféricos de hardware:

**Impressoras Bluetooth**

No caso da LIO V1 é possível conectar a Cielo com impressoras bluetooth para realizar a impressão de recibos e outras informações importantes.

Já existem parceiros que estão utilizando impressoras Bluetooth das marcas Zebra, Datex, Leopardo integradas com a Cielo LIO.

Todos os protocolos de comunicação e pareamento ficam sob responsabilidade do aplicativo do parceiro.

**Leitores de RFID**

Já existem parceiros que estão utilizando leitores RFID em suas soluções.

Todos os protocolos de comunicação e pareamento ficam sob responsabilidade do aplicativo do parceiro.

## Especificações técnicas do hardware da Cielo LIO

A plataforma Cielo LIO teve seu sistema operacional próprio baseado em Android.
Confira abaixo a tabela com as especificações técnicas da Cielo LIO:

|                      | ![LIO V1](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/lio_v1_small.png) | ![LIO V2](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/lio_v2_small.png) | ![LIO V2](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/lio_small.png) |
| -------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Versão               | **LIO V1**                                                                                      | **LIO V2**                                                                                      | **LIO +**                                                                                    |
| Sistema operacional  | Android OS Cielo 5.1.1                                                                          | Android OS Cielo 6.0 (Marshmallow)                                                              | Android 8.1 Oreo                                                                             |
| Memória              | 2GB LPDDR3                                                                                      | 1GB LPDDR3                                                                                      | 2GB                                                                                          |
| Armazenamento        | -                                                                                               | -                                                                                               | 16GB expansível (80GB micro SD)                                                              |
| Dual Chip            | Dual SIM Stand-by                                                                               | -                                                                                               | Dual Chip                                                                                    |
| Frequência           | 2.4 GHz                                                                                         | 2.4 GHz                                                                                         | 2.4 GHz                                                                                      |
| Tipo do SIM Card     | micro SIM (3FF)                                                                                 | micro SIM (3FF)                                                                                 | micro SIM e/ou Nano SIM                                                                      |
| Frequência GSM Mhz   | Quad-Band 850/900/1800/1900                                                                     | Quad-Band 850/900/1800/1900                                                                     | Quad-Band 850/900/1800/1900                                                                  |
| Tamanho em polegadas | 5"                                                                                              | 5.5"                                                                                            | 6"                                                                                           |
| Tipo de tela         | AMOLED                                                                                          | AMOLED                                                                                          | AMOLED                                                                                       |
| Resolução da tela    | 720 x 1280 pixels                                                                               | 720 x 1280 pixels                                                                               | LCD 6" HD+ 1440x720 pixels                                                                   |
| Densidade de pixels  | 293 ppi                                                                                         | 267 ppi                                                                                         | 268 ppi                                                                                      |
| Câmera               | 12.8 Mega Pixels                                                                                | 13 Mega Pixels                                                                                  | 12 Mega Pixels                                                                               |
| Resolução da câmera  | 4128 x 3096 pixels                                                                              | 4160 x 3120 pixels                                                                              | 12MP LED flash Zoom digital x4 08MPLED flash Zoom digital x4                                 |
| Flash                | Flash LED                                                                                       | Flash LED                                                                                       | Flash LED                                                                                    |
| USB                  | USB 2.0 Micro-B (Micro-USB) Somente Energia                                                     | USB 2.0 Micro-B (Micro-USB) Somente Energia                                                     | Micro USB 2.0                                                                                |
| Bluetooth            | Versão 4.0 com A2DP                                                                             | Versão 4.0 com A2DP/LE                                                                          | Versão 4.1 suporta LE                                                                        |
| WiFi                 | 802.11 a/b/g/n (2.4GHz)                                                                         | 802.11 b/g/n (2.4GHz)                                                                           | 802.11b/g/n (2.4GHz)                                                                         |
| GPS                  | A-GPS. GeoTagging                                                                               | A-GPS                                                                                           | A-GPS                                                                                        |
| Sensores             | Acelerômetro, Proximidade e Luminosidade                                                        | Acelerômetro, Proximidade e Luminosidade                                                        | Leitor de digitais, acelerômetro, luminosidade e proximidade                                 |
| Saída de áudio       | Audio Jack 3.5mm                                                                                | Audio Jack 3.5mm                                                                                | Audio Jack 3.5mm                                                                             |
| Peso                 | 363 g                                                                                           | 507 g                                                                                           | 156 g                                                                                        |
| Altura               | 34mm                                                                                            | 46mm                                                                                            | 9mm                                                                                          |
| Largura              | 84mm                                                                                            | 81mm                                                                                            | 75mm                                                                                         |
| Comprimento          | 168mm                                                                                           | 228mm                                                                                           | 158mm                                                                                        |

## Rotação de tela na Cielo LIO

As rotações na tela de exibição possuem comportamento diferente entre as versões da Cielo LIO.

Na LIO V1 a orientação da tela é travada.

Na LIO V2 é possível controlar a orientação da tela. Por padrão, a orientação da tela exibida é livre e definida de acordo com o acelerômetro do equipamento.

Caso o desenvolvedor deseje controlar e usar de forma personalizada a orientação de tela da Cielo LIO, este deverá utilizar de acordo com a documentação do Android.

[Documentação Oficial do Android](https://developer.android.com/guide/topics/manifest/activity-element.html)

Acesse o item: android:screenOrientation para obter maiores informações.

## Dados Móveis na Cielo LIO

A Cielo LIO já vem configurada com um SIM Card. A operadora do SIM Card é definida de acordo com o endereço de cadastro do estabelecimento comercial.

A Cielo envia o SIM Card da melhor operadora de acordo com o endereço de cadastro da LIO solicitada.

Esse SIM Card permite a conexão com a tecnologia 3G da Cielo LIO e possui um pacote de dados ilimitado.

# Dicas para desenvolvedores

O guia abaixo fornece as informações necessárias para ajudar os desenvolvedores a integrar ou desenvolver seus aplicativos na plataforma Cielo LIO da melhor maneira possível, de modo a oferecer uma experiência excelente para os estabelecimentos comerciais.

Recomenda-se a leitura detalhada na documentação da Cielo LIO presente no Portal de Desenvolvedores. Essa documentação reúne informações importantes para questões de simplicidade moderada

## Melhores práticas com a plataforma Cielo LIO

### Segurança de dados e Privacidade

- Proteja os dados confidenciais de clientes e funcionários. Não exponha publicamente nomes, endereços ou números de telefone.
- Nunca exponha tokens de autenticação ou senhas de qualquer tipo.
- O parceiro deve fornecer os seus dados de suporte para que os estabelecimentos comerciais (lojistas) entrem em contato no caso de problemas e/ou dúvidas.

### Rate Limiting

- As solicitações da Automação Comercial ou PDV devem ser escalonadas o máximo possível para evitar rajadas de alto volume de tráfego.
- “Cache” seus próprios dados quando você precisar armazenar valores especializados ou revisar rapidamente conjuntos de dados muito grandes.
- Não crie multi-thread com chamadas POST, pois esse comportamento pode criar atrasos sistêmicos devido a deadlocks.
- Minimize o uso de dados. Os estabelecimentos comerciais (lojistas) podem estar utilizando conexão com dados móveis limitados.

### Código de Qualidade

Seu aplicativo deve estar em conformidade com as práticas de programação Java e Android convencionais de acordo com as diretrizes para desenvolvedores do Android.

- Princípios de Design Orientado a Objetos (S.O.L.I.D.).
- Diretrizes de estilo Java.
- Entenda a diferença entre `compileSdkVersion`, `targetSdkVersion`, e `minSdkVersion`.
- Aproveite os botões nativos do Android, como os botões “Voltar” e “Início”.
- Otimize as operações visando o baixo consumo da bateria
- O aplicativo deve atender às necessidades dos estabelecimentos comerciais (lojistas) da Cielo.
- Seu aplicativo deve ter uma boa experiência de ponta a ponta, garantindo a comunicação correta entre todos os fluxos, principalmente os retornos de pagamento da Cielo LIO.

### Recursos de imagem

- Os ícones devem estar em conformidade com o dimensionamento padrão do Android
- Seguir o [Guideline do Android](https://developer.android.com/guide/practices/ui_guidelines/icon_design)

### Utilização e Usabilidade

- Recomendamos aos desenvolvedores que integrem algum tipo de utilitário de relatório de falhas em seus produtos Android. Isso ajudará você a manter a consciência operacional do seu produto. Sugerimos a utilização do [Crashlytics](http://try.crashlytics.com)
- Os desenvolvedores podem coletar métricas sobre o uso do seu aplicativo. Isso irá ajudá-los a construir melhores produtos e aumentar a conscientização a respeito de quaisquer questões impactantes.
- Garantir que o aplicativo funcione de forma otimizada, evitando que ocorram crash e demora na resposta por processamento da aplicação. Seu aplicativo será usado em condições de trabalho de ritmo rápido e dinâmico, portanto esforce-se para obter fluxos de trabalho claros, fáceis de usar e robustos, com o mínimo de passos possível.
- O design deve enfatizar clareza e acessibilidade – alto contraste, fontes legíveis, texto grande e entradas.
- Deixar claro os termos de aceite da aplicação e prover o suporte necessário ao usuário no que tange o serviço disponibilizado.
- Se você estiver adaptando um aplicativo desenvolvido para outra plataforma, verifique se ele só inclui recursos e botões relevantes para o usuário da Cielo LIO.
- Se o seu aplicativo incluir um componente voltado para o cliente, seu projeto refletirá sobre o negócio usando seu aplicativo. Essas interfaces devem ser agradáveis e profissionais.
- Recomenda-se a utilização do [Material Design](https://material.io) para desenvolvimento das aplicações para a Cielo LIO. Esta recomendação tem como objetivo facilitar o uso de boas práticas de design para o desenvolvimento de aplicações móveis.
- Seu aplicativo será usado em condições de trabalho de ritmo rápido e dinâmico. Esforce-se para obter fluxos de trabalho claros, fáceis de usar e robustos, com o mínimo de passos possível.

# Desenvolva seu aplicativo para Cielo LIO

## Introdução

Com a Cielo LIO é possível que empresas e parceiros tenham seu aplicativo rodando na plataforma da Cielo. Esses aplicativos podem ou não estar integrados com o pagamento, tudo vai depender da finalidade da empresa ou parceiro.

Abaixo, você encontra todas as informações necessárias para desenvolver um aplicativo para a Cielo LIO.

## Ambiente de Desenvolvimento

A Cielo recomenda que seja utilizada a IDE do Android Studio (versão 2.2.2 ou superior), visando garantir o funcionamento do
aplicativo na plataforma Cielo LIO.

Para mais detalhes sobre a instalação e configuração do Android Studio, [clique aqui](https://developer.android.com/index.html)

Para a criação de um novo projeto no Android Studio, [clique aqui](https://developer.android.com/training/basics/firstapp/creating-project.html)

## Linguagem de Programação

A Cielo LIO aceita aplicativos desenvolvidos em Java ou Kotlin, como linguagens oficiais. As demais linguagens são permitidas, porém é de responsabilidade do desenvolvedor.

Recomendamos que essas linguagens sejam utilizadas para garantir o funcionamento e facilidade de integração com a Cielo LIO.

## Cielo OS

O sistema operacional da plataforma Cielo LIO foi personalizado e, com isso, surgiu o Cielo OS, que é baseado em Android.

## Versão target da aplicação

Recomenda-se que o desenvolvedor utilize para a Cielo LIO+ o APK target version 27 e versão mínima 22 (essa última para garantir compatibilidade com as demais soluções V1 e V2).

## Cielo LIO+ App padrão de vendas

Você poderá configurar seu App da Cielo LIO+ como um aplicativo padrão. Para isso, deve submeter o seu app para a CieloStore, solicitando que seja definido como frente de caixa, informando qual Intent e qual nome do parâmetro receberá o valor.

Após a aprovado/certificado, o App estará disponível para ser selecionado com App Padrão de venda no menu da sua LIO+.

### Intent para receber o valor da venda

A Intent informada ao submeter o App, deve ser a tela inicial de venda do seu App.

O parâmetro de valor citado no item anterior, serve para para receber o valor da venda, caso o usuário inicie uma transação usando o App padrão da Cielo, ao invez de usar o App Padrão selecionado.

Esse valor é passado no formato de centavos, sem separação dos decimais. Por exemplo, o valor 152,25 é passado como 15225, ficando por conta do App fazer o tratamento e formatação.

Essa Intent será chamada em dois momentos:

- Quando o seu app estiver marcado como padrão, e o snpap do Pinpad for conectado.

- Quando o seu app estiver marcado como padrão, e uma transação for iniciada usando o App Cielo Vender (App padrão vendas da Cielo). Neste cenário o valor digitado no App Cielo Vender será passado como Intent Extra para o seu App.

## Recursos Indisponíveis

Ao personalizar o Android da Cielo LIO, foram removidos alguns recursos para garantir o desempenho e a segurança da plataforma.

Seguem abaixo os recursos removidos da Cielo LIO:

**Google Play Services**: Todos os serviços, APIs e apps do Google foram removidos do sistema operacional. Consequentemente, não será possível utilizar as bibliotecas que dependem desses recursos do Google.

**Componente Webview**: Este recurso visual foi removido com o objetivo de garantir a segurança na plataforma e evitar que, a partir dos aplicativos instalados na Cielo LIO, seja possível acessar links e conteúdos externos.

> **Atenção**: A Cielo não permite que o aplicativo do cliente/parceiro seja desenvolvido utilizando o recurso WebView. Esse recurso visual deixa a plataforma da Cielo LIO vulnerável. Caso a aplicação esteja utilizando o WebView, esta não atenderá aos parâmetros de certificação e não será disponibilizada na Cielo Store.

## Sugestões de substitutos

### Push-Notifications

Recurso exclusivo do Google Services, portanto não está presente na Cielo LIO.

**Alternativa**: JobScheduler

**Descrição**: É uma API para agendar vários tipos de trabalhos contra a estrutura que será executada no próprio processo da sua aplicação. Permitindo a cada ciclo de tempo que o aplicativo realize uma busca em nossos serviços de Backend.

O JobScheduler é o mais indicado devido a performance em relação ao uso de bateria, fora as muitas outras opções que ele disponibiliza (Ex: Job rodar somente quando o smartphone estiver carregando).

Referência: [Clique aqui](https://developer.android.com/reference/android/app/job/JobScheduler.html)

### Serviços de Localização (GPS)

Recurso exclusivo do Google Services, portanto não está presente na Cielo LIO.

**Alternativa**: Location Manager

**Descrição**: Essa classe fornece acesso aos serviços de localização do sistema. Esses serviços permitem que os aplicativos obtenham atualizações periódicas da localização geográfica do dispositivo ou que iniciem uma Intenção especificada pela aplicação quando o dispositivo entra na proximidade de uma determinada localização geográfica.

Referência: [Clique aqui](https://developer.android.com/reference/android/location/LocationManager.html)

### Serviços de Mapas

Recurso exclusivo do Google Services, portanto não está presente na Cielo LIO.

**Alternativa**: MapBox

**Descrição**: Uma plataforma de mapeamento de código aberto para mapas personalizados. Nossas APIs e SDKs são os blocos de construção para integrar a localização em qualquer aplicativo móvel ou web.

Referência: [Clique aqui](https://www.mapbox.com)

## APKs Removidas do Cielo OS

Abaixo, segue uma tabela com todas as APKs que foram removidas do Cielo OS e que, consequentemente, não estão disponíveis para a Cielo LIO:

|                  |                      |                         |
| ---------------- | -------------------- | ----------------------- |
| BasicSmsReceiver | FileManager          | PhaseBeam               |
| Browser          | Galaxy4              | QuickSearchBox          |
| Calculator       | Gallery              | SoundRecorder           |
| Calendar         | HoloSpiralWallpaper  | SpeechRecorder          |
| CalendarProvider | LiveWallpapers       | Todos                   |
| CBMessageWidget  | LiveWallpaperPicker  | Videos                  |
| Contacts         | MagicSmokeWallpapers | VisualizationWallpapers |
| ContactsCommon   | MtkWeatherProvider   | VoiceCommand            |
| DataTransfer     | Mms                  | VoiceDialer             |
| Dialer           | Music                | VoiceExtension          |
| Email            | MusicFX              | VoiceUnlock             |
| Exchange2        | NlpService           | WallpaperCropper        |
| FMRadio          | NoiseField           |                         |

## Frameworks de Desenvolvimento

Atualmente Cielo LIO ainda não dá suporte a aplicativos desenvolvidos em plataformas híbridas, como, por exemplo, Ionic, Titanium, Xamarin, CronApp e PhoneGap.

---

# Integração Local

## Apresentação

O objetivo da Integração Local da Cielo LIO é permitir que o aplicativo desenvolvido em Android se integre com o módulo de pedidos e pagamentos da Cielo LIO através do Cielo LIO Order Manager SDK.

Nesse modelo de integração, toda a gestão do estabelecimento comercial e da arquitetura da solução fica sob responsabilidade do aplicativo que irá utilizar o SDK nas operações de pagamento.

- O aplicativo do parceiro rodando na Cielo envia informações para o Cielo LIO Order Manager SDK.
- O Cielo LIO Order Manager SDK executa os fluxos para pagamento.
- O aplicativo do parceiro recebe as informações do pagamento e continua sua execução.

As seções abaixo possuem todas as informações necessárias para realizar a integração de forma rápida e segura.

## Cielo Lio Order Manager SDK

### Sobre

O Cielo LIO Order Manager SDK é uma biblioteca Android desenvolvida com base na Cielo LIO Order Manager API, encapsulando a complexidade da comunicação REST em uma API fluente e amigável ao desenvolvedor e permitindo uma integração simples, rápida e segura com a plataforma Cielo LIO.

O principal objetivo do Cielo LIO Order Manager SDK é simplificar a integração com o sistema de pagamentos e permitir que o desenvolvedor concentre esforços no desenvolvimento das características do seu aplicativo. Abaixo, é apresentado um exemplo em alto nível do processo de utilização do Cielo LIO Order Manager SDK por um aplicativo parceiro:

![fluxo](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/sdk-order.jpg)

1. O aplicativo do parceiro é responsável por gerenciar todas as informações do pedido e, então, enviá-las para o Cielo LIO Order Manager SDK.
2. O Cielo LIO Order Manager SDK recebe as informações e o fluxo de pagamento para o cliente. Neste fluxo, o cliente irá selecionar a forma de pagamento e digitar a senha no Pinpad, tendo a possibilidade de enviar por e-mail o comprovante do pagamento.
3. Ao término do fluxo de pagamento, o aplicativo do parceiro recebe as informações sobre o pagamento realizado e volta a ser executado na tela da Cielo LIO.

Para mais informações e detalhes sobre o desenvolvimento de um aplicativo para a Cielo LIO, acesse a documentação Desenvolva um App para LIO.

### Ambiente Sandbox - Emulador

Este aplicativo funciona como um proxy de todas as chamadas que o SDK enviaria para a LIO. Ele simplesmente trata essas chamadas e simula os tipos possíveis de retorno para a aplicação cliente, permitindo que o desenvolvedor realize os testes nos métodos do SDK e faça o debug da sua aplicação durante o desenvolvimento e a integração com o Cielo LIO Order Manager SDK, sem a necessidade de possuir um hardware da Cielo LIO.

> Não é nem mesmo necessário deixar esse app aberto. Assim que a aplicação cliente utilizar uma função do OrderManager que chamaria a LIO, essa aplicação entra em primeiro plano para seleção do que deve ser retornado (Sucesso, Erro ou Cancelamento)

Faça o download do .apk do emulador no link abaixo:

[Download do Emulador](https://s3-sa-east-1.amazonaws.com/cielo-lio-store/apps/lio-emulator/1.1.0/lio-emulator.apk)

Para instalar o aplicativo, basta seguir os seguintes passos:

- Acesse as configurações do seu aparelho e vá até o menu “Segurança”;
- Localize o item “Fontes desconhecidas”, na seção “Administração do dispositivo”
- Toque na chave ao lado e confirme sua escolha para passar a permitir a instalação de arquivos APK baixados por fontes alternativas.

### Configurar módulos e dependências

Após configurar um novo projeto no Android Studio, é necessário incluir a dependência abaixo no projeto.

Para a versão release, adicione o módulo do Cielo LIO Order Manager SDK nas dependências do Gradle:

```
compile 'com.cielo.lio:order-manager:0.19.5'
```

última versão 0.19.4 - lançada em 25/07/2018

> A partir da versão 1.17.7-beta do SDK se tornou necessária a permissão de INTERNET na aplicação cliente.
> Adicione essa permissão ao `AndroidManifest.xml` da sua aplicação.

### Credenciais

Para utilizar o Cielo LIO Order Manager SDK, é necessário inserir as seguintes credenciais na inicialização do OrderManager:

```java
Credentials credentials = new Credentials("Seu client id aqui", "Seu accessToken aqui");
```

- Client-Id
  Identificação de acesso. Sua geração ocorre no momento da criação pelo painel do desenvolvedor. Seu valor pode ser visualizado na coluna Client ID, dentro do menu 'Desenvolvedor' -> 'Client ID Cadastrados'.

- Access-Token
  Identificação do token de acesso, que armazena as regras de acesso permitidas ao Client ID. Sua geração ocorre no momento da criação do Client ID pelo painel do desenvolvedor. Seu valor pode ser visualizado clicando em 'detalhes' na coluna 'Access Tokens', dentro do menu 'Desenvolvedor' -> 'Client ID Cadastrados'.

## Criação e Gerenciamento de Ordens

O fluxo básico para utilização do SDK pode ser dividido em 7 etapas, conforme o diagrama abaixo:

![order manager sdk fluxo](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/fluxogram-lio-sdk.png)

Abaixo, iremos mostrar como realizar cada uma dessas etapas.

### Criar OrderManager

Este método permite iniciar o OrderManager, que é responsável pelas principais operações do Cielo LIO Order Manager SDK. O OrderManager representa a interface com a API REST do Order Manager.

Tudo começa com a criação do OrderManager!

```java
OrderManager orderManager = new OrderManager(credentials, context);
```

O construtor do OrderManager recebe 2 parâmetros:

| Atributo    | Descrição                                                                                                                                                                                                                                                                                              | Domínio                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
| credentials | Credenciais de acesso do Parceiro/Desenvolvedor. Depois de se registrar no Portal de Desenvolvedores e criar seu app, o Parceiro/Desenvolvedor recebe as credenciais (Client-Id e Access-Token). Elas servem para identificá-lo unicamente na plataforma LIO e diferenciar as ordens da sua aplicação. | `cielo.sdk.order.Credentials` |
| context     | O contexto da aplicação.                                                                                                                                                                                                                                                                               | `android.content.Context`     |

> **Atenção:** Recomendamos criar/inicializar o OrderManager no aplicativo do parceiro no momento em que for utilizar as funcionalidades, visando otimizar o desempenho do aplicativo

### Vincular o contexto da aplicação ao SDK

Com o método `bind()`, é possível vincular o contexto da aplicação ao SDK. Este serviço é responsável por gerenciar as funções relacionadas com as ordens da LIO

```java
ServiceBindListener serviceBindListener = new ServiceBindListener() {

    @Override public void onServiceBoundError(Throwable throwable) {
        //Ocorreu um erro ao tentar se conectar com o serviço OrderManager
    }

    @Override
    public void onServiceBound() {
        //Você deve garantir que sua aplicação se conectou com a LIO a partir desse listener
        //A partir desse momento você pode utilizar as funções do OrderManager, caso contrário uma exceção será lançada.
    }

    @Override
    public void onServiceUnbound() {
        // O serviço foi desvinculado
    }
};

orderManager.bind(context, serviceBindListener);
```

> **Atenção:** Você deve garantir que o listener `onServiceBound()` foi chamado antes de utilizar as funções do OrderManager, caso contrário uma exceção será lançada e causará um crash na sua aplicação.

O método Bind recebe dois parâmetros:

- **context:** objeto que proverá o contexto em que o serviço será vinculado.

- **serviceBindListener:** listener que notifica o estado da conexão com o serviço OrderManager.

Com o OrderManager inicializado e após a execução do método onServiceBound, se torna possível ir para a próxima etapa e criar um pedido (classe Order).

### Criar um pedido

A Cielo LIO trabalha com o conceito de Order (pedido). É necessário possuir um pedido para então realizar o(s) pagamento(s).

Este método permite criar uma Order (classe Order). Para realizar essa criação, utilize o método createDraftOrder, que disponibilizará uma Order com status DRAFT:

```java
Order order = orderManager.createDraftOrder("REFERÊNCIA_DO_PEDIDO");
```

### Adicionar itens em um pedido

Este método permite que sejam adicionados itens em um pedido.

> **Atenção:** É necessário adicionar no mínimo um item a um pedido para que seja possível dar continuidade ao pagamento.

```java
// Identificação do produto (Stock Keeping Unit)
String sku = "2891820317391823";
String name = "Coca-cola lata";

// Preço unitário em centavos
int unitPrice = 550;
int quantity = 3;

// Unidade de medida do produto String
unityOfMeasure = "UNIDADE";

order.addItem(sku, name, unitPrice, quantity, unityOfMeasure);
```

### Liberar pedido para pagamento

Este método permite atualizar o status de um pedido e liberá-lo para pagamento. O objetivo é utilizar este método depois de adicionar todos os itens no pedido.

```java
orderManager.placeOrder(order);
```

Após a execução desse método, o status da Order irá trocar de DRAFT para ENTERED, permitindo que a mesma seja paga.

> **Atenção:** É importante observar que, uma vez que uma Order tenha mudado de status para ENTERED, não será mais possível incluir itens na mesma.
> Iniciar processo de pagamento

Este método permite iniciar o processo de pagamento na Cielo LIO.

## Processo de Pagamento

Estão disponíveis algumas formas de chamar o método checkoutOrder:

![checkoutorder formas](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/checkoutOrder.jpg)

Independende da forma escolhida, você deverá utilizar o seguinte callback como parâmetro do método de `checkoutOrder()` para receber os estados relacionados ao pagamento.:

```java
PaymentListener paymentListener = new PaymentListener() {
    @Override
    public void onStart() {
        Log.d("SDKClient", "O pagamento começou.");
    }

    @Override
    public void onPayment(@NotNull Order order) {
        Log.d("SDKClient", "Um pagamento foi realizado.");
    }

    @Override public void onCancel() {
        Log.d("SDKClient", "A operação foi cancelada.");
    }

    @Override public void onError(@NotNull PaymentError paymentError) {
        Log.d("SDKClient", "Houve um erro no pagamento.");
    }
};
```

> PaymentListener: Um callback que informa sobre todas as ações tomadas durante o processo de pagamento.
> As seguintes ações podem ser notificadas:  
> • onStart - Quando se dá o início do pagamento.
> • onPayment - Quando um pagamento é realizado. Notem que um pedido pode ser pago por mais de um pagamento.
> • onCancel - Quando o pagamento é cancelado.
> • onError - Quando acontece um erro no pagamento do pedido.

O método `onPayment()` retorna um objeto `Order` com uma lista de `Payment` que possui um HashMap `PaymentFields` com a maioria dos dados da transação.
Segue abaixo a tabela com os dados mais relevantes existentes nesse mapa:

| Payment Fields - (**atributo do objeto Payment**) |
| Nome do Campo | Descrição do Campo | Valor Exemplo |
|--------------------------|--------------------------------------------------------------------|------------------------------------------|
| clientName | Nome do Portador | VISA ACQUIRER TEST CARD 03 |
| hasPassword | Validar se a operação pediu senha | true |
| primaryProductCode | Código do produto primário | 4 |
| primaryProductName | Nome do produto primário | CREDITO |
| upFrontAmount | Valor da entrada da transação | 2500 |
| creditAdminTax | Valor da taxa de administração de crédito | 0 |
| firstQuotaDate | Data de débito da primeira parcela | 25/12/2018 (dd/MM/yyy) |
| externalCallMerchantCode | Número do Estabelecimento Comercial | 0010000244470001 |
| hasSignature | Validar se a operação pediu assinatura | false |
| hasPrintedClientReceipt | Validar se imprimiu a via do cliente | false |
| applicationName | Pacote da aplicação | cielo.launcher |
| interestAmount | Valor de juros | 5000 |
| changeAmount | Valor de troco | 4500 |
| serviceTax | Taxa de serviço | 2000 |
| cityState | Cidade - Estado | Barueri - SP |
| v40Code | Tipo da transação | 5 (Lista de Tipos de transação abaixo) |
| secondaryProductName | Nome do produto secundario | PARC. ADM |
| paymentTransactionId | ID da transação de pagamento | 4c603b44-19b8-497c-b072-60d5dd6807e7 |
| pan | Número cartão tokenizado (6 primeiros dígitos – 4 últimos dígitos ou 4 últimos) | 476173-0036 ou \*\*\*\*\*\*\*\*\*\*4242 |
| originalTransactionId | ID da transação original, nos casos de cancelamento | 729d32ac-6c8d-4b0c-b670-263552f07000 |
| cardLabelApplication | Tipo de aplicação utilizada pelo cartão na transação | CREDITO DE VISA |
| secondaryProductCode | Código do produto secundário | 205 |
| documentType | (J) = Pessoa Jurídica (F) = Pessoa Física | J |
| statusCode | Status da transação1 - Autorizada 2 - Cancelada | 1 |
| merchantAddress | Endereço do estabelecimento comercial (lojista) | Alameda Grajau, 219 |
| merchantCode | Número do Estabelecimento Comercial | 0010000244470001 |
| hasConnectivity | Valida se a transação foi online | true |
| productName | forma de pagamento compilada | CREDITO PARCELADO ADM - I |
| merchantName | Nome Fantasia do Estabelecimento Comercial | LOJA ON |
| firstQuotaAmout | Valor da primeira parcela | 0 |
| cardCaptureType | Código do tipo de captura do cartão | 0 (Lista de Tipos de Captura abaixo) |
| requestDate | Data da requisição em milisegundos | 1293857600000 |
| boardingTax | Taxa de embarque | 1200 |
| applicationId | Pacote de aplicação | cielo.launcher |
| numberOfQuotas | Número de parcelas | 2 |

| Lista de Tipos de Captura |
| Código | Valor |
|---------------------------|----------------------------------|
| 0 | Transação com cartão de chip |
| 1 | Transação digitada |
| 2 | Transação com cartão de tarja |
| 3 | Transação com cartão contactless |

| Lista de Tipos de Transação - (**Isto não é válido como código primário**) |
| Código | Valor |
|-----------------------------|----------------------------------|
| 4 | Crédito à vista |
| 5 | Crédito parcelado administrativo |
| 6 | Crédito parcelado loja |
| 7 | Pré autorização |
| 8 | Débito à vista |
| 9 | Débito pré datado |
| 10 | Crediário venda |
| 11 | Crediário simulação |
| 13 | Voucher alimentação/refeição |
| 28 | Cancelamento de venda |

> Todos os valores financeiros são informados sem vírgula, ou seja 2500 são equivalentes a R\$ 25,00.

### 1. Pagamento Parcial

No Pagamento parcial, o valor do pagamento é informado dentro do fluxo de telas da Cielo LIO. Na sequência, o fluxo de pagamento da Cielo LIO é iniciado (definir o valor a ser pago, escolher a forma de pagamento, inserir o cartão, digitar a senha e visualizar e/ou enviar por e-mail o comprovante).

```java
orderManager.checkoutOrder(orderId, paymentListener);
```

Nessa forma de pagamento, é necessário apenas fazer a chamada do método enviando os seguintes parâmetros:

| Atributo        | Descrição                             | Domínio                                   |
| --------------- | ------------------------------------- | ----------------------------------------- |
| orderId         | O identificador do pedido a ser pago. | `String`                                  |
| paymentListener | Callback de pagamento.                | `cielo.sdk.order.payment.PaymentListener` |

**Fluxo da transação utilizando o pagamento parcial da Cielo LIO**

Abaixo, segue um exemplo do fluxo com as telas exibidas durante o pagamento parcial:
![fluxo parcial](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/pagamento-parcial.jpg)

### 2. Pagamento de valor

No pagamento de Valores, o valor a ser pago é informado pelo aplicativo e a forma de pagamento (crédito, débito, parcelado) é escolhida dentro do fluxo de telas da Cielo LIO.

```java
orderManager.checkoutOrder(orderId, value, paymentListener);
```

Nessa forma de pagamento é possível enviar qualquer valor a ser pago (valor total ou valor parcial do pedido), tudo depende do modelo de negócio adotado pelo aplicativo do parceiro. Para fazer a chamada é necessário enviar os seguintes parâmetros:

| Atributo        | Descrição                                               | Domínio                                   |
| --------------- | ------------------------------------------------------- | ----------------------------------------- |
| orderId         | O identificador do pedido a ser pago.                   | `String`                                  |
| value           | Valor a ser pago. R\$ 10,00 deve ser enviado como 1000. | `Long`                                    |
| paymentListener | Callback de pagamento.                                  | `cielo.sdk.order.payment.PaymentListener` |

**Fluxo da transação utilizando o pagamento de valor da Cielo LIO**

Abaixo, segue um exemplo do fluxo com as telas exibidas durante o pagamento de valor:
![fluxo parcial](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/pagamento-valor.jpg)

### 3. Pagamento direto

No Pagamento Direto, o valor a ser pago e a forma de pagamento (crédito, débito, parcelado) será definido dentro da aplicação do parceiro. Na sequência o fluxo de pagamento da Cielo LIO é iniciado (inserir o cartão, digitar a senha e visualizar e/ou enviar por e-mail comprovante).

#### Códigos de Pagamento

Para realizar o pagamento direto é necessário, primeiramente, verificar os tipos de pagamento habilitados para Cielo LIO do estabelecimento comercial utilizando a função de consulta abaixo:

```java
ArrayList<PrimaryProduct> paymentTypes = orderManager.retrievePaymentType();
```

Esta função disponibilizará uma lista de objetos do tipo PrimaryProduct onde será possível recuperar os códigos de pagamento habilitados.

Os seguintes campos serão retornados por essa função:

| Atributo          | Descrição                                                                  | Domínio                       |
| ----------------- | -------------------------------------------------------------------------- | ----------------------------- |
| id                | identificador do código no sistema.                                        | `Long`                        |
| code              | utilizado na função de pagamento.                                          | `String`                      |
| name              | Nome do método de pagamento para efeitos de exibição.                      | `String`                      |
| secondaryProducts | Listagem de códigos de pagamento secundário. ex.: À Vista, Parcelado, etc. | `ArrayList<SecondaryProduct>` |

Com os códigos de pagamentos disponíveis para a Cielo LIO do estabelecimento comercial, basta realizar a chamada de Pagamento Direto informando os códigos dos produtos:

```java

PrimaryProduct primaryProduct = paymentTypes.get(0);
SecondaryProduct secondaryProduct = primaryProduct.getSecondaryProducts().get(0);

String primaryCode = primaryProduct.getCode();
String secondaryCode = secondaryProduct.getCode();

orderManager.checkoutOrder(orderId, primaryCode, secondaryCode, paymentListener);

```

> **Atenção:** Na versão 0.19.0 do SDK foram introduzidos códigos de pagamento para as principais operações disponibilizadas na LIO, facilitando assim as chamadas de pagamento. É importante ressaltar que as formas de pagamento são configuradas de acordo com o estabelecimento comercial, e nem todas estarão disponíveis em todas os terminais. Caso o método de pagamento selecionado não esteja disponível na LIO em questão, ocorrerá uma exceção do tipo `NoSuchElementException`.

| PaymentCode            |
| ---------------------- |
| DEBITO_AVISTA          |
| DEBITO_PREDATADO       |
| CREDITO_AVISTA         |
| CREDITO_PARCELADO_LOJA |
| CREDITO_PARCELADO_ADM  |
| PRE_AUTORIZACAO        |
| VOUCHER_ALIMENTACAO    |
| VOUCHER_REFEICAO       |

Nessa forma de pagamento é possível enviar qualquer valor a ser pago e a forma de pagamento. Para fazer a chamada é necessário enviar os seguintes parâmetros:

| Atributo                           | Descrição                                                                       | Domínio                                   |
| ---------------------------------- | ------------------------------------------------------------------------------- | ----------------------------------------- |
| orderId                            | O identificador do pedido a ser pago.                                           | `String`                                  |
| value                              | Valor a ser pago. R\$ 10,00 deve ser enviado como 1000.                         | `Long`                                    |
| primaryCode                        | Código identificador do método primário de pagamento ex.: Débito, Crédito.      | `String`                                  |
| secondaryCode                      | Código identificador do método secundário de pagamento ex.: À vista, Parcelado. | `String`                                  |
| installments (**não obrigatório**) | Número de parcelas.                                                             | `Long`                                    |
| email (**não obrigatório**)        | Email informado                                                                 | `String`                                  |
| paymentListener                    | Callback de pagamento.                                                          | `cielo.sdk.order.payment.PaymentListener` |

**Fluxo da transação utilizando o pagamento direto da Cielo LIO**

```java
orderManager.checkoutOrder(orderId, value, primaryCode, secondaryCode, paymentListener);
```

ou

```java
orderManager.checkoutOrder(orderId, value, paymentCode, paymentListener);
```

Abaixo, segue um exemplo do fluxo com as telas exibidas durante o pagamento direto:
![fluxo parcial](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/pagamento-direto.jpg)

### 4. Pagamento parcelado

Para efetuar um pagamento parcelado, é preciso consultar as formas de pagamento utilizando a função disponibilizada no SDK, escolher crédito no produto primário e crédito no produto secundário **obrigatoriamente** e informar o número de parcelas no momento do checkout. É importante lembrar que se os códigos de pagamento forem informados incorretamente ou se o número de parcelas não for maior do que **0**, o sistema acusará erro.
Nessa forma de pagamento, é necessário apenas fazer a chamada do método enviando os seguintes parâmetros:

| Atributo        | Descrição                                                                       | Domínio                                   |
| --------------- | ------------------------------------------------------------------------------- | ----------------------------------------- |
| orderId         | O identificador do pedido a ser pago.                                           | `String`                                  |
| value           | Valor a ser pago. R\$ 10,00 deve ser enviado como 1000.                         | `Long`                                    |
| primaryCode     | Código identificador do método primário de pagamento ex.: Débito, Crédito.      | `String`                                  |
| secondaryCode   | Código identificador do método secundário de pagamento ex.: À vista, Parcelado. | `String`                                  |
| installments    | Número de parcelas.                                                             | `Long`                                    |
| paymentListener | Callback de pagamento.                                                          | `cielo.sdk.order.payment.PaymentListener` |

**Fluxo da transação utilizando o pagamento parcelado da Cielo LIO**

```java
orderManager.checkoutOrder(orderId, value,  primaryCode, secondaryCode, installments,  paymentListener);
```

ou

```java
orderManager.checkoutOrderStore(orderId, value,  installments,  paymentListener);
```

ou

```java
orderManager.checkoutOrderAdm(orderId, value,  installments,  paymentListener);
```

Abaixo, segue um exemplo do fluxo com as telas exibidas durante o pagamento parcelado:
![fluxo parcial](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/pagamento-parcelado.jpg)

### 5. Pagamento informando email

Neste caso é possível informar o email para facilitar o preenchimento na hora de enviar o comprovante para o cliente.
Nessa forma de pagamento, é necessário apenas fazer a chamada do método enviando os seguintes parâmetros:

| Atributo        | Descrição                                                                       | Domínio                                   |
| --------------- | ------------------------------------------------------------------------------- | ----------------------------------------- |
| orderId         | O identificador do pedido a ser pago.                                           | `String`                                  |
| value           | Valor a ser pago. R\$ 10,00 deve ser enviado como 1000.                         | `Long`                                    |
| primaryCode     | Código identificador do método primário de pagamento ex.: Débito, Crédito.      | `String`                                  |
| secondaryCode   | Código identificador do método secundário de pagamento ex.: À vista, Parcelado. | `String`                                  |
| installments    | Número de parcelas.                                                             | `Long`                                    |
| email           | Email informado                                                                 | `String`                                  |
| paymentListener | Callback de pagamento                                                           | `cielo.sdk.order.payment.PaymentListener` |

**Fluxo da transação utilizando o pagamento direto da Cielo LIO**

```java
orderManager.checkoutOrder(orderId, value, primaryCode, secondaryCode, installments, email, paymentListener);
```

Abaixo, segue um exemplo do fluxo com as telas exibidas durante o pagamento com email:
![fluxo parcial](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/pagamento-parcelado.jpg)

### 6. Pagamento informando EC

> **Atenção:** Para a utilização dessa forma de pagamento, é necessário uma pré habilitação junto a Cielo, para o recebimento com MULTI-EC.

Esse método é disponibilizado para o caso de ser necessário efetuar um pagamento em um EC diferente do principal. O EC informado deve estar configurado na LIO na hora da inicialização para que funcione ou o SDK irá enviar uma exceção do tipo `InvalidParameterException`.
Nessa forma de pagamento, é necessário apenas fazer a chamada do método enviando os seguintes parâmetros:

| Atributo        | Descrição                                                                       | Domínio                                   |
| --------------- | ------------------------------------------------------------------------------- | ----------------------------------------- |
| orderId         | O identificador do pedido a ser pago.                                           | `String`                                  |
| value           | Valor a ser pago. R\$ 10,00 deve ser enviado como 1000.                         | `Long`                                    |
| primaryCode     | Código identificador do método primário de pagamento ex.: Débito, Crédito.      | `String`                                  |
| secondaryCode   | Código identificador do método secundário de pagamento ex.: À vista, Parcelado. | `String`                                  |
| installments    | Número de parcelas.                                                             | `Long`                                    |
| email           | Email informado                                                                 | `String`                                  |
| merchantCode    | Número do EC                                                                    | `String`                                  |
| paymentListener | Callback de pagamento                                                           | `cielo.sdk.order.payment.PaymentListener` |

**Fluxo da transação utilizando o pagamento direto da Cielo LIO**

```java
orderManager.checkoutOrder(orderId, value, primaryCode, secondaryCode, installments, email, merchantCode, paymentListener);
```

ou

```java
orderManager.checkoutOrder(orderId, value, paymentCode, installments, email, merchantCode, paymentListener);
```

Abaixo, segue um exemplo do fluxo com as telas exibidas durante o pagamento com EC:
![fluxo parcial](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/pagamento-parcelado.jpg)

## Cancelamento

Para tratar a resposta do cancelamento, você deverá utilizar o seguinte callback como parâmetro do método de `cancelOrder()` para receber os estados relacionados ao cancelamento.

> CancellationListener: Um callback que informa sobre todas as ações tomadas durante o processo de cancelamento.
> As seguintes ações pode ser notificadas:
> • onSuccess - Quando um cancelamento é realizado com sucesso.
> • onCancel - Quando o usuário cancela a operação.
> • onError - Quando acontece um erro no cancelamento do pedido.

```java

CancellationListener cancellationListener = new CancellationListener() {
    @Override
    public void onSuccess(Order cancelledOrder) {
        Log.d("SDKClient", "O pagamento foi cancelado.");
    }

    @Override
    public void onCancel() {
        Log.d("SDKClient", "A operação foi cancelada.");
    }

    @Override
    public void onError(PaymentError paymentError) {
        Log.d("SDKClient", "Houve um erro no cancelamento");
    }
});

```

### Cancelar Pagamento

No método Cancelar um Pagamento, é necessário ter salvo uma instância da Order que contém as informações da Order. Essa Order pode ser recuperada no sucesso do callback do pagamento ou usando o método de Listagem de Pedidos (Orders) (link para método).
Assim que possuir a instância da Order, utilize o método abaixo passando os parâmetros conforme o exemplo abaixo:

```java
orderManager.cancelOrder(context, orderId, payment, cancellationListener);
```

Abaixo é detalhado cada um dos parâmetros enviados no método:

| Atributo             | Descrição                                                                             | Domínio                                        |
| -------------------- | ------------------------------------------------------------------------------------- | ---------------------------------------------- |
| context              | Contexto da sua aplicação.                                                            | `String`                                       |
| orderID              | O identificador do pedido a ser pago.                                                 | `Long`                                         |
| payment              | O pagamento a ser cancelado.                                                          | `cielo.sdk.order.payment.Payment`              |
| cancellationListener | Callback que informa sobre todas as ações tomadas durante o processo de cancelamento. | `cielo.sdk.order.payment.CancellationListener` |

### Receber aviso de cancelamento feito na LIO

Toda vez que é feito um cancelamento na LIO utilizando o launcher, o sistema envia um broadcast notificando quaisquer aplicações que estejam registradas sobre o mesmo. Para que sua aplicação seja notificada de um cancelamento, atualize o arquivo `AndroidManifest.xml` conforme o exemplo abaixo:

![Manifest]({{ site.baseurl_root }}/images/cielo-lio/manifest.jpg)

em seguida, é necessário implementar um `BroadcastReceiver` para tratar o evento da maneira que for pertinente a sua aplicação:

```java

public class LIOCancelationBroadcastReceiver extends BroadcastReceiver {

    String MY_CLIENT_ID = "Seu client id aqui";
    String MY_ACCESS_KEY = "Seu access key aqui";

    String INTENT_ORDER_KEY = "ORDER";
    String INTENT_TRANSACTION_KEY = "TRANSACTION";

    @Override
    public void onReceive(Context context, Intent intent) {
        ParcelableOrder order = intent.getExtras().getParcelable(INTENT_ORDER_KEY);

        if(MY_ACCESS_KEY.equalsIgnoreCase(order.getAccessKey()) && MY_CLIENT_ID.equalsIgnoreCase(order.getSecretAccessKey())) {
            ParcelableTransaction transaction  = intent.getExtras().getParcelable(INTENT_TRANSACTION_KEY);
        }
    }
}

```

## Listagem de Pedidos

Na listagem de pedidos, é possível obter todas os pedidos (Orders) abertas na Cielo LIO pelo aplicativo do parceiro.
Para isso, basta utilizar a função abaixo, que retorna os pedidos de forma paginada:

```java
//Busca 10 items da primeira página
ResultOrders resultOrders = orderManager.retrieveOrders(10, 0);
```

| ATRIBUTO | DESCRIÇÃO                                    | DOMÍNIO   |
| -------- | -------------------------------------------- | --------- |
| pageSize | quantidade de items por página               | `Integer` |
| page     | número da página requistada (iniciando em 0) | `Integer` |

> O objeto ResultOrders contém uma lista com todas as ordens abertas assinadas com as credenciais da aplicação.

## Finalizar uso do OrderManager

Após executar todas as operações de pagamento e caso não seja necessário utilizar o objeto orderManager, utilize método unbind para desvincular o contexto e evitar problemas de integridade.

Fique atento ao local onde o `unbind()` será executado para evitar problemas com ciclo de vida da Activity ou Fragment que foi vinculado ao serviço.
É importante lembrar que se o contexto for alterado, é preciso desvincular o serviço (ex.: troca de Activity)
Utilize o método abaixo para finalizar o uso do OrderManager:

```java
orderManager.unbind();
```

## Informações do terminal

Todas as informações referentes ao terminal, que foram expostas, estão disponíveis no InfoManager

```java
InfoManager infoManager = new InfoManager();
```

### Nível de Bateria

Para consultar o nível de carga da LIO, basta utilizar o métdo abaixo:

```java
infoManager.getBatteryLevel(context);
```

> O valor da bateria será retornado em uma `Float` contendo um valor de 0 a 1 em caso de sucesso e -1 em caso de erro.

### Verificar Modelo da LIO

O SDK disponibiliza um método para verificar se seu aplicativo está instalado numa LIO V1 ou V2. Basta acessar da seguinte forma:

```java
infoManager.getDeviceModel();
```

O mesmo irá retornar um enum do tipo `DeviceModel` com o modelo correspondente (`LIO_V1` ou `LIO_V2` ).

### Obtendo informações do usuário (EC e Número Lógico)

Através do SDK, é possível recuperar os dados do cliente e número lógico de maneira simples utilizando o método abaixo:

```java
infoManager.getSettings(context);
```

> Esta função, retornará um objeto do tipo Settings onde é possível recuperar as informações do usuário.
> Abaixo, segue um descritivo de atributos do objeto Setttings.

| ATRIBUTO     | DESCRIÇÃO            | DOMÍNIO  |
| ------------ | -------------------- | -------- |
| merchantCode | Código do cliente    | `String` |
| logicNumber  | Número lógico da LIO | `String` |

## Impressão [Apenas LIO V2]

A nova versão da Cielo LIO V2 permite que aplicações parceiras utilizem os métodos disponíveis da impressora para imprimir dados importantes ou necessários para o negócio do cliente. Para realizar estas operações, basta utilizar um dos métodos listados abaixo que permite a impressão de uma única linha, uma sequência de linhas, ou imagens.

```java
PrinterManager printerManager = new PrinterManager(context);
```

Independende da forma de impressão escolhida, você deverá utilizar o seguinte callback como parâmetro do método de para receber os estados relacionados à impressão:

> PrinterListener: Um callback que informa sobre todas as ações tomadas durante o processo de impressão.
> As seguintes ações pode ser notificadas:
> • onSuccess - Quando uma impressão é realizada com sucesso.
> • onError - Quando acontece um erro na impressão.
> • onWithoutPaper - Quando não há papel suficiente para realizar a impressão.

```java
PrinterListerner printerListener = new PrinterListener() {
    @Override public void onPrintSuccess(int printedLines) {
        Log.d(TAG, "onPrintSuccess");
    }

    @Override public void onError(@Nullable Throwable e) {
        Log.d(TAG, "onError");
    }

    @Override public void onWithoutPaper() {
        Log.d(TAG,"onWithoutPaper");
    }
});
```

> **Atenção:** para alterações na view do aplicativo é necessário rodar o código do callback dentro de um bloco runOnUiThread.

```java
    @Override public void onPrintSuccess(int printedLines) {
        runOnUiThread(new Runnable() {
            @Override
            public void run() {
                showDialog();
            }
        });
    }
```

### Mapa de Estilos de Impressão

Você pode formatar a sua impressão criando mapas de estilos utilizando os parâmetros disponíveis:

| Atributo                             | Descrição                                                                                                     | Valores                                                                                                     |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `PrinterAttributes.KEY_ALIGN`        | Alinhamento da impressão                                                                                      | `PrinterAttributes.VAL_ALIGN_CENTER` `PrinterAttributes.VAL_ALIGN_LEFT` `PrinterAttributes.VAL_ALIGN_RIGHT` |
| `PrinterAttributes.KEY_TEXTSIZE`     | Tamanho do texto                                                                                              | Valores inteiros                                                                                            |
| `PrinterAttributes.KEY_TYPEFACE`     | Fonte do texto                                                                                                | Trabalha com um inteiro de 0 a 8, onde cada um é uma fonte diferente.                                       |
| `PrinterAttributes.KEY_MARGINLEFT`   | Margem esquerda                                                                                               | Valores inteiros                                                                                            |
| `PrinterAttributes.KEY_MARGINRIGHT`  | Margem direia                                                                                                 | Valores inteiros                                                                                            |
| `PrinterAttributes.KEY_MARGINTOP`    | Margem superior                                                                                               | Valores inteiros                                                                                            |
| `PrinterAttributes.KEY_MARGINBOTTOM` | Margem inferior                                                                                               | Valores inteiros                                                                                            |
| `PrinterAttributes.KEY_LINESPACE`    | Espaçamento entre as linhas                                                                                   | Valores inteiros                                                                                            |
| `PrinterAttributes.KEY_WEIGHT`       | Varíavel utilizada quando se trbaalho com impressão de múltiplas colunas, para escolher o peso de cada coluna | Valores inteiros                                                                                            |

Exemplo de mapas de estilos:

```java
HashMap<String, Integer> alignLeft =  new HashMap<>();
alignLeft.put(PrinterAttributes.KEY_ALIGN, PrinterAttributes.VAL_ALIGN_LEFT);
alignLeft.put(PrinterAttributes.KEY_TYPEFACE, 0);
alignLeft.put(PrinterAttributes.KEY_TEXT_SIZE, 20);

HashMap<String, Integer> alignCenter =  new HashMap<>();
alignCenter.put(PrinterAttributes.KEY_ALIGN, PrinterAttributes.VAL_ALIGN_CENTER);
alignCenter.put(PrinterAttributes.KEY_TYPEFACE, 1);
alignCenter.put(PrinterAttributes.KEY_TEXT_SIZE, 20);

HashMap<String, Integer> alignRight =  new HashMap<>();
alignRight.put(PrinterAttributes.KEY_ALIGN, PrinterAttributes.VAL_ALIGN_RIGHT);
alignRight.put(PrinterAttributes.KEY_TYPEFACE, 2);
alignRight.put(PrinterAttributes.KEY_TEXT_SIZE, 20);
```

### Impressão de texto simples

Para imprimir textos simples utilize o método `printText()` do PrinterManager.
O método recebe como parâmetro o texto a ser impresso, um mapa de estilo de impressão e um listener para tratar o retorno da impressão.

```java
String textToPrint = "Texto simples a ser impresso.\n Com múltiplas linhas";
printerManager.printText(textToPrint, alignLeft, printerListener);
```

Exemplo de impressão de texto simples:
![Impressão texto simples]({{ site.baseurl_root }}/images/cielo-lio/print-text.png){:height="25%" width="25%"}

| Atributo        | Descrição                    | Domínio                           |
| --------------- | ---------------------------- | --------------------------------- |
| text            | Texto a ser impresso.        | `String`                          |
| style           | Mapa de estilos de impressão | `Map<String, Int>`                |
| printerListener | Callback de impressão.       | `cielo.sdk.order.PrinterListener` |

### Impressão de múltiplas colunas

Para imprimir textos em múltiplas colunas utilize o método `printMultipleColumnText()` do PrinterManager.
O método recebe como parâmetro um array de texts a serem impresso, um array com mapas de estilos de impressão, respectivamente e um listener para tratar o retorno da impressão.

```java
String[] textsToPrint = new String[] { "Texto alinhado à esquerda.", "Texto centralizado", "Texto alinhado à direita"  }

List<Map<String, Integer>> stylesMap =  new ArrayList<>();
stylesMap.add(alignLeft);
stylesMap.add(alignCenter);
stylesMap.add(alignRight);

printerManager.printMultipleColumnText(textsToPrint, stylesMap, printerListener);

```

Resultado final da impressão:
![Impressão Múltiplas Colunas]({{ site.baseurl_root }}/images/cielo-lio/print-columns.png){:height="25%" width="25%"}

| Atributo        | Descrição                             | Domínio                           |
| --------------- | ------------------------------------- | --------------------------------- |
| stringArray     | Lista de textos a serem impressos.    | `String[]`                        |
| style           | Lista de mapa de estilos de impressão | `List<Map<String, Int)>>`         |
| printerListener | Callback de impressão.                | `cielo.sdk.order.PrinterListener` |

### Impressão de imagem

Para imprimir imagens utilize o método `printImage()` do PrinterManager.
O método recebe como parâmetro o `bitmap` a ser impresso, um mapa de estilos de impressão e um listener para tratar o retorno da impressão.

```java
Bitmap bitmap = BitmapFactory.decodeResource(getResources(), R.drawable.cielo);
printerManager.printImage(bitmap, alignCenter, printerListener);
```

| Imagem a ser impressa                                                                              | Resultado final                                                                                          |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| ![Impressão Imagem]({{ site.baseurl_root }}/images/cielo-lio/cielo.png){:height="50%" width="50%"} | ![Impressão Imagem]({{ site.baseurl_root }}/images/cielo-lio/print-image.png){:height="25%" width="25%"} |

| Atributo        | Descrição                    | Domínio                           |
| --------------- | ---------------------------- | --------------------------------- |
| bitmap          | Imagem a ser impressa.       | `Bitmap`                          |
| style           | Mapa de estilos de impressão | `Map<String, Int>`                |
| printerListener | Callback de impressão.       | `cielo.sdk.order.PrinterListener` |

---

## Fluxo para Integração

![fluxo para integração](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/fluxogram-local-new.png)

1. Leia toda a documentação sobre a Integração Local.
2. Crie sua conta no Portal de Desenvolvedores da Cielo para obter todas as funcionalidades que o portal pode oferecer para você, desenvolvedor. É obrigatório possuir uma conta para gerar um Client-Id.
3. Realizando o cadastro de Client ID, o desenvolvedor recebe os tokens
4. (Client ID e Access-Token) e consegue utilizar o Cielo LIO Order Manager SDK. Realize os testes no Emulador Cielo Lio Confira o link: [Download do Emulador](https://s3-sa-east-1.amazonaws.com/cielo-lio-store/apps/lio-emulator/1.0.0/lio-emulator.apk)
5. Acesse a [Cielo Store](https://www.cieloliostore.com.br/login) e faça o upload do APK da sua aplicação. Ao término do upload, submeta seu aplicativo para certificação e preencha todas as informações necessárias.
6. Ao término do upload submeta seu aplicativo, no próprio ambiente da Cielo Store, para certificação e preencha todas as informações necessárias.
7. Assim que a certificação for concluída, o desenvolvedor receberá um e-mail e deverá acessar novamente a Cielo Store para promover o aplicativo para produção.
8. Agora seu aplicativo já está disponível para download na Cielo Store. Sucesso!! Aproveite ao máximo tudo que a Integração Local Cielo LIO pode oferecer para você!!

## Release Notes

Na tabela abaixo, é possível verificar as funcionalidades do SDK disponíveis por versão da Cielo LIO e Cielo Mobile.

| Funcionalidade                                                                                                                                                                                                                    | Versão Cielo LIO | Versão Cielo Mobile |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------- |
| createDraftOrder(String reference); placeOrder(Order order); updateOrder(Order order); checkoutOrder(String orderId, PaymentListener paymentListener); checkoutOrder(String orderId,long value, PaymentListener paymentListener); | 1.10.2           | 1.9.1               |
| retrievePaymentType(); checkoutOrder(String orderId,long value, String primaryCode, String secondaryCode, PaymentListener,paymentListener);                                                                                       | 1.12.0           | 1.10.3              |
| retrieveOrders(int pageSize, int page);                                                                                                                                                                                           | 1.13.0           | 1.10.5              |
| checkoutOrder (String orderId,long value, String primaryCode, String secondaryCode, Long installments, PaymentListener paymentListener);                                                                                          | 1.14.0           | 1.12.1              |
| cancelOrder (Context context, String orderId, Payment payment, CancellationListener paymentListener); cancelOrder(Context context, String orderId, Payment payment, Long amount, CancellationListener paymentListener);           | 1.16.7           | 1.12.10             |

> **Atenção:** Se for utilizada uma funcionalidade que não esteja disponível, será lançada uma exceção – UnsupportedOperationExcepetion –, que deve ser tratada pelo aplicativo.

Para descobrir a versão do aplicativo Cielo LIO (versão do Launcher) e Cielo Mobile, bem como utilizar todas as funcionalidades do Cielo LIO Order Manager SDK, acesse “Sobre a Cielo LIO” (Ajuda -> Sobre a Cielo LIO) para obter as informações sobre os aplicativos instalados na Cielo LIO.

---

## Code Sample

O código do exemplo do aplicativo integrado com o Cielo LIO Order Manager SDK encontra-se disponível no [GitHub](https://github.com/DeveloperCielo/LIO-SDK-Sample-Integracao-Local).

## Vídeo Demo

No vídeo abaixo, é possível ver um exemplo de aplicativo integrado com o Cielo LIO Order Manager SDK, utilizando a função de pagamento de valores do SDK.

[![Vídeo Demo](https://img.youtube.com/vi/d7y-x6p36YU/0.jpg)](https://www.youtube.com/watch?v=d7y-x6p36YU)

Clique na imagem acima, para acessar o vídeo

# Integração Remota

## Apresentação

O objetivo da Integração Remota da Cielo LIO é permitir que o lojista continue utilizando sua solução de frente de caixa (Automação Comercial ou PDV) e a integre com o módulo de pedidos e pagamentos da Cielo LIO através de uma API construída no padrão RESTful.

Dessa forma, toda a gestão do estabelecimento comercial fica sob responsabilidade da Automação Comercial e, no momento de realizar o pagamento, a Cielo LIO é utilizada.

![integração remota](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/diagrama-overview.jpg)

A API Order Manager da Cielo LIO possui as seguintes características:

- Recursos REST, de forma que seja possível acessar por meio de semântica HTTP padrão.
- Códigos de status HTTP para comunicar o sucesso/erro nas chamadas.
- Todas as requisições e respostas encontram-se no formato JSON.
- As seções abaixo possuem todas as informações necessárias para realizar a integração de forma rápida e segura.

## Vídeo Demo

No vídeo abaixo é possível ver um exemplo de Automação Comercial integrada com a API Order Manager da Cielo LIO.

[![Vídeo Demo](https://img.youtube.com/vi/QxfTkJEN1Qs/0.jpg)](https://www.youtube.com/watch?v=QxfTkJEN1Qs)

Clique na imagem acima, para acessar o vídeo.

### Code Sample

O código do exemplo da Automação Comercial integrada com a API Order Manager da Cielo LIO encontra-se disponível no [GitHub](https://github.com/cielolabsbr/SampleAutomacaoComercial1.2).

## Fluxo para Integração

![fluxo integração remota](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/fluxogram-remote-new.png)

## API Docs

Nessa documentação, o desenvolvedor encontra todas as informações sobre os Endpoints, Entidades e Recursos disponíveis na API.

Você poderá consultar os dados de entrada, exemplos de requisição e os dados de saída. Assim como entender o fluxo básico da utilização da API Order Manager da Cielo LIO.

### Endpoints

Todas as chamadas devem ser executadas utilizando as respectivas credenciais dos ambientes de sandbox e produção.

#### Sandbox

O ambiente de sandbox é destinado à realização de testes com parceiros da Cielo. Esse ambiente usa simuladores de integração. Assim, as operações não são executadas em ambiente produtivo.

Para utilizar o ambiente de sandbox, não é necessário que você forneça o número do estabelecimento. Você poderá iniciar os testes sem a necessidade de ter uma Cielo LIO. Para obter os tokens de sandbox, crie uma conta no portal e crie o Client-Id.

Utilize o endereço de sandbox abaixo para realizar os testes:

> https://api.cielo.com.br/sandbox-lio/order-management/v1

#### Produção

O ambiente de produção é o ambiente transacional integrado ao ambiente da Cielo. As operações realizadas nesse ambiente não podem ser desfeitas.

Para utilizar o ambiente de produção, é necessário que você entre em contato através do formulário. Juntamente com os dados pessoais, forneça o número do estabelecimento. Para utilizar o ambiente de produção, é necessário que você possua uma Cielo LIO.

Utilize o endereço de produção abaixo para realizar as requisições:

> https://api.cielo.com.br/order-management/v1

Já fez os testes em sandbox e deseja solicitar os tokens?

Clique em [Solicitar Tokens](https://desenvolvedores.cielo.com.br/api-portal/content/solicitar-tokens-para-producao) ou acesse o menu “Desenvolvedor” no Portal de Desenvolvedores e escolha a opção "Solicitar tokens”.

É necessário estar logado!

### HTTP Headers

Todas as chamadas da API Integração Remota Cielo LIO Order Manager necessitam que as informações abaixo estejam presentes no Header na requisição:

**Client-Id**: Identificação de acesso. Sua geração ocorre no momento da criação pelo painel do desenvolvedor. Seu valor pode ser visualizado na coluna “Client ID”, dentro do menu “Desenvolvedor” -> “Client ID Cadastrados”.

**Access-Token**:Identificação do token de acesso, que armazena as regras de acesso permitidas ao Client ID. Sua geração ocorre no momento da criação do Client ID pelo painel do desenvolvedor. Seu valor pode ser visualizado clicando em “detalhes” na coluna “Access Tokens”, dentro do menu “Desenvolvedor” -> “Client ID Cadastrados”.

**Merchant-Id**: Token que identifica o estabelecimento comercial dentro do servidor Order Manager da Cielo LIO. Sua geração ocorre durante o processo de cadastro do Client ID. Seu valor pode ser visualizado na coluna “Merchant ID”, dentro do menu “Desenvolvedor” -> “Client ID Cadastrados”.

### HTTP Status Code

| Código | Erro                  | Descrição                                                                                |
| ------ | --------------------- | ---------------------------------------------------------------------------------------- |
| 200    | OK                    | Operação realizada com sucesso.                                                          |
| 201    | Created               | A solicitação foi realizada, resultando na criação de um novo recurso.                   |
| 204    | Empty                 | Operação realizada com sucesso, mas nenhuma resposta foi retornada.                      |
| 400    | Bad Request           | A requisição possui parâmetro(s) inválido(s).                                            |
| 401    | Unauthorized          | O token de acesso não foi informado ou não possui acesso às APIs.                        |
| 403    | Forbidden             | O acesso ao recurso foi negado.                                                          |
| 404    | Not Found             | O recurso informado no request não foi encontrado.                                       |
| 413    | Request is to Large   | A requisição está ultrapassando o limite permitido para o perfil do seu token de acesso. |
| 422    | Unprocessable Entity  | A requisição possui parâmetros obrigatórios não informados.                              |
| 429    | Too Many Requests     | O consumidor estourou o limite de requisições por tempo.                                 |
| 500    | Internal Server Error | Erro não esperado; algo está quebrado na API                                             |

### Status de pedido

Abaixo é apresentada uma máquina de estados, com os possíveis estados que um pedido pode assumir desde o momento de sua criação até o seu término:

![status do pedido](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/diagrama-lifecycle-new.png)

### Entidades

#### Order

A Order é uma representação de um pedido para a venda de um ou mais produtos e/ou serviços. É fundamental que exista uma Order para que um pagamento seja realizado na Cielo LIO.

| Campo        | Tipo                | Descrição                                                                                                                                 | Obrigatório     |
| ------------ | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | --------------- |
| id           | Texto               | UUID que identifica unicamente o pedido.                                                                                                  | criado pela API |
| number       | Texto               | Número do pedido. Geralmente, esse número representa o identificador do pedido em um sistema externo através da integração com parceiros. | Não             |
| reference    | Texto               | Referência do pedido. Utilizada para facilitar o acesso ou a localização do mesmo.                                                        | Não             |
| status       | Texto               | Status do pedido (ENTERED, RE-ENTERED, PAID, CANCELED e CLOSED).                                                                          | Sim             |
| created_at   | Texto               | Data de criação do pedido. A data deve estar no formato: YYYY-MM-DDThh:mm:ssZ (Exemplo: 20151020T13:13:29.000Z).                          | criado pela API |
| updated_at   | Texto               | Data da última atualização do pedido. A data deve estar no formato: YYYY-MM-DDThh:mm:ssZ (Exemplo: 20151020T13:13:29.000Z).               | criado pela API |
| items        | Lista (Order Item)  | Lista de itens contidos no pedido.                                                                                                        | Sim             |
| notes        | Texto               | Campo disponível para uso do Merchant para comunicação.                                                                                   | Não             |
| transactions | Lista (Transaction) | Lista de transações de pagamento (ou outros tipos) efetuadas no pedido.                                                                   | Sim             |
| price        | Número              | Valor total do pedido. Exemplo: O valor de R\$ 10,00 é representado como 1000.                                                            | Sim             |
| remaining    | Número              | Valor restante do pagamento do pedido. Exemplo: O valor de R\$ 10,00 é representado como 1000.                                            | Sim             |

#### Order Item

O Order Item é uma representação dos itens presentes em uma Order. É obrigatória a existência de, no mínimo, um Item para uma Order.

| Campo           | Tipo   | Descrição                                                                                                                   | Obrigatório |
| --------------- | ------ | --------------------------------------------------------------------------------------------------------------------------- | ----------- |
| sku             | Texto  | SKU do produto. Exemplo: c2f5fb9a-5542-406e-8b79-17892329cda8.                                                              | Sim         |
| name            | Texto  | Nome do produto.                                                                                                            | Não         |
| description     | Texto  | Descrição do produto.                                                                                                       | Não         |
| unit_price      | Número | Valor unitário do produto. Exemplo: O valor de R\$ 10,00 é representado como 1000.                                          | Sim         |
| quantity        | Número | Quantidade de itens. Caso não seja informado, será considerado o valor 1.                                                   | Não         |
| unit_of_measure | Texto  | Unidade de medida (EACH, HOURS, DAYS, SECONDS, CRATE_OF_12, SIX_PACK, GALLON e LITRE).                                      | Sim         |
| details         | Texto  | Detalhes do produto.                                                                                                        | Não         |
| created_at      | Texto  | Data de criação do pedido. A data deve estar no formato: YYYY-MM-DDThh:mm:ssZ (Exemplo: 20151020T13:13:29.000Z).            | Não         |
| updated_at      | Texto  | Data de última atualização do pedido. A data deve estar no formato: YYYY-MM-DDThh:mm:ssZ (Exemplo: 20151020T13:13:29.000Z). | Sim         |

#### Transaction

A Transaction é uma representação com todos os pagamentos que foram realizados em uma Order. O objetivo é utilizá-la para consultar os pagamentos (transactions) que foram efetuados em uma Order.

| Campo              | Tipo   | Descrição                                                                   | Obrigatório |
| ------------------ | ------ | --------------------------------------------------------------------------- | ----------- |
| id                 | Texto  | "UUID" que identifica unicamente a transação.                               | Sim         |
| external_id        | Texto  | Identificador unico ordem.                                                  | Sim         |
| status             | Texto  | Status da transação (CONFIRMED, PENDING e CANCELLED).                       | Sim         |
| terminal_number    | Número | Número do terminal da Cielo LIO em que o pagamento foi realizado.           | Sim         |
| authorization_code | Número | Código de autorização da transação.                                         | Sim         |
| number             | Número | Número Sequencial Único (NSU) da transação.                                 | Sim         |
| amount             | Número | Valor da transação. Exemplo: O valor de R\$ 10,00 é representado como 1000. | Sim         |
| transaction_type   | Texto  | Tipo da transação (PAYMENT e CANCELLATION).                                 | Sim         |

#### Card

O Card é uma representação do cartão que foi utilizado para realizar o pagamento/transação.

| Campo | Tipo   | Descrição                           | Obrigatório |
| ----- | ------ | ----------------------------------- | ----------- |
| brand | Texto  | Bandeira do cartão (VISA e MASTER). | Sim         |
| mask  | Número | Número do cartão mascarado          | Sim         |

#### Payment Product

O Payment Product é uma representação da forma de pagamento utilizada para realizar um pagamento.
Ex.: Crédito, Débito, etc.

| Campo                  | Tipo   | Descrição                                                    | Obrigatório |
| ---------------------- | ------ | ------------------------------------------------------------ | ----------- |
| primary_product_name   | Texto  | Forma de pagamento (CREDITO ou DEBITO)                       | Sim         |
| secondary_product_name | Texto  | Tipo de pagamento (A VISTA, PARCELADO LOJA ou PARCELADO ADM) | Sim         |
| number_of_quotas       | Número | Número de parcelas (0 para pagamentos à vista)               | Sim         |

### Recursos

#### POST - Criar um pedido

Esse recurso realiza a criação de um pedido no servidor do Order Manager.

> Endpoint:
>
> **POST** /orders

Dados de entrada:

| Campo | Tipo  | Descrição              | Obrigatório |
| ----- | ----- | ---------------------- | ----------- |
| order | Order | Informações do pedido. | Sim         |

Exemplo de requisição:

```
{
    "number": "0992f1d5cee540d9a9648f4d6a9e4aa6",
    "reference": "PEDIDO #1234",
    "status": "DRAFT",
    "items": [{
            "sku": "ede8f84a8b8645cb8e576a593c25c6ed",
            "name": "produto 1",
            "unit_price": 500,
            "quantity": 2,
            "unit_of_measure": "EACH"
        },
        {
            "sku": "c2f5fb9a5542406e8b7917892329cda8",
            "name": "produto 2",
            "unit_price": 1500,
            "quantity": 3,
            "unit_of_measure": "EACH"
        },
        {
            "sku": "b2j4bn6j93461385r5n90453407hjk0",
            "name": "produto 3",
            "unit_price": 550,
            "quantity": 3,
            "unit_of_measure": "EACH"
        },
        {
            "sku": "55329cda842406e8cv2f5gdf96985152d",
            "name": "produto 4",
            "unit_price": 2005,
            "unit_of_measure": "EACH"
        }
    ],
    "notes": "Mesa 1",
    "price": 9155
}
```

Dados de saída:

| Campo | Tipo | Descrição                | Obrigatório |
| ----- | ---- | ------------------------ | ----------- |
| id    | body | Identificador do pedido. | Sim         |

Exemplo de resposta:

```
{
    "id": "2e1d7b07-dcee-4a09-8d09-3bb02d94169d"
}
```

#### GET - Consultar pedido

Esse recurso é utilizado para obter informações sobre um pedido específico. O id do pedido é utilizado para realizar a chamada.

> Endpoint:
>
> **GET** /orders<id>

Dados de entrada:

| Campo | Tipo           | Descrição                | Obrigatório |
| ----- | -------------- | ------------------------ | ----------- |
| id    | path parameter | Identificador do pedido. | Sim         |

Exemplo de requisição:

> **GET** https://api.cielo.com.br/order-management/v1/orders/c393ce9f-3741-413f-8ad5-2f142eaed51f

Dados de saída:

| Campo | Tipo  | Descrição                              | Obrigatório |
| ----- | ----- | -------------------------------------- | ----------- |
| order | Order | Informações sobre o pedido consultado. | Não         |

Exemplo de resposta:

```
{
    {
    "id": "b4d8a7dc-4250-48a3-bf18-d560d4508368",
    "number": "0992f1d5-cee5-40d9-a964-8f4d6a9e4aa6",
    "reference": "LOJA SUCO #1",
    "status": "ENTERED",
    "notes": "Mesa 6",
    "price": 5250,
    "created_at": "2016-09-06T19:09:49Z",
    "updated_at": "2016-09-06T19:09:49Z",
    "order_type": "PAYMENT",
    "merchant": "0010920335960001",
    "source_id": "4QeQD63ZeKsz",
    "items": [{
            "id": "0687f00a-0aea-48f7-85d0-64bc31977734",
            "sku": "0000001",
            "name": "Suco Detox",
            "unit_price": 800,
            "quantity": 1,
            "unit_of_measure": "EACH"
        },
        {
            "id": "cf561196-4e4c-436b-816b-80190e9a705f",
            "sku": "0000010",
            "name": "Suco de Uva",
            "unit_price": 450,
            "quantity": 5,
            "unit_of_measure": "EACH"
        },
        {
            "id": "16b4b10b-9967-477b-91a2-ecc02e6ff40c",
            "sku": "0000011",
            "name": "Suco de Tomate",
            "unit_price": 500,
            "quantity": 2,
            "unit_of_measure": "EACH"
        },
        {
            "id": "8500c747-1740-47cf-908a-3ab0f8b44193",
            "sku": "0000100",
            "name": "Suco de Abacaxi",
            "unit_price": 400,
            "quantity": 3,
            "unit_of_measure": "EACH"
        }
    ],
    "transactions": []
}
}
```

#### GET - Consultar todos os Pedidos

Esse recurso é utilizado para obter a lista e as informações de todos os pedidos cadastrados no Order Manager.

> Endpoint:
>
> **GET** /orders/

Dados de entrada:

| Campo | Tipo | Descrição | Obrigatório |
| ----- | ---- | --------- | ----------- |
| N/A   |      |           |             |

Exemplo de requisição:

> **GET** https://api.cielo.com.br/order-management/v1/orders/

Dados de saída:

| Campo | Tipo  | Descrição                              | Obrigatório |
| ----- | ----- | -------------------------------------- | ----------- |
| order | Order | Informações sobre o pedido consultado. | Não         |

Exemplo de resposta:

```
{
    "id": "b4d8a7dc-4250-48a3-bf18-d560d4508368",
    "number": "0992f1d5-cee5-40d9-a964-8f4d6a9e4aa6",
    "reference": "LOJA SUCO #1",
    "status": "ENTERED",
    "notes": "Mesa 6",
    "price": 5250,
    "created_at": "2016-09-06T19:09:49Z",
    "updated_at": "2016-09-06T19:09:49Z",
    "order_type": "PAYMENT",
    "merchant": "0010920335960001",
    "source_id": "4QeQD63ZeKsz",
    "items": [{
            "id": "0687f00a-0aea-48f7-85d0-64bc31977734",
            "sku": "0000001",
            "name": "Suco Detox",
            "unit_price": 800,
            "quantity": 1,
            "unit_of_measure": "EACH"
        },
        {
            "id": "cf561196-4e4c-436b-816b-80190e9a705f",
            "sku": "0000010",

            "name": "Suco de Uva",
            "unit_price": 450,
            "quantity": 5,
            "unit_of_measure": "EACH"
        },
        {
            "id": "16b4b10b-9967-477b-91a2-ecc02e6ff40c",
            "sku": "0000011",
            "name": "Suco de Tomate",
            "unit_price": 500,
            "quantity": 2,
            "unit_of_measure": "EACH"
        },
        {
            "id": "8500c747-1740-47cf-908a-3ab0f8b44193",
            "sku": "0000100",
            "name": "Suco de Abacaxi",
            "unit_price": 400,
            "quantity": 3,
            "unit_of_measure": "EACH"
        }
    ],
    "transactions": []
}
```

#### PUT- Alterar status de um pedido

Esse recurso realiza a alteração do status de um pedido criado. O id do pedido é utilizado para realizar a chamada.

As possíveis alterações de status são:

- PLACE (Liberar um pedido para pagamento, exibir pedido na Cielo LIO)
- PAY (Alterar um pedido para pago)
- CLOSE (Fechar um pedido)

> Endpoint:
>
> **PUT** /orders/<id>?operation=<operation>

Dados de entrada:

| Campo     | Tipo            | Descrição                                                                                                                                                           | Obrigatório |
| --------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| id        | path parameter  | Identificador do pedido.                                                                                                                                            | Sim         |
| operation | query parameter | Operação que deve ser executada. As possíveis operações são: place (Liberar um pedido para pagamento), pay (deixar um pedido como pago) e close (Fechar um pedido). | Sim         |

Exemplo de requisição:

> **PUT** https://api.cielo.com.br/order-management/v1/orders/db815e66-e5b6-497c-8444-2120cc87d33a?operation=PLACE

Dados de saída:

| Campo | Tipo | Descrição | Obrigatório |
| ----- | ---- | --------- | ----------- |
| N/A   |      |           |             |

Exemplo de resposta:

```
N/A
```

O retorno 200 dessa operação representa sucesso na requisição.

#### DELETE - Excluir um pedido

Esse recurso é utilizado para excluir um pedido do servidor do Order Manager. O id do pedido é utilizado para realizar a chamada.

> Somente os pedidos com status **DRAFT** podem ser excluídos.
>
> Endpoint:
>
> **DELETE** /orders/<id>

Dados de entrada:

| Campo | Tipo           | Descrição                | Obrigatório |
| ----- | -------------- | ------------------------ | ----------- |
| id    | path parameter | Identificador do pedido. | Sim         |

Exemplo de requisição:

> **DELETE** https://api.cielo.com.br/order-management/v1/orders/db815e66-e5b6-497c-8444-2120cc87d33a

Dados de saída:

| Campo | Tipo | Descrição | Obrigatório |
| ----- | ---- | --------- | ----------- |
| N/A   |      |           |             |

Exemplo de resposta:

```
N/A
```

O retorno 200 dessa operação representa sucesso na requisição.

#### POST - Adicionar Item/Itens em um Pedido

Esse recurso é utilizado para adicionar um ou mais itens em um pedido já criado. O id do pedido é utilizado para realizar a chamada.

> Somente os pedidos com status **DRAFT** podem ser excluídos.
>
> Endpoint:
>
> **POST** /orders/<id>/items

Dados de entrada:

| Campo | Tipo           | Descrição                | Obrigatório |
| ----- | -------------- | ------------------------ | ----------- |
| id    | path parameter | Identificador do pedido. | Sim         |

Exemplo de requisição:

```
{
    "sku": "ede8f84a8b8645cb8e576a593c25c6ed",
    "name": "produto 1"
    "unit_price": 500,
    "quantity": 2,
    "unit_of_measure": "EACH"
}
```

Dados de saída:

| Campo | Tipo | Descrição | Obrigatório |
| ----- | ---- | --------- | ----------- |
| N/A   |      |           |             |

Exemplo de resposta:

```
N/A
```

O retorno 200 dessa operação representa sucesso na requisição.

#### GET - Consultar os itens de um pedido

Esse recurso é utilizado para consultar os itens presentes em um pedido. O id do pedido é utilizado para realizar a chamada.

> Endpoint:
>
> **GET** /orders/<id>/items

Dados de entrada:

| Campo | Tipo           | Descrição                | Obrigatório |
| ----- | -------------- | ------------------------ | ----------- |
| id    | path parameter | Identificador do pedido. | Sim         |

Exemplo de requisição:

> **GET** https://api.cielo.com.br/order-management/v1/orders/c393ce9f-3741-413f-8ad5-2f142eaed51f/items

Dados de saída:

| Campo      | Tipo              | Descrição                    | Obrigatório |
| ---------- | ----------------- | ---------------------------- | ----------- |
| orderItems | Lista (OrderItem) | Lista de itens de um pedido. | Sim         |

Exemplo de resposta:

```
[{
        "id": 1,
        "sku": "ede8f84a8b8645cb8e576a593c25c6ed",
        "name": "produto 1"
        "unit_price": 500,
        "quantity": 2,
        "unit_of_measure": "EACH"
    },
    {
        "id": 2,
        "sku": "c2f5fb9a5542406e8b7917892329cda8",
        "name": "produto 1"
        "unit_price": 1500,
        "quantity": 3,
        "unit_of_measure": "EACH"
    }
]
```

#### PUT - Alterar um item em um pedido

Esse recurso permite alterar informações de um item de um pedido. O id do pedido e o id_item são utilizados para realizar a chamada.

> Somente os pedidos com status **DRAFT** podem ter itens alterados.
>
> Endpoint:
>
> **PUT** /orders/<id>/items/<id_item>

Dados de entrada:

| Campo   | Tipo           | Descrição                        | Obrigatório |
| ------- | -------------- | -------------------------------- | ----------- |
| id      | path parameter | Identificador do pedido.         | Sim         |
| id_item | path parameter | Identificador do item do pedido. | Sim         |

Exemplo de requisição:

> **PUT** https://api.cielo.com.br/order-management/v1/orders/a9398720-9f78-4fa4-a5d4-ba54ba8009e7
> /items/8484df74-eca6-4850-8e4c-35653af0bd31

```
{
    "sku": "ede8f84a8b8645cb8e576a593c25c6ed",
    "unit_price": 500,
    "quantity": 2,
    "unit_of_measure": "EACH"
}
```

Dados de saída:

| Campo | Tipo | Descrição | Obrigatório |
| ----- | ---- | --------- | ----------- |
| N/A   |      |           |             |

O retorno 200 dessa operação representa sucesso na requisição.

#### DELETE - Excluir Item de um pedido

Esse recurso é utilizado para excluir um item presente em um pedido. O id do pedido e o id_item são utilizados para realizar a chamada.

> Somente os pedidos com status **DRAFT** podem ter itens alterados.
>
> Endpoint:
>
> **DELETE** /orders/<id>/items/<id_item>

Dados de entrada:

| Campo   | Tipo           | Descrição                        | Obrigatório |
| ------- | -------------- | -------------------------------- | ----------- |
| id      | path parameter | Identificador do pedido.         | Sim         |
| id_item | path parameter | Identificador do item do pedido. | Sim         |

Exemplo de requisição:

> **DELETE** https://api.cielo.com.br/order-management/v1/orders/a9398720-9f78-4fa4-a5d4-ba54ba8009e7/items/8484df74-eca6-4850-8e4c-35653af0bd31

Dados de saída:

| Campo | Tipo | Descrição | Obrigatório |
| ----- | ---- | --------- | ----------- |
| N/A   |      |           |             |

O retorno 200 dessa operação representa sucesso na requisição.

#### POST - Adicionar uma Transação

> Recurso utilizado somente para **Ambiente de Sandbox**

Esse recurso permite que o desenvolvedor simule as transações financeiras, adicionando-as manualmente, sendo possível entender o funcionamento em uma Order.

> Endpoint:
>
> **POST** /orders/<id>/transactions

Dados de entrada:

| Campo        | Tipo                | Descrição                | Obrigatório |
| ------------ | ------------------- | ------------------------ | ----------- |
| Transactions | Lista (Transaction) | Informações da Transação | Sim         |

Exemplo de requisição:

> **POST** https://api.cielo.com.br/order-management/v1/orders/a9398720-9f78-4fa4-a5d4-ba54ba8009e7/transactions

```
{
  "id": "442bbdbe-41c8-4e22-83ee-e1a849ed3cb5",
  "external_id": "0b37f0d8-017a-4b11-91b9-ec1bb3e8fed3",
  "status": "CONFIRMED",
  "terminal_number": "12345678",
  "authorization_code": "008619",
  "number": "672836",
  "amount": 2000,
  "transaction_type": "PAYMENT",
  "payment_fields": {
    "primary_product_name": "CREDITO",
    "secondary_product_name": "A VISTA",
    "number_of_quotas": 0
  },
  "card": {
    "brand": "VISA",
    "mask": "************5487"
  }
}
```

Dados de saída:

| Campo | Tipo   | Descrição                  | Obrigatório |
| ----- | ------ | -------------------------- | ----------- |
| id    | number | Identificador da Transação | SIM         |

```
{
id: "00219dd0-1c13-46da-91e5-1c313f0d2e83"
}
```

Em ambiente de Sandbox, onde não há necessidade de ter uma Cielo LIO, e consequentemente não é necessário possuir o número do estabelecimento, faz total sentido fazer essa chamada deste recurso.

Já em ambiente de Produção quem irá criar as transactions é a própria Cielo LIO conforme os pagamentos forem efetuados.

#### GET - Consultar as transações de um pedido

Esse recurso é utilizado para obter as informações de todas as transações realizadas em um pedido. O id do pedido é utilizado para realizar a chamada.
Em ambiente de produção, uma vez que um pagamento for realizado na Cielo LIO a transactions será adicionada automaticamente no pedido e então, será possível obter as informações do pagamento realizado a partir da chamada deste recurso.

> Endpoint:
>
> **GET** /orders/<id>/transactions

Dados de entrada:

| Campo | Tipo           | Descrição                | Obrigatório |
| ----- | -------------- | ------------------------ | ----------- |
| id    | path parameter | Identificador do pedido. | Sim         |

Exemplo de requisição:

> **GET** https://api.cielo.com.br/order-management/v1/orders/c393ce9f-3741-413f-8ad5-2f142eaed51f/transactions

Dados de saída:

| Campo        | Tipo                | Descrição                         | Obrigatório |
| ------------ | ------------------- | --------------------------------- | ----------- |
| transactions | Lista (Transaction) | Lista de transações de um pedido. | SIM         |

Exemplo de resposta:

```
[
{
  "id": "442bbdbe-41c8-4e22-83ee-e1a849ed3cb5",
  "external_id": "0b37f0d8-017a-4b11-91b9-ec1bb3e8fed3",
  "status": "CONFIRMED",
  "terminal_number": "77102648",
  "authorization_code": "008619",
  "number": "672836",
  "amount": 2000,
  "transaction_type": "PAYMENT",
  "payment_fields": {
  "primary_product_name": "CREDITO",
  "secondary_product_name": "A VISTA",
    "number_of_quotas": 0
  },
  "card": {
    "brand": "VISA",
    "mask": "************3542"
  }
}
]
```

#### Cancelar Pedidos

O cancelamento de pedidos é realizado apenas através da Cielo LIO.
Selecione a função Cancelamento de Vendas e digite o CNPJ da empresa (o mesmo que pode ser visualizado através do comprovante de pagamento). O sistema irá solicitar a senha para realização da operação, que pode ser obtida através de abertura de ticket na página de Suporte do Portal de desenvolvedores.
Siga todos os passos indicados nas telas seguintes para o cancelamento da venda. É importante salientar que um cancelamento só pode ser realizado em ser valor integral.

#### GET - Consultar as transações canceladas de um pedido

Esse recurso é utilizado para obter as informações de todas as transações canceladas em um pedido. O id do pedido é utilizado para realizar a chamada.
Em ambiente de produção, uma vez que o cancelamento for realizado na Cielo LIO a transactions será adicionada automaticamente no pedido juntamente com a transaction do pagamento original.

> Endpoint:
>
> **GET** /orders/<id>/transactions

Dados de entrada:

| Campo | Tipo           | Descrição                | Obrigatório |
| ----- | -------------- | ------------------------ | ----------- |
| id    | path parameter | Identificador do pedido. | Sim         |

Exemplo de requisição:

> **GET** https://api.cielo.com.br/order-management/v1/orders/c393ce9f-3741-413f-8ad5-2f142eaed51f/transactions

Dados de saída:

| Campo        | Tipo                | Descrição                         | Obrigatório |
| ------------ | ------------------- | --------------------------------- | ----------- |
| transactions | Lista (Transaction) | Lista de transações de um pedido. | SIM         |

Exemplo de resposta:

```
[
  {
    "id": "46019c39-989e-46e9-aa7d-d8e9414396b4",
    "external_id": "95185.99407021694",
    "status": "CONFIRMED",
    "terminal_number": "77102648",
    "authorization_code": "008619",
    "number": "672837",
    "amount": 2000,
    "transaction_type": "CANCELLATION",
    "payment_fields": {
    "primary_product_name": "CREDITO",
    "secondary_product_name": "A VISTA",
    "number_of_quotas": 0
  },
    "card": {
      "brand": "VISA",
      "mask": "************3542"
    }
  },
  {
    "id": "442bbdbe-41c8-4e22-83ee-e1a849ed3cb5",
    "external_id": "0b37f0d8-017a-4b11-91b9-ec1bb3e8fed3",
    "status": "CONFIRMED",
    "terminal_number": "77102648",
    "authorization_code": "008619",
    "number": "672836",
    "amount": 2000,
    "transaction_type": "PAYMENT",
    "payment_fields": {
    "primary_product_name": "CREDITO",
    "secondary_product_name": "A VISTA",
    "number_of_quotas": 0
   },
    "card": {
    "brand": "VISA",
    "mask": "************3542"
    }
  }
]
```

### Fluxo Básico Utilização API Order manager Cielo LIO

Abaixo você encontra um fluxo básico para enviar um pedido para a Cielo LIO utilizando a Integração Remota:

![fluxo_basico](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/fluxogram-order-manager-slim.png)

### Notificações de Mudanças na Order

O maior motivo da disponibilização da API RESTful do Order Manager é permitir que aplicações parceiras se integrem à plataforma da Cielo na cloud. Porém, uma vez que as aplicações parceiras submetem pedidos, estes devem ser pagos localmente na própria Cielo LIO. Sendo assim, as aplicações parceiras precisam de uma forma de receber notificações de mudanças do status e das transações realizadas na Order.

Para tal, é necessário que o parceiro disponibilize um Backend RESTful, que irá receber as notificações seguindo o formato abaixo. Uma vez recebidas as informações, o Backend tem a liberdade de ser utilizado da forma mais adequada ao modelo de negócio.

#### POST - Notificação de Mudança de Status

A cada modificação de status em um pedido, o servidor do Order Manager envia, via comando, as informações para o Backend do parceiro.

> **Atenção:** O backend do parceiro deve possuir o status anterior

Requisição do Order Manager

> **POST** <url_cadastrada_pelo_parceiro>

Exemplo de informação enviada pelo Order Manager

```json
{
  "id": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
  "number": "Pedido #547",
  "status": "CLOSED",
  "price": 2936,
  "created_at": "2018-11-29T15:54:25Z",
  "updated_at": "2018-11-29T15:54:25Z",
  "items": [
    {
      "id": 0101010101,
      "sku": "AVULSO",
      "name": "Valor Avulso",
      "description": "Valor Avulso",
      "unit_price": 2936,
      "quantity": 1,
      "unit_of_measure": "EACH",
      "details": "Valor Avulso",
      "reference": null,
      "uuid": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
      "order_id": 0101010101,
      "created_at": "2018-11-29T15:54:25Z",
      "updated_at": "2018-11-29T15:54:25Z",
      "sku_type": null
    }
  ],
  "transactions": [
    {
      "id": 01010101,
      "uuid": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
      "external_id": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
      "transaction_type": "payment",
      "status": "CONFIRMED",
      "description": "",
      "terminal_number": "01010101",
      "number": "010101",
      "authorization_code": "010101",
      "amount": 2936,
      "order_id": 0101010101,
      "created_at": "2018-11-29T15:54:25Z",
      "updated_at": "2018-11-29T15:54:25Z",
      "payment_fields": {
        "pan": "************1111",
        "v40Code": 1,
        "typeName": "VENDA A DEBITO",
        "cityState": "SAO PEDRO DA ALDEIA RJ",
        "clientName": "********",
        "serviceTax": 0,
        "statusCode": 1,
        "boardingTax": 0,
        "hasPassword": true,
        "hasWarranty": false,
        "productName": "DEBITO A VISTA",
        "requestDate": 1543506847000,
        "changeAmount": 0,
        "documentType": "J",
        "entranceMode": "010101010101",
        "hasSignature": false,
        "merchantCode": "0101010101010101",
        "merchantName": "*********",
        "applicationId": "cielo.launcher",
        "totalizerCode": 81,
        "upFrontAmount": 0,
        "creditAdminTax": 0,
        "firstQuotaDate": 0,
        "interestAmount": 0,
        "isExternalCall": true,
        "numberOfQuotas": 0,
        "applicationName": "cielo.launcher.DIRECT_SALE",
        "avaiableBalance": 0,
        "cardCaptureType": 0,
        "finalCryptogram": "818E32AB68FE0A60",
        "hasConnectivity": true,
        "merchantAddress": "R. TESTE",
        "paymentTypeCode": 1,
        "firstQuotaAmount": 0,
        "hasSentReference": false,
        "isFinancialProduct": true,
        "primaryProductCode": 2000,
        "primaryProductName": "DEBITO",
        "hasSentMerchantCode": false,
        "cardLabelApplication": "Debit",
        "paymentTransactionId": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
        "secondaryProductCode": 1,
        "secondaryProductName": "A VISTA",
        "originalTransactionId": "0",
        "receiptPrintPermission": 1,
        "hasPrintedClientReceipt": false,
        "isDoubleFontPrintAllowed": false,
        "isOnlyIntegrationCancelable": false
      },
      "access_key": null
    }
  ]
}
```

#### POST - Notificação de Transação Realizada

A cada transação/pagamento realizada em um pedido, o servidor do Order Manager envia, via comando, as informações para o Backend do parceiro.

Requisição do Order Manager

> **POST** <url_cadastrada_pelo_parceiro>

Exemplo de informação enviada pelo Order Manager

```json
{
  "id": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
  "order_id": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
  "trasaction": {
    "id": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
    "external_id": "f0f0f0f0-f0f0-f0f0-f0f0-f0f0f0f0f0f0",
    "description": "",
    "status": "CONFIRMED",
    "terminal_number": "###324625",
    "authorization_code": "0#1#133",
    "number": "##50##",
    "amount": "1",
    "transaction_type": "PAYMENT",
    "payment_fields": {
      "primary_product_name": "CREDITO",
      "secondary_product_name": "A VISTA",
      "number_of_quotas": "0"
    },
    "card": {
      "brand": "MASTERCARD",
      "mask": "************0566"
    }
  }
}
```

# Cielo Store

## Sobre

A Cielo Store é a loja de aplicativos da Cielo LIO.

Foi um ambiente criado para parceiros, empresas de software e desenvolvedores possam criar seus aplicativos, publicar e disponibilizar seus aplicativos na Cielo Store para serem utilizados por clientes que usam a plataforma Cielo LIO.

Os lojistas poderão acessar a Cielo Store por meio da Cielo LIO e fazer download dos aplicativos que melhor atendem seu modelo de negócio e que têm por objetivo facilitar a gestão e controle de suas vendas, melhorar o relacionamento deles com seus clientes e impulsionar suas vendas

Os desenvolvedores poderão acessar o Dev Console para fazer a publicação de seus aplicativos e disponibilizar na Cielo Store.

## Arquitetura

Para entender a arquitetura da Cielo Store é necessário entender os conceitos abaixo:

- **Dev Console**
  Ambiente exclusivo para o desenvolvedor fazer o upload dos seus aplicativos.
  [Saiba mais](https://developercielo.github.io/manual/cielo-lio#dev-console)

- **Loja Privada**
  Modelo específico utilizado para distribuição de aplicativos próprios para os lojistas.
  [Saiba mais](https://developercielo.github.io/manual/cielo-lio#loja-privada)

- **Loja Publica**
  Aplicativos desenvolvidos para serem disponibilizados na loja de aplicativo Cielo Store. Esses aplicativos poderão ser baixados por estabelecimentos comerciais (lojistas) acessando a Cielo Store via Cielo LIO.
  [Saiba mais](https://developercielo.github.io/manual/cielo-lio#loja-publica)

## Dev Console

### Sobre

O Dev Console é o ambiente exclusivo para o desenvolvedor realizar o upload e gestão dos aplicativos desenvolvidos para a Cielo LIO.

No Dev Console o desenvolvedor consegue visualizar todos os seus aplicativos publicados sejam eles aplicativos próprios ou públicos.

Acesse agora o Dev Console: https://www.cieloliostore.com.br

### Status de um aplicativo

Todos os aplicativos publicados no Dev Console possuem os seguintes status:

**1 - Desenvolvimento**

Nesse estágio o desenvolvedor consegue realizar testes do seu aplicativo em uma Cielo LIO. E caso precise fazer alguma correção, basta publicar uma nova versão do aplicativo pelo Dev Console e então atualizar na Cielo LIO.

Para obter uma LIO durante o desenvolvimento, o desenvolvedor pode se credenciar na Cielo e solicitar uma Cielo LIO. Após o recebimento da LIO, basta solicitar a habilitação para LIO de Dev.

[Saiba mais](https://developercielo.github.io/manual/cielo-lio#lio-para-desenvolvedores)

**2 - Certificação**

Uma vez concluído os testes o desenvolvedor envia o aplicativo para Certificação. Nessa etapa o time da Ceritficação da Cielo entra em ação e irá validar o fluxo de funcionamento do aplicativo principalmente nas etapas integradas ao pagamento.

[Saiba mais](https://developercielo.github.io/manual/cielo-lio#promover-aplicativo-para-produção)

**3 - Produção**

Assim que o aplicativo for aprovado na certificação, o desenvolvedor poderá promover para produção.

[Saiba mais](https://developercielo.github.io/manual/cielo-lio#certificação-de-aplicativos)

No caso de Aplicativo Público em produção este estará disponpivel para download na Cielo Store

[Saiba mais](https://developercielo.github.io/manual/cielo-lio#aplicativos-públicos)

No caso de Aplicativo Próprio o desenvolvedor deverá solicitar a distribuição para as LIOs que devem receber seu aplicativo.

[Saiba mais](https://developercielo.github.io/manual/cielo-lio#distribuição-de-aplicativos-póprios)

### LIO para Desenvolvedores

Os desenvolvedores que desejam obter uma Cielo LIO, podem se credenciar na Cielo e solicitar o equipamento. Todo esse procedimento pode ser realizados via [site da Cielo](https://www.cielo.com.br/).

Após o recebimento da Cielo LIO, o desenvolvedor deve entrar em contato via canal do Portal de Desenvolvedores e solicitar a habilitação de sua LIO para LIO de Dev preenchendo as informações necessárias.

_É preciso ter uma conta criado no Dev Console para fazer essa solicitação_.

Nosso time irá realizar os procedimentos necessários e então, todos os aplicativos publicados pelo desenvolvedor que estejam no status de Desenvolvimento poderão ser baixados em sua Cielo LIO de desenvolvimento.

[Clique Aqui](https://desenvolvedores.cielo.com.br/api-portal/pt-br/content/suporte) para solicitar a habilitação de sua LIO para LIO de Dev.

### Promover Aplicativo para Desenvolvimento

O desenvolvedor deve realizar o upload do aplicativo no Dev Console e não mais receber automaticamente na Lio.

A partir desse momento, na lista de versões da tela de detalhe do aplicativo, terá uma opção "visualizar" na tabela.
Ao clicar nela, aparecerá um QR Code. Nesse momento, basta abrir o aplicativo Test Your App, que estará na Lio de dev, e ler esse QR Code.

Para realizar os testes de aplicativos em desenvolvimento, o desenvolvedor deve seguir os seguintes passos:

- Efetuar o upload do apk no Dev Console.

- Deve clicar em "instalar" na versão desejada, dentro da tela de detalhes do aplicativo, para gerar o QR Code.

![Devconsole](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/instalarapp.png)

- Abrir o aplicativo "Test Your App" em sua LIO de desenvolvimento e apontar para o QR Code gerado no Dev Console.

![QR Code](https://desenvolvedores.cielo.com.br/api-portal/sites/default/files/qrcode.png)

- A versão do app será baixada na Lio.

### Certificação de Aplicativos

O objetivo da certificação de aplicativos é garantir que todos os aplicativos presentes na plataforma Cielo LIO, sejam próprios ou públicos, estejam de acordo com as regras e critérios estabelecidos pela Cielo.

Para a Certificação de APPs ser efetivada com sucesso, é necessário possuir os seguintes itens para a aprovação da APP

- Fluxo de pagamento funcione corretamente
- Os conteúdos no aplicativos não violem as regras da Cielo
- Os SKUs dos produtos são enviados corretamente
- Informações para vitrine da Cielo Store estejam preenchidas corretamente, exclusivo para aplicativos públicos
- Gerar valores para teste até R\$0,05 centavos
- Não mencionar a palavra Cielo
- Caso o APP tenha webview, não ficar disponível a URL para a troca de URL dentro do APP. A URL não deverá aparecer.
- Não conter palavrão
- Não exibir imagens inapropriadas
- Não exibir imagens/nomes de concorrentes
- A versão a ser certificada deve ser maior do que a versão anterior. EX: versão anterior 1.0 / versão atual 1.1
- Preencher corretamente o formulário de envio para certificação. Informar as funções do SDK utilizadas pelo APP, Changelog do APP (mudanças feitas para a versão que está sendo enviada para certificação), dados de acesso ao APP (caso ele possua) fornecidos por completo, versão do SDK utilizada, versão do OS utilizada.
- Caso o APP rode em um servidor local, enviar um vídeo mostrando o fluxo do APP. Vídeos deverão ser atualizados conforme enviarem uma nova versão para certificação. Após gravar o vídeo do APP, mostrar a versão e data do vídeo.
- 100% das transações dever ser via Cielo

"Qualquer informação necessária que esteja faltando, resultará na reprovação automática do aplicativo"

### Promover Aplicativo para Produção

Assim que o aplicativo for aprovado na certificação, o desenvolvedor receberá um e-mail de notificação e então, deverá promover seu aplicativo para produção de forma que este fique:

- Disponível para download na Cielo Store (Aplicativo Público)
- Disponível para distribuição à lojistas específicos (Aplicativo Próprio)

### Mensagens de Erro

A tabela apresenta os possíveis erros que o desenvolvedor pode encontrar durante a utilização do Dev Console:

| Referência                                                              | Mensagem                                                                                                                                                                                  | Cenário                                                                                                                                                       | O que fazer?                                                                           |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| APP CREATED_ERROR                                                       | Aplicativo com esse package name já existe                                                                                                                                                | Desenvolvedor tentou enviar uma aplicação com package name já existente na loja.                                                                              | Alterar no arquivo Manifest o packageName da aplicação                                 |
| APP APK_PARSER_ERROR                                                    | O arquivo .apk é obrigatório                                                                                                                                                              | Desenvolvedor tentou executar o upload de uma aplicação e não anexou o arquivo .apk                                                                           | Clicar no botão "Adicione um APK" e certificar de que foi escolhido o arquivo correto. |
| APP APK_PARSER_ERROR                                                    | Não foi possível obter o atributo Name / Não foi possível obter o atributo Package Name / Não foi possível obter o atributo Version Name / Não foi possível obter o atributo Version Code | Desenvolvedor tentou executar o upload de uma aplicação onde o arquivo manifest ou o apk está corrompido ou com problemas na configuração do arquivo manifest | Rebuildar o apk e verificar se não existem erros no arquivo Manifest do Android        |
| SCREENSHOTS CREATED_WARNING                                             | Aplicativo criado, porém as screenshots não foram salvas!                                                                                                                                 | Na criação do app, o Desenvolvedor enviou screenshots onde os arquivos de imagem contém extensões incomuns ou desconhecidas.                                  | Editar o app e enviar arquivos de imagens com extensões conhecidas.                    |
| SCREENSHOTS UPDATED_WARNING                                             | Aplicativo atualizado, porém as screenshots não foram salvas!                                                                                                                             | Na edição do app, o Desenvolvedor enviou screenshots onde os arquivos de imagem contém extensões incomuns ou desconhecidas.                                   | Editar novamente o app e enviar arquivos de imagens com extensões conhecidas.          |
| VERSION PROMOTE_ERROR (esse cenário só ocorre com aplicativos públicos) | É necessário um EC cadastrado para promover essa versão para produção.                                                                                                                    | Após a aplicação ter tido a certificação aprovada, o Desenvolvedor tentou promover o app para produção, porém ainda não possui um EC.                         | Solicitar à Cielo a criação de um EC para poder promover a aplicação para promoção.    |

Caso você desenvolvedor não encontre o erro nesta tabela, abra um ticket para a equipe de suporte reportando o problema encontrado e lembre-se de listar as evidências do erro como prints de tela e mensagens de erro recebidas.

[Clique Aqui](https://desenvolvedores.cielo.com.br/api-portal/pt-br/content/suporte)

### Cielo App Data

Com a API Cielo App Data o desenvolvedor de um app poderá ter acesso à informações de compra dos seus aplicativos em um determinado terminal LIO.

#### Geração do Token

Para isso é necessário, previamente, gerar o API Token no Dev Console, que será usado na API App Data. Para geração do token siga o seguinte passo à passo:

1. Acesse e faça o seu login no Dev Console através do [link](https://www.cieloliostore.com.br)
2. Na aba **Apps públicos** selecione o App desejado
3. Clique na aba **API Token** e depois no botão **Gerar Token**
4. Uma vez o token gerado, copie e guarde o mesmo.

**Endpoint:** https://cieloliostore-api.m4u.com.br/api/v1/me

#### HTTP Headers

Todas as chamadas da API Cielo App Data necessitam que o API Token gerado no Dev Console esteja presente no Header das requisições:

- **Token:** Identificação do token de acesso, que armazena informações do App Público que deseja informações.

#### HTTP Query Parameters

Complementando o Header das requisições, a API Cielo App Data necessita que todas as chamadas contenham o EC (Número do Estabelecimento Comercial) e o Número Lógico (identificador do terminal LIO) nas suas requisições:

- **ec:** Identificação do Estabelecimento Comercial desejado para consulta.
- **logic_number:** Identificação do Terminal LIO desejado para consulta.

#### API

> **GET** / Detalhes de um produto

**ec** (required in query parameter) - “String”
**logic_number** (required in query parameter) - “String”
**token** (required in header) - “String”

Exemplo de resposta:

```
{
    "app": {
      "name": "string",
      "package_name": "string"
    },
    "purchase": {
        "status": "SUBSCRIBED",
        "plan": {
            "id": "string",
            "name": "string",
            "value": 0
        },
        "created_at": "string"
    },
    "payment": {
        "status": "PENDING"
    }
}
```

#### Opções de retorno por campo

**purchase.status:** “SUBSCRIBED” | “UNSUBSCRIBED”
**payment.status:** “PENDING” | “AT_RECURRENCE” | “PAID” | “OBLIGOR” | “CANCELED” | “CIELO_PURCHAASE”

**purchase.status:** “SUBSCRIBED”
**purchase.status:** “UNSUBSCRIBED”

**payment.status:** “PENDING” (Pagamentos com status pendente)
**payment.status:** “AT_RECURRENCE” (Pagamentos com status em recorrência)
**payment.status:** “PAID” (Pagamentos com status pago)
**payment.status:** “OBLIGOR” (Status do pagamento como inadimplente)
**payment.status:** “CANCELED” (Pagamentos cancelados)
**payment.status:** “CIELO_PURCHASE” (pagamentos isentos(compras de teste/desenvolvimento))

## Loja Privada

A loja privada foi um modelo criado para permitir a distribuição dos aplicativos próprios desenvolvidos pelo parceiro. É necessário solicitar a criação da Loja Privada para então ser possível fazer o upload de um aplicativo próprio no Dev Console.

[Clique Aqui](https://desenvolvedores.cielo.com.br/api-portal/pt-br/content/suporte) para solicitar a criação da Loja Privada.

A partir da Loja Privada criada, o desenvolvedor poderá publicar seu aplicativo no Dev Console selecionando sua loja privada.

A loja privada é essencial para realizar a distribuição de aplicativos próprios lojistas específicos.

### Upload de novos Aplicativos e novas versões na loja privada

Para realizar o upload de novos aplicativos próprios, acesse o Dev Console e adicione um novo aplicativo selecionando a opção de loja privada e em seguida selecione a loja privada referente a sua empresa.

Caso o desenvolvedor esteja realizando uma alteração ou atualização no aplicativo próprio, o desenvolvedor deverá fazer o upload de uma nova versão do aplicativo. Para isso clique em Detalhes do seu aplicativo e inicie o procedimento para adicionar uma nova versão.

Para enviar uma nova versão do aplicativo é obrigatório que:

- Garantir que a versão mais recente do aplicativo esteja com o mesmo package name da versão anterior;

- Alterar o “version code” e o “version name” dentro do arquivo manifest do aplicativo.

### Distribuição de Aplicativos na loja privada

Aqueles desenvolvedores que optarem por desenvolver aplicativos próprios e distribuir apenas para lojistas específicos devem efetuar o vinculo do EC do cliente a sua loja privada, pelo própio DevConsole

### Download de Aplicativo da loja privada na LIO

Para realizar o download de aplicativos próprios na Cielo LIO, execute o seguinte procedimento

Clique na aba Ajuda -> Minha LIO -> Buscar atualizações

## Loja Publica

Os aplicativos públicos são indicados para aqueles desenvolvedores e parceiros que desejam disponibilizar e escalar sua aplicação e permitir o download em todas os equipamentos de Cielo LIO distribuídos nos estabelecimentos comerciais (lojistas) no Brasil via aplicativo da Cielo Store.

Para conhecer mais sobre a Cielo Store, [Clique Aqui](https://developercielo.github.io/manual/cielo-lio#cielo-store)

### Upload de novos Aplicativos Públicos e novas versões

Para realizar o upload de novos aplicativos públicos, acesse o Dev Console e adicione um novo aplicativo selecionando a opção de loja pública e em seguida selecione o arquivo do aplicativo.

Caso o desenvolvedor esteja realizando uma alteração ou atualização no aplicativo público, o desenvolvedor deverá fazer o upload de uma nova versão do aplicativo. Para isso clique em Detalhes do seu aplicativo e inicie o procedimento para adicionar uma nova versão.

Para enviar uma nova versão do aplicativo é obrigatório que:

- Garantir que a versão mais recente do aplicativo esteja com o mesmo package name da versão anterior;

- Alterar o “version code” e o “version name” dentro do arquivo manifest do aplicativo.

### Aplicativos Públicos na Cielo Store

Assim que o aplicativo público for certificado, o desenvolvedor deverá promover para produção seu aplicativo e a partir desse momento este será adicionado na vitrine da Cielo Store e disponível para download via Cielo LIO.

Ou seja, estabelecimentos comerciais (lojistas) poderão acessar a Cielo Store via Cielo LIO, realizar o download de sua aplicação e então começar a utilização.

### Download de Aplicativo Públicos na Cielo LIO

Para realizar o download de aplicativos públicos na Cielo LIO, execute o seguinte procedimento
Clique na aba Apps -> Clique no aplicativo Cielo Store -> Escolha o aplicativo que deseja realizar o download
