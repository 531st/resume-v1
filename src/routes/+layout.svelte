<script>
</script>

<body>
    <div class="main-container">
        <slot />
    </div>
    
</body>


<style>
    body {
        margin: 0;
        display: block; gap: 0px;
        overflow: hidden;
    }

   
    ::-webkit-scrollbar {
        width: 0;  /* Remove scrollbar space */
        background: transparent;  /* Optional: just make scrollbar invisible */
    }
    /* Optional: show position indicator in red */
    ::-webkit-scrollbar-thumb {
        background: #FF0000;
    }

    .main-container {
        min-height: 98.5vh;
        min-width: 60vh;
        padding: 5px 5px 5px 5px;
        background: rgb(32,32,32);
        background: radial-gradient(circle, rgba(32,32,32,1) 0%, rgba(16,16,16,1) 95%);    
        font-family: 'Oswald', sans-serif; 
        position: relative;
        display: flex;
        flex-direction: column;
        align-content: center;
    }

</style>