<template>
  <div class="home">
    <div class="container">
      <div class="paginate">

            <nav aria-label="Page navigation" v-if="!search">
                <ul class="pagination justify-content-center">
                    
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">A</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">B</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">C</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">D</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">E</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">F</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">G</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">H</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">I</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">J</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">K</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">L</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">M</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">N</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">O</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">P</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">Q</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">R</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">S</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">T</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">U</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">V</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">W</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">X</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">Y</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" href="#">Z</a></li>
                    
                </ul>
            </nav>

        </div>

       
      
       
        <div class="mb-4 sticky-top">
             
             <input class="form-control" aria-label="Search" type="text" v-model="search" placeholder="search...">
       
        </div>
        
      
        <div>

            <ul class="list-group" v-bind:key="vocabulary.id" v-for="vocabulary in filterVocabularies">
                <li class="list-group-item bg-secondary">
                    <router-link class="text-white" :to="{ name: 'vocabulary', params: { vocabulary: vocabulary }}">
                        {{ vocabulary.word }}
                    </router-link>
                </li>
                
                <!-- <Vocabulary v-bind:vocabulary="vocabulary"/> -->
            </ul>
        </div>

        

    </div>
  </div>
</template>

<script>
// @ is an alias to /src

//import Vocabularies from '../components/Vocabularies.vue' 
import Vocabulary from './Vocabulary.vue'

