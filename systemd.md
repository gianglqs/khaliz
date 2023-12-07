sudo systemctl daemon-reload
sudo systemctl restart nextjs_hy.service

sudo systemctl status nextjs_hy.service

journalctl -xeu nextjs_hy.service
