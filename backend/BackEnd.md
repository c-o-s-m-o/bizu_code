# Bizu_Code

# BackEnd fake Rest API json Server

# Install dependency json server

# ____Comandos____

//Cria um arquivo package.json para a inserção das dependências necessárias.

    $ npm init -y
        
//Download da dependência json-server, automaticamente incluirá dentro do arquivo packege.json "json-server": "versão atual usada".

    $ npm i json-server
        


//Criar uma pasta chamada bancodb, dentro desta pasta criar um arquivo chamado db.json, pois o json-server, cria uma api baseada nesse arquivo json.

//Modelo de endpoint 
    {
        "produto":[
            {
                "id": 1,
                "name": "exemplo"

            },
            {
                "id": 2,
                "name": "exemplo 2"
            }
        ]
    }

//Dentro do arquivo package.json adcionar uma linha da dentro de "script":{}, "start": "" chamando nosso arquivo db.json

    "scripts":{
        "start": "json-server --watch banco/db.json --port 3001"
    }

//Nessa linha estamos chamndo nossa dependência instalada json-sever , deixamos ela monitorando o aquivo db.json e setamos uma porta para acesso a api.

//Iniciando a API 
    
    $ npm start 


//Acesso ao Endpoint:

//Resources 
    http://localhost:3001/produto


