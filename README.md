# Introduzione a React

React è una libreria Javascript e si focalizza sulla parte UI di una WEB Application e non fa nessuna assunzione sul resto delle tecnologie utilizzate. Utilizza un Virtual DOM del DOM (Document Object Model) da rappresentare, rendendo la programmazione più facile e la visualizzazione più veloce. Pertanto React rappresenta la V del pattern di sviluppo MVC.

Uno dei benefici di React è che è semplice, presenta una sintassi di tipo dichiarativa, che è l'opposto della programmazione imperativa. Ad esempio un codice imperativo del tipo:

```
for(var i=0; i<nums.length; i++){
	var number = nums[i]*2;
	array.push(number);
}
```

mentre un esempio di programmazione dichiarativa è il seguente:

```
var array = nums.map(function(num){
	return num * 2;
});
```
La differenza è che il programmatore, con la seguente dichiarazione, esprime, dichiara, l'intento logico e la relazione esistente tra i dati ed il risultato finale e l'esecuzione è affidata al parser senza specificarne la procedura, mentre con la for esplicitiamo le istruzioni passo passo, e quindi il flusso che si dovrà seguire per raggiungere il risultato da ottenere.

Un'applicazione React è componibile, cioè ho una collezione di componenti (riutilizzabili!) che concorrono alla creazione della mia UI. Quindi l'idea generale di React è di suddividire la mia UI in componenti, come tanti piccoli mattoncini Lego.

Infine React è veloce. Tra la mia APP e il DOM, ho un layer detto Virtual Dom. La mia APP non manipola il DOM direttamente ma, tramite Javascript, il Virtual Dom. Solo la parte che cambia verrà poi effettivamente aggiornata nel DOM favorendo tempi di reazione molto più veloci della norma.

Per lavorare con React, è bene conoscere: HTML, CSS, JS e preferibilmente Bootstrap. E' bene avere NodeJS :)

# Il primo componente React

Includo gli script di react e react-dom, inoltre utilizzo lo script di babel che rimpiazza, dalla v15.0 JSTransform e quindi non includo più lo script JSXTransformer (dalla v14.0), che cercava, all'interno di HTML, la tag ```<script type="text/jsx">``` da interpretare. Ora avrò una tag del tipo ```<script type="text/babel">```. In questo modo, grazie a Babel, avrò accesso alle novità di ECMAScript2015.

###Starter Kit

```
<!DOCTYPE html>
<html>
<head>
	<title>Esempio di Hello World</title>
	<meta charset="utf-8" />
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">

	<!-- REACT -->
	<script src="https://cdnjs.cloudflare.com/ajax/libs/react/15.0.1/react.min.js"></script>
	<script src="https://cdnjs.cloudflare.com/ajax/libs/react/15.0.1/react-dom.min.js"></script>
	<!-- BABEL -->
	<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.23/browser.min.js"></script>
 
</head>
<body>

	<script type="text/babel">

  </script>

</body>
</html>
```