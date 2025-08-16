# Lab 20 Final Project

## 1.  Project Setup
```
mkdir -p ~/web_project/{css,js,images,backup}
cd ~/web_project
```
<img width="729" height="100" alt="Screenshot (239)" src="https://github.com/user-attachments/assets/6f5486e7-bdd4-4e04-80d8-1f95554420a2" />

## 2.  Now your structure looks like:
```
web_project/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
└── backup/
    └── backup.sh
```

## 3. Create Files

#### -   HTML (index.html)

<img width="728" height="435" alt="Screenshot (240)" src="https://github.com/user-attachments/assets/2fdd84e3-b814-4bed-b4fc-9c811527d1e9" />

#### -   CSS (css/style.css)

<img width="740" height="366" alt="Screenshot (242)" src="https://github.com/user-attachments/assets/fb3cb796-921a-444d-b58e-16e5383d8ecd" />
<img width="735" height="145" alt="Screenshot (243)" src="https://github.com/user-attachments/assets/63d7c7c4-07e6-4fce-b3f2-e16fcf8924d4" />

#### -   JavaScript (js/script.js)

<img width="736" height="434" alt="Screenshot (245)" src="https://github.com/user-attachments/assets/6ab02102-2227-4d5a-ba7a-ec1d5060cb62" />

## 4.  Permissions
```
chmod -R 755 ~/web_project
```
## 5.  Backup Script (backup.sh)

<img width="731" height="443" alt="Screenshot (255)" src="https://github.com/user-attachments/assets/1309628f-e130-430a-b397-189d22d08fc6" />

## 6.  Make it executable:
```
chmod +x backup.sh
```

## 7.  Run it:
```
./backup.sh
```
## 8.  Start a simple server:
```
python3 -m http.server 5500
```
<img width="993" height="588" alt="Screenshot (249)" src="https://github.com/user-attachments/assets/9dd591e1-331e-4163-b5a2-7e8c0aa8f96b" />
<img width="990" height="588" alt="Screenshot (250)" src="https://github.com/user-attachments/assets/e6be1c54-4078-402a-a9c7-e48e705b9215" />

