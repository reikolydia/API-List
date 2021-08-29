# API LIST

A list of authentication-***less*** API endpoints.

A good place to start testing is with the [httpbin.org](https://httpbin.org/) service.

### To use Windows Powershell: ###

HTTP **GET**

```
Invoke-RestMethod -Uri ' endpoint URL ' -Method GET
```

HTTP **POST**

```
Invoke-WebRequest -Uri ' rest url ' -Method POST -Body @{ post_header='postbody' }
```

HTTP **DELETE**

```
Invoke-RestMethod -Uri ' endpoint URL ' -Method DELETE
```

HTTP **PATCH**

```
Invoke-RestMethod -Uri ' endpoint URL ' -Method PATCH -Body @{ patch_header='patchbody' }
```

HTTP **PUT**

```
Invoke-RestMethod -Uri ' endpoint URL ' -Method PUT -Body @{ put_header='putbody' }
```
