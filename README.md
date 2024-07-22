Desafio Vaga Devops
===================

Supondo que já tenha o Docker instalado e configurado, para executar este projeto:

Tinha um erro que estava indicando que havia uma incompatibilidade entre a versão do Ruby especificada do Gemfile e a versão do Ruby disponível no ambiente Docker onde está construindo sua imagem.
Foi ajustado para a versão 3.2.2.

Foi ajustado o parametro RAILS_ENV=development, para deploy da aplicação.

## Inicialização

```bash
docker-compose up -d
```

Este comando compilará a imagem docker do projeto e criará 3 instâncias da aplicação
juntamente com uma instância do web server (nginx)

## Remoção

```bash
docker-compose down --remove-orphans -v
```

Removerá tudo que está definido no arquivo `docker-compose.yml`

## Verificação

Consegue-se verificar a aplicação pela URL:

```
http://localhost
```


