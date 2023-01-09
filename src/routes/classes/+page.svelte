<div class="main-container">
    <h1 class="center jp eventHeader">選択クラス</h1>
    <div bind:this={tabList} class="flex class-cards" role="tablist" aria-label="class list">
      <button
        on:click={switch1}
        bind:this={tab1}
        aria-selected="true"
        class="class orange"
        aria-controls="kids-tab"
        role="tab"
      >
        <span class="sr-only" tabindex="-1">Slider title</span>
        <span class="class-names">Kidsルーム</span><br />
        <span class="subtext">年中•年長</span>
      </button>
      <button
      bind:this={tab2}
      on:click={switch2}
        aria-selected="false"
        class="class yellow"
        aria-controls="a-tab"
        role="tab"
      >
        <span class="sr-only" tabindex="-1">Slider title</span>
        <span class="prevent-select class-names">Aルーム</span><br />
        <span class="prevent-select subtext">小学１•２年生</span>
      </button>
      <button
      bind:this={tab3}
      on:click={switch3}
        aria-selected="false"
        class="class green"
        aria-controls="b-tab"
        role="tab"
      >
        <span class="sr-only" tabindex="-1">Slider title</span>
        <span class="class-names">Bルーム</span><br />
        <span class="subtext">小学３•４年生</span>
      </button>
      <button
      bind:this={tab4}
      on:click={switch4}
        aria-selected="false"
        class="class blue"
        aria-controls="c-tab"
        role="tab"
      >
        <span class="sr-only" tabindex="-1">Slider title</span>
        <span class="class-names">Cルーム</span><br />
        <span class="subtext">小学５•６年生</span>
      </button>
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
</div>

<script>
  let tabList;
  let tab1;
  let tab2;
  let tab3;
  let tab4;
  let panel1;
  let panel2;
  let panel3;
  let panel4;


  function switch1(){
    panel1.removeAttribute("hidden");
    panel2.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
  }
  function switch2(){
    panel2.removeAttribute("hidden");
    panel1.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
  }
  function switch3(){
    panel3.removeAttribute("hidden");
    panel2.setAttribute('hidden', true);
    panel1.setAttribute('hidden', true);
    panel4.setAttribute('hidden', true);
  }
  function switch4(){
    panel4.removeAttribute("hidden");
    panel1.setAttribute('hidden', true);
    panel2.setAttribute('hidden', true);
    panel3.setAttribute('hidden', true);
  }
 
</script>