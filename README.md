# Storsy: Storage Easy 🇺🇦
This page [storsy.github.io](https://storsy.github.io).

## How to use
Step 1: [Just init new storage](https://storsy.qip.cx) 👨‍💻

🔑 And you receive credentials for your new storage 🗄️ (MySQL, Redis, more..).
Usage it for development your inspiring ideas!🤩🙌

... more features:

### Backup/Restore
```shell
curl -H ... storsy.qip.cx/backup/mysql -O
```
### REST CRUD API
Prototyping on the fly, soft-delete out of the box.

#### Endpoints
```
mysql/:table/:id
GET    mysql/:table/:id?with=deleted
DELETE mysql/:table/:id?force

redis/:key/:value
```

#### fetch()
```javascript
const headerCredentials = {
    'X-ACCESS-KEY': '...',
    'X-PROTOTYPE': 'true'
};
fetch('storsy.qip.cx/mysql/users', {})
```
