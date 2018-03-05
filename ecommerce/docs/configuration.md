## Configuration

### mysql

docker container ls

-get mysql ID

example:

55981bcba14d

THEN: 

docker exec -it <55981bcba14d> bash

This will open a bash terminal inside the container where one can communicate with mysql via the bash terminal.

THEN

Once in the Docker container's bash terminal you'll need to connect with the command below (—password: 'graphcool')

example:

mysql -pgraphcool



The password was found by searching the repo and found here:

https://github.com/graphcool/prisma/blob/c65e76293b49b29f5d81d54f54e93e9e286bf5f9/cli/packages/prisma-cli-core/src/commands/local/docker/env