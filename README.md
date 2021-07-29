#### **On12- Back-end {reprograma} :purple_heart: Semana 12** 🚀

### Introdução a banco de dados e MongoDB
**Comandos MongoDB**
---
### Criação do banco de dados:  :seedling:
	use sementeira
### Criação da collection : 
	db.createCollection('vendas')     
### Inserindo os documentos:

	db.vendas.insert({

		"vendedor": {
		"nome": "Renato Gabriel",
		"telefone": "(81) 98755-0101",
		"funcao": "Atendente de vendas"

		},

		"cliente": {
		"nome": "Ellen Souza",
		"telefone": "(81) 98763-3130",
		"bairro": "Arruda",
		"cidade": "Recife"

		},

		"compra": "Muda de plantas",
		"especie": "Suculenta",
		"quantidade": 10,
		"valor": 3.00,
		"total": 30.00,
		"dataHora": ISODate("2021-07-26T10:00:00Z")

	}) 

---
### Atualização dos documentos:
Atualizando campo já existente: (incluindo sobrenome da cliente)
- db.getCollection('vendas').update({"cliente.nome": "Raquel"},{$set:{"cliente.nome": "Raquel Freitas"}})
---
###   Exclusão de documentos (pelo nome do cliente):
- db.getCollection('vendas').remove({ "cliente":  "Raquel Freitas" })

---
### Consulta com projeção: 
Ver apenas compra e cliente:
- db.getCollection('vendas').find({},{"compra":1, "cliente":1, "_id":0}) 

---
###  Consulta utilizando combinação entre os seletores:
Ver apenas vendas em Recife com total menor que e incluso,100 reais:
- db.getCollection('vendas').find({
    "cliente.cidade": "Recife",
    "total": {$lte:100}
    })
---
###   Consulta paginada e ordenada : 
Ordenando pelo nome do vendedor e dataHora: 
- db.getCollection('vendas').find().sort({"vendedor.nome":1,"dataHora":-1})

Ordenando pela ultima compra realizada: 
- db.getCollection('vendas').find().sort({dataHora:1}).skip(4).limit(1)

Ordenar pela primeira compra realizada: 
- db.getCollection('vendas').find().sort({dataHora:-1}).skip(4).limit(1)

Limitando resultados: 
- db.getCollection('vendas').find({}).limit(2)

Pulando resultados: 
- db.getCollection('vendas').find({}).skip(2)
