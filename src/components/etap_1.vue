<template>
    
    <div id="container">
    <div id="box">
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
                <button>Wyślij</button>
            </div>
            </form>
        </div>
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
        height: 100vh;
        display: flex;
        flex-direction: column;
        align-items: center;
        font-family: "Lato";
        text-transform:uppercase;
        background-color: #1e000e;

        #box{
            width:  50vw;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;


        #title{
            height: 10vh;
            font-size: 3em;
            color:#f4c621;
            display:flex;
            justify-content: flex-start;
            align-items: center;
            font-weight: 900;
        }

        #text{
            color:#aeaeae;
            height: 20vh;
            font-size:2em;
            display:flex;
            justify-content: flex-start;
            align-items: center;
        }

        #form{
            color:#aeaeae;
            display:flex;
            justify-content: flex-start;
            align-items: center;
            height: 20vh;

                #subject{
                    width: 25vw;
                    height: 5vh;
                    border-radius: 10px;
                    background-color: #110008;
                    
                    
                    

                        input{
                            margin: 0;
                            padding: 0;
                            padding-left:0.5vw;
                            border: none;
                            outline: none;
                            width:100%;
                            height: 100%;
                            background:none;
                            font-size:1.2vw;
                            font-family: "Lato";
                            color:#aeaeae;
                        }
                    }
                #send{
                    button{
                    margin-top:3vh;
                    width: 12.5vw;
                    height: 5vh;
                    border-radius: 10px;
                    font-size:2.5vh;
                    font-weight: 900;
                    font-family:"Lato";
                    border:none;
                    outline:none;
                    background-color: #f4c621;
                    color:#1e000e;
                    
                    }
                }
                
            }
        }
    }
</style>