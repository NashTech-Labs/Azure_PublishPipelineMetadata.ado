# Azure_PublishPipelineMetadata.ado
Use this template to publish Pipeline Metadata to the Evidence store in Azure DevOps Pipeline environment.


## Use Cases

You can directly call a particular template as per the requirement. for example: 

 ```yaml
  # azure-pipeline.yml
  resources:
  repositories:
    - repository: Template
      type: github
      name: your_username/Azure_PublishPipelineMetadata.ado
      ref: <respective branch name>
      endpoint: 'githubServiceConnectioNname'

  steps:
  # passing the parameters
  - template: Azure_PublishPipelineMetadata.yml
    
  ```
Make sure to adjust the repository name, branch name, and parameter values according to your project's requirements.
