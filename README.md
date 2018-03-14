# HCI Bench setup.

```
$ ssh-copy-id root@hci-bench02.go-lab.jp
$ ansible -i hosts -u root -m ping hci-bench02.go-lab.jp
$ ansible-playbook -i hosts --ask-vault-pass setup.yml -C
$ ansible-playbook -i hosts --ask-vault-pass setup.yml
```


edit setting.

```
$ git checkout -b vsan-cluster-01_case-101
$ git push origin vsan-cluster-01_case-101

$ vi files/conf/perf-conf.yaml.j2
$ git add files/conf/perf-conf.yaml.j2
$ git commit
$ git push
```
