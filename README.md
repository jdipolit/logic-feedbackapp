# logic-feedbackapp

Código destinado para a demo de Logic Apps Standard (Stateful).

Ela contém um workflow para leitura e outro para escrita ao banco de dados:

- flow-get-feedback
- flow-post-feedback

Estes métodos vão interagir com uma base Cosmos SQL e serão expostos via APIM.

Este projeto também faz parte de um laboratório destinado a estudo de ALM em diferentes tipos de aplicativos lógicos.

## Recursos
1. **Shared:**
    - Storage Account: stfeedbackapp
    - App Service Plan: asp-feedbackapp
    - API Management: apim-feedbackapp

2. **Hom:**
    - Cosmos: cosmos-feedbackapp-hom
    - Logic App: logic-feedbackapp-hom  

3. **Prod:**
    - Cosmos: cosmos-feedbackapp-prod
    - Logic App: logic-feedbackapp-prod

## Estrutura padrão de uma solução de Logic Apps

```textile
    MyBundleBasedLogicAppProjectName
    | .vscode
    | Artifacts
    || Maps 
        ||| MapName1
        ||| ...
    || Schemas
        ||| SchemaName1
        ||| ...
    | WorkflowName1
    || workflow.json
    || ...
    | WorkflowName2
    || workflow.json
    || ...
    | workflow-designtime
    | .funcignore
    | connections.json
    | host.json
    | local.settings.json
```
