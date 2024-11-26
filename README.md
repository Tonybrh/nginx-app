# Requisitos e passos para rodar os projetos
- Ter o docker instalado
- Ter uma máquina Ubuntu

### No arquivo /etc/hosts deve adicionar ao localhost os IPs da aplicação da forma abaixo

<pre> 
  127.0.0.1 app1.local
  127.0.0.1 app2.local
  127.0.0.1 app3.local
  127.0.0.1 phpmyadmin.local
  127.0.0.1 phpmyadmin2.local
  127.0.0.1 phpmyadmin3.local
</pre>

### Executar o comando para subir os containers

<pre>sudo docker compose up -d</pre>

### Para visualizar os containers em execução rode o comando

<pre>sudo docker ps</pre>

## Nota: O projeto deve ser acessável pelos endereços abaixo
- http://app1.local 
- http://app2.local
- http://app3.local

>  Bem como também deve ser possível enxergar o conteúdo html ao requisitar o IP de cada aplicação usando o comando abaixo

<pre>curl http://10.10.10.10 </pre>

# Caso deseje contribuir siga o padrão de commits abaixo

### Para uma nova implementação
> [FEAT] - mensagem do commit

### Para uma atualização

> [UPDATE] - mensagem do commit

### Para a correção de alguma funcionalidade ou bug

> [FIX] - mensagem do commit

### Para a configuração de um novo serviço

> [CONFIG] - mensagem do commit

## Dúvidas pendentes

- Cada aplicação deve ter seu próprio banco de dados ou cada uma deve ter o seu pŕoprio
- Por que o nginx redireciona para https quando tento acessar o http?
- É necessário configurar o https?
