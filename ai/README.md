This is a hack solution that does not need nvidia-docker to run. You still need to have nvidia-docker installed on the machine and make sure that you run at least once:
```
nvidia-docker run nvidia/cuda:8.0-devel-ubuntu16.04 nvidia-smi
```
This command will create a volume drive where all the drivers are. MAke sure that you note the version `NVIDIA-SMI 375.82                 Driver Version: 375.82`. This will be the version you need to use in the docker-compose file. 

Sometimes you need to run longer time the dockers, then it's better to run it on the machine so the connection it's not intrerupted

use `dmscp -r . beer42:///root/dockers/ai` to copy the content of this folter to the server


