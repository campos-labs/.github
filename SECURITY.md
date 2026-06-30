# Política de Segurança

A segurança dos projetos, credenciais e dados é tratada como parte do nosso fluxo de desenvolvimento.
Este repositório reúne projetos de portfólio, estudos técnicos e soluções demonstrativas. Ainda assim, seguimos boas práticas para evitar exposição indevida de credenciais, dados sensíveis ou configurações internas.

## Relato de Vulnerabilidades e Vazamentos

Se você encontrar uma vulnerabilidade, credencial, token, chave de API, `connection string` ou qualquer informação sensível exposta em nossos repositórios, **não abra uma Issue pública**.
Entre em contato de forma privada com os mantenedores da organização para que possamos avaliar o caso, revogar credenciais se necessário e corrigir o problema com segurança.

## Tratamento de Credenciais e Dados Sensíveis

* Não versionamos senhas, tokens, chaves de API, `connection strings` ou arquivos `.env` reais.
* Não versionamos dados reais de clientes, empresas, usuários ou terceiros.
* Arquivos de exemplo devem usar valores fictícios ou placeholders, como `.env.example`.
* Exports de ferramentas low-code, automações, notebooks ou pipelines devem ser higienizados antes de entrar no Git.
* Caso algum segredo seja exposto acidentalmente, a credencial deve ser revogada e substituída.

## Escopo

Esta política se aplica aos repositórios públicos da organização, salvo quando um projeto tiver uma política de segurança própria.
