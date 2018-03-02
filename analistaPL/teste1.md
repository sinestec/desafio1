# Teste Estabilis: Analista de infraestrutura Pleno

Criar uma infraestrutura como código e orquestrar um ambiente com Docker Swarm.

## Informações:

* Você receberá no seu e-mail o Access Key/Secret Key para poder acessar/criar sua infraestrutura na Amazon AWS.
* Você deverá publicar o seu projeto no GitHub e informar por e-mail o link do projeto.

## Instruções:

* Criar uma infraestrutura na Amazon AWS utilizando o Terraform.
    
    * Subir a VPC com Nat Gateway.
    * Subir 3 instâncias EC2 t2.micro com EBS attached de 20GB na rede pública.
    * Subir 3 instâncias EC2 t2.micro com EBS attached de 20GB na rede privada.

* Construção do Cluster Docker Swarm.

    * Orquestrar o Cluster Swarm utilizando o Ansible.
    * Estrutura do Cluster:
        * 3 Manager na rede pública.
        * 3 Worker na rede privada.

* Criar uma serviço (service) no Cluster de Docker Swarm.

    * Construir o Dockerfile do projeto utilizando uma imagem default do Nginx.
    * Gerar uma imagem com o seu nome e publicá-la no Docker Hub.
    * Gerar o compose da sua aplicação Web "seu nome" expondo a porta 80.
    * Subir um serviço (service) "seu nome" no Cluster Docker Swarm.
