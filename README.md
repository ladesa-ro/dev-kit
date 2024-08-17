<h1 align="center">Kit de Desenvolvimento do Ladesa</h1>

<p align="center">Recursos feitos para o desenvolvimento dos serviços em ambiente local 💝.</p>

<p align="center">
 <a href="https://github.com/ladesa-ro/dev-kit/blob/main/LICENSE" target="_blank"><img alt="📝 License: MIT" src="https://img.shields.io/badge/%F0%9F%93%9D_license-MIT-21bb42.svg"></a>
</p>

<img align="right" alt="Logotipo do Ladesa: fundo verde com fonte branca escrito o nome da organização." src="https://avatars.githubusercontent.com/u/143351320?s=64&v=4" height="64">

O _Kit de Desenvolvimento do Ladesa_ fornece aos colaboradores um conjunto de recursos, como guias e passo-a-passo, para qualquer colaborador conseguir iniciar a jornada de desenvolvimento dos serviços do Ladesa.

## Vamos Começar

### Configurar e Acessar a Linha de Comando

- <https://docs.ladesa.com.br/developers/tutorials/os/command-line/>

### Configurar o Git

- [Git](https://git-scm.com/downloads)
- <https://docs.ladesa.com.br/developers/tutorials/source-code/git/>

### Configurar o Docker

- [Docker Engine](https://docs.docker.com/engine/install/)
- <https://docs.ladesa.com.br/developers/tutorials/platforms/containers/docker/>

## Recursos do Kit de Desenvolvimento do Ladesa

### Obter o ladesa-ro/dev-kit

```sh
git clone https://github.com/ladesa-ro/dev-kit.git
cd dev-kit
```

### Iniciar Proxy Reverso

Durante o desenvolvimento dos serviços do Ladesa, você pode deparar com os seguintes endereços:

- <http://mq.ladesa.localhost>;
- <http://sso.ladesa.localhost>;
- <http://api.ladesa.localhost>;
- <http://web.ladesa.localhost/sisgha>;
- <http://web.ladesa.localhost/sisgea>.

Note que para cada domínio *.ladesa.localhost, é necessário outros sistemas em execução para lidar com essas requisições.

O propósito do proxy reverso é ser quem recebe qualquer requisição para os endereços acima e encaminhe corretamente para o serviço correto.

Então, quando você acessar qualquer endereco *.ladesa.localhost, quem irá receber suas solicitações é o proxy reverso. Assim, ele poderá olhar nas regras do negócio e encaminhar corretamente os seus pacotes para o servidor correto.

```sh
cd reverse-proxy
```

```sh
make up
```

Acesso ao dashboard do Traefik em: <http://traefik.ladesa.localhost>.

### Message Broker RabbitMQ

```sh
cd message-broker
```

```sh
make up
```

Acesso ao dashboard do RabbitMQ em: <http://mq.ladesa.localhost>.

## Licença

[MIT](./LICENSE) © 2022 – presente, Ladesa.
