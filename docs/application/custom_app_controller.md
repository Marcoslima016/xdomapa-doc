
<!--========================== CABECALHO ==========================-->

#CustomAppController class
:page_facing_up: [ Source](https://github.com/Marcoslima016/flutter_packages/blob/main/projeto-custom_app/custom_app/lib/custom_app/out/app_controller/app.controller.interface.dart#L14)



Classe extendida no controller da aplicação. 


<!--========================= INTRODUCAO =========================-->




Exemplo prático de uma subclasse AppController que extende a classe CustomAppController:
```dart
class AppController extends CustomAppController {
  
  @override
  AppConfig appConfig; 

  @override
  AuthPreferences authPreferences = AuthPreferences(privateRoute: "/teste");

  AppStartConfig appStartConfig;

  static final AppController instance = AppController._();

  AppController._() {
    appStartConfig = AppStartConfig(appSession: appSession);

    appConfig = AppConfig(
      setInitialRoute: appStartConfig.initialRoute,
    );
  }
}
```


**Inheritance**

**Implementations**

CustomAppControllerRequireds

**Implementers**

<!--========================= CONSTRUTORES =========================-->
##Construtores

CustomAppController({}); 

<!--========================= PROPRIEDADES =========================-->

##Propriedades

appConfig -> [AppConfig](app_config.md)

authPrefernes -> AuthPreferences

<!--=========================== METODOS ===========================-->


##Metodos
