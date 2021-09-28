# redispubsub
Padrão Pub/Sub utilizando Redis como exemplo para entregar mensagens em tempo real.


## Instruções
1. Build o projeto: docker-compose build
2. Levante os containers: docker-compose up -d
3. Entre no bash do composer: docker-compose exec app bash
4. No app bash execute para se inscrever no canal: php index.php
5. Abra uma nova aba no bash e execute novamente: docker-compose exec app bash
6. No app bash execute: redis-cli -h redis
7. Publique uma mensagem no canal exemplo: PUBLISH canal_exemplo 'Hello'
8. Verifique no passo 4 se a mensagem foi recebida no canal
