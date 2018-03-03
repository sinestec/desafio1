# Teste Estabilis: Analista de infraestrutura Pleno

_Criar uma infraestrutura como código (IaC) e em seguida orquestrar um ambiente com [Docker Swarm](https://docs.docker.com/engine/swarm/)._

## Informações:

* Você receberá no seu e-mail o Access Key/Secret Key para poder acessar/criar sua infraestrutura na [Amazon AWS](https://aws.amazon.com/pt/).
* Você deverá publicar o seu projeto no GitHub e informar por e-mail o link do projeto.

## Instruções:

* **Criar uma infraestrutura na Amazon AWS utilizando o [Terraform](https://www.terraform.io/).**
    
    * Subir a VPC com Nat Gateway.
    * Subir 3 instâncias EC2 t2.micro com EBS attached de 20GB na rede pública.
    * Subir 3 instâncias EC2 t2.micro com EBS attached de 20GB na rede privada.

* **Construção do Cluster [Docker Swarm](https://docs.docker.com/engine/swarm/).**

    * Orquestrar o Cluster Docker Swarm utilizando o [Ansible](https://www.ansible.com/).
    * Estrutura do Cluster:
        * _3 Manager na rede pública._
        * _3 Worker na rede privada**_

* **Criar uma serviço (service) no Cluster de [Docker Swarm](https://docs.docker.com/engine/swarm/).**

    * Construir o Dockerfile do projeto utilizando uma imagem default do [Nginx](https://nginx.org/en/).
    * Gerar uma imagem com o seu nome e publicá-la no [Hub Docker](https://hub.docker.com/).
    * Gerar o [Docker Compose](https://docs.docker.com/compose/) da sua aplicação Web "seu nome" expondo a porta 80.
    * Subir um serviço (service) "seu nome" no Cluster [Docker Swarm](https://docs.docker.com/engine/swarm/).
