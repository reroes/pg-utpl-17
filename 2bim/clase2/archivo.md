


	public class LeerArchivoTexto{
		private Scanner entrada;

   		// permite al usuario abrir el archivo
		public void abrirArchivo(){
      		try
      		{
         		entrada = new Scanner( new File( "archivo1.csv" ) );
      		} // fin de try
      		catch ( FileNotFoundException fileNotFoundException )
      		{
         		System.err.println( "Error al abrir el archivo." );
         		System.exit( 1 );
      		} // fin de catch
   	} // fin del m�todo abrirArchivo

   	// lee registro del archivo
  	public void leerRegistros()
   	{
      
      		
      		try // lee registros del archivo, usando el objeto Scanner
      		{
         
         	while ( entrada.hasNext() )
         	{
             		// System.out.println(entrada.nextLine());
             		String cadena = entrada.nextLine();
             		
                    
         	} // fin de while
      		} // fin de try
      		catch ( NoSuchElementException elementException )
      		{
         		System.err.println( "El archivo no esta bien formado." );
         		entrada.close();
         		System.exit( 1 );
      		} // fin de catch
      		catch ( IllegalStateException stateException )
      		{
         		System.err.println( "Error al leer del archivo." );
         		System.exit( 1 );
      		} // fin de catch
      	return lista;
   	} // fin del m�todo leerRegistros

  	 // lee registro del archivo
   
   	// cierra el archivo y termina la aplicaci�n
  	public void cerrarArchivo()
   	{
      		if ( entrada != null )
         	entrada.close(); // cierra el archivo
   	} // fin del m�todo cerrarArchivo
}
