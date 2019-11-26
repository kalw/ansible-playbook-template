#### Run the tests:
    
Run the whole test matrix (envlist = py{27,37}-ansible{22,26,27,28} in tox.ini) testing on debian, ubuntu and centos docker imgae

    PLAYBOOK_FILE=playbook.yml tox -c molecule/default/tox.ini

Specify some python / ansible matrix

    TOXENV="py27-ansible27" PLAYBOOK_FILE=playbook.yml tox -c molecule/default/tox.ini

Specify docker image to test

    TOXENV="py27-ansible27" PLAYBOOK_FILE=playbook.yml tox -c molecule/default/tox.ini