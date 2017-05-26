# Terraform wrapper
This simple shell wrapper downloads specified Terraform version. Can be used as replacement for real ```terraform``` command, as it launches it with proper arguments after it has checked it's in correct version.

It was written to be part of of Continuous Deployment pipelines (Infrastructure as Code) to easily control version on any environment it may be launched (specifically on build nodes).

# Configuration
You control Terraform version in two ways
  * with **TFVERSION** environment variable
  * with **terraform.version** file placed in the same directory as **tfw** script (used only when env variable is unset)
