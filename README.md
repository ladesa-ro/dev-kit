<div align="center">

  <h1>Kit de Desenvolvimento do Ladesa</h1>

  <!-- <a href="https://refine.dev/">
      <img alt="refine logo" src="https://refine.ams3.cdn.digitaloceanspaces.com/readme/refine-readme-banner.png">
  </a> -->

  <!-- <br/>
  <br/> -->

  <!-- <div align="center">
      <a href="https://refine.dev">Home Page</a> |
      <a href="https://refine.dev/docs/">Documentation</a> |
      <a href="https://refine.dev/examples/">Examples</a> |
      <a href="https://discord.gg/refine">Discord</a> |
      <a href="https://refine.dev/blog/">Blog</a>
  </div> -->
</div>

<div align="center">

O Ladesa Dev Kit é um repositório que conta com recursos feitos para a melhor configuração de ambiente local de
desenvolvimento com o objetivo de melhorar a produtividade dos colaboradores dos sistemas.
<br />
<br />

</div>

---

## Configuração de Desenvolvimento

### Obter o código do projeto

```sh
git clone https://github.com/ladesa-ro/dev-kit.git
cd dev-kit
```

## Recursos

### Proxy Reverso

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

[MIT](./LICENSE)

© 2022 – _presente_ Ladesa.
