```bash
lsbom -f -l -s -pf /var/db/receipts/org.nodejs.node.pkg.bom | while read f; do sudo rm /usr/local/${f}; done
sudo rm -rf /var/db/receipts/org.nodejs.* /usr/local/{lib/node{,/.npm,_modules},bin,share/man}/{npm*,node*,man1/node*}
```
