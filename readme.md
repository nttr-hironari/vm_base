# vagrant 検証用 雛形

## 使い方

site.yml で必要な role を追記し, `vagrant up`

```
---
- hosts: all
  user: vagrant
  become: yes
  roles:
    - init
    - git
    - vim
    - python36 <- python3.6系を使いたい場合
```
