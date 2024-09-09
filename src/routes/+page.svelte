<script>
    import 'adorable-css';
    import svelteLogo from "$lib/favicon.png";

    let count = 0;
    let menu_items = ['Home','About'];
    
    const handleClick = () => {
        count += 1;
    }
</script>

<div class="w(100vw) h(9vh) bg(#0080ff.5) fixed(0,0) text(left) hbox gap(20)"
    style="backdrop-filter:blur(10px)">
    <div class="w(100vw) h(3vh) bg(#1074a8.5) text(center) layer(top)">🚨개발중인 사이트입니다.🚨</div>
    <img src={svelteLogo} alt="로고" class="w(7vh) h(7vh) ml(2.5vw) inline-block">
    <h1 class="font(1.9vw) inline-block hover:font(2vw) transition(.5s) bold">SVELTE</h1>
    {#each menu_items as item}
        <h1 class="font(1.3vw) inline-block hover:font(1.4vw) transition:(.5s)">{item}</h1> 
    {/each}

</div>
<div class="w(100vw) mt(12vh)">
    <button on:click={handleClick} clas="bg(gray)">이 버튼은 {count}번 눌린 버튼입니다.</button>
    <p>Test<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>Test</p>
</div>


<style>

</style>