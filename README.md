
build -t pocteo/ansible-helm .
docker run -it --rm --name tmp-ansible -v $(pwd):/ansible/playbooks pocteo/ansible-helm playbook.yml
