function greet() {
  if ('speechSynthesis' in window) {
    var utterance = new SpeechSynthesisUtterance('Boa noite, Igor!');
    window.speechSynthesis.speak(utterance);
  } else {
    console.log('Your browser does not support text to speech.');
  }
}
greet();
