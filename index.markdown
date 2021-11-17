<div id="nnn-sortableTrash" class="sortable-code"></div> 
<div id="nnn-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="nnn-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="nnn-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "s=0\n" +
    "for i in range(2):\n" +
    "	s=s+i\n" +
    "print(s)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "nnn-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.VariableCheckGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "vartests": [
        {
            "message": "",
            "initcode": "",
            "code": "",
            "variables": {
                "s": 2
            }
        },
        {
            "message": "",
            "initcode": "",
            "code": "",
            "variables": {}
        }
    ]
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#nnn-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#nnn-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
