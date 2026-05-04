# Attendance Control
![Static Badge](https://img.shields.io/badge/docker-28.3-blue?logo=docker)

[🇺🇸 English](README.md) | [🇧🇷 Português](README.pt-br.md)

O **Attendance Control** é um projeto de controle de presença de pessoas em ambientes organizacionais — também conhecido como sistema de ponto.

O sistema foi projetado incialmente como um projeto de faculdade para funcionar em empresas do **Movimento Empresa Júnior** ([MEJ](https://brasiljunior.org.br/conheca-o-mej)), as quais possuiam necessidades de controle de presença específicas, entretanto o projeto está sendo inteiramente refatorado para abranger quaisquer tipos de organizações.


## 📋 Dependências

- [Docker](https://www.docker.com/)

## 🚀 Como executar localmente

Primeiramente clone o repoitório e acesse o diretório:

```console
$ git clone https://github.com/rafaeldailymartins/attendance-control.git
$ cd attendance-control
```
Crie um novo arquivo `.env` na raiz do projeto contendo as variáveis de ambiente. Um exemplo pode ser encontrado no arquivo `.env.template`. Lembre-se de alterar as chaves secretas do projeto por razões de segurança — elas estão com o valor `changethis` no template.

Para executar o projeto localmente para o desenvolvimento, com a feature de auto-reload, basta executar o comando docker:

```console
$ docker compose up --watch
```

## 📦 Implantação
Para produção, é necessário primeiro mudar a variável de ambiente `ENV` no arquivo `.env` para:
```env
ENV=production
```

Em seguida deve-se subir o conteinêr docker apenas com o arquivo `docker-compose.yml`:

```console
$ docker compose -f docker-compose.yml up --build
```

## 👨‍💻 Autor

Criado e mantido por:

| [<img src="https://avatars.githubusercontent.com/u/162728324?v=4" width="60px;"/><br /><sub><b>Rafael Daily</b></sub>](https://github.com/rafaeldailymartins)
| :---: |