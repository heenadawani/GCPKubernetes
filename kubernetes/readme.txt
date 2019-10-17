export TF_VAR_project="$(gcloud config list \
  --format 'value(core.project)'
)"
export TF_VAR_region="us-east1"
export TF_VAR_user="admin"
export TF_VAR_password="m8XBWrg2zt8R8JoH"
terraform init
terraform plan
terraform apply
kubectl get service
