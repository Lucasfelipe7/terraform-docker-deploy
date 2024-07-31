Neste repositório, você encontrará os passos para realizar o deploy de uma aplicação na nuvem AWS utilizando containers (Docker) e Terraform.

Primeiramente, desenvolvi uma aplicação Java simples, que foi então containerizada com Docker. A imagem do container foi publicada no Docker Hub. Após esse processo, iniciei um projeto Terraform para definir e provisionar a infraestrutura necessária na AWS, criando uma instância EC2 que serve como servidor para hospedar a aplicação Java. Além disso, configurei o controle de acesso utilizando security groups. Por fim, a API é publicada na internet, tornando-a acessível a todos!


## :rocket: Tecnologias utilizadas

* Terraform
* AWS - EC2
* Docker
* Spring Boot

## Pré Requisitos

- AWS CLI
- Terraform CLI
- Public and Private KeyPair for SSH

## Passos necessários

- Criar um usuário com acesso programático (aws_access_key_id & aws_secret_access_key)
- Instalar a AWS CLI no seu computador e executar o 'aws configure'
- Instalar o Terraform CLI no seu computador
- Gerar um KeyPair para poder acessar a EC2 via SSH (ssh-keygen)
- Executar 'terraform init' dentro da pasta 'infra' no terminal
- Executar 'terraform plan' dentro da pasta 'infra' para verificar o plano de criação do terraform

- Executar 'terraform apply' dentro da pasta 'infra' para criar a infraestrutura
- Executar 'terraform destroy' dentro da pasta 'infra' destruir toda a infraestrutura criada
