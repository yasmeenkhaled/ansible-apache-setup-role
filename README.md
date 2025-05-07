# Install_Apache Ansible Role

Ansible role to install and configure Apache (httpd) web server on RHEL/CentOS systems, change its default port from **80 to 88**, and upload a test web page

that test on ubuntu 

![image](https://github.com/user-attachments/assets/ea1a95f9-21b0-411e-bf18-6e3cdc84dd00)


---

## 📌 Role Features

- Install Apache (`httpd`)
- Enable and start Apache service
- Backup the original `httpd.conf` file
- Change Apache listen port from `80` to `88`
- Update SELinux to allow port 88
- Open port 88 in `firewalld`
- Upload custom `index.html` page
- Handler to restart Apache after changes

---

## 📁 Role Structure
```
Install_Apache/
├── defaults/
│   └── main.yml
├── files/
|   └── index.html
├── handlers/
│   └── main.yml
├── meta/
│   └── main.yml
├── tasks/
│   └── main.yml
├── tests/
│   └── test.yml
├── vars/
│   └── main.yml
└── .travis.yml
```
---

# ansible-apache-setup-role
