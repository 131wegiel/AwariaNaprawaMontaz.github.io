echo "# AwariaNaprawaMontaz.sos.tech" >> README.md 
git init 
git add README.md 
git commit -m "pierwszy commit" 
git branch -M main 
git remote add origin https://AwariaNaprawaMontaz.sos.tech.git
git push -u origin main
firewall-cmd --permanent --zone=public --add-port=53/tcp
firewall-cmd --permanent --zone=public --add-port=53/udp
firewall-cmd --reload
