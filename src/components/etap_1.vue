<template>
    
    <div id="container">
        <div id="title">
            Wyślij swoją propozycję tematu
        </div>
        <div id="text">
            Zbieramy propozycje tematów na najbliższą edycję konkursu. Jeśli chcesz, możesz dodać swoją propozycję poniżej:
        </div>
        <div id="form">
            <form>
            <div id="subject">
                <input type="text" name="subject" placeholder="Wpisz swoją propozycję...">
            </div>
            <br>
            <div id="send">
                <input type="submit" value="Wyślij">
            </div>
            </form>
        </div>
    </div>     
</template>

<script>
export default {
    name:"etap_1"
}
</script>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');
    #container{
        width: 100vw;
        display: flex;
        justify-content: flex-start;
        flex-direction: column;
        font-family: "Lato";
        text-transform:uppercase;

    #title{
        width: 100%;
        height: 8rem;
        font-size: 4em;
        color:#f4c621;
        display:flex;
        justify-content: center;
        align-items: center;
    }

    #text{
        color:#aeaeae;
        font-size:2.5em;
    }

    #form{
        color:#aeaeae;
        display:flex;
        flex-direction: column;
        justify-content: flex-start;

            #subject{
                width: 50rem;
                height: 7rem;
                border-radius: 10px;
                background-color: #f4c621;

                    input{
                        margin: 0;
                        padding: 0;
                        border: none;
                        outline: none;
                        width:100%;
                        height: 100%;
                        background:none;
                    }
            #send{
                width: 21rem;
                height: 7rem;
                border-radius: 10px;
                background-color: #f4c621;
                color:black;

                    input{
                        margin: 0;
                        padding: 0;
                        border: none;
                        outline: none;
                        width:100%;
                        height: 100%;
                        background:none;
                        }
                }
            }
        }
    }
</style>