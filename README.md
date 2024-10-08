# custom-images

Custom images used in personal demos, workshops,..

In order to create and upload an image use the following command:

> [!IMPORTANT]  
> - Review and modify `vars.yaml` file
> - Login to the target repository before executing `image-creator` playbook

```sh
ansible-playbook image-creator.yaml -e image_name=<image-name> -e image_version=<image-name>
```

> [!TIP]  
> Remember to make your repository public if needed

## Images

### yq-tool

```sh
# Image used to create Tekton Tasks with yq configured (to update yaml files values)
ansible-playbook image-creator.yaml -e image_name=yq-tool -e image_version=1.0.0
```

### git-utils

```sh
# Image used for running git commands
ansible-playbook image-creator.yaml -e image_name=git-utils -e image_version=1.0.0
```