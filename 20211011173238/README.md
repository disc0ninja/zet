# Packer Templates 
 
## Parts of a template: 
 
1. ***source***: Where you want to build the images 
  - can be provided inside of *builds*
1. ***build***: Unit of execution 
  1. Can be named
  1. Multiple sources == multiple images output at once 
  1. Combine sources with *provisioning*/*post processing*
  1. ***[provisioner](query=packer%20provisioner)***: Configuration 
    - Customize your image
    - Scripts/ Configuration Management (eg: terraform/ansible)
    - run sequentially
    - can be *source* specific with the ***only*** argument
  1. ***post-processor*** Transformation 
    - Transform *build* outputs into something else (eg. checksums/ami) 
    - Integration with other services (eg. ami/vagrant/docker images)
    - Can be chained together via *post-processors* block 
 

