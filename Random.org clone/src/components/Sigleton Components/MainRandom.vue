<template>
    <div class="advisory">
        <b>Advisory:</b> We only operate services from the RANDOM.ORG domain. Other sites that claim to be operated by us are impostors. If in doubt, <a href="mailto:contact@random.org">contact us</a>.
    </div>
    <main>
        <div class="main-text">
            <h2>What's this fuss about <em>true</em> randomness?</h2>
            <div class="paragraphs-and-generator-container">
                <div class="paragraphs-container">
                    <p>
                        Perhaps you have wondered how predictable machines like
                        computers can generate randomness.  In reality, most random numbers
                        used in computer programs are <em>pseudo-random</em>, which means they
                        are generated in a predictable fashion using a mathematical
                        formula.  This is fine for many purposes, but it may not be random
                        in the way you expect if you're used to dice rolls and lottery drawings.
                    </p>
                    <p>
                        RANDOM.ORG offers <em>true</em> random numbers to anyone on
                        the Internet.  The randomness comes from atmospheric noise, which
                        for many purposes is better than the pseudo-random number
                        algorithms typically used in computer programs.  People use RANDOM.ORG for holding drawings, lotteries and sweepstakes, to drive online games, for scientific applications and for art and music.
                        The service has existed since 1998 and was built by <a href="https://www.random.org/mads/">Dr Mads Haahr</a> of the <a href="http://www.scss.tcd.ie/">School of Computer Science
                        and Statistics</a> at <a href="http://www.tcd.ie/">Trinity College,
                        Dublin</a> in Ireland.  Today, RANDOM.ORG is operated by <a href="https://www.random.org/company/">Randomness and Integrity Services Ltd</a>.
                    </p>
                </div>
                <RandomNumberGenerator/>
            </div>            
        </div>
    </main>
</template>

<script>
import RandomNumberGenerator from './RandomNumberGenerator.vue';

    export default{
        data(){
            return{

            }
        },
        components:{RandomNumberGenerator}
    }
</script>

<style scoped>
    .advisory{
        font-size: 0.82rem;
        background-color: #FFFF90;
        padding: 6px;
    }

    h2{
        color: #6F6FC4;
        font-weight: 400;
        font-family: 'Times New Roman', Times, serif;
        font-size: 1.6rem
    }

    .paragraphs-and-generator-container{
        margin-top: 0;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .paragraphs-container{
        width: 600px;
        font-size: 0.82rem;
        line-height: 22px;

        p{
            a{
                color:#6F6FC4;
            }

            &:first-child{
                margin-top: 0;
            }
        }
    }
</style>