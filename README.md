# springboot-security-keycloak
Spring Boot 3.1.4

Reference ::

https://www.keycloak.org/downloads

https://www.keycloak.org/getting-started/getting-started-zip

https://www.keycloak.org/docs/latest/securing_apps/#_spring_boot_adapter


KeyCloak Download  : https://www.keycloak.org/downloads

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/f77cfae7-17c8-49df-9547-43ab4e1cc2fb)

UnZip the file

Go to keycloak-22.0.4\bin

Run kc.bat start-dev

Open http://localhost:8080

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/112d4a2a-7d30-4df1-95dd-21132d32e4e6)

Enter admin / admin / admin Click on Create

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/8d64c765-cd32-47a4-918f-886359567a7a)

Click On Administration Console

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/027f3160-35d6-4709-976f-8dbdd575febf)

Enter admin / admin
![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/8c648b65-6da7-4596-9f57-bfcd4d9f0b26)

Click On Master -> Create Realm 

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/d98b85d4-d1e4-467f-ba5f-fd5132c5e5bf)

Enter Name and Click on Create

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/1415e9d2-8118-41bd-b876-a1bdc25ce164)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/161885e3-bda7-423b-8f16-2ec99c7317eb)

Click on Clients -> Create Client

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/3ed31cb5-4379-41b7-99b8-8eae4a2f7e56)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/5d8138c4-2af1-44f9-8314-f498d6b12b94)

Next

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/5b16947e-f29d-4633-9dc8-4a6aba32282f)


Root URL is the Spring boot service end point
Save

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/38e704f4-098e-4ded-9ec1-9b73659b5da1)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/f1a329a6-8ed4-42d7-b650-dc6de3cc6a88)

Click on Realm Roles -> Create role 

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/1e1e335b-27aa-4d40-a609-afd8685149ce)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/a49d8c97-9690-41d6-a658-ee76b0cb43a5)

Roles admin, user and Save

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/5e8032f0-f175-49a2-a718-28c610e52ce7)

Click Users -> Add User -> Credentials (Password) -> Assign above roles

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/001560f1-4a06-4d77-93e8-c6f3b05fc98b)

Create Admin and DevUser (2 Users)
![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/27010b5c-1663-424b-984b-13438d70803c)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/f80418ef-3701-4ced-b8a3-faa4006f0a99)


![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/0d8b6961-6abe-4e3a-96d9-923743fa170c)

Assign A Role
![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/eef37c95-0ec7-4488-8791-b849d76573ca)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/75656597-5246-487a-809d-ae4004f68d72)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/ede1855d-8bc8-4ebf-b328-6dd878be3267)

I Changed Spring Boot Port to 9090 (Check Client Root URL and change)
Go to http://localhost:8080/realms/springbootrealm/.well-known/openid-configuration

Copy the end point : "token_endpoint": "http://localhost:8080/realms/springbootrealm/protocol/openid-connect/token"

Open POSTMAN

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/a0ae057b-9600-4ea3-b7c7-8dcc1c52c7b6)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/9225280b-b394-4687-8006-1e2d283fb242)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/49bb4790-b6e6-4dc6-aa92-426448d0ce14)

Send
![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/4d642df9-fbc2-439a-8a12-fd71330b603a)

![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/19162e31-858f-4c8c-89a6-fc72d4afef16)


![image](https://github.com/srss-pocs/springboot-security-keycloak/assets/145287517/7875be3f-a0d9-4f7a-8ea9-50343eec1805)






































































