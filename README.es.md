# Stablecoins-Infinity-Profit-Bot
Antiguo bot de ganancias infinitas TUSD-USDT

- [English](https://github.com/itxtoledo/Stablecoins-Infinity-Profit-Bot/blob/master/README.en.md)
- [Español - no completado](https://github.com/itxtoledo/Stablecoins-Infinity-Profit-Bot/blob/master/README.es.md)

## Cómo funciona

Es sencillo. Este bot aprovecha la pequeña variación entre las monedas estables. En cada operación obtienes un poco más que las tarifas de Binance. Cada comercio es más rentable que el anterior.

¿Sabes que? ¡Es libre de riesgos! ¡Solo podemos tener ganancias!

## Instalar

1. Baixe a útlima [release](https://github.com/itxtoledo/Stablecoins-Infinity-Profit-Bot/releases), descompacte e edite o arquivo config.json inserindo sua API key e Secret key da Binance.
    - Insira qual par o Bot irá operar, em *MARKET* coloque o ID do mercado como está na Binance, em nosso exemplo iremos definir USDT.
    - Insira a moeda do mercado que você irá operar, no exemplo abaixo estamos definindo TUSD como *CURRENCY*.
    - Escolha qual será o seu *SPREAD_BUY* e *SPREAD_SELL*, usaremos aqui o padrão.
    - Escolha o *MAX_ASK*, aqui você define o valor máximo para o Bot efetuar a compra de um ativo.
    - *INITIAL_INVESTMENT*, como o próprio nome diz, deve ser o valor que você alocou na moeda definida em *MARKET* para iniciar o Bot.
    - Agora se você deseja executar esse Bot em um servidor, a chave *LISTEN_PORT* é muito importante, por padrão aqui vem setado em 3333.

```bash
{
    "API_KEY": "your_api_key",
    "SECRET_KEY": "your_secret_key",
    "CURRENCY": "TUSD",
    "MARKET" : "USDT",
    "SPREAD_SELL" : 0.00100,
    "SPREAD_BUY" : 0.00150,
    "LOOP_TIME": 15,
    "MAX_ASK": 1,
    "INITIAL_INVESTMENT": 20,
    "LISTEN_PORT" : 3333
}
```

2. Instale o NodeJS: https://nodejs.org/en/
Obs.: No desenvolvimento e testes foram utilizadas as seguintes versões:
```
Node v12.5.0
NPM 6.9.0
```
3. Vá para a pasta bot com o terminal e execute

```bash
npm install
```

## Utilização

1. Ter mais de US $20 em sua conta da Binance na moeda do mercado selecionado. 

Nota:

No arquivo config.json você encontrará o mercado USDT, caso queira negociar neste mercado você deverá comprar Tether antes de ligar o BOT.

2. Gere uma API, se não souber como se faz isso siga este tutorial: https://www.youtube.com/watch?v=OdzjaE6O31E
3. Coloque a API nos campos do arquivo config.json
4. Cancele todas as ordens que estiverem abertas no par que você for negociar
5. Inicie o BOT na pasta dele

```bash
  npm start
```

6. Seja paciente e espere seu saldo na moeda definida em *MARKET* aumentar

## Observações
Estamos atualizando frequentemente o BOT, perdas podem ocorrer, por isso só instale a versão em desenvolvimento se souber o que está fazendo.

O Bot possui uma API para consulta dos dados em tempo real. Para usá-la basta acessar o IP do seu servidor e a porta definida no arquivo de configurações. Caso esteja executando localmente, para acessar a api o caminho seria como algo assim:
```bash
  localhost:3333
```
## Créditos
1. Idea [@usdkhey](https://github.com/usdkhey)
2. Algoritmo [@itxtoledo](https://github.com/itxtoledo)

## Comunidad
Únete a nuestras comunidades en Telegram:
[Português](https://t.me/bitragem)
[English](https://t.me/bitragemEnglish)
[Español](https://t.me/bitragemSpanish)

## Patrocinadores
Tiago A Boaventura - 28/05/2019

## Haz tu donación y ayuda a nuestro proyecto
```bash
  USDS: 0x349d3038f6384fe5bdf18ba3bb38cb5f8ef86949
  USDC: 0x349d3038f6384fe5bdf18ba3bb38cb5f8ef86949
  TUSD: 0x349d3038f6384fe5bdf18ba3bb38cb5f8ef86949
  USDT: 1Ed87MBpJHc23eytYYRp6uP9H831Qtcwek
  BTC: 1GzbMuVjhHLibL9fvayfE5UUWg4enKTVR3
  LTC: LgJpDPgM3friu848oZnAMM9iVfX8TBLWhF
  ETH: 0x349d3038f6384fe5bdf18ba3bb38cb5f8ef86949
  DASH: Xwb4bKtbuLXsbfAtvbe6VCq5hmQJKA2tmF
```

## Licencia
[MIT](https://choosealicense.com/licenses/mit/)
