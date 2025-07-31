# 🚀 Ansible Server Maintenance

Tento repozitář obsahuje základní playbook pro běžnou správu serveru:

✅ Aktualizace systému  
✅ Správa uživatelů a SSH klíčů  
✅ Instalace a kontrola logrotate  
✅ Základní nastavení firewallu



# struktura projektu

Ansible_Demo_Server_Maintanance <br> 
├── inventory <br>
├── playbook.yml<br>
├── roles/<br>
│   ├── update/<br>
│   │   └── tasks/<br>
│   │       └── main.yml<br>
│   ├── users/
│   │   └── tasks/<br>
│   │       └── main.yml<br>
│   ├── logrotate/<br>
│   │   └── tasks/<br>
│   │       └── main.yml<br>
│   ├── firewall/<br>
│   │   └── tasks/<br>
│   │       └── main.yml<br>
├── README.md<br>



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
