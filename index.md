# Japan Pics

<button id='foodbutton'>Hide Food Pics</button>

<div class='food'>
Test
</div>




<script>
 # If I were the code reviewer and not the author, I would not approve inline js
 (function () {
    const foodButton = document.getElementById('foodbutton');

    function pressFoodButton() {
      console.log('hi')
    }
  
    foodButton.addEventListener('click', pressFoodButton);
  
 })();
</script>
