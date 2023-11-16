# chatwootBrasil

<details>
<summary>Exibir aba TODOS apenas para Admin's</summary>

```bash
mv /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue.old
wget -O /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue https://raw.githubusercontent.com/ssteeltm/chatwootBrasil/main/ChatList.vue 
```

```bash
sudo -i -u chatwoot
```

```bash
cd chatwoot
rake assets:precompile RAILS_ENV=production
exit
```

```bash
systemctl restart chatwoot.target
```

</details>
