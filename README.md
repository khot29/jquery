# jquery

## for finding the id of the row that input is checked in an iframe table
```
 $("#select_Contact").on("click", function() {
    let contactid = "";
  $('table tr:not(:first):has(input:checked)',iframe.document).each(function(){
          contactid += $(this).find('td:eq(1)').text() + " " ;    
    });
    $("#field8").val(contactid.split(' ').slice(0,-1).join(','));
  });
```
