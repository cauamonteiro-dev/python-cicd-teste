Evidências do Pipeline

1. O que representa a etapa de CI neste projeto?

A etapa de Continuous Integration (CI) representa a execução automatizada dos testes da calculadora sempre que alterações são enviadas ao repositório. O pipeline configura o ambiente Python, instala as dependências necessárias e executa o pytest para verificar se o código continua funcionando corretamente.

2. O que impede a execução do Continuous Delivery quando existe um defeito?

O Continuous Delivery depende do sucesso da etapa de CI. Caso algum teste falhe, o job de CI é encerrado com erro e, por meio da configuração de dependência entre os jobs, o Continuous Delivery não é executado. Dessa forma, um código com defeitos não gera um novo artefato.

3. Qual seria a próxima etapa necessária para transformar este pipeline em Continuous Deployment?

Seria necessário adicionar uma etapa de implantação automática que utilize o artefato gerado pelo Continuous Delivery e o publique em um ambiente de execução, como um servidor ou serviço de hospedagem. Assim, após os testes e a geração do artefato, a aplicação seria disponibilizada automaticamente.
