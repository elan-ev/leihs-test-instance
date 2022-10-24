# **leihs** test setup

To deploy [leihs-test.vm2.elan.codes](https://leihs-test.vm2.elan.codes):

0. Initialize git submodules:

        ❯ git submodule update --init leihs && cd leihs && git submodule update --init --recursive

1. Create a Debian 11 LXC container with *at least 8GB RAM*

2. Make sure you can SSH into leihs-test.vm2.elan.codes without password

3. To generate TLS certificates, run:

        ❯ ansible-playbook -i hosts prep.yml

4. Start deploying Leihs by running:

        ./scripts/deploy

5. Get yourself a coffee ☕️

6. Register admin account on [leihs-test.vm2.elan.codes](https://leihs-test.vm2.elan.codes)
