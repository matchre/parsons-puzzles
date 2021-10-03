<div id="sortableTrash" class="sortable-code"></div> 
<div id="sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="feedbackLink" value="Get Feedback" type="button" /> 
    <input id="newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def moyenne(ma_liste):\n" +
    "    # On vérifie que l&#039;argument est bien une liste.\n" +
    "    assert(isinstance(ma_liste, list)), &quot;Il n&#039;y a pas de liste !&quot;\n" +
    "    # On vérifie que la liste n&#039;est pas vide.\n" +
    "    assert(len(ma_liste) != 0), &quot;La liste est vide !&quot;\n" +
    "    # On vérifie que tous les éléments de la liste sont bien des nombres.\n" +
    "    for elem in ma_liste:\n" +
    "        assert(isinstance(elem, int) or isinstance(elem, float)), &quot;Un élément n&#039;est pas un nombre !&quot;\n" +
    "    # Le calcul de la moyenne en lui-même\n" +
    "    somme = 0\n" +
    "    for i in range(0, len(ma_liste)):\n" +
    "        somme = somme + ma_liste[i]\n" +
    "    return somme/len(ma_liste)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en"
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
