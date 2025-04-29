# CryptoMonitor - Monitor de Cotações de Bitcoin

## Visão Geral do Projeto

O CryptoMonitor é um aplicativo Android desenvolvido em Kotlin que fornece monitoramento em tempo real do preço do Bitcoin (BTC) em Reais Brasileiros (BRL), consumindo a API pública do Mercado Bitcoin. O aplicativo segue as melhores práticas modernas de desenvolvimento Android e demonstra princípios de arquitetura limpa.


## Especificações Técnicas

### Componentes Principais

#### Camada de Dados

- **TickerResponse.kt**: Classe de dados que representa a estrutura da resposta da API.
- **Ticker.kt**: Classe modelo contendo informações de preço da criptomoeda.

#### Camada de Rede

- **MercadoBitcoinService.kt**: Interface Retrofit para comunicação com a API.
- **MercadoBitcoinServiceFactory.kt**: Classe factory para criação de instância Retrofit.

#### Camada de Apresentação

- **MainActivity.kt**: Activity principal que gerencia as interações da UI.
- **activity_main.xml**: Arquivo de layout principal do aplicativo.


### Funcionalidades Principais

- Exibição do preço do Bitcoin em tempo real no formato BRL.
- Timestamp da última atualização de preço.
- Capacidade de atualização manual.
- Tratamento de erros para operações de rede.
- Formatação de moeda de acordo com os padrões brasileiros.


## Detalhes de Implementação

### Abordagem Arquitetural

O aplicativo segue um padrão MVVM simplificado com:

- Separação clara de responsabilidades entre camadas.
- Corrotinas para operações assíncronas.
- Retrofit para requisições de rede.
- Gson para serialização/desserialização JSON.


### Integração com API

O aplicativo consome o seguinte endpoint REST:

GET https://www.mercadobitcoin.net/api/BTC/ticker/


Os dados de resposta incluem:

- Preços atuais de compra/venda.
- Máximas/mínimas de 24 horas.
- Volume de negociação.
- Timestamp da última atualização.


## Ambiente de Desenvolvimento

- **SDK Mínimo**: API 21 (Android 5.0 Lollipop).
- **SDK Alvo**: API mais recente estável.
- **Linguagem**: Kotlin 1.6+.
- **Ferramentas**: Android Studio Electric Eel ou superior.


## Bibliotecas Utilizadas

- **Retrofit 2.9.0**: Cliente HTTP para Android.
- **Gson 2.9.0**: Conversão de JSON para objetos Kotlin.
- **Corrotinas 1.6.0**: Programação assíncrona.
- **AndroidX**: Componentes modernos do Android.

## Exemplos
![image](https://github.com/user-attachments/assets/a23ba89a-bb35-4bff-8804-be8f08134548)
///
![image](https://github.com/user-attachments/assets/baedc99b-c3c7-4ba6-938e-26ff1017c43c)
///
![image](https://github.com/user-attachments/assets/b20b996b-5550-4fa8-bbe7-975de5275447)
///
![image](https://github.com/user-attachments/assets/2e598cf4-dc38-4301-879c-92e1abe40210)






