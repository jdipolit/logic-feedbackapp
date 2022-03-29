# logic-feedbackapp

Código destinado para a demo de Logic Apps Standard (Stateful):
1. flow-get-feedback
2. flow-post-feedback

Estes métodos vão interagir com uma base Cosmos SQL e serão expostos via APIM

Recursos
1. **Shared:**
    * Storage Account: stfeedbackapp
    * App Service Plan: asp-feedbackapp
    * API Management: apim-feedbackapp

2. **Hom:**
    * Cosmos: cosmos-feedbackapp-hom
    * Logic App: logic-feedbackapp-hom  

3. **Prod:**
    * Cosmos: cosmos-feedbackapp-prod
    * Logic App: logic-feedbackapp-prod


Ao configurar os Logic Apps pela primeira vez, não esquecer de verificar se a configuração *AzureCosmosDB_connectionString* está preenchida com a string do Cosmos
