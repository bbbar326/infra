# ディレクトリ構成

```
inventories/
   production/
      hosts               # 本番用サーバのアドレス情報
   staging/
      hosts               # ステージング用サーバのアドレス情報
   develop/
      hosts               # 開発用サーバのアドレス情報

site.yml
webservers.yml
dbservers.yml

roles/
    common/
        tasks/            
            main.yml      
        handlers/         
            main.yml      
        templates/        
        files/            
        vars/             
            main.yml      
        defaults/         
            main.yml      
        meta/             
            main.yml      
```

# 雛形作成

```bash
ansible-playbook -i localhost, -c local hinagata.yml
```
