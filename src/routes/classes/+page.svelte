<div class="main-container">
    <h1 class="center jp eventHeader">選択クラス</h1>
    <div bind:this={tabList} class="flex class-cards" role="tablist" aria-label="class list">
      <div>
        <button
          on:click={switch1}
          bind:this={tab1}
          aria-selected="true"
          class="class orange"
          aria-controls="kids-tab"
          role="tab"
        >
        </button>
        <p on:keypress={switch1}
        bind:this={tab1} class="sr-only" tabindex="-1">Slider title</p>
        <p class="class-names">プレキッズ</p><br />
        <p class="subtext">年小</p>
      </div>
      <div>
        <button
          on:click={switch2}
          bind:this={tab2}
          aria-selected="true"
          class="class orange"
          aria-controls="kids-tab"
          role="tab"
        >
        </button>
        <p on:keypress={switch2}
        bind:this={tab2} class="sr-only" tabindex="-1">Slider title</p>
        <p class="class-names">キッズクラス</p><br />
        <p class="subtext">年中•年長</p>
      </div>
      <div>
        <button
          on:click={switch3}
          bind:this={tab3}
          aria-selected="true"
          class="class orange"
          aria-controls="kids-tab"
          role="tab"
        >
        </button>
        <p on:keypress={switch3}
        bind:this={tab3} class="sr-only" tabindex="-1">Slider title</p>
        <p class="class-names">ジュニアーキッズクラス</p><br />
        <p class="subtext">年中•年長</p>
      </div>
      <div>
        <button
          on:click={switch4}
          bind:this={tab4}
          aria-selected="true"
          class="class orange"
          aria-controls="kids-tab"
          role="tab"
        >
        </button>
        <p on:keypress={switch4}
        bind:this={tab4} class="sr-only" tabindex="-1">Slider title</p>
        <p class="class-names">ジュニアーAクラス</p><br />
        <p class="subtext">年中•年長</p>
      </div>
      <div>
        <button
          on:click={switch5}
          bind:this={tab5}
          aria-selected="true"
          class="class orange"
          aria-controls="kids-tab"
          role="tab"
        >
        </button>
        <p on:keypress={switch5}
        bind:this={tab5} class="sr-only" tabindex="-1">Slider title</p>
        <p class="class-names">ジュニアーBクラス</p><br />
        <p class="subtext">年中•年長</p>
      </div>
      <div>
        <button
          on:click={switch6}
          bind:this={tab6}
          aria-selected="true"
          class="class orange"
          aria-controls="kids-tab"
          role="tab"
        >
        </button>
        <p on:keypress={switch6}
        bind:this={tab6} class="sr-only" tabindex="-1">Slider title</p>
        <p class="class-names">ジュニアーCクラス</p><br />
        <p class="subtext">年中•年長</p>
      </div>


      
      
    </div>

    <article
      bind:this={panel1}
      class="class-container"
      id="kids-tab"
      role="tabpanel"
      tabindex="0"
    >
      <h1>Example 1</h1>
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Delectus
        praesentium, tenetur doloremque cupiditate aut exercitationem
        blanditiis sunt inventore magnam maxime laboriosam, deserunt officia
        ipsam quis earum? Natus, iusto vero. Architecto?
      </p>
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Delectus
        praesentium, tenetur doloremque cupiditate aut exercitationem
        blanditiis sunt inventore magnam maxime laboriosam, deserunt officia
        ipsam quis earum? Natus, iusto vero. Architecto?
      </p>
    </article>
    <article
      hidden
      bind:this={panel2}
      class="class-container"
      id="a-tab"
      role="tabpanel"
      tabindex="0"
    >
      <h1>Example 2</h1>
      <p>
        This is an example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
      <p>
        This is an example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
    </article>
    <article
      hidden
      bind:this={panel3}
      class="class-container"
      id="b-tab"
      role="tabpanel"
      tabindex="0"
    >
      <h1>Example 3</h1>
      <p>
        Another example Lorem ipsum dolor sit, amet consectetur adipisicing
        elit. Delectus praesentium, tenetur doloremque cupiditate aut
        exercitationem blanditiis sunt inventore magnam maxime laboriosam,
        deserunt officia ipsam quis earum? Natus, iusto vero. Architecto?
      </p>
      <p>
        Another example Lorem ipsum dolor sit, amet consectetur adipisicing
        elit. Delectus praesentium, tenetur doloremque cupiditate aut
        exercitationem blanditiis sunt inventore magnam maxime laboriosam,
        deserunt officia ipsam quis earum? Natus, iusto vero. Architecto?
      </p>
    </article>
    <article
      hidden
      bind:this={panel4}
      class="class-container"
      id="c-tab"
      role="tabpanel"
      tabindex="0"
    >
      <h1>Example 4</h1>
      <p>
        Yet another example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
      <p>
        Yet another example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
    </article>
    <article
      hidden
      bind:this={panel5}
      class="class-container"
      id="c-tab"
      role="tabpanel"
      tabindex="0"
    >
      <h1>Example 5</h1>
      <p>
        Yet another example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
      <p>
        Yet another example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
    </article>
    <article
      hidden
      bind:this={panel6}
      class="class-container"
      id="c-tab"
      role="tabpanel"
      tabindex="0"
    >
      <h1>Example 6</h1>
      <p>
        Yet another example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
      <p>
        Yet another example Lorem ipsum dolor sit, amet consectetur
        adipisicing elit. Delectus praesentium, tenetur doloremque
        cupiditate aut exercitationem blanditiis sunt inventore magnam
        maxime laboriosam, deserunt officia ipsam quis earum? Natus, iusto
        vero. Architecto?
      </p>
    </article>
</div>

<script>
  let tabList;
  let tab1;
  let tab2;
  let tab3;
  let tab4;
  let tab5;
  let tab6;
  let panel1;
  let panel2;
  let panel3;
  let panel4;
  let panel5;
  let panel6;


  function switch1(){
    panel1.removeAttribute("hidden");
    panel2.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
    panel5.setAttribute('hidden', true);
    panel6.setAttribute('hidden', true);
  }
  function switch2(){
    panel2.removeAttribute("hidden");
    panel1.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
    panel5.setAttribute('hidden', true);
    panel6.setAttribute('hidden', true);
  }
  function switch3(){
    panel3.removeAttribute("hidden");
    panel2.setAttribute('hidden', true);
    panel1.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
    panel5.setAttribute('hidden', true);
    panel6.setAttribute('hidden', true);
  }
  function switch4(){
    panel4.removeAttribute("hidden");
    panel1.setAttribute('hidden', true);
    panel2.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel5.setAttribute('hidden', true);
    panel6.setAttribute('hidden', true);
  }
  function switch5(){
    panel5.removeAttribute("hidden");
    panel1.setAttribute('hidden', true);
    panel2.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
    panel6.setAttribute('hidden', true);
  }
  function switch6(){
    panel6.removeAttribute("hidden");
    panel1.setAttribute('hidden', true);
    panel2.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel5.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
  }
 
</script>