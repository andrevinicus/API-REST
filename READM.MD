## Criar um novo registros
Não deixar criar mais de um registro por placa por veiculo!

POST /registro
body 
'''json
{
    "nome_motorista": "Fulano de tal"
    "placa_veiculo": "ABC123"
    "peso_bruto": "10000,
}
'''
## Listar todos os caminhoes
GET /registro
body: vazio

## Atulizar o registro com peso final
PATCH /registro/:placa/finaliza

atuliza apenas com os dados do body
passado, ou seja, uma atualizaçao parcial.
body:

'''json
{
    "pesso_final": "3500
}
'''
DELETE /registro/:placa

Só pode excluir registro se o caminhao ainda estiver no patio

body: vazio

