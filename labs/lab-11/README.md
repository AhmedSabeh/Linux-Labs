# Lab 11: Service Management

## Objective
How to check the status of services, view logs, and see which services start automatically at boot.

---

## Steps

1. **Check the status of a system service**  
      *   Example: Nginx service  
   ```
   sudo systemctl status nginx
   ```
-   Output:

<img width="1049" height="414" alt="Screenshot (219)" src="https://github.com/user-attachments/assets/c413a9d8-8ced-4eea-acda-b33fb27e9734" />

2. **View recent system logs**
```
sudo journalctl -n 20
```
-   (Shows the last 20 log entries.)

3. **Look for any error messages in the logs**
```
sudo journalctl -p err -n 20
```
-   (Shows the last 20 log entries with error priority.)

4. **Check which services are enabled to start at boot**
```
systemctl list-unit-files --type=service --state=enabled
```
