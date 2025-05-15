# Validate the code set proper indentaions and check version using command
terraform --version
terraform fmt
terraform validate

# install cloud plugins in local and initialise work directory execute plan cmd for ensuring our infra ok for deploy
terrfarm init
terraform plan --auto-approve

# To deploy our infra on cloud platform 
terraform apply --auto-approve

# make sure state.tf file keep on remote backend to avoid conflicts
using remote backend block

# design infra in such way that node_groups are scalable and descale on behaiour of metrics
enable autoscaling set mi and max machines
