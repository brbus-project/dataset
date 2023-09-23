# Dataset BRBus

O dataset BRBus é um dataset criado com os dados espaciais dos ônibus disponibilizados por APIs das seguintes cidades brasileiras:

- [Curitiba (PR) - Urbanização de Curitiba S/A (URBS)](https://www.urbs.curitiba.pr.gov.br)
- [Brasília - Secretaria de Transporte e Mobilidade de Brasília (Semob)](https://semob.df.gov.br)
- [Rio de Janeiro (RJ) - Empresa Municipal de Informática (IplanRio)](https://iplanrio.prefeitura.rio)
- [São Paulo (SP) - São Paulo Transporte S/A (SPTrans)](https://www.sptrans.com.br)

## Dicionário de dados

Os dados estão salvos em arquivos CSV contendo a seguinte estrutura:

| Campo | Descrição | Tipo |
|---|---|---|
| bus_id | Identificador do ônibus | Número | 
|  city | Cidade de operação do ônibus | Texto | 
|  city_code | Identificador da cidade de operação do ônibus na base de dados do IBGE | Número |
|  agency | Nome da operadora do ônibus | Texto | 
|  line_code | Código da linha do ônibus | Número |
|  line_url | URL para página da operadora da linha (Moovit) | Texto | 
|  line_fare | Tarifa da linha | Número |
|  is_adapted | Verificador de acessibilidade no ônibus | Número (0 = Falso, 1 = Verdadeiro) |
|  is_eletric | Indicador se o ônibus é eletrico ou não | Número (0 = Falso, 1 = Verdadeiro) |
|  latitude | Latitude do ônibus | Número |
|  longitude | Longitude do ônibus | Número |
|  bus_speed | Velocidade do veículo em km/h | Número |
|  bus_direction | Sentido da linha que o ônibus está operando | 1 = Ida , 2 = Volta
|  updated_at | Data/hora de obtenção da informação | Texto (ISO 8601) | 


## Prefixos
Para evitar duplicidade de valores, cada cidade possui um prefixo específico que é utilizado para gerar um novo ID dos ônibus e nomear os arquivos. 

| Cidade | Prefixo |
|---|---|
| Curitiba | CUR
| Brasília | BRA
| Rio de Janeiro | RIO
| São Paulo | SAO
