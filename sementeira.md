db.vendas.insertMany([

    {
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
            "valor":  3.00,
            "total":  30.00,
            "dataHora": ISODate("2021-07-26T10:00:00Z")
    },
    {
            "vendedor": {
                        "nome": "Rayssa Vieira",
                        "telefone": "(81) 98483-1010",
                        "funcao": "Atendente de vendas" 
            },
            "cliente": {
                    "nome": "Karine Silva",
                    "telefone": "(81) 98415-2124",
                    "bairro": "Casa amarela",
                    "cidade": "Recife"
            }, 
            "compra": "Muda de plantas",
            "especie": "Jabuticabeira",
            "quantidade": 2,
            "valor":  45.00,
            "total": 90.00,
            "dataHora": ISODate("2021-07-26T11:00:00Z")
    },
    {
            "vendedor": {
                    "nome": "Renato Gabriel",
                    "telefone": "(81) 98755-0101",
                    "funcao": "Atendente de vendas" 
            },
            "cliente": {
                    "nome": "Raquel",
                    "telefone": "(81) 99817-1510",
                    "bairro": "Arruda",
                    "cidade": "Recife"
            }, 
            "compra": "Muda de plantas",
            "especie": "Costela de adao",
            "quantidade": 3,
            "valor":  34.50,
            "total":  103.50,
            "dataHora": ISODate("2021-07-23T14:12:00Z")
    },
    {
        "vendedor": {
                    "nome": "Renato Gabriel",
                    "telefone": "(81) 98755-0101",
                    "funcao": "Atendente de vendas" 
        },
            "cliente": {
                "nome": "Maria das gracas",
                "telefone": "(81) 98717-3030",
                "bairro": "Jaqueira",
                "cidade": "Recife"
            }, 
            "compra": "Muda de plantas",
            "especie": "Alecrim",
            "quantidade": 10,
            "valor":  17.00,
            "total": 170.00,
            "dataHora": ISODate("2021-07-23T14:00:00Z")

      },
      {
            "vendedor": {
                "nome": "Rayssa Vieira",
                "telefone": "(81) 98755-0101",
                "funcao": "Atendente de vendas" 
            },
            "cliente": {
                "nome": "Henrique",
                "telefone": "(81) 98916-1401",
                "bairro": "Bomba do hemeterio",
                "cidade": "Recife"
            }, 
            "compra": "Pacote de Sementes",
            "espécie": "Flores sortidas",
            "quantidade": 1,
            "valor": 7.80,
            "total":  7.80,
            "dataHora": ISODate("2021-07-23T14:15:00Z")
    }
])