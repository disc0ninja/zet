# Packer by HashiCorp

Utilizes [query=Immutable%20infrastructure](Immutable infrastructure)  

- "Image" based 
- Cross-platform 
- Utilizes native tooling 
- Integrates with configuration management 
  - Ansible
  - Chef
  - Terraform
- Transitions to containers

Uses [query=Packer%20templates](templates) written in HashiCorp Configuration Language similar to [query=terraform](terraform) for configuration.

## CLI Tool Commands 
- **fmt**: formats the template file specified 
- **validate**: Checks syntax/configuration
- **build**: Start building the image defined in the template 
  - **-debug**: pause after each step, gives SSH access 
  - **-var**
  - **-only**
  - **-on-error**


## Resources 
<Documenation>(https://www.packer.io/docs)

