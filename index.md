# Japan Pics

<button id='foodbutton'>Hide Food Pics</button>

<div class='foodpics'>
Test
</div>




<script>
 // If I were the code reviewer and not the author, I would not approve inline js
 // jQuery is there, why not use it?
 $().ready(function () {
    const foodButton = document.getElementById('foodbutton');
    const hideFoodText = "Hide Food Pics";
    const showFoodText = "Show Food Pics";

    function pressFoodButton() {
      if (foodButton.innerText === hideFoodText) {
        foodButton.innerText = showFoodText;
        $('.foodpics').hide();
      }
      else {
        foodButton.innerText = hideFoodText;
        $('.foodpics').show();
      }
    }
  
    foodButton.addEventListener('click', pressFoodButton);
  
 });
</script>
