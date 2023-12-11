run FE as service background:
first start : pm2 start yarn --name "hyster-yale-frontend" -- start
stop : pm2 stop hyster-yale-frontend
restart : pm2 restart hyster-yale-frontend
delete : pm2 delete hyster-yale-frontend
