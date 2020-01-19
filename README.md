

# Installation

``` 
npm install -g angular-cli 
```



**Usage** 

```
ng --help 
```



 ## Generating and serving an Angular8 project via a development server

```
ng new PROJECT_NAME
cd PROJECT_NAME
ng serve
```
>Navigate to ``` http://localhost:4200/.``` The app will automatically reload if you change any of the source files.

>you can use ``` ng serve --open ``` or ``` ng s --o ``` to Navigate automatically to ``` http://localhost:4200/.```  

>You can configure the default HTTP port and the one used by the LiveReload server with this command-line :

```
ng serve --open --port 0.0.0.0
Note: `0.0.0.0` means port number such as 4300 or 4500 
you can type any number you want 
``` 




## Generating Components, Directives, Pipes and Services

>You can use the ng generate (or just ng g) command to generate Angular components or Directives or anything :


### Component

```
ng generate component my-new-component
```
or 
```
ng g c my-new-component
```

> Note: `my-new-component` means component name . you can type any name you want , and so on 




______________________________________________________________________________________________






### Directive

```
ng generate directive my-new-directive
```

or 

```
ng g d my-new-directive
```



______________________________________________________________________________________________






### Pipe


```
ng generate pipe my-new-pipe
```

or 

```
ng g p my-new-pipe
```



______________________________________________________________________________________________







### Service


```
ng generate service my-new-service
```

or 

```
ng g s my-new-service
```



______________________________________________________________________________________________






### Class


```
ng generate class my-new-class
```

or 

```
ng g cl  my-new-class
```



______________________________________________________________________________________________






### Interface


```
ng generate interface my-new-interface
```

or 

```
ng g i  my-new-interface
```



______________________________________________________________________________________________






### Enum


```
ng generate enum my-new-enum
```

or 

```
ng g e  my-new-enum
```



______________________________________________________________________________________________






### Module


```
ng generate module my-module
```

or 

```
ng g m my-module
```



______________________________________________________________________________________________





## Creating a build

```
ng build --prod
```
>The build artifacts will be stored in the dist/ directory.



______________________________________________________________________________________________




## Proxy To Backend

>Using the proxying support in webpack's dev server we can highjack certain urls and send them to a backend server. 
>We do this by passing a file to `--proxy-config`

   
>Say we have a server running on `http://localhost:3000/api`
and we want all calls `http://localhost:4200/api` to go to that server.


We ***create*** a file ***next*** to projects `package.json` called `proxy.conf.json` with the content

```
{
  "/api": {
    "target": "http://localhost:3000",
    "secure": false
  }
}
```
and then we ***edit** the package.json file's ***start*** script to be
```
"start": "ng serve --proxy-config proxy.conf.json",
```

and now ***run*** it with ` npm start `

[Watch a Configure Proxy video](https://www.youtube.com/watch?v=z1MUmTjYKH8)


______________________________________________________________________________________________



## 3rd Party Library Installation

Simply install your library via `npm install lib-name --save` .




______________________________________________________________________________________________



## Updating angular-cli

You can check your current **version** of Angular CLI using the following command.

```
ng --version
```
If you're using Angular CLI 1.0.0-beta.28 or less, 
you need to ***uninstall*** angular-cli package.

To update the latest angular-cli package installed globally in your system,
you need to run the following commands.

***For Windows*** 

Open Powershell on Administrator Mode
```
npm uninstall -g angular-cli  
```
***For Mac***
```
sudo npm uninstall -g angular-cli 
```

**Then we need to clear the cache using the following command.**

```
 npm cache verify
```
Then you need to hit the following command.
```
npm cache clean
```

**Now, install the Angular CLI using the following command.**
```
npm install -g angular-cli@latest
```
>After updating both the global and local package, clear the cache to avoid errors.

```
npm cache verify
npm cache clean
```  




______________________________________________________________________________________________





## Update Angular Packages

If you have created an Angular project, then go inside that folder then open CMD and type the following command.

```
ng update
```