export default {

  name: "home",

  components: {
    Vocabulary
  },

  data() {
    
    return{
      
      search:"",

      vocabularies:[
        {
          "word": "As ugly as sin", 
          "synonym": "", 
          "example": "Have you seen the new neighbour's dog? It's as ugly as sin!", 
          "video": ""
          }, 
          {
          "word": "At daggers drawn", 
          "synonym": "", 
          "example": "The two sides have been at daggers drawn for some months now with no sign of improvements in relations.", 
          "video": "https://www.youtube.com/embed/zpKDSlvNqpU"
          },
          {
          "word": "Curb", 
          "synonym": "Edge, Bent, Crooked, Curved", 
          "example": "Dean pulled away from the curb, keeping his speed to a parade crawl.", 
          "video": "https://www.youtube.com/embed/KfqqdLnWKW4?t=5s"
          }, 
          {
          "word": "Curd", 
          "synonym": "Clot, Clump, Lump", 
          "example": "In curd soaps, however, which form the basis of most household soap, the uncombined alkali and the glycerin are separated by  'salting out,' and the soap in this condition contains about 30% of water.", 
          "video": "https://www.youtube.com/embed/kRb3hKlpiYk?t=5s"
          }, 
          {
          "word": "Curdle", 
          "synonym": "Solidify, Thicken, Clot", 
          "example": "Take care not to let the soup boil or it will curdle.", 
          "video": "https://www.youtube.com/embed/dsFsoay"
          }, 
          {
          "word": "Cure somebody of something", 
          "synonym": "", 
          "example": "I ate so many sweets that day that I was cured of my sugar craving for months.", 
          "video": ""
          }, 
          {
          "word": "Curfew", 
          "synonym": "Time limit, Check in time, Late hour", 
          "example": "Sally's parents are so laid back, they haven't even given her a curfew on school nights.", 
          "video": "https://www.youtube.com/embed/dgRkUvCa6mc"
          }, 
          {
          "word": "Curio", 
          "synonym": "Bauble, Curiosity, Knickknack", 
          "example": "Be careful of the fragile curios on the end tables.", 
          "video": "https://www.youtube.com/embed/Wh5yheDDkBA"
          }, 
          {
          "word": "Curiosity killed the cat", 
          "synonym": "", 
          "example": ": I know curiosity killed the cat, but I can't stop the investigation until I know where the donations are really going.", 
          "video": "https://www.youtube.com/embed/8BYFzVTI1"
          }, 
          {
          "word": "Curiosity killed the cat", 
          "synonym": "Inquiring, Curios, Inquisitive.", 
          "example": "I know curiosity killed the cat, but I can't stop the investigation until I know where the donations are really going.", 
          "video": "https://www.youtube.com/embed/8BYFzVTI1"
          }, 
          {
          "word": "Curl up and die", 
          "synonym": "Ashamed, Embarrassed, Awkard", 
          "example": "If I don't get asked to the prom, I'll be so embarrassed that I might as well just curl up and die!", 
          "video": ""
          }, 
          {
          "word": "Curl up", 
          "synonym": "Edges, Rounded, Border", 
          "example": "If something flat, such as paper, curls up, the edges start to become rounded.", 
          "video": "https://www.youtube.com/embed/LHHFl2VqBNE"
          }, 
          {
          "word": "Curl up", 
          "synonym": "Position, Hug, Snuggle", 
          "example": "We sat curled up on the sofa, watching the late film.", 
          "video": "https://www.youtube.com/embed/LHHFl2VqBNE"
          }, 
          {
          "word": "Curl your lip", 
          "synonym": "Annoyed, Disgusted, Bored", 
          "example": "Don't you curl your lip at me! I did nothing wrong here!", 
          "video": ""
          }, 
          {
          "word": "Curlew", 
          "synonym": "Albatross, Seagull", 
          "example": "A curlew flew past me, borne out of the darkness, and its cry made me feel sad and shiver.", 
          "video": "https://www.youtube.com/embed/J0g8xZycyvA"
          }, 
          {
          "word": "Curling", 
          "synonym": "Bending, Crooked, Curved", 
          "example": "A curling labyrinth designed to discourage grave robbers from ever finding the inner burial chamber.", 
          "video": "https://www.youtube.com/embed/IWxeuWY"
          }, 
          {
          "word": "Curmudgeon", 
          "synonym": "Complainer, Crank, Fusser, Grouch", 
          "example": "Only a curmudgeon would object to the nursing home's holiday decorations.", 
          "video": "https://www.youtube.com/embed/1tW4jnycsJY"
          }, 
          {
          "word": "Currant", 
          "synonym": "Gooseberry, Berry", 
          "example": "Pour the currant sauce over the dish, garnish with the fresh oregano or parsley, and serve.", 
          "video": "https://www.youtube.com/embed/XdIzOy3NUog"
          }, 
          {
          "word": "Currawong", 
          "synonym": "Bell magpie, Wild birds", 
          "example": "However, it can be encountered in mixed", 
          "video": "https://www.youtube.com/embed/BzyKGZZpryw"
          }, 
          {
          "word": "Currency", 
          "synonym": "Acceptance, Popularity", 
          "example": "His ideas enjoyed wide currency during the last century.", 
          "video": "https://www.youtube.com/embed/J5GcrNvW69A"
          }, 
          {
          "word": "Currency", 
          "synonym": "Money, Foreign currency", 
          "example": "Five people were indicted for making and selling counterfeit currency.", 
          "video": "https://www.youtube.com/embed/J5GcrNvW69A"
          }, 
          {
          "word": "Current", 
          "synonym": "Mood, Feelings, Spirits", 
          "example": "A strong current of nationalism is running through the country.", 
          "video": "https://www.youtube.com/embed/QzHFNp_I5BM?t=3s"
          }, 
          {
          "word": "Current", 
          "synonym": "Steady flow, Stream, Airstream", 
          "example": "Ocean currents.", 
          "video": "https://www.youtube.com/embed/QzHFNp_I5BM?t=3s"
          }, 
          {
          "word": "Curry favor", 
          "synonym": "Butter up, Sweet talk", 
          "example": "Flattery won't work; the only way of currying favor with him is through hard work.", 
          "video": "https://www.youtube.com/embed/DOWz"
          }, 
          {
          "word": "Curry", 
          "synonym": "Food seasoning, Sauce, Condaminent, Relish", 
          "example": "Sarah makes amazing fish curry.", 
          "video": "https://www.youtube.com/embed/No5yizQVxt4?t=5s"
          }, 
          {
          "word": "Curry", 
          "synonym": "Prepare, Clean, Comb, Powder, Groom", 
          "example": "She took the currycomb from the wall and began grooming Princess.", 
          "video": "https://www.youtube.com/embed/No5yizQVxt4?t=5s"
          }, 
          {
          "word": "Curse", 
          "synonym": "Blood, Period, Mensuration", 
          "example": "Even the curse seemed to wrap about her like some trailing sable robe.", 
          "video": "https://www.youtube.com/embed/_g9fcWIDwH4?t=5s"
          }, 
          {
          "word": "Curse", 
          "synonym": "Damnation, Speak angrily, Swear word", 
          "example": "At every blow there was a curse.", 
          "video": "https://www.youtube.com/embed/_g9fcWIDwH4?t=5s"
          }, 
          {
          "word": "Curse", 
          "synonym": "Trouble, Unhappiness", 
          "example": "Noise is the curse of modern city life.", 
          "video": "https://www.youtube.com/embed/_g9fcWIDwH4?t=5s"
          }, 
          {
          "word": "Curse", 
          "synonym": "Voodoo, The evil eye, Magic, Hex", 
          "example": "Things were going so badly", 
          "video": "https://www.youtube.com/embed/_g9fcWIDwH4?t=5s"
          }, 
          {
          "word": "Cursory", 
          "synonym": "Careless, Brief, Rapid, Casual", 
          "example": "I gave the letter a fairly cursory reading.", 
          "video": "https://www.youtube.com/embed/E6YmLdxMnrk"
          }, 
          {
          "word": "Curt", 
          "synonym": "Rude, Blunt, Sharp, Short", 
          "example": "'The matter is closed,' was his curt reply.", 
          "video": "https://www.youtube.com/embed/cPBTdN8Z3n8?t=6s"
          }, 
          {
          "word": "Curtail", 
          "synonym": "Lessen, reduce.", 
          "example": "Civil liberties were further curtailed", 
          "video": ""
          }, 
          {
          "word": "Curtain call", 
          "synonym": "", 
          "example": "After Mary walks off the set and the lights dim, the cast returns for a curtain call.", 
          "video": "https://www.youtube.com/embed/HWBkxY4i9Zk"
          }, 
          {
          "word": "Curtsy", 
          "synonym": "Salute, bow.", 
          "example": "When a girl or woman curtsies, she bends quickly at the knees, with one foot in front of the other, often while holding her skirt, especially to show respect.", 
          "video": ""
          }, 
          {
          "word": "Curvature", 
          "synonym": "Curve, arc.", 
          "example": "At any point a sounding line would hang in the line of the radius of curvature of the water surface.", 
          "video": "https://www.youtube.com/embed/HVDpPNCKSjU"
          }, 
          {
          "word": "Cushion of air", 
          "synonym": "", 
          "example": "A hovercraft travels on a cushion of air.", 
          "video": ""
          }, 
          {
          "word": "Cushion the blow", 
          "synonym": "", 
          "example": "He's lost his job, but the redundancy money will cushion the blow.", 
          "video": ""
          }, 
          {
          "word": "Cushy", 
          "synonym": "Comfortable, easy.", 
          "example": "The work at a call centre is not a cushy job.", 
          "video": "https://www.youtube.com/embed/QuwKLowI"
          }, 
          {
          "word": "Cusp", 
          "synonym": "Variation,  distinction.", 
          "example": "Molars with quadrate crowns and a blunt conical cusp at each corner, the last notably smaller than the rest, sometimes rudimentary or absent.", 
          "video": "https://www.youtube.com/embed/8YyxR6KLIao from 0:16"
          }, 
          {
          "word": "Cuss", 
          "synonym": "Profane, expletive.", 
          "example": "An example of a cuss is the word 'hell'.", 
          "video": "https://www.youtube.com/embed/RZxkkHpWalE"
          }, 
          {
          "word": "Custodial sentence", 
          "synonym": "Imprison, jail.", 
          "example": "Custodial sentences may only be imposed on adults who have committed an indictable offence.", 
          "video": "https://www.youtube.com/embed/1fwRRU"
          }, 
          {
          "word": "Custodian", 
          "synonym": "Caretaker, guardian.", 
          "example": "Arakcheev was a faithful custodian to enforce order and acted as the sovereign's bodyguard.", 
          "video": "https://www.youtube.com/embed/Am2Fmi_OJPU  up to 0:10 second"
          }, 
          {
          "word": "Custom", 
          "synonym": "Business, trade.", 
          "example": "You have the right to withhold your custom if you so wish.", 
          "video": "https://www.youtube.com/embed/MXqaGR3Dd28"
          }, 
          {
          "word": "Custom", 
          "synonym": "Convention, tradition.", 
          "example": "It is the custom for the bride to wear a white dress on her wedding day.", 
          "video": "https://www.youtube.com/embed/MXqaGR3Dd28  up to 0:15 second"
          }, 
          {
          "word": "Custom", 
          "synonym": "Corporation tax, tax credit.", 
          "example": "Going through the customs at the airport is sometimes tiresome.", 
          "video": "https://www.youtube.com/embed/MXqaGR3Dd28 from 0:30 second"
          }, 
          {
          "word": "Custom", 
          "synonym": "Innovate, design.", 
          "example": "She ordered for a custom", 
          "video": ""
          }, 
          {
          "word": "Custom", 
          "synonym": "Routine, practice.", 
          "example": "He left the house at nine exactly, as is his custom.", 
          "video": "https://www.youtube.com/embed/MXqaGR3Dd28  from 0:18 to 0:26 second"
          }, 
          {
          "word": "Customer base", 
          "synonym": "", 
          "example": "Vodafone increased its customer base by 4.2 million.", 
          "video": ""
          }, 
          {
          "word": "Customer", 
          "synonym": "", 
          "example": "Customerñfacing is not an easy job.", 
          "video": ""
          }, 
          {
          "word": "Customs officer", 
          "synonym": "", 
          "example": "The customs officer was looking carefully at all the luggage.", 
          "video": "https://www.youtube.com/embed/QbxKAr2vXvc"
          }, 
          {
          "word": "Cut sb to the quick", 
          "synonym": "", 
          "example": "Her thoughtless remark cut him to the quick.", 
          "video": "https://www.youtube.com/embed/PaO168t1ErE  up to 1:17 second"
          }, 
          {
          "word": "Cut a corner", 
          "synonym": "", 
          "example": "We could finish this project early only if we cut corners.", 
          "video": "https://www.youtube.com/embed/xh5isvCQ6XI  from 0:15 second"
          }, 
          {
          "word": "Cut a dash", 
          "synonym": "", 
          "example": "Wearing his uniform, my grandfather cut a dash on his wedding day.", 
          "video": "https://www.youtube.com/embed/QKO5fFmpgvc?t=5s"
          }, 
          {
          "word": "Cut a fine figure / cut quite a figure/dash", 
          "synonym": "", 
          "example": "The young soldier cut a fine figure in his new uniform.", 
          "video": ""
          }, 
          {
          "word": "Cut a swathe through sth", 
          "synonym": "", 
          "example": "The storm cut a swathe through the village.", 
          "video": ""
          }, 
          {
          "word": "Cut a tooth", 
          "synonym": "", 
          "example": "A feast will be arranged to celebrate a son cutting his first tooth.", 
          "video": ""
          }, 
          {
          "word": "Cut across sth", 
          "synonym": "", 
          "example": "Support for environmental issues cuts across traditional party lines.", 
          "video": ""
          }, 
          {
          "word": "Cut across/through", 
          "synonym": "Including and containing.", 
          "example": "Support for environmental issues cuts across traditional party lines.", 
          "video": "https://www.youtube.com/embed/ZKvHhDkZasY"
          }, 
          {
          "word": "Cut and dried", 
          "synonym": "", 
          "example": "Most fire investigations are pretty cut and dried, but this one has left more questions than answers.", 
          "video": "https://www.youtube.com/embed/_hHqCE4Gfd8  up to 0:10 second"
          }, 
          {
          "word": "Cut and dried", 
          "synonym": "", 
          "example": "The business world prefer cut and dried information as it speeds productivity.", 
          "video": ""
          }, 
          {
          "word": "Cut and dried", 
          "synonym": "", 
          "example": "When the new manager arrived, he didn't find the situation as cut and dried as he had expected.", 
          "video": "https://www.youtube.com/embed/_hHqCE4Gfd8 up to 0:09 second"
          }, 
          {
          "word": "Cut and paste", 
          "synonym": "", 
          "example": "The assignment was a plagiarized one, as it was written by cut and paste from internet sources.", 
          "video": "https://www.youtube.com/embed/8Q7_Xl9QdQM"
          }, 
          {
          "word": "Cut and thrust", 
          "synonym": "", 
          "example": "She enjoys the cut and thrust of party politics.", 
          "video": "https://www.youtube.com/embed/j3wxcMZee2A"
          }, 
          {
          "word": "Cut back", 
          "synonym": "False economy, horn.", 
          "example": "If exercise is causing you pain, you should cut back.", 
          "video": "https://www.youtube.com/embed/891qoUygP1s"
          }, 
          {
          "word": "Cut back/down", 
          "synonym": "", 
          "example": "If exercise is causing you pain, you should cut back.", 
          "video": "https://www.youtube.com/embed/891qoUygP1s"
          }, 
          {
          "word": "Cut both/two ways", 
          "synonym": "", 
          "example": "The promotion cuts both ways because though Iíll make more money, Iíll have to be away from my family more often.", 
          "video": "https://www.youtube.com/embed/g_t6vXmn6t8  up to 1:26 second"
          }, 
          {
          "word": "Cut down on", 
          "synonym": "", 
          "example": "The doctor told him to cut down on cigarettes.", 
          "video": "https://www.youtube.com/embed/hX8XTOR"
          }, 
          {
          "word": "Cut down", 
          "synonym": "", 
          "example": "She used to work 50 hours a week, but recently she's cut down.", 
          "video": "https://www.youtube.com/embed/FWc4ZUiNXgY"
          }, 
          {
          "word": "Cut in", 
          "synonym": "", 
          "example": "It's urgent, Raoul cut in.", 
          "video": ""
          }, 
          {
          "word": "Cut in", 
          "synonym": "", 
          "example": "She was dancing with Jack, when Tom suddenly cut in.", 
          "video": ""
          }, 
          {
          "word": "Cut in", 
          "synonym": "", 
          "example": "She cut in on a station wagon, forcing the driver to brake.", 
          "video": ""
          }, 
          {
          "word": "Cut in", 
          "synonym": "Interrupting & preventing from speaking.", 
          "example": "I was just talking to Jan, when Dave cut in on us/our conversation.", 
          "video": "https://www.youtube.com/embed/cXYgI1FZygw"
          }, 
          {
          "word": "Cut into sth", 
          "synonym": "", 
          "example": "I don't like doing the shopping on Saturday afternoon because it  cuts into my weekend.", 
          "video": ""
          }, 
          {
          "word": "Cut it out!", 
          "synonym": "", 
          "example": "Can you cut it out! I am in no mood for your little jokes.", 
          "video": ""
          }, 
          {
          "word": "Cut it", 
          "synonym": "", 
          "example": "Just cut it now! I have to study now.", 
          "video": "https://www.youtube.com/embed/JDQ7YkaSZS0"
          }, 
          {
          "word": "Cut it/that out", 
          "synonym": "", 
          "example": "Cut it out, you two ñI'm tired of listening to you argue!", 
          "video": "https://www.youtube.com/embed/JDQ7YkaSZS0"
          }, 
          {
          "word": "Cut loose", 
          "synonym": "", 
          "example": "Don't be too hard on them", 
          "video": "https://www.youtube.com/embed/ZWkwdDjS464"
          }, 
          {
          "word": "Cut no ice with sb", 
          "synonym": "", 
          "example": "I've heard her excuses and they cut no ice with me.", 
          "video": "https://www.youtube.com/embed/oNEujMO4LsU up to 1:36 second"
          }, 
          {
          "word": "Cut off your nose to spite your face", 
          "synonym": "", 
          "example": "I know you're mad at your dad, but don't cut off your nose to spite your face", 
          "video": "https://www.youtube.com/embed/sBbfp9OJdQM"
          }, 
          {
          "word": "Cut off", 
          "synonym": "Abandon, abandonment.", 
          "example": "31 March is the cutoff date for applications to be accepted.", 
          "video": "https://www.youtube.com/embed/ESTkZVdW1QQ"
          }, 
          {
          "word": "Cut one's losses", 
          "synonym": "", 
          "example": "The project is heading for failure.  Let's cut our losses before it's too late.", 
          "video": "https://www.youtube.com/embed/DS1tZ2oRCbM"
          }, 
          {
          "word": "Cut oneís losses", 
          "synonym": "", 
          "example": "The project is heading for failure.  Let's cut our losses before it's too late.", 
          "video": ""
          }, 
          {
          "word": "Cut oneís own throat", 
          "synonym": "", 
          "example": "Tony has already missed a lot of classes.  He's cutting his own throat.", 
          "video": ""
          }, 
          {
          "word": "Cut one’s losses", 
          "synonym": "", 
          "example": "The project is heading for failure.  Let's cut our losses before it's too late.", 
          "video": ""
          }, 
          {
          "word": "Cut one’s own throat", 
          "synonym": "", 
          "example": "Tony has already missed a lot of classes.  He's cutting his own throat.", 
          "video": ""
          }, 
          {
          "word": "Cut out", 
          "synonym": "", 
          "example": "One of the plane's engines cut out, so they had to land with only one.", 
          "video": ""
          }, 
          {
          "word": "Cut out", 
          "synonym": "Break, burn.", 
          "example": "One of the plane's engines cut out, so they had to land with only one.", 
          "video": "https://www.youtube.com/embed/DxvffAQb060"
          }, 
          {
          "word": "Cut sb dead", 
          "synonym": "", 
          "example": "I said 'Good morning' but he just cut me dead.", 
          "video": ""
          }, 
          {
          "word": "Cut sb down to size", 
          "synonym": "", 
          "example": "Someone should cut that man down to size!", 
          "video": ""
          }, 
          {
          "word": "Cut sb in", 
          "synonym": "", 
          "example": "Shall we cut you in on the deal/ game?", 
          "video": ""
          }, 
          {
          "word": "Cut sb off", 
          "synonym": "", 
          "example": "We got cut off before she could give me directions.", 
          "video": ""
          }, 
          {
          "word": "Cut sb off", 
          "synonym": "", 
          "example": "We got cut off before she could give me directions.", 
          "video": ""
          }, 
          {
          "word": "Cut sb out of your will", 
          "synonym": "", 
          "example": "They cut me out of the conversation.", 
          "video": ""
          }, 
          {
          "word": "Cut sb out", 
          "synonym": "", 
          "example": "They cut me out of the conversation.", 
          "video": ""
          }, 
          {
          "word": "Cut sb short", 
          "synonym": "", 
          "example": "He started to explain, but she cut him short.", 
          "video": "https://www.youtube.com/embed/W8PRA0MJRJg"
          }, 
          {
          "word": "Cut sb some slack", 
          "synonym": "", 
          "example": "'Andrew's late again.' 'Cut him some slack'", 
          "video": "https://www.youtube.com/embed/_207PeT"
          }, 
          {
          "word": "Cut sb up", 
          "synonym": "", 
          "example": "I got/was cut up several times on the motorway this morning", 
          "video": ""
          }, 
          {
          "word": "Cut sb/sth off", 
          "synonym": "", 
          "example": "When his  wife died, he cut himself off from other people.", 
          "video": ""
          }, 
          {
          "word": "Cut sth down", 
          "synonym": "", 
          "example": "Patients were asked if they had cut down their use of painkillers.", 
          "video": ""
          }, 
          {
          "word": "Cut sth off", 
          "synonym": "", 
          "example": "If this bill is not paid within five days, your gas supply will be cut off.", 
          "video": ""
          }, 
          {
          "word": "Cut sth off", 
          "synonym": "", 
          "example": "Remember to cut off the fat before you fry the steak.", 
          "video": ""
          }, 
          {
          "word": "Cut sth out", 
          "synonym": "", 
          "example": "She cut out his picture from the magazine.", 
          "video": ""
          }, 
          {
          "word": "Cut sth out", 
          "synonym": "", 
          "example": "Since my heart attack I've cut fatty foods out altogether.", 
          "video": ""
          }, 
          {
          "word": "Cut sth up", 
          "synonym": "", 
          "example": "Cut the chicken breast up into small pieces.", 
          "video": "https://www.youtube.com/embed/DtALNCfs1Ng  up to 0:09 second"
          }, 
          {
          "word": "Cut the cards", 
          "synonym": "", 
          "example": "In many card games, to cut the cards or to cut the deck is a procedure used just prior to the cards being dealt to the players.", 
          "video": ""
          }, 
          {
          "word": "Cut the crap!", 
          "synonym": "", 
          "example": "Just cut the crap and tell me what you really want from me.", 
          "video": "https://www.youtube.com/embed/q8NfsTmOYuQ"
          }, 
          {
          "word": "Cut the ground from under feet", 
          "synonym": "", 
          "example": "When we launched the new product, we cut the ground from under our competitors' feet.", 
          "video": ""
          }, 
          {
          "word": "Cut the ground from under sb's feet", 
          "synonym": "", 
          "example": "Raimaís friend actually cut the ground from her feet by making a better project than that of Raima.", 
          "video": ""
          }, 
          {
          "word": "Cut through sth", 
          "synonym": "", 
          "example": "She always manages to cut through the complex theory and get at the facts.", 
          "video": ""
          }, 
          {
          "word": "Cut to the chase", 
          "synonym": "", 
          "example": "I didn't have long to talk so I cut to the chase and asked whether he was still married.", 
          "video": "https://www.youtube.com/embed/KVZ55FaxqVs"
          }, 
          {
          "word": "Cut to the chase", 
          "synonym": "", 
          "example": "I didn't have long to talk so I cut to the chase and asked whether he was still married.", 
          "video": "https://www.youtube.com/embed/KVZ55FaxqVs"
          }, 
          {
          "word": "Cut to the quick", 
          "synonym": "", 
          "example": "Alan was cut to the quick when Joe expressed doubt about his sincerity.", 
          "video": ""
          }, 
          {
          "word": "Cut up rough", 
          "synonym": "", 
          "example": "Looking at the result of the son, Mom immediately cut up rough.", 
          "video": ""
          }, 
          {
          "word": "Cut up", 
          "synonym": "", 
          "example": "There are a couple of kids who are always cutting up in class.", 
          "video": ""
          }, 
          {
          "word": "Cut your losses", 
          "synonym": "", 
          "example": "Let's cut our losses and sell the business before prices drop even further.", 
          "video": "https://www.youtube.com/embed/DS1tZ2oRCbM"
          }, 
          {
          "word": "Cut your political/professional, etc. teeth", 
          "synonym": "", 
          "example": "She cut her political teeth on student debates.", 
          "video": ""
          }, 
          {
          "word": "Cut", 
          "synonym": "", 
          "example": "Scrapping of price fixing legislation led to a cut", 
          "video": ""
          }, 
          {
          "word": "Cutback", 
          "synonym": "", 
          "example": "The company has made cutbacks and closed one of its factories.", 
          "video": ""
          }, 
          {
          "word": "Cutback", 
          "synonym": "", 
          "example": "The closure of the Manchester printing factory is the company's biggest single cutback so far.", 
          "video": "https://www.youtube.com/embed/891qoUygP1s"
          }, 
          {
          "word": "Cute", 
          "synonym": "Quick", 
          "example": "Don't be cute with me, Vicki.", 
          "video": "https://www.youtube.com/embed/m6YyaKtzgaw  from 0:40 second"
          }, 
          {
          "word": "Cutesy", 
          "synonym": "Honeyed, sugary.", 
          "example": "She sent me one of those awful birthday cards with a cutesy kitten on it.", 
          "video": "https://www.youtube.com/embed/CM3HoVIcshs"
          }, 
          {
          "word": "Cuticle", 
          "synonym": "Shell, epidermis.", 
          "example": "The point of the heel crushed the tip of his index finger, splitting the nail as far as the cuticle.", 
          "video": "https://www.youtube.com/embed/ryFXNeSZkxs"
          }, 
          {
          "word": "Cutlass", 
          "synonym": "Sword, knife.", 
          "example": "A cutlass, was found at culpritís home.", 
          "video": "https://www.youtube.com/embed/pEgTMnclgYw"
          }, 
          {
          "word": "Cutlery", 
          "synonym": "Table knife, spoon.", 
          "example": "We had no fridge, cooker, cutlery or crockery.", 
          "video": "https://www.youtube.com/embed/ipA26tqtapQ"
          }, 
          {
          "word": "Cutout", 
          "synonym": "Battery, plug.", 
          "example": "The cutout fuse burnt suddenly, so electricity supply turned off.", 
          "video": "https://www.youtube.com/embed/DxvffAQb060 up to 0:16 second"
          }, 
          {
          "word": "Cutout", 
          "synonym": "Motif, pattern.", 
          "example": "As she is a fan of Amitav Bachchan, she may have a cutout of the respective actor.", 
          "video": ""
          }, 
          {
          "word": "Cutting edge", 
          "synonym": "", 
          "example": "The company is at the cutting edge of aeronautics.", 
          "video": "https://www.youtube.com/embed/AaPJlumBTwo from 0:10 second"
          }, 
          {
          "word": "Cutting", 
          "synonym": "", 
          "example": "cutting", 
          "video": ""
          }, 
          {
          "word": "Cutting", 
          "synonym": "Arrogant, unkind.", 
          "example": "He can be very cutting when he chooses to be!", 
          "video": ""
          }, 
          {
          "word": "Cutting", 
          "synonym": "Bud, aerial root.", 
          "example": "She bought a cutting of Neem to plant at her homeís rooftop.", 
          "video": ""
          }, 
          {
          "word": "Cutting", 
          "synonym": "Excerpt, write", 
          "example": "She always stores cutting of the news of her favorite actors.", 
          "video": ""
          }, 
          {
          "word": "Cutting", 
          "synonym": "Subway, trench.", 
          "example": "Constructing a cutting for train is expensive.", 
          "video": ""
          }, 
          {
          "word": "Cuttlefish", 
          "synonym": "Crustacean,  crayfish.", 
          "example": "That restaurant has an item on cuttlefish.", 
          "video": ""
          }, 
          {
          "word": "Cutup", 
          "synonym": "Silly, stupid.", 
          "example": "It's hard to believe Ella was a cutup in school ", 
          "video": ""
          }, 
          {
          "word": "Cyan", 
          "synonym": "Azure, earth", 
          "example": "She wore a cyan colored top at the party.", 
          "video": "https://www.youtube.com/embed/Z70h0IrQoCI"
          }, 
          {
          "word": "Cyberpet", 
          "synonym": "Digital pet, virtual pet.", 
          "example": "His son wanted a cyberpet on his eighth birthday.", 
          "video": "https://www.youtube.com/embed/aAMP2NJmHkM"
          }, 
          {
          "word": "Cyberspace", 
          "synonym": "The internet, firewall.", 
          "example": "You can find the answer to almost any question in cyberspace.", 
          "video": "https://www.youtube.com/embed/ANGTub3hzzw"
          }, 
          {
          "word": "Cybersquat", 
          "synonym": "Access number, account name.", 
          "example": "The controversy opens a new front in the battle over cybersquatting.", 
          "video": "https://www.youtube.com/embed/55DCGvkGewU"
          }, 
          {
          "word": "Cybrarian", 
          "synonym": "", 
          "example": "Doing the work of cybrarian is not that much easy.", 
          "video": "https://www.youtube.com/embed/j3s9FVE7yiM"
          }, 
          {
          "word": "Cyclamen", 
          "synonym": "", 
          "example": "A cyclamen is a plant with white, pink, or red flowers.", 
          "video": "https://www.youtube.com/embed/z9ixUPGxso4"
          }, 
          {
          "word": "Cyclical", 
          "synonym": "", 
          "example": "Changes in the economy  have followed a cyclical pattern.", 
          "video": "https://www.youtube.com/embed/X9kOV_mClcU"
          }, 
          {
          "word": "Cyclops", 
          "synonym": "", 
          "example": "Euripides in the Cyclops essentially follows the Homeric account.", 
          "video": "https://www.youtube.com/embed/_LMIzgFZddM"
          }, 
          {
          "word": "Cygnet", 
          "synonym": "Young bird, swan.", 
          "example": "This cygnet has a broken leg.", 
          "video": "https://www.youtube.com/embed/3Yf"
          }, 
          {
          "word": "Cylindrical", 
          "synonym": "Rounded, cylindric.", 
          "example": "Cylindrical organs may exhibit similar phenomena.", 
          "video": "https://www.youtube.com/embed/k7JeH6L_hsA"
          }, 
          {
          "word": "Cymbal", 
          "synonym": "Chime, bell.", 
          "example": "Banging the cymbal loudly, the musician marched through the parade to his own beat.", 
          "video": "https://www.youtube.com/embed/pTdVI0MMVDY"
          }, 
          {
          "word": "Cynic", 
          "synonym": "", 
          "example": "I'm too much of a cynic to believe that he'll keep his promise.", 
          "video": ""
          }, 
          {
          "word": "Cynosure", 
          "synonym": "Enchantress, angel.", 
          "example": "Jane has been the cynosure of the media since she won the award for best supporting actress.", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Cypher", 
          "synonym": "Number, code.", 
          "example": "The message was written in cypher.", 
          "video": "https://www.youtube.com/embed/MCxt4j4QF4Q"
          }, 
          {
          "word": "Cypress", 
          "synonym": "Christmas tree, conifer.", 
          "example": "It stands in a large open space and is approached by an avenue of cypresses and eucalyptus.", 
          "video": "https://www.youtube.com/embed/ADp4LYu"
          }, 
          {
          "word": "Cyst", 
          "synonym": "Blister, boil.", 
          "example": "He had a cyst removed from near his eye.", 
          "video": "https://www.youtube.com/embed/sZqzBtcmwxs"
          }, 
          {
          "word": "Dab hand at something", 
          "synonym": "", 
          "example": "Why don't you call Suzy? She's a dab hand at organising barbecues.", 
          "video": ""
          }, 
          {
          "word": "Dab hand", 
          "synonym": "", 
          "example": "She was a dab hand at tennis and played for her school.", 
          "video": ""
          }, 
          {
          "word": "Dab", 
          "synonym": "Press, pat.", 
          "example": "She dabbed at her eyes with a tissue", 
          "video": "https://www.youtube.com/embed/8JjhiZYgbNA  up to 0:15 second"
          }, 
          {
          "word": "Dabble", 
          "synonym": "Float, dip.", 
          "example": "They dabbled their feet in the rock pools.", 
          "video": "https://www.youtube.com/embed/meG5rzoYRns up to 0:09 second"
          }, 
          {
          "word": "Dabble", 
          "synonym": "Shoot, attempt.", 
          "example": "He first dabbled in politics when he was at law school.", 
          "video": "https://www.youtube.com/embed/meG5rzoYRns  from 0:13 second"
          }, 
          {
          "word": "Dachshund/ sausage dog/ wiener dog", 
          "synonym": "", 
          "example": "She discovered her love for animals while breeding dachshunds and selling them worldwide.", 
          "video": "https://www.youtube.com/embed/Etp1xUnthOQ"
          }, 
          {
          "word": "Dacron", 
          "synonym": "Acrylic, acetate.", 
          "example": "Common materials include kevlar, twaron, dacron, hemp, and canvas.", 
          "video": "https://www.youtube.com/embed/eH2O1FOz5Mw"
          }, 
          {
          "word": "Daddy longlegs/ crane fly", 
          "synonym": "Aphid, insect.", 
          "example": "Although crane fly is small in size, but it can be harmful.", 
          "video": "https://www.youtube.com/embed/nR3J3vTq4Z4"
          }, 
          {
          "word": "Dado rail", 
          "synonym": "", 
          "example": "The walls have been panelled up to the dado rail.", 
          "video": "https://www.youtube.com/embed/BWYXvOiAEgs"
          }, 
          {
          "word": "Daffodil", 
          "synonym": "", 
          "example": "The daffodils are starting to wilt.", 
          "video": "https://www.youtube.com/embed/R5tKjD9mrqM"
          }, 
          {
          "word": "Daffy", 
          "synonym": "Silly, stupid.", 
          "example": "She thought of Cherry as being too daffy to be self", 
          "video": "https://www.youtube.com/embed/xyCqJqzZgFw"
          }, 
          {
          "word": "Dag", 
          "synonym": "Fright, blowsy.", 
          "example": "Though she was a beautiful girl, unfortunately her husband was a dag.", 
          "video": ""
          }, 
          {
          "word": "Dagger", 
          "synonym": "Poniard, kris.", 
          "example": "Jenn whipped out a dagger, but he knocked it away.", 
          "video": "https://www.youtube.com/embed/MN2VK9ShzQk"
          }, 
          {
          "word": "Daggy", 
          "synonym": "Dirty, untidy.", 
          "example": "If they were sophisticated, they thought it was really daggy.", 
          "video": "https://www.youtube.com/embed/qboflvM8NCs"
          }, 
          {
          "word": "Daguerreotype", 
          "synonym": "Exposure, capture.", 
          "example": "The first photograph of the moon was a daguerreotype, made by Dr J.", 
          "video": "https://www.youtube.com/embed/cM"
          }, 
          {
          "word": "Dahlia", 
          "synonym": "", 
          "example": "Plant out dahlias and other tender subjects, if risk of frost is past.", 
          "video": "https://www.youtube.com/embed/WT"
          }, 
          {
          "word": "Daily bread", 
          "synonym": "Charge, cost.", 
          "example": "With the amount of daily bread I make, its just enough to support my family.", 
          "video": "https://www.youtube.com/embed/0ZftotP85o4"
          }, 
          {
          "word": "Daily bread.", 
          "synonym": "Aliment", 
          "example": "He earned, indeed, his daily bread, but he had neither linen, clothes, nor shoes.", 
          "video": "https://www.youtube.com/embed/ddz6ZeYvkL0"
          }, 
          {
          "word": "Daily", 
          "synonym": "Home help, cleaner.", 
          "example": "My daily did not come at work today.", 
          "video": ""
          }, 
          {
          "word": "Daintily", 
          "synonym": "Elegant, adorable.", 
          "example": "She skipped daintily down the street, holding her father's hand.", 
          "video": "https://www.youtube.com/embed/d1dsn1hQbaw"
          }, 
          {
          "word": "Dais", 
          "synonym": "Basement, platform.", 
          "example": "The mayor and the governor will sit on the dais until it is time for them to speak.", 
          "video": "https://www.youtube.com/embed/vJN9T7qMiPM"
          }, 
          {
          "word": "Daisy", 
          "synonym": "", 
          "example": "This corolla occurs in many composite plants, as in the florets of dandelion, daisy and chicory.", 
          "video": "https://www.youtube.com/embed/WdzOpnY_40s"
          }, 
          {
          "word": "Dally with sth", 
          "synonym": "", 
          "example": "He had occasionally  dallied with the idea of starting his own  business but he had never actually done anything about it.", 
          "video": ""
          }, 
          {
          "word": "Dalmatian", 
          "synonym": "", 
          "example": "Dalmatian puppies are born with plain white coats and their first spots usually appear within 3 to 4 weeks after birth, however spots are visible on their skin.", 
          "video": "https://www.youtube.com/embed/KA92CJVEHUQ"
          }, 
          {
          "word": "Dam sth up", 
          "synonym": "", 
          "example": "If we don't dam up the river, this rain will cause a flood.", 
          "video": ""
          }, 
          {
          "word": "Damage limitation", 
          "synonym": "", 
          "example": "The government is involved in a damage", 
          "video": ""
          }, 
          {
          "word": "Damages", 
          "synonym": "", 
          "example": "They were awarded $500,000 in damages.", 
          "video": ""
          }, 
          {
          "word": "Dame", 
          "synonym": "Woman, lady.", 
          "example": "Who does that dame think she is?", 
          "video": "https://www.youtube.com/embed/noe8sCIszzw"
          }, 
          {
          "word": "Damn all", 
          "synonym": "", 
          "example": "I know damn all about computers.", 
          "video": ""
          }, 
          {
          "word": "Damn sb with faint praise", 
          "synonym": "", 
          "example": "Her mother", 
          "video": "https://www.youtube.com/embed/kG3lMmV0daY"
          }, 
          {
          "word": "Damn you/them/it, etc.", 
          "synonym": "", 
          "example": "You got the last ticket ", 
          "video": ""
          }, 
          {
          "word": "Damn", 
          "synonym": "", 
          "example": "As a child she was taught that she would be damned for her sins.", 
          "video": "https://www.youtube.com/embed/1vrNsAmutyo up to 0:09 second"
          }, 
          {
          "word": "Damn", 
          "synonym": "", 
          "example": "The inquiry into the disaster damns the company for its lack of safety precautions.", 
          "video": "https://www.youtube.com/embed/1vrNsAmutyo from 0:19 second"
          }, 
          {
          "word": "Damnable", 
          "synonym": "", 
          "example": "This damnable car! It just won't start on, cold mornings!", 
          "video": "https://www.youtube.com/embed/usogiDj29G8"
          }, 
          {
          "word": "Damnation", 
          "synonym": "Infernal, damn.", 
          "example": "He believed that he would be condemned to eternal damnation for what he had done.", 
          "video": "https://www.youtube.com/embed/zi93XoQxz4U"
          }, 
          {
          "word": "Damnedest", 
          "synonym": "Extraordinary, unique.", 
          "example": "Well that's the damnedest excuse I've ever heard!", 
          "video": "https://www.youtube.com/embed/ApnjpGvWc7Q"
          }, 
          {
          "word": "Damp Proof Course", 
          "synonym": "Course, row.", 
          "example": "The damp proof course may be horizontal or vertical.", 
          "video": "https://www.youtube.com/embed/Zfcfcbiw014"
          }, 
          {
          "word": "Damp squib", 
          "synonym": "Disappointment, shame.", 
          "example": "After all that media attention, the whole event turned out to be a bit of a damp squib, with very few people attending.", 
          "video": "https://www.youtube.com/embed/kdOjw_H1YBQ"
          }, 
          {
          "word": "Damp sth down", 
          "synonym": "Drain, slash.", 
          "example": "He had tried to damp down speculation about the state of his marriage.", 
          "video": ""
          }, 
          {
          "word": "Damp sth down fire", 
          "synonym": "Smother,  blow.", 
          "example": "Water was pumped from a nearby lake in an attempt to damp down the flames.", 
          "video": ""
          }, 
          {
          "word": "Damson", 
          "synonym": "Dried fruit, mulberry.", 
          "example": "Damson is a kind of plum.", 
          "video": "https://www.youtube.com/embed/fspXqPxiyC8"
          }, 
          {
          "word": "Dance attendance on sb", 
          "synonym": "Praising insincerely , too eagerly.", 
          "example": "I can't stand the way she has to have someone dancing attendance on her the whole time.", 
          "video": ""
          }, 
          {
          "word": "Dance to sb's tune", 
          "synonym": "Slobber, flatter.", 
          "example": "The senators are dancing to the tune of the President.", 
          "video": ""
          }, 
          {
          "word": "Dance to someoneís tune", 
          "synonym": "", 
          "example": "He is the company's major shareholder so the management has to dance to his tune.", 
          "video": ""
          }, 
          {
          "word": "Dandelion", 
          "synonym": "Oleander, passion flower.", 
          "example": "The children took turns blowing the dandelion clock.", 
          "video": "https://www.youtube.com/embed/syryfpTRM3U"
          }, 
          {
          "word": "Dandle", 
          "synonym": "Handle, cradle.", 
          "example": "He dandled his son on his knee.", 
          "video": "https://www.youtube.com/embed/nhUThhY7Thg"
          }, 
          {
          "word": "Dandruff", 
          "synonym": "Hairpiece,  hirsute.", 
          "example": "Dandruff is a skin condition that mainly affects the scalp", 
          "video": "https://www.youtube.com/embed/g8mgF8UR"
          }, 
          {
          "word": "Dandy", 
          "synonym": "Gentleman, alpha male.", 
          "example": "An upper", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Danger money / hazardous", 
          "synonym": "Earning money, commission.", 
          "example": "They don't get a penny of payment, let alone danger money.", 
          "video": ""
          }, 
          {
          "word": "Dank", 
          "synonym": "Wet, cold.", 
          "example": "In the cathedral vaults the air was dank and stale.", 
          "video": "https://www.youtube.com/embed/Wy_j6wzNf84"
          }, 
          {
          "word": "Dapper", 
          "synonym": "Smart, elegant.", 
          "example": "Hercule Poirot is the dapper detective of the Agatha Christie novels.", 
          "video": "https://www.youtube.com/embed/sSOdY33Q6sc"
          }, 
          {
          "word": "Dappled", 
          "synonym": "Patterns , shapes.", 
          "example": "The dappled sunlight fell across her face as she lay beneath the tree.", 
          "video": "https://www.youtube.com/embed/cwa5H2Bt64A"
          }, 
          {
          "word": "Daredevil", 
          "synonym": "Superhero, adventurer.", 
          "example": "Such sad cases sometimes appear accidental and sometimes appear to involve risky daredevil behavior", 
          "video": "https://www.youtube.com/embed/UXMEELyoBVc"
          }, 
          {
          "word": "Dark  horse", 
          "synonym": "Horse racing,  runner.", 
          "example": "You never can tell, some dark horse many come along and win a House of Lords seat.", 
          "video": "https://www.youtube.com/embed/jC0wqbetXfU"
          }, 
          {
          "word": "Dark ' horse", 
          "synonym": "Private,  dissimulate.", 
          "example": "Anna's such a dark horse ", 
          "video": "https://www.youtube.com/embed/xDZcVraEFBk"
          }, 
          {
          "word": "Dark horse", 
          "synonym": "", 
          "example": "Anna's such a dark horse", 
          "video": "https://www.youtube.com/embed/xDZcVraEFBk"
          }, 
          {
          "word": "Dark", 
          "synonym": "Feeling sad, unhappy.", 
          "example": "Her husband's sudden death was the start of a dark chapter in her life.", 
          "video": "https://www.youtube.com/embed/U9JZiD36srA"
          }, 
          {
          "word": "Dark", 
          "synonym": "Gloomy, sightless.", 
          "example": "It was too dark to see much.", 
          "video": "https://www.youtube.com/embed/dCOhxjI"
          }, 
          {
          "word": "Dark", 
          "synonym": "Morally wrong,  scandalous.", 
          "example": "There's a darker side to his character.", 
          "video": "https://www.youtube.com/embed/U9JZiD36srA"
          }, 
          {
          "word": "Dark", 
          "synonym": "Secrecy, privacy.", 
          "example": "I've just been promoted, but keep it dark ", 
          "video": "https://www.youtube.com/embed/dCOhxjI"
          }, 
          {
          "word": "Darkie", 
          "synonym": "Nigro, darky.", 
          "example": "I'm also very easy to recognize; the darkie in the middle jumping around with the guitar, you know.", 
          "video": "https://www.youtube.com/embed/y_Jj8WdoW6Y"
          }, 
          {
          "word": "Darn", 
          "synonym": "Knitting, sewing.", 
          "example": "She still darns the holes in her socks.", 
          "video": "https://www.youtube.com/embed/QkzP"
          }, 
          {
          "word": "Darning needle", 
          "synonym": "Knitting needle, knitter.", 
          "example": "I bought a set of Clover Chibi darning needles.", 
          "video": "https://www.youtube.com/embed/jREZE0rvFY4"
          }, 
          {
          "word": "Dart a glance/look at sb", 
          "synonym": "Glide,  scoot.", 
          "example": "She darted an angry look at me.", 
          "video": ""
          }, 
          {
          "word": "Dart", 
          "synonym": "Collar, shoulder.", 
          "example": "The dart of her dress is very nice.", 
          "video": "https://www.youtube.com/embed/uFXuIBmuiLs"
          }, 
          {
          "word": "Dart", 
          "synonym": "Shoot,  fly.", 
          "example": "We made a dart for the exit.", 
          "video": "https://www.youtube.com/embed/uFXuIBmuiLs"
          }, 
          {
          "word": "Darts", 
          "synonym": "Board game", 
          "example": "His favorite game is darts.", 
          "video": "https://www.youtube.com/embed/vqDUgPpcI_k"
          }, 
          {
          "word": "Dash sbís hopes", 
          "synonym": "Disheartenment, melancholy.", 
          "example": "Saturday's 2ñ0 defeat dashed their hopes of reaching the final.", 
          "video": ""
          }, 
          {
          "word": "Dash sth off", 
          "synonym": "Hurrying, doing things quickly.", 
          "example": "She dashed the letter off in five minutes.", 
          "video": ""
          }

      ]
    }
  },

  computed: {
      filterVocabularies: function(){
          return this.vocabularies.filter((vocabulary)=>{
              return vocabulary.word.match(this.search);
          })
      }

  }
};
</script>

<style scoped>

    .paginate{
        margin: 20px;
    }

</style>