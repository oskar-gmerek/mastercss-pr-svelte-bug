<script>
    import blackongreen from '$lib/images/blackongreen.png'
</script>

<h1 class="font:40  font:heavy italic m:50 text:center ">BLACK text on GREEN background</h1>


<div class="flex gap:30 jc:center">


        
        <a href="/whiteonblue"  class="bg:white p:30 fg:blue f:heavy r:100 capitalize">Go to WHITE text on BLUE background</a>

    

        
        <a href="/blueonyellow"  class="fg:blue p:30 bg:yellow-70 f:heavy r:100 capitalize">Go to BLUE text on YELLOW background</a>
        <a href="/blackongreen"  class="fg:blue p:30 bg:yellow-70 f:heavy r:100 capitalize">Go to BLACK text on GREEN background (like this)</a>

</div>

<div class="flex flex:column jc:center w:500 b:3|solid|red">
    <h2 class="@fade|1s|infinite">SCREENSHOT OF CORRECT STYLES  (CURRENT PAGE)</h2>
    
    <img src={blackongreen}>
</div>