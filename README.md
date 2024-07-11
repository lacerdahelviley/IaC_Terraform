# IaC_Terraform

Este repositório contém configurações e scripts do Terraform para a provisão e gerenciamento de infraestrutura na nuvem, utilizando a abordagem de Infrastructure as Code (IaC).

## Índice

- [Visão Geral](#visão-geral)
- [Pré-requisitos](#pré-requisitos)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Configuração Inicial](#configuração-inicial)
- [Uso](#uso)
- [Melhores Práticas](#melhores-práticas)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Visão Geral

O objetivo deste projeto é fornecer um exemplo prático de como utilizar o Terraform para criar e gerenciar recursos de infraestrutura na nuvem. Ele inclui definições de recursos, provedores e variáveis, seguindo as melhores práticas para organização e manutenção de código.

## Pré-requisitos

Antes de começar, certifique-se de ter os seguintes pré-requisitos instalados em sua máquina:

- [Terraform](https://www.terraform.io/downloads.html) v1.0.0 ou superior
- Conta na AWS com credenciais configuradas
- [AWS CLI](https://aws.amazon.com/cli/) configurado com suas credenciais

## Estrutura do Projeto

A estrutura do diretório do projeto é organizada da seguinte forma:

```
IaC_Terraform/
├── main.tf
├── variables.tf
├── outputs.tf
└── README.md
```

- `main.tf`: Contém a configuração principal do Terraform.
- `variables.tf`: Define as variáveis utilizadas no projeto.
- `outputs.tf`: Define os outputs do Terraform.
- `README.md`: Documentação do projeto.

## Configuração Inicial

1. Clone o repositório para sua máquina local:

    ```sh
    git clone https://github.com/lacerdahelviley/IaC_Terraform.git
    cd IaC_Terraform
    ```

2. Inicialize o diretório do Terraform:

    ```sh
    terraform init
    ```

3. Configure suas variáveis no arquivo `variables.tf` ou utilize um arquivo `terraform.tfvars` para definir valores específicos.

## Uso

Para provisionar a infraestrutura definida no Terraform, siga os passos abaixo:

1. **Planejar as mudanças**: Execute o comando `terraform plan` para ver o que será criado, modificado ou destruído.

    ```sh
    terraform plan
    ```

2. **Aplicar as mudanças**: Execute o comando `terraform apply` e confirme a execução digitando "yes".

    ```sh
    terraform apply
    ```

3. **Destruir a infraestrutura**: Quando você não precisar mais da infraestrutura, pode destruí-la com o comando `terraform destroy`.

    ```sh
    terraform destroy
    ```

## Melhores Práticas

- **Versionamento de Código**: Utilize controle de versão (Git) para gerenciar seu código Terraform.
- **Modularização**: Separe recursos em módulos reutilizáveis para melhor organização e manutenção.
- **Segurança**: Nunca compartilhe suas credenciais da nuvem em arquivos de configuração ou repositórios públicos.
- **Documentação**: Mantenha sua documentação atualizada para facilitar a colaboração e manutenção do projeto.

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões, correções ou melhorias, por favor, abra uma issue ou envie um pull request.

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
