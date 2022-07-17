## Pipeline

Pipeline allows us to automate the deployment process. It includes a set of instructions which are executed on the server during the build and deployment process.

This project uses CircleCi to create a pipeline.

The jobs and workflows are defined in **config.yml** file.

![Pipeline](/documantion/shots/pipeline.png)

1. When changes are pushed to github this triggers the pipeline.

2. In the **build** process the environment is prepared, Node and other dependencies are installed and the build scripts are executed. In case of an error the pipeline is stopped and the error shown. If all is successful the app is production ready.

![build](/documantion/shots/build.png)

3. In the **hold** process the approval is needed. Once approved the pipeline is moving to the deployment process.

4. In the **deploy** process the deploy scripts are executed, and EB is updating the environment. When all is successful the app is deployed and the app includes all changes visible to the user.

![deploy](/documantion/shots/deploy.png)

![deployed project](/documantion/shots/workflow.png)

![env variables](/documantion/shots/envs.png)
