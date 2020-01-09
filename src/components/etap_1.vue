<template>
    
    <div id="form">
        <h1>Wyślij swoją propozycję tematu</h1>
        <p>Zbieramy propozycje tematów na najbliższą edycję konkursu. Jeśli chcesz, możesz dodać swoją propozycję poniżej:</p>
        <form action="julia.warakomska1a@gmail.com" method="post">
            <input type="text" name="wpisz_temat">Wpisz swoją propozycję...
            <input type="submit" value="Wyślij">
        </form>
    </div>
</template>

<script>
export default {
    name:"etap_1"
}
</script>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');
    #etap_1{
        width: 100vw;
        display: flex;
        flex-direction: column;
        font-family: "Lato";
        text-align:center;
        text-transform:uppercase;
        }

    h1 {
        font-size: 4em;
        color:#f4c621;
    }

    p {
        font-family: "Lato";
        text-align:center;
        color:#aeaeae;
        font-size:2.5em;
    }

    form {
        font-family: "Lato";
        text-align:center;
        color:#aeaeae;
    }
    #wpis {
        color:#f4c621;
        font-size:2em;
        outline:none;
        width:25em;
        height:2.1em;
        border:none;
    }

    input {
        font-family: "Lato";
        text-align:center;
    }
</style>