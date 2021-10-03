<div id="sortableTrash" class="sortable-code"></div> 
<div id="sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="feedbackLink" value="Get Feedback" type="button" /> 
    <input id="newInstanceLink" value="Reset Problem" type="button" /> 
</p> 


<form name="submit-to-google-sheet">
  <input name="email" type="email" placeholder="Email" required>
  <input name="firstName" type="text" placeholder="First Name">
  <input name="lastName" type="text" placeholder="Last Name">
  <button type="submit">Send</button>
</form>

<script src="https://wzrd.in/standalone/formdata-polyfill"></script>
<script src="https://wzrd.in/standalone/promise-polyfill@latest"></script>
<script src="https://wzrd.in/standalone/whatwg-fetch@latest"></script>

<script>
  const scriptURL = 'https://script.google.com/macros/s/AKfycbydAPY9dFkdTT7zhC5X7z22HiDCIpq4LHwVGgwTAx2JQkL-bvyTORn3UDzZFfsbfR0k/exec'
  form.addEventListener('submit', e => {
    e.preventDefault()
    fetch(scriptURL, { method: 'POST', body: new FormData(form)})
      .then(response => console.log('Success!', response))
      .catch(error => console.error('Error!', error.message))
  })    
</script>






<script type="text/javascript"> 

function _0x25d1(){var _0x519816=['\x20\x20\x20\x20#\x20On\x20vérifie\x20que\x20l&#039;argument\x20est\x20bien\x20une\x20liste.\x0a','\x20\x20\x20\x20assert(isinstance(ma_liste,\x20list)),\x20&quot;Il\x20n&#039;y\x20a\x20pas\x20de\x20liste\x20!&quot;\x0a','LineBasedGrader','\x20\x20\x20\x20#\x20On\x20vérifie\x20que\x20la\x20liste\x20n&#039;est\x20pas\x20vide.\x0a','\x20\x20\x20\x20somme\x20=\x200\x0a','\x20\x20\x20\x20assert(len(ma_liste)\x20!=\x200),\x20&quot;La\x20liste\x20est\x20vide\x20!&quot;\x0a','def\x20moyenne(ma_liste):\x0a','\x20\x20\x20\x20\x20\x20\x20\x20somme\x20=\x20somme\x20+\x20ma_liste[i]\x0a','preventDefault','_graders','184605KvJsBs','asdfadsfadsf\x20#distractor\x0a','8nolGoI','423020ebKYje','4492755GYLUDM','\x20\x20\x20\x20for\x20i\x20in\x20range(0,\x20len(ma_liste)):\x0a','\x20\x20\x20\x20#\x20On\x20vérifie\x20que\x20tous\x20les\x20éléments\x20de\x20la\x20liste\x20sont\x20bien\x20des\x20nombres.\x0a','\x20\x20\x20\x20return\x20somme/len(ma_liste)\x0a','init','225066WACDuI','188868CadpHR','shuffleLines','\x20\x20\x20\x20\x20\x20\x20\x20assert(isinstance(elem,\x20int)\x20or\x20isinstance(elem,\x20float)),\x20&quot;Un\x20élément\x20n&#039;est\x20pas\x20un\x20nombre\x20!&quot;\x0a','click','10FKOvux','1625208tJixqE','84pMjyNq','\x20\x20\x20\x20#\x20Le\x20calcul\x20de\x20la\x20moyenne\x20en\x20lui-même\x0a','32914mIfZbi','asdfadsfasdf\x20#distractor'];_0x25d1=function(){return _0x519816;};return _0x25d1();}function _0x1c5c(_0x1dd76b,_0x197ba2){var _0x25d127=_0x25d1();return _0x1c5c=function(_0x1c5c88,_0x394b70){_0x1c5c88=_0x1c5c88-0x176;var _0x5c7a60=_0x25d127[_0x1c5c88];return _0x5c7a60;},_0x1c5c(_0x1dd76b,_0x197ba2);}(function(_0x33cc82,_0x593767){var _0xd8a255=_0x1c5c,_0x75f291=_0x33cc82();while(!![]){try{var _0x47e87f=parseInt(_0xd8a255(0x191))/0x1+parseInt(_0xd8a255('0x18a'))/0x2+parseInt(_0xd8a255('0x190'))/0x3+-parseInt(_0xd8a255('0x189'))/0x4*(parseInt(_0xd8a255(0x187))/0x5)+parseInt(_0xd8a255(0x179))/0x6*(parseInt(_0xd8a255(0x17b))/0x7)+parseInt(_0xd8a255('0x178'))/0x8+parseInt(_0xd8a255('0x18b'))/0x9*(-parseInt(_0xd8a255(0x177))/0xa);if(_0x47e87f===_0x593767)break;else _0x75f291['push'](_0x75f291['shift']());}catch(_0x7e7d17){_0x75f291['push'](_0x75f291['shift']());}}}(_0x25d1,0x29d4e),function(){var _0x24cbd0=_0x1c5c,_0x2718f1=_0x24cbd0(0x183)+_0x24cbd0('0x17d')+_0x24cbd0('0x17e')+_0x24cbd0(0x180)+_0x24cbd0(0x182)+_0x24cbd0('0x18d')+'\x20\x20\x20\x20for\x20elem\x20in\x20ma_liste:\x0a'+_0x24cbd0('0x193')+_0x24cbd0(0x17a)+_0x24cbd0(0x181)+_0x24cbd0(0x18c)+_0x24cbd0(0x184)+_0x24cbd0('0x18e')+'asdfadsf\x20#distractor\x0a'+_0x24cbd0(0x188)+'adsfasdfadsf\x20#distractor\x0a'+_0x24cbd0('0x17c'),_0x45183c=new ParsonsWidget({'sortableId':'sortable','max_wrong_lines':0xa,'grader':ParsonsWidget[_0x24cbd0('0x186')][_0x24cbd0('0x17f')],'exec_limit':0x9c4,'can_indent':!![],'x_indent':0x32,'lang':'en','trashId':'sortableTrash'});_0x45183c[_0x24cbd0('0x18f')](_0x2718f1),_0x45183c[_0x24cbd0('0x192')](),$('#newInstanceLink')[_0x24cbd0('0x176')](function(_0x17f03c){var _0x48f115=_0x24cbd0;_0x17f03c['preventDefault'](),_0x45183c[_0x48f115(0x192)]();}),$('#feedbackLink')[_0x24cbd0(0x176)](function(_0xc3a471){var _0x3714c9=_0x24cbd0;_0xc3a471[_0x3714c9('0x185')](),_0x45183c['getFeedback']();});}());
</script>
