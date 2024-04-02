<!-- create user database -->
CREATE USER 'billing_jagoan'@'%' IDENTIFIED BY 'jagoan2022'; GRANT ALL PRIVILEGES ON radius.* TO 'billing_jagoan'@'%'; FLUSH PRIVILEGES;

<!-- testing radtest -->
radtest testuser password 172.21.0.4:1812 0 testing123

<!-- resource from -->
https://github.com/junelsolis/freeradius-admin