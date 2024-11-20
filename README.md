# Lab Deploy com Cloud Run
Sistema desenvolvido em Go que recebe um CEP, identifica a cidade correspondente e retorna o clima atual.

## Passos para execução local
* Configure o campo `WEATHER_API_KEY` no arquivo `.env` com a sua chave de acesso do [Weatherstack](https://www.weatherapi.com/).
* Execute o comando:
  ```bash
  docker-compose up -d
  ```
* Após a inicialização da aplicação, acesse o endpoint:
  ```
  http://localhost:8080/temperature/{cep}
  ```
  Substitua `{cep}` pelo CEP do local que deseja consultar.
  
  Exemplo: [http://localhost:8080/temperature/01001000](http://localhost:8080/temperature/01001000)

## Deploy no Google Cloud Run
A aplicação hospedada no Google Cloud Run pode ser acessada diretamente pela URL:
```
https://lab-cloudrun-celiotk-jb3zj3vxnq-rj.a.run.app/temperature/{cep}
```
Exemplo: [https://lab-cloudrun-celiotk-jb3zj3vxnq-rj.a.run.app/temperature/01001000](https://lab-cloudrun-celiotk-jb3zj3vxnq-rj.a.run.app/temperature/01001000)