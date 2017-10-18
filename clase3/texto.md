# Clases en Java

```java

public class Asignatura {
    private String nombre;
    private int creditos;
    
    public void establecer_nombre(String n){
        nombre = n;
    }
    
    public void establecrer_creditos(int n){
        creditos = n;
    }
    
    public String obtener_nombre(){
        return nombre;
    }
    
    public int obtener_creditos(){
        return creditos;
    }
    
    @Override
    public String toString(){
        String cadena = String.format("%s con número de crédito", 
                obtener_nombre(), obtener_nombre());
        return cadena;
    }
}
```

```java

public class Asignatura {
    private String nombre;
    private int creditos;
    
    public Asignatura(String n, int cred){
        nombre = n;
        creditos = cred;
    }
    public void establecer_nombre(String n){
        nombre = n;
    }
    
    public void establecrer_creditos(int n){
        creditos = n;
    }
    
    public String obtener_nombre(){
        return nombre;
    }
    
    public int obtener_creditos(){
        return creditos;
    }
    
    @Override
    public String toString(){
        String cadena = String.format("%s con número de crédito", 
                obtener_nombre(), obtener_nombre());
        return cadena;
    }
}
```