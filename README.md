# OAuth2 & Spring boot 3 & Social login
## Step by step demonstration for loging with github account and google account
### 01) Add OAuth2 Client dependency
![image](https://github.com/SupuniAbeysinghe/OAuth2_Social_Login-Demo/assets/121711723/f2f16099-91b5-4d4c-bbc2-a4613c042daf)
### 02)	Create the springboot application and open it in intelijIDE

<br/>

# Create Authorization server

# GitHub
**1. Settings - > developer settings**
<br/>


![2](https://github.com/SupuniAbeysinghe/OAuth2_Social_Login-Demo/assets/121711723/0729e10d-9ebb-4438-88f3-5e6949d997dd)

**2. Then create a new app**
<br/>

![image](https://github.com/SupuniAbeysinghe/OAuth2_Social_Login-Demo/assets/121711723/34a26dec-29a3-4ebd-b2a2-b0a9e3a32deb)

**3. Then generate new secret key and save Client Id and secret key**
<br/><br/>

# Google Account

[http://console.cloud.google.com](http://console.cloud.google.com)

**1. create a new project**
<br/>

![image](https://github.com/SupuniAbeysinghe/OAuth2_Social_Login-Demo/assets/121711723/291e2259-e8ee-4f53-b3ad-06e73cd97315)

**2. Then create an application**

*APIs and service - > Credentials-> OAuth 2.0 Client IDs*

**3. Then save the clientId and secret key**
<br/><br/>

# Create the Resource Server

## create the end points and update the application.properties / application.yml file

### application.properties

```
spring.security.oauth2.client.registration.github.clientId= <GITHUB CLIENT ID>
spring.security.oauth2.client.registration.github.clientSecret= <GITHUB SECRET KEY>
spring.security.oauth2.client.registration.google.clientId= <GOOGLE CLIENT ID>
spring.security.oauth2.client.registration.google.clientSecret= <GOOGLE SECRET KEY>

```

# OR

### application.yml

```
spring:
  security:
    oauth2:
      client:
        registration:
          github:
            clientId: <GITHUB CLIENT ID>
            clientSecret: <GITHUB SECRET KEY>
          google:
            clientId: <GOOGLE CLIENT ID>
            clientSecret: <GOOGLE SECRET KEY>

```





