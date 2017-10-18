# Clases en Java

```java
public class Principal {
    
    public static void main(String[] args) {
        // Se crean las asignaturas
        Asignatura a1 = new Asignatura();
        a1.establecer_nombre("Matemáticas");
        a1.establecrer_creditos(8);
        
        Asignatura a2 = new Asignatura();
        a2.establecer_nombre("Física");
        a2.establecrer_creditos(6);
        
        Titulo t1 = new Titulo();
        t1.establecer_nombre("Licenciado en Físico Matemáticas");
        t1.establecer_nombre_universidad("Universidad Politécnica");
        
        Titulo t2 = new Titulo();
        t2.establecer_nombre("Magister en Docencia Matemática");
        t2.establecer_nombre_universidad("Universidad Valenciana");
        
        Docente docente = new Docente();
        docente.establecer_nombres("Luis V");
        docente.establecer_apellidos("Perez J");
        docente.establecer_asignatura_1(a1);
        docente.establecer_asignatura_2(a2);
        docente.establecer_tit_tercer_nivel(t1);
        docente.establecer_tit_cuarto_nivel(t2);
        System.out.println(docente);
        
        
    }
}

```

```java
public class Principal {
    
    public static void main(String[] args) {
        // Se crean las asignaturas
        Asignatura a1 = new Asignatura("Matemática", 8);
        Asignatura a2 = new Asignatura("Física", 6);
        
        // Se crean los títulos
        Titulo t1 = new Titulo("Licenciado en Físico Matemáticas", "Universidad Politécnica");
        Titulo t2 = new Titulo("Magister en Docencia Matemática", "Universidad Valenciana");
                
        Docente docente = new Docente("Luis V", "Perez J", t1, t2, a1, a2);
        System.out.println(docente);
        
        
    }
}

```
