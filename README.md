# validate-Email
Metodo para validar un Email 
##Ejemplo
Este metodo permite poder validar un Email y regresarnos un Booleano como resultado
```java
private boolean isValidEmail(String email) {

    String EMAIL_PATTERN = "^[_A-Za-z0-9-\\+]+(\\.[_A-Za-z0-9-]+)*@"
            + "[A-Za-z0-9-]+(\\.[A-Za-z0-9]+)*(\\.[A-Za-z]{2,})$";

    Pattern pattern = Pattern.compile(EMAIL_PATTERN);
    Matcher matcher = pattern.matcher(email);

    return matcher.matches();
    
}
```
