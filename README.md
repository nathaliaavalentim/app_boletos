# app_boletos

Passos:
1)Executar: python manage.py runserver

2)No navegador, digite: http://127.0.0.1:8000/boletos/upload/

3) Faça o upload do arquivo csv

4) A simulação dos emails enviados aparecerão no console do IDE (Configuração de settings.py)

5) Testes unitários:
Garante que um e-mail foi enviado com os detalhes corretos.
Verifica se a URL do boleto gerado está correta, e se o arquivo PDF foi criado. Remove o arquivo gerado para limpar após o teste.

6) Testes de integração:
Teste de Processamento de CSV Inválido e Teste de Processamento de CSV Válido.

7)Execução de testes: python manage.py test boletos.tests.integration.tests e python manage.py test boletos.tests.unit.tests

8)Comando Docker: docker-compose up --build
docker pull nathaliavalentim/imagem_app_boletos:1
Disponível em:
docker.io/nathaliavalentim/imagem_app_boletos   

9) No navegador, digite: http://localhost:8000/boletos/upload/
