## Terraform VPC creation
provider "aws" {
  version = "~>2.7"
  region  = "us-west-2"
}

# Create a VPC
resource "aws_vpc" "java_home" {
  cidr_block = "10.0.0.0/16"
  instance_tenancy = "default"
}
resource "aws_subnet" "main" {
  vpc_id     = "${aws_vpc.java_home.id}"
  cidr_block = "10.0.1.0/24"
  tags = {
    Name = "Main"
  }
}
