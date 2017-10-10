# cifrado-cesar
function cipher (sentence){
  var convertToArray = sentence.split('');
  var arrayConvertToAscii = [];
  for(var i = 0; i < convertToArray.length; i++ ){
  arrayConvertToAscii.push((sentence.charCodeAt(i)-65 + 33) % 26 + 65);
  }
  //convirtiendo los valores ASCII a 
  var arrayAsciiToCipher = [];
  for(var j = 0; j <arrayConvertToAscii.length; j++ ){
  arrayAsciiToCipher.push(arrayConvertToAscii.fromCharCode(j));
  arrayAsciiToCipher.toString();
  }
  return arrayAsciiToCipher ;
}

var inWord = prompt('ingrese una frase');
cipher(inWord);
