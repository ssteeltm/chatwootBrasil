# chatwootBrasil

[Wiki ChatwootBrasil](https://github.com/ssteeltm/chatwootBrasil/wiki)



<details>
<summary>Exibir aba TODOS apenas para Admin's</summary>



```bash
sudo -i -u chatwoot
```

```bash
mv /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue.old
wget -O /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue https://raw.githubusercontent.com/ssteeltm/chatwootBrasil/main/ChatList.vue 
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



<details>
<summary>Chatwoot Desconectando</summary>


### Setar no /home/chatwoot/chatwoot/.env
```bash
RACK_TIMEOUT_SERVICE_TIMEOUT=0
```

```bash
systemctl restart chatwoot.target
```

</details>
