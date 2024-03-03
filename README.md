"# Infa_Auto_CA1_Terrafrom" 

1. Login to the AWS Academy Learner Lab and Start Lab.

2. Download security credentials, the key pair named labuser in .pem and .ppk format and PuTTY through the AWS Details and Readme tabs of the AWS Academy Learner Lab.

3. Download and unzip the Git repository.

          cd ~ && git clone https://github.com/PatrickCulligan/Infa_Auto_CA1_Terraform && cd Infa_Auto_CA1_Terraform && ls

4. vi into provider.tf as the access token should never by store in git

provider "aws" {
  access_key = "<AK>"
  secret_key = "<SK>"
  token = "<T>"
  region = "us-east-1"
}

5. - terraform init
- terraform plan && terraform apply -auto-approvels

6. Infastruture is Launched
