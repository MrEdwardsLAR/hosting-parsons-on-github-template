<div id="PP1-sortableTrash" class="sortable-code"></div> 
<div id="PP1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="PP1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="PP1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "name = &quot;Bob&quot;\n" +
    "print(&quot;Hello&quot; + name)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "PP1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#PP1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#PP1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

<div id="pp2-sortableTrash" class="sortable-code"></div> 
<div id="pp2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="pp2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="pp2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def sumNum(number1, number2):\n" +
    "	sum = number1, number2)\n" +
    "    return sum";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "pp2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#pp2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#pp2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
