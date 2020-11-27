# NTP
Buscar a Hora via Protocolo NTP (JAVA)

Inserção de servidores da América do Sul, sugestão de padronização de código, sugestão de acesso a host por laço for ao invés de while e inserção de funcionalidade de formatação do retorno Date para String.

Exemplo de consumo:
```Java
 try {     
    System.out.println("Data e hora com um padrão: " + NTP.getDatePattern("HH:mm:ss dd/MM/yyyy"));
    System.out.println("Data e hora do tipo Date: " + NTP.getDateTime()); 
    System.out.println("Data do tipo Date: " + NTP.getDate());
    System.out.println("Hora do tipo Date: " + NTP.getTime());
    System.out.println("Data e hora do tipo String: " + NTP.getDateTimeToString()); 
    System.out.println("Data do tipo String: " + NTP.getDateToString());
    System.out.println("Hora do tipo String: " + NTP.getTimeToString());
} catch (Exception e)  {    
    e.printStackTrace();
}
```
Resultado:

Data e hora com um padrão: 11:34:38 08/11/2018.

Data e hora do tipo Date: Thu Nov 08 11:34:38 BRST 2018.

Data do tipo Date: Thu Nov 08 00:00:00 BRST 2018

Hora do tipo Date: Thu Jan 01 11:34:38 BRT 1970

Data e hora do tipo String: 08/11/2018 11:34:38

Data do tipo String: 08/11/2018

Hora do tipo String: 11:34:38
