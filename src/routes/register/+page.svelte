<script>
	import { prevent_default } from "svelte/internal";



  let formcenter;

  let first;

  let card1;

  let card2;

  function change() {
    card1.style.display="none"
    card2.style.display="flex"
  }

  function submit(){

  }



// const form = document.getElementById('formcenter');


// let field = document.getElementById('calendar');

// Handle date changes
// field.addEventListener('input', function () {

//   // Get the date
//   let date = new Date(`${field.value}T00:00`);
//   console.log(date);
//   requested = field.value;
  
// });

// const button = document.getElementById('first');

// button.addEventListener('click', (e) => {

//     e.preventDefault();
//     document.getElementById("card1").style.display="none";
//     document.getElementById("card2").style.display="flex";
//   // console.log(values);

// });

// form.addEventListener('submit', (e) => {
  
//   e.target.submit();

// });





</script>


<form bind:this={formcenter} id="formcenter" class="formcenter center" action="/register" method="POST">

    <div bind:this={card1} id="card1">
      <h2 class="jp-titles jpform">クラスを選んで下さい</h2>
        <div class="selectors">
          <ul class="formbuttons class-cards">
            <li>
              <input type="radio" id="check_1" name="classesChecked" value="kidsルーム">
              <label class="prevent-select" for="check_1">Kidsルーム</label>
            </li>
            <li>
              <input type="radio" id="check_2" name="classesChecked" value="aルーム">
              <label class="prevent-select" for="check_2">Aルーム</label>
            </li>
            <li>
              <input type="radio" id="check_3" name="classesChecked" value="bルーム">
              <label class="prevent-select" for="check_3">Bルーム</label>
            </li>
            <li>
              <input type="radio" id="check_4" name="classesChecked" value="cルーム">
              <label class="prevent-select" for="check_4">Cルーム</label>
            </li>
          </ul>
        </div>

        <h2 class="jp-titles jpform">ご希望の日付を選んで下さい</h2>

        <input type="date" id="calendar" class="calendar jp " name="calendar" placeholder="MM/DD/YYYY" required>

        <p class="jp jpform">メール</p>
            <input id="email" class="email jp" autocomplete="off"  placeholder="メール" type="email" name="email">
      
        <p class="jp jpform">名前</p>
            <input id="name" class="email jp" autocomplete="off"  placeholder="名前" type="text" name="name">
      
        <button bind:this={first} on:click={change} class="btn-primary jp" type="button" id="first">登録</button>
    </div>

    <div bind:this={card2} id="card2" class="thanks">
      <h1>確認</h1>
      
      <p class="selection"> Thank you,&nbsp;<span class="spanColor" id="selection4"> PLACEHOLDER </span>. You have selected&nbsp;<span class="spanColor" id="selection1"> PLACEHOLDER </span>.</p>
      
      <p class="text">We look forward to seeing you on&nbsp;<span class="spanColor" id="selection2"> PLACEHOLDER </span>.</p>
    
      <p>Please click confirm and we'll send you an email at&nbsp;<span class="spanColor" id="selection3"> PLACEHOLDER </span>.</p>
    
      <button on:click={submit} class="btn-primary jp confirm" type="submit">確認
      </button>
      
    
    </div>

</form>

<style>
  .thanks{
    display: none;
    flex-direction: column;
    align-content: center;
}
</style>

