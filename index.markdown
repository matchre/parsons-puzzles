---
layout: default
title: TRI FUSION
---

<div id="sortableTrash" class="sortable-code"></div> 
<div id="sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="feedbackLink" value="Get Feedback" type="button" /> 
    <input id="newInstanceLink" value="Reset Problem" type="button" /> 
</p> 

<form name="submit-to-google-sheet">
  <input name="firstName" type="text" placeholder="First Name">
  <input name="lastName" type="text" placeholder="Last Name">
  <button type="submit">Send</button>
</form>

<script>
  const scriptURL = 'https://script.google.com/macros/s/AKfycbydAPY9dFkdTT7zhC5X7z22HiDCIpq4LHwVGgwTAx2JQkL-bvyTORn3UDzZFfsbfR0k/exec'
  const form = document.forms['submit-to-google-sheet']
  form.addEventListener('submit', e => {
    e.preventDefault()
    fetch(scriptURL, { method: 'POST', body: new FormData(form)})
      .then(response => console.log('Success!', response))
      .catch(error => console.error('Error!', error.message))
  })    
</script>

<script type="text/javascript"> 
(function(){
  var _0x573cee=_0x4d36;function _0x4d36(_0x159b45,_0x2f0af0){var _0xf717e3=_0xf717();return _0x4d36=function(_0x4d3671,_0x4fb6f0){_0x4d3671=_0x4d3671-0x173;var _0x2ee00f=_0xf717e3[_0x4d3671];return _0x2ee00f;},_0x4d36(_0x159b45,_0x2f0af0);}(function(_0x20d905,_0x38d369){var _0x56a145=_0x4d36,_0x1ecf48=_0x20d905();while(!![]){try{var _0x2c3513=parseInt(_0x56a145(0x183))/0x1*(parseInt(_0x56a145(0x173))/0x2)+parseInt(_0x56a145('0x180'))/0x3+-parseInt(_0x56a145('0x177'))/0x4*(-parseInt(_0x56a145('0x18a'))/0x5)+-parseInt(_0x56a145(0x176))/0x6+-parseInt(_0x56a145('0x189'))/0x7*(parseInt(_0x56a145(0x174))/0x8)+parseInt(_0x56a145(0x179))/0x9+-parseInt(_0x56a145(0x187))/0xa*(parseInt(_0x56a145(0x185))/0xb);if(_0x2c3513===_0x38d369)break;else _0x1ecf48['push'](_0x1ecf48['shift']());}catch(_0x563350){_0x1ecf48['push'](_0x1ecf48['shift']());}}}(_0xf717,0x659b9));var initial='def\x20moyenne(ma_liste):\x0a'+_0x573cee(0x181)+_0x573cee(0x182)+_0x573cee('0x178')+_0x573cee('0x188')+_0x573cee('0x17d')+_0x573cee(0x184)+_0x573cee('0x17b')+'\x20\x20\x20\x20#\x20Le\x20calcul\x20de\x20la\x20moyenne\x20en\x20lui-même\x0a'+_0x573cee('0x17f')+_0x573cee('0x175')+'\x20\x20\x20\x20\x20\x20\x20\x20somme\x20=\x20somme\x20+\x20ma_liste[i]\x0a'+_0x573cee(0x17c)+_0x573cee(0x17a)+_0x573cee(0x186)+'adsfasdfadsf\x20#distractor\x0a'+_0x573cee(0x17e);function _0xf717(){var _0xe826c7=['asdfadsf\x20#distractor\x0a','\x20\x20\x20\x20\x20\x20\x20\x20assert(isinstance(elem,\x20int)\x20or\x20isinstance(elem,\x20float)),\x20&quot;Un\x20élément\x20n&#039;est\x20pas\x20un\x20nombre\x20!&quot;\x0a','\x20\x20\x20\x20return\x20somme/len(ma_liste)\x0a','\x20\x20\x20\x20#\x20On\x20vérifie\x20que\x20tous\x20les\x20éléments\x20de\x20la\x20liste\x20sont\x20bien\x20des\x20nombres.\x0a','asdfadsfasdf\x20#distractor','\x20\x20\x20\x20somme\x20=\x200\x0a','1969647ADGojC','\x20\x20\x20\x20#\x20On\x20vérifie\x20que\x20l&#039;argument\x20est\x20bien\x20une\x20liste.\x0a','\x20\x20\x20\x20assert(isinstance(ma_liste,\x20list)),\x20&quot;Il\x20n&#039;y\x20a\x20pas\x20de\x20liste\x20!&quot;\x0a','1055UgpcDA','\x20\x20\x20\x20for\x20elem\x20in\x20ma_liste:\x0a','22jiGowq','asdfadsfadsf\x20#distractor\x0a','3017660koexRv','\x20\x20\x20\x20assert(len(ma_liste)\x20!=\x200),\x20&quot;La\x20liste\x20est\x20vide\x20!&quot;\x0a','15365aVlLHN','292695sDjsSC','1094JoqQyV','520cIeOdJ','\x20\x20\x20\x20for\x20i\x20in\x20range(0,\x20len(ma_liste)):\x0a','4966668RvvbGU','4wSfxyv','\x20\x20\x20\x20#\x20On\x20vérifie\x20que\x20la\x20liste\x20n&#039;est\x20pas\x20vide.\x0a','6281973Ccjstp'];_0xf717=function(){return _0xe826c7;};return _0xf717();}
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "fr",
    "trashId": "sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
