# Case Engenheiro(a) de Dados - LabLift

O case foi elaborado para ser feito em 1 hora, mas você terá até 05/04/2021 23:55 para resolvê-lo. Se não tiver disponibilidade neste período, por favor entre em contato para avaliarmos o caso. 

Nos esforçamos para propor um case divertido. Esperamos que sua experiência seja positiva :)

Doações de sangue são fundamentais para o sistema de saúde, e manter a recorrência dos doadores é um desafio para bancos de sangue. Neste case você irá criar uma API para um sistema que prevê se um doador fará sua próxima doação neste mês! O modelo treinado é fornecido. A sua submissão será testada em uma máquina local (mais instruções em [Submissão e próximos passos](#Submissão_e_próximos_passos).

## Parte 1
Implemente uma função que recebe um `patient_id` do arquivo `blood_donation_hist.csv` e retorna um dicionário com os resultados calculados abaixo. 

| Campo                       | Cálculo                                                      | Tipo    |
|-----------------------------|--------------------------------------------------------------|---------|
| months_since_last_donation  | Quantidade de meses entre última doação e o dia 01/04/2021   | Inteiro |
| number_of_donations         | Quantidade de registros                                      | Inteiro |
| total_volume_donated_cc     | Soma de volume_donated_cc                                    | Inteiro |
| months_since_first_donation | Quantidade de meses entre primeira doação e o dia 01/04/2021 | Inteiro |


Exemplo: `{"months_since_last_donation": 2, "number_of_donations": 20, "total_volume_donated_cc": 5000, "months_since_first_donation": 45}`

## Parte 2
Crie uma API que recebe um id_paciente, realiza o pré-processamento desenvolvido na parte 1, e retorna se o paciente irá doar sangue utilizando o modelo no arquivo `blood_donation_model.joblib`. O corpo da resposta da API deve conter o  `patient_id`, as variáveis agregadas e predição, conforme exemplo abaixo:
Exemplo: `{"patient_id": 3, "months_since_last_donation": 2, "number_of_donations": 20, "total_volume_donated_cc": 5000, "months_since_first_donation": 45, "prediction": 1}`

# Submissão e próximos passos
Faça upload do seu código em algum repositório git público e envie o link do mesmo para o e-mail contato@lablift.com.br. Iremos responder confirmando o recebimento e com orientações para a última etapa (entrevista).

Em caso de dúvidas, não hesite em entrar em contato pelo e-mail acima!
