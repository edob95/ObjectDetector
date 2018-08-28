La presente cartella costituisce la consegna del progetto numero 10 del corso di Software Engineering. L'obbiettivo del progetto è quello di realizzare un modello di machine learning atto al riconoscimento di un oggetto specifico (nel mio caso una bottiglia di San Bernardo), ed esportare il modello stesso nell'applicazione Android fornita da TensorFlow.

La cartella denominata HowTo contenente 3 guide differenti, la prima per l'installazione di TensorFlow, la seconda per l'esecuzione della fase di training e tutto il setup che la precede, la terza per l'esportazione del modello ottenuto all'interno dell'applicazione Android.
Attraverso le tre guide è possibile replicare il lavoro da me svolto (installazione training ed esportazione).

La cartella Bernardi_Object_Detection contiene tutti i file che sono necessari per l'addestramento del modello di machine learning e i file che vengono prodotti da tale processo. La spiegazione degli stessi e il loro uso è fornito all'interno della guida numero 2, dedicata alla fase di training.

La cartella AndroidFolder è una repository fornita da TensorFlow all'interno della quale è presente tra i vari file la cartella costituente il progetto Android dell'applicazione che andrà ad essere utilizzata. Per il suo setup e la sua installazione è spiegato tutto nella guida numero 3.

La cartella JavaDoc contiene la documentazione dell'applicazione Android fornita da TensorFlow.

Infine il file san_bernardo_detection_200k.apk è il file APK ottenuto da AndroidStudio (come ottenere il file è spiegato nella guida numero 3) che permette l'installazione dell'app contenente il modello di machine learning da me addestrato.


Il lavoro da me svolto è stato quindi tutto quello che può essere replicato seguendo gli howTo ovvero il seguente:

- Installazione di tensorflow e di tutte le componenti aggiuntive necessarie.
- Collezione del dataset costituito inizialmente da circa 400 foto, riquadro delle stesse per mezzo del software LabelImg ed ottenimento dei file xml.
- Modifica del file xml_to_csv.py come mostrato nell'how to, e conversione degli xml per mezzo di esso e del file generate_tfrecord.py.
- Comprensione dei passi da eseguire per l'addestramento del modello di machine learning per mezzo di tensorflow.
- Comprensione su come eseguire l'addestramento per mezzo di GoogleCloud per disporre di una maggior potenza computazionale.
- Esecuzione dell'addestramento per mezzo di tensorflow e di GoogleCloud vista la scarsa potenza del mio calcolatore.
- Esportazione del modello addestrato sull'applicazione fornita da TensorFlow.
- Ripetizione di tutti i passi con un dataset di 1000 immagini.

Essenzialmente il codice da me scritto sono solamente le modifiche che vengono illustrate nel corso degli HowTo.
La difficoltà principale è stata quella di comprendere tutti i passi illustrati.
La parte corposa del lavoro è stata la collezione del dataset e la fase di training; i file utilizzati per la conversione del dataset, i modelli pre addestrati ed i file di configurazione sono già disponibili in rete alcuni di essi forniti da TensorFlow. L'applicazione Android è stata sviluppata da TensorFlow, la stessa viene utilizzata per verificare la bontà del modello addestrato e la capacità di riconoscere l'oggetto specifico.
