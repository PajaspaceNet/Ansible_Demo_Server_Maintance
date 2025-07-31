# 🚀 Ansible Server Maintenance

Tento repozitář obsahuje základní playbook pro běžnou správu serveru:

✅ Aktualizace systému  
✅ Správa uživatelů a SSH klíčů  
✅ Instalace a kontrola logrotate  
✅ Základní nastavení firewallu



# struktura projektu

<pre>

ansible-server-maintenance/
├── inventory
├── playbook.yml
├── roles/
│   ├── update/
│   │   └── tasks/
│   │       └── main.yml
│   ├── users/
│   │   └── tasks/
│   │       └── main.yml
│   ├── logrotate/
│   │   └── tasks/
│   │       └── main.yml
│   ├── firewall/
│   │   └── tasks/
│   │       └── main.yml
├── README.md

</pre>



---

## 📁 Struktura

- `inventory` – seznam serverů
- `playbook.yml` – hlavní playbook
- `roles/` – jednotlivé role (update, users, logrotate, firewall)

---

## ⚙️ Použití

1️⃣ Nastav `inventory`  
2️⃣ Spusť:
```bash
ansible-playbook -i inventory playbook.yml
