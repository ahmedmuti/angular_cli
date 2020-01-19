

**Installation**

``` 
npm install -g angular-cli 
```



**Usage**

```
ng --help 
```



**Generating and serving an Angular8 project via a development server**

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




**Generating Components, Directives, Pipes and Services**

>You can use the ng generate (or just ng g) command to generate Angular components or Directives or anything :


**Component**

```
ng generate component my-new-component
```

or 

```
ng g c my-new-component
```

> Note: `my-new-component` means component name . you can type any name you want 


**Directive**

```
ng generate directive my-new-directive
```

or 

```
ng g d my-new-directive
```

**Pipe**


```
ng generate pipe my-new-pipe
```

or 

```
ng g p my-new-pipe
```


**Service**


```
ng generate service my-new-service
```

or 

```
ng g s my-new-service
```

**Class**


```
ng generate class my-new-class
```

or 

```
ng g cl  my-new-class
```

**Interface**


```
ng generate interface my-new-interface
```

or 

```
ng g i  my-new-interface
```

**Enum**


```
ng generate enum my-new-enum
```

or 

```
ng g e  my-new-enum
```

**Module**


```
ng generate module my-module
```

or 

```
ng g m my-module
```

