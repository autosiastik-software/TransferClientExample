# Transfer Client Example

Das Verhalten der Transfer Client Komponente kann mit folgenden Parametern beeinflusst werden:  
  
Options:

`qrCodeSize`:  
Steuert die Größe des QR Code Images.  
Default: 600  
  
`transferFileSize`:  
Für Bilddateien wird eine Kompression vorgenommen. Diese kann in KB angegeben werden.  
Default: 600  

`polling`:  
Standardmäßig findet die Kommunikation via Websocket statt. Als Fallback Variante kann gepollt werden. Dann fragt die Komponente alle 2 Sek. beim Server nach, ob eine Datei übertragen wurde.  
Default: false  

`showTransferFile`:  
Gibt an, ob die übertragene Datei auf der Oberfläche angezeigt werden soll. Im Falle eines übertragene Bildes wird dieses in einem img Tag gerendert.  
Default: true  

`showLoader`:  
Gibt an, ob ein Loading Spinner angezeigt werden soll, wenn die Übertragung gestartet wurde.  
Default: true  
  
Die Options können dem Konstruktor wie folgt übergeben werden:  
  
```
const ft = new FileTransfer({
	qrCodeSize: 400,
	transferFileSize: 1000
});
```
