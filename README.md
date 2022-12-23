# rachit-practical


For running the above Terraform code 
Following are the prerequisites :
Which I have defined under the locals section in main.tf

  Environment         = "dev"
  Terraform           = "true"
  ami                 = "ami-0530ca8899fac469f"                ## Base image of Ubuntu 20.04
  instance_type       = "t3a.small"
  key_name            = "rachit1"
  cidr_blocks         = ["49.36.191.98/32"]                    ## Local Machine IP needed to connect to VPN
  Owner               = "RACHIT"
  name                = "rachit"
  region              = "us-west-2"
  pritunl_script      = "pritunl.sh"                           ## SCRIPT TO LAUNCH PRITUNL SERVER IN HOST
  certificate_arn     = "arn:aws:acm:us-west-2:421320058418:certificate/73b9c44b-3865-4f0a-b508-dc118857ae2e""
  image_id            = "ami-080beefdfafc6e5c4"                ## Custom Image build using Packer 
  mongo_script        = "mongo_install.sh"                     ## Script to launch Instances having MongoDB installed
  name_prefix         = "rachi"
  host_headers        = ["rachitvpn.***************"]      ## Domain for VPN Server
  
  
  Changing the above values according to your needs one can run the above terraform code.
  
 
