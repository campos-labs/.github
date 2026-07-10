# Política de Segurança

A segurança das nossas aplicações, infraestrutura e dados é tratada como prioridade ao longo de todo o ciclo de desenvolvimento.  
Esta política define as diretrizes para o relato seguro de vulnerabilidades e nossas práticas de conformidade.

## Relato de Vulnerabilidades

Caso você identifique uma falha de segurança, credencial exposta ou qualquer vulnerabilidade, **não abra uma Issue pública**.

Utilize o recurso nativo de **Private Vulnerability Reporting** do GitHub para garantir a confidencialidade do relato, quando disponível:

1. Acesse a aba **Security** no repositório afetado.
2. No menu lateral, clique em **Advisories**.
3. Clique em **Report a vulnerability** e forneça os detalhes técnicos.

Nossa equipe tratará o relato de forma confidencial, avaliando o impacto e aplicando as correções necessárias com segurança.

## Práticas e Conformidade

Para mitigar riscos e garantir a integridade dos repositórios da organização, adotamos as seguintes práticas contínuas:

* **Gestão de Segredos:** É proibido versionar senhas, tokens, chaves de API, `connection strings` ou arquivos `.env` reais.
* **Dados Sensíveis:** Não versionamos dados reais de usuários. Exemplos usam valores sintéticos ou *placeholders*.
* **Higienização:** Exportações *low-code*, configurações e *pipelines* devem ser higienizados antes do commit.
* **Revogação:** Na exposição acidental, a credencial é revogada, substituída e o incidente analisado.

## Versões Suportadas

Atualmente, apenas a branch principal (`main`) dos nossos projetos recebe atualizações e correções ativas de segurança.
