![banner](http://pos.unifacef.com.br/wp-content/uploads/2015/12/logo_pos_site_2016-1-300x48.png)

# Trabalho da Pós Graduação da Uni-FACEF
# Curso: Desenvolvimento de Aplicações Web e Móveis Escaláveis
# Módulo: Mensageria/Streams


## Status:

🚧 Concluído! 🚧:

## Índice 📖

- **[Descrição](#descricao)**
- **[Execução](#execucao)**
- **[Autor](#Autor)**

## Descrição 📌 <a name="descricao"></a>
Objetivo do projeto é simular alguns erros no envio de mensagens para Queue DLQ (dead letter queue) e após atingir o limite de 3 tentativas de envio de mensagem a mesma ser direcionada para a fila de Queue Parking-Lot.

## Execução ✅ <a name="execucao"></a>
1. Iniciar o container do RabbitMQ
```
docker-compose up -d
```

2. Acessar a interface gráfica do RabbitMQ
```
localhost:15672
usuario: guest
senha: guest
```

3. Iniciar o projeto
```
./mvnw spring-boot:run
```

4. Acompanhar na fila de Queues as mensagens que vão entrar na fila order-messages-queue.dlq e após o limite de 3 tentativas serão direcionadas para a fila de Queue order-messages-queue.pkl

---
## Autor: Alex Felipe Barbosa - Matricula: 22289 <a name="autor"></a>

---

<a href="http://www.alexbarbosa.info/">
 <img style="border-radius: 50%;" src="https://avatars3.githubusercontent.com/u/12144620?s=460&u=b9785347e44440d8a08fbbaf61a72288c05671e0&v=4" width="100px;" alt=""/>
 <br />
 <sub><b>Alex Felipe Barbosa</b></sub></a> <a href="http://www.alexbarbosa.info/" title="Blog"></a>
  
<br>[![Twitter Badge](https://img.shields.io/badge/-@alexf_barbosa-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/alexf_barbosa)](https://twitter.com/alexf_barbosa) [![Linkedin Badge](https://img.shields.io/badge/-AlexFelipeBarbosa-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/alexfelipebarbosa/)](https://www.linkedin.com/in/alexfelipebarbosa/) 
[![Gmail Badge](https://img.shields.io/badge/-alex@alexbarbosa.info-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:alex@alexbarbosa.info)](mailto:alex@alexbarbosa.info)






