# Heading 1

- Orange
- Banana
- Apple

## Heading 2

1. First
2. Second
3. Third

- [Join Devops](https://www.joindevops.com/)
- ![Alt text](https://assets.digitalocean.com/articles/alligator/boo.svg)
- ![sample](https://lh4.googleusercontent.com/Zq-yYj2zo0CMXLzCXzFSO7gIThX-bI7U5KavnIugCuE72TLQknKUxE5NSYrLvh9eMNxyUswatuoHjPO4sb6Hrc8=w1280)

### Heading 3

- To write a command: `sh helloworld.sh`

#### Heading 4

```yaml
- name: Install cart component
  hosts: cart
  become: yes
  tasks:
  - name: setup NPM source
    ansible.builtin.shell: "curl -sL https://rpm.nodesource.com/setup_lts.x | bash"

  - name: Install NodeJS
    ansible.builtin.yum:
      name: nodejs
      state: installed
```

##### Heading 5

###### Heading 6
