# jquery

## for finding the id of the row that input is checked in an iframe table
```
$(document).ready(function() {
  $("#select_Contact").on("click", function() {
    let contactid = "";
  $('table tr:not(:first):has(input:checked)',iframe.document).each(function(){
          contactid += $(this).find('td:eq(1)').text() + " " ;    
    });
    console.log(contactid)
    $("#field8").val(contactid);
  });
});
```
