# ansible
ansible-playbook playbook.yml

## Step1: Setup foundation

ansible-playbook playbook.yml  --skip-tags "apim" --extra-vars "apim_gitops_repo_value=https://github.com/rh-soln-pattern-api-versioning/api-versioning-helm apim_gitops_repo_tag_value=1.0.0"


## Step2: Setup APIM - version 1.0.0

ansible-playbook playbook.yml  --skip-tags "main" --extra-vars "apim_gitops_repo_value=https://github.com/rh-soln-pattern-api-versioning/api-versioning-helm apim_gitops_repo_tag_value=1.0.0"


## Step3: Setup APIM - version 1.1.0

ansible-playbook playbook.yml  --skip-tags "main" --extra-vars "apim_gitops_repo_value=https://github.com/rh-soln-pattern-api-versioning/api-versioning-helm apim_gitops_repo_tag_value=1.1.0"

## Step4: Setup APIM - version 2.0.0

ansible-playbook playbook.yml  --skip-tags "main" --extra-vars "apim_gitops_repo_value=https://github.com/rh-soln-pattern-api-versioning/api-versioning-helm apim_gitops_repo_tag_value=2.0.0"


