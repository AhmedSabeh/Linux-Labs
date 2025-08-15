# Lab 9: Network Exploration

## Objective
Practice testing network connectivity, checking network interfaces, and downloading web content.

---

## Steps

1. **Test connectivity to google.com**
   ```
   ping -c 4 google.com
   ```
Example output:

<img width="921" height="230" alt="Screenshot (211)" src="https://github.com/user-attachments/assets/b3f5a163-66dc-4781-86d4-dd6fc45a6b08" />

2. **Display your network interface information and IP addresses**

-   Modern systems:
```
ip addr
```
-   Older systems:
```
ifconfig
```
3. **Use curl to download the homepage of a website**
```
curl -o webpage.html https://example.com
```
-   Or using wget:
```
wget -O webpage.html https://example.com
```
4. **Verify the file was saved**
```
ls -l webpage.html
cat webpage.html | head -n 10
```
-   (Shows the first 10 lines of the downloaded HTML)
-   Output:

<img width="911" height="360" alt="Screenshot (212)" src="https://github.com/user-attachments/assets/363c4047-3edd-4eb8-902e-d1e0595786e1" />
