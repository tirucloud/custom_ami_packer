## ami creation using packer

```bash
packer init aws-ubuntu.pkr.hcl
packer fmt aws-ubuntu.pkr.hcl
packer validate aws-ubuntu.pkr.hcl
packer build aws-ubuntu.pkr.hcl
 
cd ami-Creation/
packer build -var-file="variables.pkrvars.hcl" .
```
