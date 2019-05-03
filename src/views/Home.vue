<template>
  <div class="home">
    <div class="container">
      <div class="paginate">

            <nav aria-label="Page navigation" v-if="!search">
                <ul class="pagination justify-content-center">
                    
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('A')">A</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('B')">B</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('C')">C</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('D')">D</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('E')">E</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('F')">F</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('G')">G</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('H')">H</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('I')">I</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('J')">J</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('K')">K</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('L')">L</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('M')">M</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('N')">N</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('O')">O</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('P')">P</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('Q')">Q</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('R')">R</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('S')">S</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('T')">T</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('U')">U</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('V')">V</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('W')">W</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('X')">X</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('Y')">Y</a></li>
                    <li class="page-item"><a class="page-link bg-dark text-white" @click="findChar('Z')">Z</a></li>
                    
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

  methods: {

    findChar: function(value){
        
        this.value = value;

    }

  },


  data() {
    
    return{
      
      search:"",
      value:"",

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
            "word": "Be much obliged", 
            "synonym": "Relieved and thankful.", 
            "example": "'Here's the information you requested.' 'Oh, I'm much obliged to you.'", 
            "video": "https://www.youtube.com/embed/Isx5J7uIs5E"
            }, 
            {
            "word": "Not rock the boat", 
            "synonym": "", 
            "example": "After the recent riots, it was decided not to rock the boat by introducing strict measures.", 
            "video": ""
            }, 
            {
            "word": "Put skin in the game", 
            "synonym": "", 
            "example": "I got good news today.  Apparently a serious investor is willing to put skin in the game.", 
            "video": ""
            }, 
            {
            "word": "Reach first base", 
            "synonym": "", 
            "example": "If you go to the interview dressed like that, you won't get to first base!", 
            "video": ""
            }, 
            {
            "word": "Reach first base", 
            "synonym": "", 
            "example": "If you go to the interview dressed like that, you won't get to first base!", 
            "video": ""
            }, 
            {
            "word": "Well I'll be damned!", 
            "synonym": "", 
            "example": "She's marrying a man who she met two months ago?", 
            "video": ""
            }, 
            {
            "word": "Well what do you know!", 
            "synonym": "Surprised, Aw shucks, Charming, Boo", 
            "example": "So they're getting married, are they? Well, what do you know!", 
            "video": ""
            }, 
            {
            "word": "a little bird told me", 
            "synonym": "", 
            "example": "A little bird told me that you are thinking of quitting your job.", 
            "video": ""
            }, 
            {
            "word": "an old hand", 
            "synonym": "", 
            "example": "My uncle’s an old hand at car repair. He will know what that problem is", 
            "video": ""
            }, 
            {
            "word": "as Large as life", 
            "synonym": "Visibility, visible.", 
            "example": "I looked up from my newspaper and there he was, as large as life, Tim Trotter!", 
            "video": ""
            }, 
            {
            "word": "as quick as lightning", 
            "synonym": "", 
            "example": "Wow! Your shower was as quick as lightning.", 
            "video": ""
            }, 
            {
            "word": "by the skin of one’s teeth", 
            "synonym": "", 
            "example": "I passed my exam by the skin of my teeth", 
            "video": ""
            }, 
            {
            "word": "down To the last ...", 
            "synonym": "Core, extreme.", 
            "example": "He has calculated the costs down to the last penny.", 
            "video": ""
            }, 
            {
            "word": "every now and then/again.", 
            "synonym": "Sometimes, Episodic, Occasional.", 
            "example": "We meet up for lunch now and then, but not as often as we used to.", 
            "video": ""
            }, 
            {
            "word": "get wind of something", 
            "synonym": "", 
            "example": "My Dad has a new girlfriend. I got wind of it over dinner tonight.", 
            "video": ""
            }, 
            {
            "word": "have a bee in one’s bonnet", 
            "synonym": "", 
            "example": "Milan has a bee in his bonnet all day, but he won’t tell me what’s wrong.", 
            "video": ""
            }, 
            {
            "word": "have a card up one’s sleeve", 
            "synonym": "", 
            "example": "I think Josh has a card up his sleeve cause he wants me to wear a dress to the fast", 
            "video": ""
            }, 
            {
            "word": "my flesh and blood", 
            "synonym": "", 
            "example": "I have to hire Mia. She’s my own flesh and blood.", 
            "video": ""
            }, 
            {
            "word": "my lips are sealed", 
            "synonym": "", 
            "example": "Don’t worry , I won’t tell your mother how much you spent. My lips are sealed.", 
            "video": ""
            }, 
            {
            "word": "not let the grass grow under feet.", 
            "synonym": "", 
            "example": "As soon as he received the permit, he started to build.  He never lets the grass grow under his feet!", 
            "video": "https://www.youtube.com/embed/j"
            }, 
            {
            "word": "on cloud nine", 
            "synonym": "", 
            "example": "Andrea was on cloud nine when she bought her new car.", 
            "video": ""
            }, 
            {
            "word": "right down to", 
            "synonym": "", 
            "example": "Amalie was dressed completely in black, right down to black lipstick and a black earring.", 
            "video": ""
            }, 
            {
            "word": "up a blind alley", 
            "synonym": "", 
            "example": "The suspect's 'revelations' lead the police up a blind alley.", 
            "video": ""
            }, 
            {
            "word": "up a blind alley", 
            "synonym": "", 
            "example": "The suspect's 'revelations' lead the police up a blind alley.", 
            "video": ""
            }, 
            {
            "word": "whole bag of tricks", 
            "synonym": "", 
            "example": "Let's call on George and his bag of tricks; maybe he can help us solve the problem.", 
            "video": ""
            }, 
            {
            "word": "Chime in", 
            "synonym": "", 
            "example": "'It's very difficult,' I said. 'Impossible,' she chimed in.", 
            "video": "https://www.youtube.com/embed/yjRPrvk1_Vg"
            }, 
            {
            "word": "fair", 
            "synonym": "", 
            "example": "They seemed only fair", 
            "video": "https://www.youtube.com/embed/zwqpI0oBK24"
            }, 
            {
            "word": "pass  sth  on", 
            "synonym": "", 
            "example": "It's possible to pass on the virus to others through physical contact.", 
            "video": ""
            }, 
            {
            "word": "sound like a broken record", 
            "synonym": "", 
            "example": "I hate to sound like a broken record, but we just don't have enough people on the payroll to work effciently.", 
            "video": ""
            }, 
            {
            "word": "accept/take sth on faith", 
            "synonym": "", 
            "example": "I have no firm evidence that Bob's responsible for the errors", 
            "video": ""
            }, 
            {
            "word": "pass", 
            "synonym": "", 
            "example": "I got myself a pass into the barracks.", 
            "video": "https://www.youtube.com/embed/vz4t0CchIrM"
            }, 
            {
            "word": "Faith can move mountains", 
            "synonym": "", 
            "example": "If you believe that faith can move mountains then you can do anything.", 
            "video": ""
            }, 
            {
            "word": "Go for a song", 
            "synonym": "", 
            "example": "Wow, I can't believe they let so many things at their yard sale go for a song.", 
            "video": "https://www.youtube.com/embed/Z2bccEGWaEs"
            }, 
            {
            "word": "pass", 
            "synonym": "", 
            "example": "The monastery is in a remote mountain pass.", 
            "video": "https://www.youtube.com/embed/vz4t0CchIrM"
            }, 
            {
            "word": "Call the tune", 
            "synonym": "Who pays the piper calls the tune.", 
            "example": "My staff has to do what I say because I'm the boss, and I call the tune here!", 
            "video": ""
            }, 
            {
            "word": "Have faith!", 
            "synonym": "", 
            "example": "Have faith! Everything will work out.", 
            "video": ""
            }, 
            {
            "word": "pass", 
            "synonym": "", 
            "example": "As the years passed, her condition worsened.", 
            "video": "https://www.youtube.com/embed/vz4t0CchIrM"
            }, 
            {
            "word": "Sing a different tune", 
            "synonym": "Sing another tune.", 
            "example": "You will sing another tune as soon as you find out how right I am!", 
            "video": ""
            }, 
            {
            "word": "keep faith with sth/sb", 
            "synonym": "", 
            "example": "The company has not kept faith with its promise to invest in training.", 
            "video": ""
            }, 
            {
            "word": "passable", 
            "synonym": "", 
            "example": "Because of the heavy snow, roads in the area were passable only with care.", 
            "video": "https://www.youtube.com/embed/m8kiqS6vQeM"
            }, 
            {
            "word": "Fine tuning", 
            "synonym": "", 
            "example": "She spent hours fine", 
            "video": "https://www.youtube.com/embed/dN80QwD76R0"
            }, 
            {
            "word": "passable", 
            "synonym": "", 
            "example": "Mary can speak passable Russian.", 
            "video": "https://www.youtube.com/embed/m8kiqS6vQeM"
            }, 
            {
            "word": "put/place your faith in sth/sb", 
            "synonym": "", 
            "example": "Some people put their faith in strong leaders rather than sound policies", 
            "video": ""
            }, 
            {
            "word": "Blow the whistle", 
            "synonym": "", 
            "example": "The company stopped using certain chemicals only after some workers blew the whistle on it.", 
            "video": "https://www.youtube.com/embed/SaFzI9J_UJM"
            }, 
            {
            "word": "passage", 
            "synonym": "", 
            "example": "A narrow passage led directly through the house into the garden.", 
            "video": "https://www.youtube.com/embed/9pwLdWbp3Sw"
            }, 
            {
            "word": "put/place your faith in sth/sb", 
            "synonym": "", 
            "example": "", 
            "video": ""
            }, 
            {
            "word": "Clean as a whistle", 
            "synonym": "Extremely clean.", 
            "example": "It leaves your face feeling clean as a whistle but not bone", 
            "video": "https://www.youtube.com/embed/1uBZcU7kU3U"
            }, 
            {
            "word": "passage", 
            "synonym": "", 
            "example": "A short passage for a trumpet solo.", 
            "video": "https://www.youtube.com/embed/9pwLdWbp3Sw"
            }, 
            {
            "word": "the faithful", 
            "synonym": "", 
            "example": "We heard bells calling the faithful to prayer", 
            "video": "https://www.youtube.com/embed/157s_v0FF34"
            }, 
            {
            "word": "A penny for your thoughts", 
            "synonym": "Mind and personality.", 
            "example": "You haven't said very much ñ a penny for your thoughts.", 
            "video": "https://www.youtube.com/embed/_Rr1GueAusg"
            }, 
            {
            "word": "Have an ace up your sleeve", 
            "synonym": "", 
            "example": "I have an ace up my sleeve for this race my stamina.", 
            "video": "https://www.youtube.com/embed/0xYB1HAeNRE"
            }, 
            {
            "word": "Yours faithfully", 
            "synonym": "", 
            "example": "He served the family faithfully for 40 years.", 
            "video": ""
            }, 
            {
            "word": "passage", 
            "synonym": "", 
            "example": "We booked passage on a cruise ship.", 
            "video": "https://www.youtube.com/embed/9pwLdWbp3Sw"
            }, 
            {
            "word": "Hold all the aces", 
            "synonym": "", 
            "example": "In a situation like this, it's the big companies who hold all the aces.", 
            "video": ""
            }, 
            {
            "word": "faith healer", 
            "synonym": "", 
            "example": "Her injuries are healed rapidly by a faith healer, but she is forced to spend two weeks having bed rest.", 
            "video": "https://www.youtube.com/embed/boQ5IknrWes"
            }, 
            {
            "word": "work  your  passage", 
            "synonym": "", 
            "example": "He worked his passage home as a steward.", 
            "video": ""
            }, 
            {
            "word": "Back to square one", 
            "synonym": "", 
            "example": "We'll have to go back to square one if the government pulls our funding on this project.", 
            "video": "https://www.youtube.com/embed/oFHF6aAjVQk"
            }, 
            {
            "word": "faith school", 
            "synonym": "", 
            "example": "I would never send my child to a faith school.", 
            "video": "https://www.youtube.com/embed/GA8rGVB9h8I"
            }, 
            {
            "word": "passage", 
            "synonym": "", 
            "example": "The government prohibits the passage of foreign troops and planes across its territory.", 
            "video": "https://www.youtube.com/embed/9pwLdWbp3Sw"
            }, 
            {
            "word": "Drum something into someoneís head", 
            "synonym": "", 
            "example": "The teacher drummed the names of the state capitals into our heads.", 
            "video": ""
            }, 
            {
            "word": "fairy", 
            "synonym": "", 
            "example": "It's that bit in the story where the fairy grants the little girl three wishes.", 
            "video": "https://www.youtube.com/embed/jVT3l4pazUc"
            }, 
            {
            "word": "pass out", 
            "synonym": "", 
            "example": "I was hit on the head and passed out.", 
            "video": "https://www.youtube.com/embed/Vt5HtAGGZ5E"
            }, 
            {
            "word": "Beggars canít be choosers", 
            "synonym": "", 
            "example": "I would have preferred a house of my own rather than sharing, but beggars can't be choosers, I suppose.", 
            "video": "https://www.youtube.com/embed/8XpZ5xVoj4s"
            }, 
            {
            "word": "fajita", 
            "synonym": "", 
            "example": "The fajita was in the traditional thin wrapping paper.", 
            "video": "https://www.youtube.com/embed/qoS_7muRhJo"
            }, 
            {
            "word": "the passage of time", 
            "synonym": "", 
            "example": "Memories fade with the passage of time.", 
            "video": "https://www.youtube.com/embed/ME84cdVMGao"
            }, 
            {
            "word": "Bend over backwards", 
            "synonym": "", 
            "example": "Mann insisted that he bent over backwards to be objective in presenting the story.", 
            "video": "https://www.youtube.com/embed/d2hj_1lpoR8"
            }, 
            {
            "word": "fake tan", 
            "synonym": "", 
            "example": "He was wearing too much fake tan and looked orange.", 
            "video": "https://www.youtube.com/embed/yGyECRNtK40"
            }, 
            {
            "word": "passage", 
            "synonym": "", 
            "example": "He again urged passage of a constitutional amendment outlawing abortion.", 
            "video": "https://www.youtube.com/embed/9pwLdWbp3Sw"
            }, 
            {
            "word": "Bide your time", 
            "synonym": "", 
            "example": "She was biding her time until she could get her revenge.", 
            "video": ""
            }, 
            {
            "word": "fakir", 
            "synonym": "", 
            "example": "The fakir paused to gaze around his audience.", 
            "video": "https://www.youtube.com/embed/xDTh6A17zpE"
            }, 
            {
            "word": "passbook", 
            "synonym": "", 
            "example": "Each inmate received $22 of the gift, deposited into a prison passbook account.", 
            "video": "https://www.youtube.com/embed/lHlniYOB9i4"
            }, 
            {
            "word": "Blank cheque", 
            "synonym": "", 
            "example": "We know there are limits to funding and we don't have a blank cheque.", 
            "video": "https://www.youtube.com/embed/J36GG6cu07A"
            }, 
            {
            "word": "falcon", 
            "synonym": "", 
            "example": "He glanced about and saw David coming with a falcon on his hand.", 
            "video": "https://www.youtube.com/embed/2"
            }, 
            {
            "word": "pass degree", 
            "synonym": "", 
            "example": "You need six credits for a pass degree and eight credits for an honours degree.", 
            "video": ""
            }, 
            {
            "word": "Bone of contention", 
            "synonym": "", 
            "example": "Money is a common bone of contention in many marriages.", 
            "video": "https://www.youtube.com/embed/9CdMMSV8ypg"
            }, 
            {
            "word": "falconer", 
            "synonym": "", 
            "example": "For thousands of years, falconers have taught falcons to fly away, catch other birds, and bring them back.", 
            "video": "https://www.youtube.com/embed/7kkdsGImmz8"
            }, 
            {
            "word": "passÈ", 
            "synonym": "", 
            "example": "Wines from that region were quite popular for a while, but now they're rather passÈ.", 
            "video": "https://www.youtube.com/embed/PIuSCoYGH_Y"
            }, 
            {
            "word": "Bring nothing to the table", 
            "synonym": "", 
            "example": "While others are interesting or have stories to tell a person who brings nothing to the table simply drags others down.", 
            "video": ""
            }, 
            {
            "word": "falconry", 
            "synonym": "", 
            "example": "The falconry display has over 50 birds of prey.", 
            "video": "https://www.youtube.com/embed/h4MuM3E0frw"
            }, 
            {
            "word": "passenger train", 
            "synonym": "", 
            "example": "Two passenger trains were involved in the accident.", 
            "video": "https://www.youtube.com/embed/TMGlH7_EAig"
            }, 
            {
            "word": "Drive a hard bargain", 
            "synonym": "", 
            "example": "Sal is known to drive a hard bargain, so I doubt you'll get that car for the price you want.", 
            "video": "https://www.youtube.com/embed/38z8EUz4GRI"
            }, 
            {
            "word": "fall flat on your face", 
            "synonym": "", 
            "example": "we might fall flat on our faces and end up bankrupt", 
            "video": ""
            }, 
            {
            "word": "passer", 
            "synonym": "", 
            "example": "The gunmen opened fire, killing a policeman and a passer", 
            "video": "https://www.youtube.com/embed/pstxVEsE0Ro"
            }, 
            {
            "word": "Leave the door open", 
            "synonym": "", 
            "example": "The management were intelligent enough to leave the door open for further negotiations with the union.", 
            "video": ""
            }, 
            {
            "word": "fall to your knees / fall down on your knees", 
            "synonym": "", 
            "example": "The people all fell to their knees and began to pray.", 
            "video": ""
            }, 
            {
            "word": "pass", 
            "synonym": "", 
            "example": "It's a pass", 
            "video": "https://www.youtube.com/embed/LUI"
            }, 
            {
            "word": "Meet half", 
            "synonym": "", 
            "example": "I'll agree to some of your requests if you'll meet me halfway and allow me to implement some of my ideas.", 
            "video": ""
            }, 
            {
            "word": "fall between two stools", 
            "synonym": "", 
            "example": "The work fell between two stools, being neither genuinely popular nor truly scholarly", 
            "video": "https://www.youtube.com/embed/4fltePFcVB0"
            }, 
            {
            "word": "in passing", 
            "synonym": "", 
            "example": "When asked if he had told the police about the incident, Mr Banks said he had mentioned it in passing to a detective.", 
            "video": ""
            }, 
            {
            "word": "Nitty", 
            "synonym": "The essence; the essential points.", 
            "example": "Once we are down to the nitty", 
            "video": "https://www.youtube.com/embed/ZnNdHiRCURQ"
            }, 
            {
            "word": "fall by the wayside", 
            "synonym": "", 
            "example": "Many readers will fall by the wayside as the terminology becomes more complicated", 
            "video": "https://www.youtube.com/embed/G1tVhEHQroA"
            }, 
            {
            "word": "the passing of time/the years.              TIME", 
            "synonym": "", 
            "example": "My parents seem to have mellowed with the passing of the years.", 
            "video": ""
            }, 
            {
            "word": "As fit as a fiddle", 
            "synonym": "", 
            "example": "My grandmother's 89, but she's as fit as a fiddle.", 
            "video": "https://www.youtube.com/embed/61nJ_5xkiSA"
            }, 
            {
            "word": "be away with the fairies", 
            "synonym": "", 
            "example": "It's no good asking her to take care of the children", 
            "video": "https://www.youtube.com/embed/7KIpFtIBD1o"
            }, 
            {
            "word": "pass out", 
            "synonym": "", 
            "example": "The new officers passed out from Britannia Royal Naval College on Thursday 1 August .", 
            "video": "https://www.youtube.com/embed/Vt5HtAGGZ5E"
            }, 
            {
            "word": "Play your cards right", 
            "synonym": "", 
            "example": "If you play your cards right, you could make quite a lot of money out of this.", 
            "video": ""
            }, 
            {
            "word": "a passing resemblance", 
            "synonym": "", 
            "example": "He bears more than a passing resemblance to = he is noticeably similar to the young Marlon Brando.", 
            "video": ""
            }, 
            {
            "word": "fall flat", 
            "synonym": "Be unsuccessful, not succeed,", 
            "example": "His jokes fell flat", 
            "video": ""
            }, 
            {
            "word": "Play for time", 
            "synonym": "", 
            "example": "We can't sign the agreement yet", 
            "video": ""
            }, 
            {
            "word": "fall foul of sth", 
            "synonym": "", 
            "example": "Manufacturers may fall foul of the new government guidelines.", 
            "video": ""
            }, 
            
            {
            "word": "Chuck sth in", 
            "synonym": "Drop", 
            "example": "I've decided to chuck in my job.", 
            "video": ""
            }, 
            {
            "word": "Chuck", 
            "synonym": "Overhand", 
            "example": "Chuck it over there/into the corner.", 
            "video": "https://www.youtube.com/embed/SmFpxaQim5k"
            }, 
            {
            "word": "Chuckle", 
            "synonym": "Giggle", 
            "example": "She was chuckling as she read the letter.", 
            "video": "https://www.youtube.com/embed/dqMfiLluV5Y"
            }, 
            {
            "word": "Chuffed", 
            "synonym": "Delighted", 
            "example": "He was really chuffed with his present.", 
            "video": "https://www.youtube.com/embed/xsxpWAJFGdc"
            }, 
            {
            "word": "Chum up", 
            "synonym": "Intimately", 
            "example": "She chummed up with some girls from Bristol on holiday.", 
            "video": ""
            }, 
            {
            "word": "Chummy", 
            "synonym": "Mate", 
            "example": "They're very chummy with their neighbor's", 
            "video": "https://www.youtube.com/embed/CGM73KlqQZY"
            }, 
            {
            "word": "Chunky", 
            "synonym": "Stocky", 
            "example": "His wife Annie was dour and a bit on the chunky side.", 
            "video": "https://www.youtube.com/embed/QWOABSfrUGU"
            }, 
            {
            "word": "Chunter", 
            "synonym": "Protest", 
            "example": "All were chuntering about being the last to know what was happening.", 
            "video": "https://www.youtube.com/embed/hx_qDNkDWzo"
            }, 
            {
            "word": "Churlish", 
            "synonym": "Impolite", 
            "example": "They invited me to dinner and I thought it would be churlish to refuse.", 
            "video": "https://www.youtube.com/embed/Q6J6s6SjaN0"
            }, 
            {
            "word": "Churn sth out", 
            "synonym": "Overproduce", 
            "example": "She churns out a new best", 
            "video": "https://www.youtube.com/embed/hnOtsr9AA_A"
            }, 
            {
            "word": "Churn", 
            "synonym": "Shake", 
            "example": "The storm churned the sea.", 
            "video": "https://www.youtube.com/embed/1L6h0Q_WEKY"
            }, 
            {
            "word": "Chutzpah", 
            "synonym": "Unpleasant", 
            "example": "I lack the wherewithal to start my own competing certifying board, to say nothing of the chutzpah.", 
            "video": "https://www.youtube.com/embed/grMQviBpVA0"
            }, 
            {
            "word": "Cinder", 
            "synonym": "Fumes", 
            "example": "The cake was burned to a cinder.", 
            "video": "https://www.youtube.com/embed/Ja_ZiQDUr"
            }, 
            {
            "word": "Cipher", 
            "synonym": "Code", 
            "example": "The message was written in cipher.", 
            "video": "https://www.youtube.com/embed/MCxt4j4QF4Q"
            }, 
            {
            "word": "Circumference", 
            "synonym": "Eccentric", 
            "example": "What is the circumference of a circle with diameter 12 cm?", 
            "video": "https://www.youtube.com/embed/OUJPa_fLJX0"
            }, 
            {
            "word": "Circumlocution", 
            "synonym": "Implicit", 
            "example": "Politicians are experts in circumlocution.", 
            "video": "https://www.youtube.com/embed/AgExcXzZmT8"
            }, 
            {
            "word": "Circumnavigate", 
            "synonym": "", 
            "example": "They circumnavigated Cape Horn Island in canoes.", 
            "video": "https://www.youtube.com/embed/kYLKRzgY2CQ"
            }, 
            {
            "word": "Circumscribe", 
            "synonym": "Restricting", 
            "example": "There followed a series of tightly circumscribed visits to military installations.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Circumspect", 
            "synonym": "vigilant", 
            "example": "Officials were circumspect about saying what the talks had achieved.", 
            "video": "https://www.youtube.com/embed/Nl8OHac4awI"
            }, 
            {
            "word": "Circumstance", 
            "synonym": "Condition", 
            "example": "I think she coped very well under the circumstances.", 
            "video": "https://www.youtube.com/embed/eS9vSkvZs9I"
            }, 
            {
            "word": "Circumstances", 
            "synonym": "Economic situation.", 
            "example": "Grants are available depending on your circumstances.", 
            "video": "https://www.youtube.com/embed/nOdkYfuqNKQ"
            }, 
            {
            "word": "Circumstantial", 
            "synonym": "Conflicted", 
            "example": "The case against her was circumstantial.", 
            "video": "https://www.youtube.com/embed/3g5qh_hvIgA"
            }, 
            {
            "word": "Circumvent", 
            "synonym": "Insure", 
            "example": "Ships were registered abroad to circumvent employment and safety regulations.", 
            "video": "https://www.youtube.com/embed/HRX8WjOX2Ws"
            }, 
            {
            "word": "Circus", 
            "synonym": "Amusement park", 
            "example": "She ran away to join the circus.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Circus", 
            "synonym": "Midway", 
            "example": "Piccadilly Circus is a road junction and public space of London's West End in the City of Westminster.", 
            "video": ""
            }, 
            {
            "word": "Claim", 
            "synonym": "Assert, face", 
            "example": "She rejected claims that she had lied.", 
            "video": "https://www.youtube.com/embed/d2QiyRRT7IM up to 0:18 second"
            }, 
            {
            "word": "Clam up", 
            "synonym": "", 
            "example": "Arthur clammed up when I asked about his family.", 
            "video": ""
            }, 
            {
            "word": "Clam up", 
            "synonym": "Falling silent and not speaking.", 
            "example": "He just clams up if you ask him about his childhood.", 
            "video": "https://www.youtube.com/embed/b6ZBH8AyRGs"
            }, 
            {
            "word": "Clamp down on", 
            "synonym": "Limiting and restricting.", 
            "example": "The government is clamping down on teenage drinking.", 
            "video": "https://www.youtube.com/embed/c5Ia7AabCRM"
            }, 
            {
            "word": "Class act", 
            "synonym": "", 
            "example": "Her career is just beginning but she's already a class act.", 
            "video": "https://www.youtube.com/embed/LvHfchm2HXA  up to 0:26 second"
            }, 
            {
            "word": "Classify", 
            "synonym": "Categorize, stratify", 
            "example": "The books are classified by subject.", 
            "video": "https://www.youtube.com/embed/HvqU6TNXb_c upto  0:10 second"
            }, 
            {
            "word": "Close but no cigar", 
            "synonym": "", 
            "example": "It was close but no cigar for Johnny as he came second once again.", 
            "video": "https://www.youtube.com/embed/2t7VOmEOv7Q"
            }, 
            {
            "word": "Close but no cigar", 
            "synonym": "", 
            "example": "The ball touched the goal post", 
            "video": ""
            }, 
            {
            "word": "Close but no cigar", 
            "synonym": "", 
            "example": "The ball touched the goal post", 
            "video": ""
            }, 
            {
            "word": "Close down", 
            "synonym": "", 
            "example": "When the factory closed down, the employees lost their jobs.", 
            "video": "https://www.youtube.com/embed/XVMEIqegZEY"
            }, 
            {
            "word": "Close shave", 
            "synonym": "Difficult situations and unpleasant experiences.", 
            "example": "I had a close shave this morning", 
            "video": "https://www.youtube.com/embed/vfFH3R8asQo"
            }, 
            {
            "word": "Close to home", 
            "synonym": "", 
            "example": "Alan looks embarrassed.  Bob's comment must have been close to home.", 
            "video": ""
            }, 
            {
            "word": "Cloud on the horizon", 
            "synonym": "", 
            "example": "They are happily married and for the moment there appear to be no clouds on the horizon.", 
            "video": "https://www.youtube.com/embed/pedWNS50QQA up to 1:26 second"
            }, 
            {
            "word": "Cloud on the horizon.", 
            "synonym": "", 
            "example": "They are happily married and for the moment there appear to be no clouds on the horizon.", 
            "video": "https://www.youtube.com/embed/pedWNS50QQA"
            }, 
            {
            "word": "Co", 
            "synonym": "Appoint, Intake.", 
            "example": "She was co", 
            "video": "https://www.youtube.com/embed/nbKtkIMMWSQ"
            }, 
            {
            "word": "Co", 
            "synonym": "Integrate, Blend.", 
            "example": "Rock and roll music was largely co", 
            "video": "https://www.youtube.com/embed/nbKtkIMMWSQ"
            }, 
            {
            "word": "Coast is clear", 
            "synonym": "Safe and secure.", 
            "example": "You can come out now, the coast is clear.", 
            "video": "https://www.youtube.com/embed/BAXeL_yZeNk"
            }, 
            {
            "word": "Cock and bull story", 
            "synonym": "", 
            "example": "He gave me some cock", 
            "video": "https://www.youtube.com/embed/ajBCGboVeI0"
            }, 
            {
            "word": "Cog in the machine", 
            "synonym": "", 
            "example": "The police quickly realized that the suspect was just a cog in the machine.", 
            "video": ""
            }, 
            {
            "word": "Cold feet", 
            "synonym": "", 
            "example": "My sister didn’t get cold feet until she put her wedding gown on.", 
            "video": ""
            }, 
            {
            "word": "Collaborate", 
            "synonym": "Cooperate, merge", 
            "example": "Didn't you collaborate with him on one of your books?", 
            "video": "https://www.youtube.com/embed/jD6ZAlmDk4U up to 0:10 second"
            }, 
            {
            "word": "Come a cropper", 
            "synonym": "", 
            "example": "She came an almighty cropper when her back wheels hit an icy patch.", 
            "video": "https://www.youtube.com/embed/YlIw2jlOw8o"
            }, 
            {
            "word": "Come a long way", 
            "synonym": "", 
            "example": "Tony has come a long way since he opened his first little restaurant.", 
            "video": ""
            }, 
            {
            "word": "Come a long way", 
            "synonym": "", 
            "example": "Tony has come a long way since he opened his first little restaurant.", 
            "video": ""
            }, 
            {
            "word": "Come apart at the seams", 
            "synonym": "", 
            "example": "Bob has had so many problems lately, he's coming apart at the seams.", 
            "video": ""
            }, 
            {
            "word": "Come back to bite you", 
            "synonym": "Shock.", 
            "example": "If I don't do something now, the issue might come back to bite me.", 
            "video": ""
            }, 
            {
            "word": "Come down like a ton of bricks", 
            "synonym": "", 
            "example": "If my boss catches me slacking off at the job he will come down like a ton of bricks.", 
            "video": ""
            }, 
            {
            "word": "Come hell or high water", 
            "synonym": "", 
            "example": "I'll get you to the airport by noon, come hell or high water!", 
            "video": "https://www.youtube.com/embed/W7If3bAluJY"
            }, 
            {
            "word": "Come hell or high water.", 
            "synonym": "", 
            "example": "Come hell or high water, I've got to be on time for the interview.", 
            "video": "https://www.youtube.com/embed/9wbEBiGWlck"
            }, 
            {
            "word": "Come out in the wash.", 
            "synonym": "", 
            "example": "Yes, he was furious when it happened, but don't worry", 
            "video": ""
            }, 
            {
            "word": "Come rain or shine", 
            "synonym": "", 
            "example": "He goes to the gym club every day, come rain or shine.", 
            "video": ""
            }, 
            {
            "word": "Come to a head.", 
            "synonym": "", 
            "example": "The conflict came to a head yesterday when rioting broke out in the streets.", 
            "video": "https://www.youtube.com/embed/mKccU9qj5pE"
            }, 
            {
            "word": "Come to an end", 
            "synonym": "denouement, ending.", 
            "example": "Everyone wishes the war would come to an end soon.", 
            "video": "https://www.youtube.com/embed/Brj8d5HKpEs"
            }, 
            {
            "word": "Come to blows", 
            "synonym": "", 
            "example": "The debate was so intense that the participants almost came to blows.", 
            "video": "https://www.youtube.com/embed/REfHoTDQmwo"
            }, 
            {
            "word": "Come to blows", 
            "synonym": "Fighting", 
            "example": "Demonstrators nearly came to blows with the police during the March.", 
            "video": ""
            }, 
            {
            "word": "Come to grief", 
            "synonym": "", 
            "example": "Their plans for a golf course came to grief when it was decided to build a motorway.", 
            "video": ""
            }, 
            {
            "word": "Come to grief", 
            "synonym": "", 
            "example": "Their plans for a golf course came to grief when it was decided to build a motorway.", 
            "video": ""
            }, 
            {
            "word": "Come to light / bring  sth  to light", 
            "synonym": "Revealing secrets & becoming known.", 
            "example": "Fresh evidence has recently come to light that suggests that he didn't in fact commit the murder.", 
            "video": "https://www.youtube.com/embed/z"
            }, 
            {
            "word": "Come up in the world", 
            "synonym": "", 
            "example": "My old school friend has bought an apartment overlooking Central Park.  She has certainly come up in the world.", 
            "video": ""
            }, 
            {
            "word": "Come up in the world", 
            "synonym": "", 
            "example": "My old school friend has bought an apartment overlooking Central Park.  She has certainly come up in the world.", 
            "video": ""
            }, 
            {
            "word": "Come up roses", 
            "synonym": "", 
            "example": "After several disappointments, everything seems to be coming up roses for the tennis player this year.", 
            "video": ""
            }, 
            {
            "word": "Come up roses", 
            "synonym": "", 
            "example": "After several disappointments, everything seems to be coming up roses for the tennis player this year.", 
            "video": ""
            }, 
            {
            "word": "Come up roses.", 
            "synonym": "", 
            "example": "After several disappointments, everything seems to be coming up roses for the tennis player this year.", 
            "video": ""
            }, 
            {
            "word": "Come within an ace of something", 
            "synonym": "", 
            "example": "She came within an ace of winning the match.", 
            "video": ""
            }, 
            {
            "word": "Come/go down in the world", 
            "synonym": "", 
            "example": "Fancy her taking a job like that", 
            "video": ""
            }, 
            {
            "word": "Come/go under the hammer", 
            "synonym": "Buying & selling", 
            "example": "A private collection of her early paintings is expected to go under the hammer next year.", 
            "video": ""
            }, 
            {
            "word": "Come/suffer under the lash", 
            "synonym": "Denounce, disapproval.", 
            "example": "The sales team came under the lash for poor results.", 
            "video": ""
            }, 
            {
            "word": "Come/turn up trumps", 
            "synonym": "", 
            "example": "Against all expectations, our team came up trumps in the cup final. ", 
            "video": ""
            }, 
            {
            "word": "Come/turn up trumps", 
            "synonym": "", 
            "example": "Against all expectations, our team came up trumps in the cup final. ", 
            "video": ""
            }, 
            {
            "word": "Comfort", 
            "synonym": "Ease, relaxation", 
            "example": "Good chocolate is one of life's little comforts.", 
            "video": "https://www.youtube.com/embed/3KVxujU7drI"
            }, 
            {
            "word": "Commodious", 
            "synonym": "Convenient, Large", 
            "example": "You must know that the Widow Dufeu was not a commodious person.", 
            "video": "https://www.youtube.com/embed/7BQ1tK1ylL8"
            }, 
            {
            "word": "Commodity", 
            "synonym": "Asset, Product", 
            "example": "He had also a trick to mingle his commodity, that that which was bad might go off with the least mistrust.", 
            "video": "https://www.youtube.com/embed/zNdixEMLZDI"
            }, 
            {
            "word": "Commodity", 
            "synonym": "Product, item", 
            "example": "The country's most valuable commodities include tin and diamonds.", 
            "video": "https://www.youtube.com/embed/MxGqwk6mcJ0"
            }, 
            {
            "word": "Commodore", 
            "synonym": "Commute, Compare", 
            "example": "They passed over the pond toward Fair Haven, seemingly deterred from settling by my light, their commodore honking all the while with a regular beat.", 
            "video": "https://www.youtube.com/embed/DLun5UP8Ajo"
            }, 
            {
            "word": "Common de'nominator", 
            "synonym": "Common Divisor, Denominator", 
            "example": "Literacy is defended with the argument that it is some kind of common denominator.", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs,https://www.youtube.com/results?search_query=pronounce+de%27nominator"
            }, 
            {
            "word": "Common de'nominator", 
            "synonym": "Common Measure, Numerator", 
            "example": "He proposes, instead, the term, 'common denominator of value.'", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs,https://www.youtube.com/results?search_query=pronounce+de%27nominator"
            }, 
            {
            "word": "Common", 
            "synonym": "", 
            "example": "In the same way, men and women would riot to defend a right to use common land", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs,https://www.youtube.com/embed/hAtLy"
            }, 
            {
            "word": "Common", 
            "synonym": "Accepted, Trivial", 
            "example": "She will only utilize it for common good.", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs"
            }, 
            {
            "word": "Common", 
            "synonym": "Acute Rhinitis,Acute Viral Nasopharyngitis", 
            "example": "They all are affected by common", 
            "video": "https://www.youtube.com/embed/GdNq_"
            }, 
            {
            "word": "Common", 
            "synonym": "Probable, Habitual", 
            "example": "This was a common practice during the festival of Thargelia, in honour of Phœbus.", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs"
            }, 
            {
            "word": "Common", 
            "synonym": "Public Things, Common Things", 
            "example": "These things are common", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs,https://www.youtube.com/embed/Udj"
            }, 
            {
            "word": "Common", 
            "synonym": "Standard, Homely", 
            "example": "All the systems of writing of the ancient people of Asia had one thing in common.", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs"
            }, 
            {
            "word": "Common", 
            "synonym": "Trite, Stereotype", 
            "example": "They are valuable, but he can do but common things with them because he knows not their possibilities.", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs"
            }, 
            {
            "word": "Common", 
            "synonym": "Typical, Regular", 
            "example": "One of them common Pullmans is good enough fur Marthy and me.", 
            "video": "https://www.youtube.com/embed/lH1vDWV4dNs"
            }, 
            {
            "word": "Commoner", 
            "synonym": "Bourgeois, Peasant", 
            "example": "How little hope there is in the commoner phases of religion!", 
            "video": "https://www.youtube.com/embed/XkIx084wAIE"
            }, 
            {
            "word": "Commonplace", 
            "synonym": "Uneventful, Natural", 
            "example": "It is a curious question why sacred song should so often be dull and commonplace.", 
            "video": "https://www.youtube.com/embed/M2oCNcj9Syg"
            }, 
            {
            "word": "Commotion", 
            "synonym": "Agitation, Outcry", 
            "example": "The commotion of pursuit and investigation was sweeping past her tent.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Commune", 
            "synonym": "Collective, Community", 
            "example": "The candle", 
            "video": "https://www.youtube.com/embed/e51fo1hYvKc"
            }, 
            {
            "word": "Commune", 
            "synonym": "Cooperative, Village", 
            "example": "The abominable and shameful peace had been signed, the wretched Commune crushed.", 
            "video": "https://www.youtube.com/embed/e51fo1hYvKc"
            }, 
            {
            "word": "Commune", 
            "synonym": "Family, Neighborhood", 
            "example": "If a peasant of Marosfalva had it it would do good to the commune.", 
            "video": "https://www.youtube.com/embed/e51fo1hYvKc"
            }, 
            {
            "word": "Communicate", 
            "synonym": "Broadcast, Inform", 
            "example": "She must communicate the dread defiling fact with her own lips!", 
            "video": "https://www.youtube.com/embed/idt2JP5cUas"
            }, 
            {
            "word": "Communicate", 
            "synonym": "Unfold, Interface", 
            "example": "She must communicate the dread defiling fact with her own lips!", 
            "video": "https://www.youtube.com/embed/idt2JP5cUas"
            }, 
            {
            "word": "Communication", 
            "synonym": "Connection, Impression", 
            "example": "Ambrose was the only person who ever received any communication from Giles Headley.", 
            "video": "https://www.youtube.com/embed/lWAjr3IRR44"
            }, 
            {
            "word": "Communications", 
            "synonym": "Talk, Interchange", 
            "example": "Polar ice would have been thawed by this reopening of communication.", 
            "video": "https://www.youtube.com/embed/lWAjr3IRR44"
            }, 
            {
            "word": "Communion", 
            "synonym": "Rapport, Intimacy", 
            "example": "She would soon be fourteen now, and must think of her first communion.", 
            "video": "https://www.youtube.com/embed/mZFDZ4dqkAw"
            }, 
            {
            "word": "Communique", 
            "synonym": "Directive, New", 
            "example": "We've just received the first communique from the advance guard, sir.", 
            "video": "https://www.youtube.com/embed/MOT7dALTnGw"
            }, 
            {
            "word": "Community", 
            "synonym": "Association, Colony", 
            "example": "It is evident that the man who passed the sentence could commute it, he said.", 
            "video": "https://www.youtube.com/embed/NHTgB7dJYaI"
            }, 
            {
            "word": "Community", 
            "synonym": "Center, Company", 
            "example": "These meetings were productive of great good to the community and to individuals.", 
            "video": "https://www.youtube.com/embed/NHTgB7dJYaI"
            }, 
            {
            "word": "Community", 
            "synonym": "Populace, General Public", 
            "example": "No person, no home, no community can be beyond the reach of this call.", 
            "video": "https://www.youtube.com/embed/NHTgB7dJYaI"
            }, 
            {
            "word": "Community", 
            "synonym": "Territory, Commonwealth", 
            "example": "Philistinism was the note of the age and community in which he lived.", 
            "video": "https://www.youtube.com/embed/NHTgB7dJYaI"
            }, 
            {
            "word": "Community", 
            "synonym": "Turf, Locality", 
            "example": "He pleaded for the machine—for the safety of the community, for the majesty of the law.", 
            "video": "https://www.youtube.com/embed/NHTgB7dJYaI"
            }, 
            {
            "word": "Commute", 
            "synonym": "Go back and forth, Drive", 
            "example": "He seemed at times to be asking God to commute these penalties.", 
            "video": "https://www.youtube.com/embed/QaTv"
            }, 
            {
            "word": "Commute", 
            "synonym": "Subway, Train", 
            "example": "He seemed at times to be asking God to commute these penalties.", 
            "video": "https://www.youtube.com/embed/QaTv"
            }, 
            {
            "word": "Compact", 
            "synonym": "Bunched, Crowded", 
            "example": "What if she were disobeying the Compact—death to the Wicked Compact!", 
            "video": "https://www.youtube.com/embed/fPo3nbshji0"
            }, 
            {
            "word": "Compact", 
            "synonym": "Solid, Close", 
            "example": "A compact little group of men rounded the bend and approached.", 
            "video": "https://www.youtube.com/embed/fPo3nbshji0"
            }, 
            {
            "word": "Compact", 
            "synonym": "Thick, Hard", 
            "example": "The officers and other white men stood about in a compact and silent group.", 
            "video": "https://www.youtube.com/embed/fPo3nbshji0"
            }, 
            {
            "word": "Companion", 
            "synonym": "Ally, Crony", 
            "example": "The man who faced the redhead was as light as his companion was ponderous.", 
            "video": "https://www.youtube.com/embed/zjsZdFUwnyo"
            }, 
            {
            "word": "Companion", 
            "synonym": "Comrade, Proyector", 
            "example": "As Philothea turned towards her companion, she met Aspasia's earnest gaze.", 
            "video": "https://www.youtube.com/embed/zjsZdFUwnyo"
            }, 
            {
            "word": "Companion", 
            "synonym": "Convoy, Aide", 
            "example": "And, of this island realm, he and his companion were the undisputed sovereigns.", 
            "video": "https://www.youtube.com/embed/zjsZdFUwnyo"
            }, 
            {
            "word": "Companionable", 
            "synonym": "Affable, Amicable", 
            "example": "In the social circle he is companionable, but not a very good conversationalist.", 
            "video": "https://www.youtube.com/embed/X9wqHnLDvNI"
            }, 
            {
            "word": "Companionship", 
            "synonym": "Togetherness, Amity", 
            "example": "She had gone to him for some measure of the companionship she had missed in losing her father.", 
            "video": "https://www.youtube.com/embed/kkjqWoqoVqQ"
            }, 
            {
            "word": "Companionway", 
            "synonym": "Stair, Step", 
            "example": "Behind her she heard the commotion of many men descending the companionway.", 
            "video": "https://www.youtube.com/embed/53aaJcpM4Uw"
            }, 
            {
            "word": "Company", 
            "synonym": "Association,Band", 
            "example": "Left Alexander Spring, in company with Windich, to look for water ahead.", 
            "video": "https://www.youtube.com/embed/WfN7pFMUquQ"
            }, 
            {
            "word": "Company", 
            "synonym": "Circle, Mob", 
            "example": "'I shall be very glad to have your company, Robert,' said Hester.", 
            "video": "https://www.youtube.com/embed/WfN7pFMUquQ"
            }, 
            {
            "word": "Company", 
            "synonym": "Community, Troop", 
            "example": "I will now favor the company with a song of my own composure.", 
            "video": "https://www.youtube.com/embed/WfN7pFMUquQ"
            }, 
            {
            "word": "Company", 
            "synonym": "Corps, League", 
            "example": "The company smiled, and the philosopher answered, 'I am Plato.'", 
            "video": "https://www.youtube.com/embed/WfN7pFMUquQ"
            }, 
            {
            "word": "Company", 
            "synonym": "Coterie, Throng", 
            "example": "Let us run away, for fear he should make us enlist in his company!", 
            "video": "https://www.youtube.com/embed/WfN7pFMUquQ"
            }, 
            {
            "word": "Comparative", 
            "synonym": "Provisional, Parallel", 
            "example": "Garson contrived to present an aspect of comparative indifference.", 
            "video": "https://www.youtube.com/embed/Qtpfrf"
            }, 
            {
            "word": "Comparative", 
            "synonym": "Relative, Connected", 
            "example": "To do this it will be necessary to refer to comparative ethnography.", 
            "video": "https://www.youtube.com/embed/Qtpfrf"
            }, 
            {
            "word": "Comparative", 
            "synonym": "Relative,", 
            "example": "In a comparative study we see the work force is increasing in Japan, whereas it is declining in U.S.", 
            "video": "https://www.youtube.com/embed/uTIf_p21MD4"
            }, 
            {
            "word": "Compare", 
            "synonym": "Balance, Analyze", 
            "example": "Or I might compare them to cherubs, haunting that holy place.", 
            "video": "https://www.youtube.com/embed/weTiJMO03oc"
            }, 
            {
            "word": "Compare", 
            "synonym": "Inspect, Contrast", 
            "example": "On the score of health they may compare favourably with any race.", 
            "video": "https://www.youtube.com/embed/weTiJMO03oc"
            }, 
            {
            "word": "Compatible", 
            "synonym": "Suited, well matched", 
            "example": "This keyboard is compatible with all of our computers.", 
            "video": "https://www.youtube.com/embed/xMeTcOosmoU"
            }, 
            {
            "word": "Compel", 
            "synonym": "Impel, urge", 
            "example": "He felt compelled to resign from his job.", 
            "video": "https://www.youtube.com/embed/O"
            }, 
            {
            "word": "Compensate", 
            "synonym": "Repay, recoup", 
            "example": "Victims of the crash will be compensated for their injuries.", 
            "video": "https://www.youtube.com/embed/TOvEZ0TSADg from 0:13 to 0:25 second"
            }, 
            {
            "word": "Competence", 
            "synonym": "Capability, ability", 
            "example": "Her competence as a teacher is unquestionable.", 
            "video": "https://www.youtube.com/embed/aIIoPQRmARI up to 0:21 second"
            }, 
            {
            "word": "Compile", 
            "synonym": "Assemble, compose", 
            "example": "We're compiling some facts and figures for a documentary on climate change.", 
            "video": "https://www.youtube.com/embed/xsPidCriKeI up to 0: 12 second"
            }, 
            {
            "word": "Complaint", 
            "synonym": "Objection, protest", 
            "example": "My only complaint was the lack of refreshments.", 
            "video": "https://www.youtube.com/embed/1FFWrQr0hHI up to  0:10 second"
            }, 
            {
            "word": "Completion", 
            "synonym": "Accomplishment, execution", 
            "example": "The stadium is due for completion in 2008.", 
            "video": "https://www.youtube.com/embed/PAI1SfkNVPM up to 0:11 second"
            }, 
            {
            "word": "Complicate", 
            "synonym": "Complex, intricate", 
            "example": "These new regulations just complicate matters further.", 
            "video": "https://www.youtube.com/embed/i0YmTinrv7M up to 0:15 second"
            }, 
            {
            "word": "Compliment", 
            "synonym": "Praise, commendation", 
            "example": "He complimented me on my writing.", 
            "video": "https://www.youtube.com/embed/n2azbB6Qmlg"
            }, 
            {
            "word": "Component", 
            "synonym": "Constituent, part", 
            "example": "Our company makes components for aircraft engines.", 
            "video": "https://www.youtube.com/embed/_jYT"
            }, 
            {
            "word": "Compostable", 
            "synonym": "Biodegradation, Humus, Mulch, Organic fertilizer .", 
            "example": "Compostable garden waste.", 
            "video": "https://www.youtube.com/embed/pl773nzWH1c?t=5s"
            }, 
            {
            "word": "Compote", 
            "synonym": "Dessert, Sweet", 
            "example": "When done, place the compote in the centre of the dish, piling it up high.", 
            "video": "https://www.youtube.com/embed/AJb"
            }, 
            {
            "word": "Compound eye", 
            "synonym": "Eye, Oculus, Optic", 
            "example": "On the compound eye of a butterfly as many as 17,325 facettes have been counted.", 
            "video": "https://www.youtube.com/embed/_xYLLrdURGk"
            }, 
            {
            "word": "Compound fracture", 
            "synonym": "Open fracture", 
            "example": "There's a compound fracture above the knee, and a dislocation below.", 
            "video": "https://www.youtube.com/embed/1AW2JTsuKgg"
            }, 
            {
            "word": "Compound leaf", 
            "synonym": "Leafage, Foliage", 
            "example": "It has lost the leaflets from its compound leaf, and a single one remains.", 
            "video": "https://www.youtube.com/embed/GHzlUjeZIQI?t=47s"
            }, 
            {
            "word": "Compound", 
            "synonym": "Blend, Mixture, Mix, Fusion", 
            "example": "The air smelled like a compound of diesel and petrol fumes.", 
            "video": "https://www.youtube.com/embed/EBj5Rg1mpzw"
            }, 
            {
            "word": "Compound", 
            "synonym": "Worsen, Make worse", 
            "example": "Prisoners' lack of contact with the outside world compounds their problems.", 
            "video": "https://www.youtube.com/embed/EBj5Rg1mpzw"
            }, 
            {
            "word": "Comprehend", 
            "synonym": "Understand, Grasp, Take in, See", 
            "example": "He couldn't comprehend her reasons for marrying Lovat.", 
            "video": "https://www.youtube.com/embed/Q_hAKpqsfzk"
            }, 
            {
            "word": "Comprehensive insurance", 
            "synonym": "Assurance, Acutuary, Benefit", 
            "example": "Fidelity to the emperor and to the teaching of the Roman Catholic doctrine formed part of the aims of this comprehensive corporation.", 
            "video": "https://www.youtube.com/embed/Jt3olmyzaks"
            }, 
            {
            "word": "Comprehensive", 
            "synonym": "Broad, Extensive, Full", 
            "example": "Is this list comprehensive or are there some names missing?", 
            "video": "https://www.youtube.com/embed/wCQyFOLEBBQ"
            }, 
            {
            "word": "Comprehensive", 
            "synonym": "Inclusive, complete", 
            "example": "Presentations on making a career in media, finance and IT could have been more comprehensive.", 
            "video": "https://www.youtube.com/embed/DoefmP6Og_U"
            }, 
            {
            "word": "Compression", 
            "synonym": "Squeezing, Grinding", 
            "example": "Firmly compress the soil in the pot so that the plant is secure.", 
            "video": "https://www.youtube.com/embed/zoJ90FgvmsA"
            }, 
            {
            "word": "Compressor", 
            "synonym": "Crusher, pressure, Squeezer", 
            "example": "The compressor may be driven by a steam engine or in any other convenient manner.", 
            "video": "https://www.youtube.com/embed/G8i7PhFEQns"
            }, 
            {
            "word": "Comprise", 
            "synonym": "Incorporate, contain", 
            "example": "The orchestra was comprised of amateur and professional musicians.", 
            "video": "https://www.youtube.com/embed/kgJ0uwdNAF4"
            }, 
            {
            "word": "Compromise", 
            "synonym": "Agreement, Settlement, Understanding", 
            "example": "Eventually they reached a compromise.", 
            "video": "https://www.youtube.com/embed/Je_Ryrfkz4c?t=5s"
            }, 
            {
            "word": "Compromise", 
            "synonym": "Undermine, Weaken, Damage", 
            "example": "We were not prepared to compromise on safety.", 
            "video": "https://www.youtube.com/embed/Je_Ryrfkz4c?t=5s"
            }, 
            {
            "word": "Compulsion", 
            "synonym": "Obligation, Force, Enforcement", 
            "example": "The payment was made under compulsion.", 
            "video": "https://www.youtube.com/embed/wREZYd77CUQ"
            }, 
            {
            "word": "Compulsion", 
            "synonym": "Want, Urge, Impulse, Need", 
            "example": "He felt a compulsion to babble on about what had happened.", 
            "video": "https://www.youtube.com/embed/wREZYd77CUQ"
            }, 
            {
            "word": "Compulsory purchase order", 
            "synonym": "Mortages, Real estate", 
            "example": "The City Council has applied for a compulsory purchase order.", 
            "video": "https://www.youtube.com/embed/mFK_lwKrggY"
            }, 
            {
            "word": "Compunction", 
            "synonym": "Misgiving, Worries, Uneasy", 
            "example": "They used their tanks without compunction.", 
            "video": "https://www.youtube.com/embed/OF56wsN2Qm0"
            }, 
            {
            "word": "Computer aided design", 
            "synonym": "Animation", 
            "example": "The geometric design of these systems relies on modern computer aided design software.", 
            "video": "https://www.youtube.com/embed/S37snL6i_hU"
            }, 
            {
            "word": "Computer generated imagery", 
            "synonym": "Images produced by a computer.", 
            "example": "Computer", 
            "video": "https://www.youtube.com/embed/EsUeRvuoMMg"
            }, 
            {
            "word": "Computerate", 
            "synonym": "Computer", 
            "example": "Many movies have been computerated, which is sad as actors are no longer needed for acting.", 
            "video": "https://www.youtube.com/embed/qrcn4ydFqTA"
            }, 
            {
            "word": "Comrade", 
            "synonym": "Friend, Companion, Partner", 
            "example": "An old college comrade.", 
            "video": "https://www.youtube.com/embed/HtHKAN8g"
            }, 
            {
            "word": "Comrade", 
            "synonym": "Political member, Ally", 
            "example": "You're right, comrade.", 
            "video": "https://www.youtube.com/embed/HtHKAN8g"
            }, 
            {
            "word": "Con", 
            "synonym": "Prisoner, Captive, Hostage", 
            "example": "The con was held without charge.", 
            "video": "https://www.youtube.com/embed/WT6J_NQbx4I"
            }, 
            {
            "word": "Con", 
            "synonym": "Trick, Swindle. Deception", 
            "example": "The Charter is a glossy public relations con.", 
            "video": "https://www.youtube.com/embed/WT6J_NQbx4I"
            }, 
            {
            "word": "Concatenation", 
            "synonym": "Series, Sequence, Succession", 
            "example": "A concatenation of events which had finally led to the murder.", 
            "video": "https://www.youtube.com/embed/XekHadzqno4"
            }, 
            {
            "word": "Concave", 
            "synonym": "Curved inwards, Hollow, Hollowed out", 
            "example": "Concaved lenses.", 
            "video": "https://www.youtube.com/embed/DSzlkAzgvGA"
            }, 
            {
            "word": "Concavity", 
            "synonym": "Impression, Hole, Indentation", 
            "example": "And otherwise unlike a volcanic crater is the concavity itself.", 
            "video": "https://www.youtube.com/embed/r04QRUmXwfQ"
            }, 
            {
            "word": "Conceal", 
            "synonym": "Hide, Keep out of sight, Tuck away", 
            "example": "A line of sand dunes concealed the distant sea.", 
            "video": "https://www.youtube.com/embed/uWmCft8tnhY"
            }, 
            {
            "word": "Concede a goal/point", 
            "synonym": "A clean sheet, Aggregate", 
            "example": "Liverpool can not afford to concede a goal tonight", 
            "video": ""
            }, 
            {
            "word": "Concede", 
            "synonym": "Admit, Acknowledge, Accept", 
            "example": "I had to concede that I'd overreacted.", 
            "video": "https://www.youtube.com/embed/bPdEReEKsEw"
            }, 
            {
            "word": "Conceit", 
            "synonym": "Comparison, Image, Imagery", 
            "example": "The idea of the wind's singing is a prime romantic conceit.", 
            "video": "https://www.youtube.com/embed/0AXD6JHU9RI?t=5s"
            }, 
            {
            "word": "Conceit", 
            "synonym": "Pride, Vanity, Self", 
            "example": "He was puffed up with conceit.", 
            "video": "https://www.youtube.com/embed/0AXD6JHU9RI?t=5s"
            }, 
            {
            "word": "Conceive", 
            "synonym": "Image, Imagining, Dream", 
            "example": "I think my uncle still conceives of me as a four", 
            "video": "https://www.youtube.com/embed/xHloin_yOiU"
            }, 
            {
            "word": "Conceive", 
            "synonym": "Invent, Think up, Think of, Dream up", 
            "example": "The dam project was originally conceived in 1977.", 
            "video": "https://www.youtube.com/embed/xHloin_yOiU"
            }, 
            {
            "word": "Concentrate", 
            "synonym": "Attention, Focus, Direct", 
            "example": "She couldn't concentrate on the film.", 
            "video": "https://www.youtube.com/embed/bys1O4YuAmA"
            }, 
            {
            "word": "Concentrate", 
            "synonym": "Focus, centralize", 
            "example": "Most of the fighting was concentrated in the mountains.", 
            "video": "https://www.youtube.com/embed/_dZJFUnORK0 up to 0:15 second"
            }, 
            {
            "word": "Concentrate", 
            "synonym": "Gather, Come together", 
            "example": "The nation's wealth was concentrated in the hands of the governing elite.", 
            "video": "https://www.youtube.com/embed/bys1O4YuAmA"
            }, 
            {
            "word": "Concentrate", 
            "synonym": "Remove water, Extract, Distillation", 
            "example": "Apple juice concentrate.", 
            "video": "https://www.youtube.com/embed/bys1O4YuAmA"
            }, 
            {
            "word": "Concentration camp", 
            "synonym": "Prison camp, Detention camp, Jail", 
            "example": "They liberated all war prisoners from the concentration camp.", 
            "video": "https://www.youtube.com/embed/s2dRbQLvBmE"
            }, 
            {
            "word": "Concentration", 
            "synonym": "Cluster, Mass, Flock", 
            "example": "Islay is famous for its spectacular concentrations of barnacle geese.", 
            "video": "https://www.youtube.com/embed/s2IJGu1wxuU"
            }, 
            {
            "word": "Concentric", 
            "synonym": "Side", 
            "example": "Think of religious exemptions as a series of concentric circles.", 
            "video": "https://www.youtube.com/embed/qsiaOZ7m_gE"
            }, 
            {
            "word": "Conception", 
            "synonym": "Conceiveing, Fertilizing", 
            "example": "An unfertilized egg before conception.", 
            "video": "https://www.youtube.com/embed/ZVoTwh93or0"
            }, 
            {
            "word": "Conceptual", 
            "synonym": "Theoretical, Visionary, Abstract", 
            "example": "Conceptual thinking is often the most demanding kind of mental activity.", 
            "video": "https://www.youtube.com/embed/3KwctQaacgw?t=2s"
            }, 
            {
            "word": "Concern yourself", 
            "synonym": "Involve, Worry, Panic", 
            "example": "Thereís nothing in the doctorís report to concern yourself about.", 
            "video": ""
            }, 
            {
            "word": "Concern", 
            "synonym": "Business, Company, Firm", 
            "example": "The town's only travel agent was a small, debt", 
            "video": "https://www.youtube.com/embed/9iK2GcDhSLk"
            }, 
            {
            "word": "Concern", 
            "synonym": "Worry, Disturb, Trouble", 
            "example": "The roof of the barn concerns me because eventually it will fall in.", 
            "video": "https://www.youtube.com/embed/9iK2GcDhSLk"
            }, 
            {
            "word": "Concert grand", 
            "synonym": "Concert grand, concert piano", 
            "example": "Does a concert grand have any pupose for playing music at home?", 
            "video": "https://www.youtube.com/embed/oDBiQYI4BYA"
            }, 
            {
            "word": "Concerted", 
            "synonym": "Jointly planned, collaborative.", 
            "example": "The richer countries of the world should take concerted action to help the poorer countries.", 
            "video": "https://www.youtube.com/embed/KgdGDAqfnlY"
            }, 
            {
            "word": "Concertina", 
            "synonym": "Air guitar,accordion", 
            "example": "Such songs were often accompanied on mobile instruments of guitars, fiddles, concertina and harmonica.", 
            "video": "https://www.youtube.com/embed/ErX4EfZErmk"
            }, 
            {
            "word": "Concerto", 
            "synonym": "Arrangement, bolero.", 
            "example": "Mozart's concerto for flute and harp.", 
            "video": "https://www.youtube.com/embed/5VBNTUkW9h8"
            }, 
            {
            "word": "Concessionaire", 
            "synonym": "Businessman, entrepreneur.", 
            "example": "He said that no loan agreement had been signed by the selected concessionaire and creditor banks.", 
            "video": "https://www.youtube.com/embed/476FsuS0lOI"
            }, 
            {
            "word": "Concessionary", 
            "synonym": "Cheap, economic", 
            "example": "Neither the treaty, the additional act, nor the colonial law expressly modified the land, commercial and concessionary regime established in the Congo.", 
            "video": "https://www.youtube.com/embed/ugeJvSxtVRQ"
            }, 
            {
            "word": "Conch", 
            "synonym": "Crustacean, barnacle", 
            "example": "I held the conch to my ear and heard the ocean inside.", 
            "video": "https://www.youtube.com/embed/g8OyhOWznB0"
            }, 
            {
            "word": "Conchie", 
            "synonym": "Quibble, nagging.", 
            "example": "They were all conchies and socialists and they kept on about negotiating an end to the war.", 
            "video": "https://www.youtube.com/embed/luywioaLosY"
            }, 
            {
            "word": "Concierge", 
            "synonym": "Attendant keeper", 
            "example": "The concierge opened the door and bowed.", 
            "video": "https://www.youtube.com/embed/IkmsiD2pLew"
            }, 
            {
            "word": "Conciliate", 
            "synonym": "Appease, pacify.", 
            "example": "Concessions were made to conciliate the peasantry.", 
            "video": "https://www.youtube.com/embed/3t1dfLE5AIo"
            }, 
            {
            "word": "Concise", 
            "synonym": "Short, brief.", 
            "example": "His arguments were concise, simple, and clear.", 
            "video": "https://www.youtube.com/embed/eJadN3YeE4o"
            }, 
            {
            "word": "Conclave", 
            "synonym": "Summit, council.", 
            "example": "The conclave of politicians was held on a Friday, giving the attendees the weekend to mull over the sordid details of their discussions.", 
            "video": "https://www.youtube.com/embed/mfSkAFt5114 from 0:24 second"
            }, 
            {
            "word": "Conclude", 
            "synonym": "Finish, end", 
            "example": "The report concluded that the drug was safe.", 
            "video": "https://www.youtube.com/embed/C1rKKubwJWM from 0:16 second to 0:32 second"
            }, 
            {
            "word": "Conclude", 
            "synonym": "Finish, end.", 
            "example": "Before I conclude, I'd like to thank you all for coming.", 
            "video": "https://www.youtube.com/embed/lYnwBgMljZ0"
            }, 
            {
            "word": "Conclude", 
            "synonym": "Judge, determine.", 
            "example": "It would be wrong, however, to conclude that moral considerations have led up to this state of things.", 
            "video": "https://www.youtube.com/embed/C1rKKubwJWM from 0:13 second"
            }, 
            {
            "word": "Conclusive", 
            "synonym": "Assuredly, definite.", 
            "example": "He had conclusive  evidence/ proof of her guilt.", 
            "video": "https://www.youtube.com/embed/iWCsQk"
            }, 
            {
            "word": "Concoct", 
            "synonym": "Prepare, assemble.", 
            "example": "She concocted the most amazing dish from all sorts of leftover food.", 
            "video": "https://www.youtube.com/embed/vcqsqV556KM"
            }, 
            {
            "word": "Concomitant", 
            "synonym": "Associated, related.", 
            "example": "Often loss of  memory is a natural concomitant of  old age.", 
            "video": "https://www.youtube.com/embed/TLXBKq3kYZU"
            }, 
            {
            "word": "Concord", 
            "synonym": "Likeable, amity.", 
            "example": "The war will end when the two countries reach a concord on the disputed territory that aligns their borders.", 
            "video": "https://www.youtube.com/embed/aSAJGY0p4hU"
            }, 
            {
            "word": "Concordance", 
            "synonym": "Chapter,  extract.", 
            "example": "All English Major students have to read Shakespeare Concordance at some point of their academic life.", 
            "video": "https://www.youtube.com/embed/OVLlSDNZ_zg"
            }, 
            {
            "word": "Concordat", 
            "synonym": "Conclave, cistern.", 
            "example": "There was the Concordat of July 1933 between the Holy See and the German Reich.", 
            "video": "https://www.youtube.com/embed/a5Eppw17IbY"
            }, 
            {
            "word": "Concourse", 
            "example": "In the main concourse were businessmen begging rides to Amsterdam.", 
            "video": "https://www.youtube.com/embed/7iWcuig_fUU"
            }, 
            {
            "word": "Concrete adj", 
            "synonym": "Clear, certain", 
            "example": "They think she killed her husband, but they have no concrete evidence.", 
            "video": "https://www.youtube.com/embed/90SZuCdEqe8 up to 0:10 second"
            }, 
            {
            "word": "Concrete n", 
            "synonym": "Material, solid", 
            "example": "The villagers demanded a concrete path at village, to the new leader.", 
            "video": "https://www.youtube.com/embed/90SZuCdEqe8 from 0:15 second"
            }, 
            {
            "word": "Concrete v", 
            "synonym": "Cover, hide", 
            "example": "Why did you concrete over that  nice garden?", 
            "video": ""
            }, 
            {
            "word": "Concrete jungle", 
            "synonym": "Block, inner city.", 
            "example": "Farmgate is one of the concrete jungles of  Dhaka.", 
            "video": "https://www.youtube.com/embed/WZ1N48ndPKQ"
            }, 
            {
            "word": "Concrete mixer", 
            "synonym": "Cement mixer, blender.", 
            "example": "Sure, a man feels like he's been crammed into a concrete mixer when he's burning up light", 
            "video": ""
            }, 
            {
            "word": "Concrete", 
            "synonym": "Definite, specific", 
            "example": "We've got a general idea of what we want, but nothing concrete at the moment.", 
            "video": "https://www.youtube.com/embed/90SZuCdEqe8 up to 0:11"
            }, 
            {
            "word": "Concur", 
            "synonym": "Agree, accept.", 
            "example": "The new report concurs with previous findings.", 
            "video": "https://www.youtube.com/embed/Q2krzp16X_E"
            }, 
            {
            "word": "Concussion n", 
            "synonym": "Collapse, coma.", 
            "example": "He's been dizzy and  confused since the accident. Do you think he has concussion?", 
            "video": "https://www.youtube.com/embed/gNmCqqBOKiU up to 0:16 second"
            }, 
            {
            "word": "Condemn sb to do sth", 
            "synonym": "Execute, capital punishment", 
            "example": "She was condemned to death and executed two weeks later.", 
            "video": ""
            }, 
            {
            "word": "Condemn", 
            "synonym": "Criticize, disapprove", 
            "example": "The terrorist action has been condemned as an act of barbarism and  cowardice.", 
            "video": "https://www.youtube.com/embed/2V9eFp879II"
            }, 
            {
            "word": "Condemned", 
            "synonym": "Hung, behead.", 
            "example": "The country condemns the use of violence on prisoners.", 
            "video": "https://www.youtube.com/embed/95eJQrmabdY"
            }, 
            {
            "word": "Condensation", 
            "synonym": "Precipitation, smog.", 
            "example": "We get a lot of condensation on the walls in the winter.", 
            "video": "https://www.youtube.com/embed/meEpXF6A56U"
            }, 
            {
            "word": "Condense", 
            "synonym": "Lessen, absorb.", 
            "example": "I condensed ten pages of  comments into/to two.", 
            "video": "https://www.youtube.com/embed/WwOfeyaIqA4 up to 0:16 second"
            }, 
            {
            "word": "Condenser", 
            "synonym": "Capacitor, evaporating dish", 
            "example": "The condenser is a flat rectangular wooden vessel, which is surrounded with another one containing cold water.", 
            "video": "https://www.youtube.com/embed/1JQxZVQftd0  up to 0:16 second"
            }, 
            {
            "word": "Condescend to do sth", 
            "synonym": "", 
            "example": "I wonder if Michael will condescend to visit us?", 
            "video": ""
            }, 
            {
            "word": "Condescend to sb", 
            "synonym": "", 
            "example": "He explains things without condescending  to his audience.", 
            "video": "https://www.youtube.com/embed/TNEtRz1cQn8 up to 0:40 second"
            }, 
            {
            "word": "Condiment", 
            "synonym": "Curry powder, spice.", 
            "example": "But put an extra condiment into your dish, and it will poison you.", 
            "video": "https://www.youtube.com/embed/h6yqnYrMFSU"
            }, 
            {
            "word": "Conditioner", 
            "synonym": "", 
            "example": "Conditioner makes hair silky and smooth.", 
            "video": "https://www.youtube.com/embed/19VskVrnENg from 0:10 second"
            }, 
            {
            "word": "Condo", 
            "synonym": "Rest home, apartment", 
            "example": "She was too lively to be trapped in the condo on her own.", 
            "video": "https://www.youtube.com/embed/f9y2K9zuqgE"
            }, 
            {
            "word": "Condolence", 
            "synonym": "Solace, sympathy.", 
            "example": "Dignitaries from all over the world came to offer their condolences.", 
            "video": "https://www.youtube.com/embed/xD4I2_JTqyY"
            }, 
            {
            "word": "Condominium", 
            "synonym": "", 
            "example": "The condominium smelled of breakfast, and he looked around, satisfied to find it clean again.", 
            "video": "https://www.youtube.com/embed/p695Tl"
            }, 
            {
            "word": "Condominium", 
            "synonym": "Territory, country.", 
            "example": "We are the citizens of an independent condominium.", 
            "video": "https://www.youtube.com/embed/p695Tl"
            }, 
            {
            "word": "Condone", 
            "synonym": "Disregard, deliberately ignore.", 
            "example": "The college cannot condone any behaviour that involves illicit drugs.", 
            "video": "https://www.youtube.com/embed/ODtATDPpi4k"
            }, 
            {
            "word": "Condor", 
            "synonym": "New World Vulture, andean condor.", 
            "example": "The largest bird is the condor, and there is another bird of the vulture tribe, with a black and white wing feather formerly used by the Incas in their head", 
            "video": "https://www.youtube.com/embed/XIGQtUG5YX0"
            }, 
            {
            "word": "Conducive", 
            "synonym": "Productive of,instrumental in.", 
            "example": "The harsh lights and cameras were hardly conducive to a relaxed atmosphere.", 
            "video": "https://www.youtube.com/embed/hH4eQmPe5kE"
            }, 
            {
            "word": "Conduct yourself", 
            "synonym": "", 
            "example": "I trust you will conduct yourself properly while you are staying with your French host family.", 
            "video": ""
            }, 
            {
            "word": "Conduct", 
            "synonym": "Accompaniment, performance.", 
            "example": "The orchestra was conducted by Mira Shapur.", 
            "video": "https://www.youtube.com/embed/dnyfC3XYR1s  up to 0:13 second"
            }, 
            {
            "word": "Conduct", 
            "synonym": "Lead, guide.", 
            "example": "He conducted us through his personal gallery of the Civil War.", 
            "video": "https://www.youtube.com/embed/dnyfC3XYR1s up to 0:08 second"
            }, 
            {
            "word": "Conduct", 
            "synonym": "Manage, direction.", 
            "example": "The experiments were conducted by scientists in New York.", 
            "video": "https://www.youtube.com/embed/_49Ye9PO"
            }, 
            {
            "word": "Conduction", 
            "synonym": "Generation, flow.", 
            "example": "His most important work was concerned with the conduction of heat and with spectroscopy.", 
            "video": "https://www.youtube.com/embed/7qtsUzPkhbI up to 0:09 second"
            }, 
            {
            "word": "Conduit", 
            "synonym": "Plumb, pipeline.", 
            "example": "Here two reservoirs of a combined capacity of 668 million gallons have been constructed, and a conduit some 36 m.", 
            "video": "https://www.youtube.com/embed/RGqaXgC"
            }, 
            {
            "word": "Cone sth off", 
            "synonym": "", 
            "example": "Part of the road had been coned off for repair work.", 
            "video": ""
            }, 
            {
            "word": "Cone", 
            "synonym": "Conical surface, cornet.", 
            "example": "It was holding two brown, dried and dead flowers that were shaped like cones with lots of buds covering it.", 
            "video": "https://www.youtube.com/embed/RHQw2cxh1LA"
            }, 
            {
            "word": "Cone", 
            "synonym": "Cornet, funnel.", 
            "example": "I was able to hold the ice", 
            "video": ""
            }, 
            {
            "word": "Cone", 
            "synonym": "Pine cone, acorn.", 
            "example": "Then he walked ahead, kicking a pine cone.", 
            "video": ""
            }, 
            {
            "word": "Confection", 
            "synonym": "Fairy cake, baked goods.", 
            "example": "Her favorite desert is fruit cake confection.", 
            "video": "https://www.youtube.com/embed/q1mFNAkerQw"
            }, 
            {
            "word": "Confectioners sugar", 
            "synonym": "Caster sugar, powdered sugar.", 
            "example": "Begin adding 1 cup sifted confectioners sugar, 1 tablespoon at a time.", 
            "video": "https://www.youtube.com/embed/L3M0Z0pRk08"
            }, 
            {
            "word": "Confederacy", 
            "synonym": "Alliance, federation.", 
            "example": "The Italian confederacy is known as the Lombard League.", 
            "video": "https://www.youtube.com/embed/jRRi9lLYyvs"
            }, 
            {
            "word": "Confederate", 
            "synonym": "Associate, partner.", 
            "example": "Where was his confederate, the girl who had stolen Richard's wallet?", 
            "video": ""
            }, 
            {
            "word": "Confer", 
            "synonym": "Award to, honour with.", 
            "example": "An honorary doctorate was conferred on him by Columbia University.", 
            "video": ""
            }, 
            {
            "word": "Confer", 
            "synonym": "Speak, converse.", 
            "example": "The officials were conferring with allies.", 
            "video": "https://www.youtube.com/embed/fqIzME4fZzE"
            }, 
            {
            "word": "Conference call", 
            "synonym": "Teleconference, meeting.", 
            "example": "The conference call has been rearranged for later in the week.", 
            "video": "https://www.youtube.com/embed/zjFoyEQQlSA"
            }, 
            {
            "word": "Confess", 
            "synonym": "Reveal, admit.", 
            "example": "He confessed that he had attacked the old man.", 
            "video": "https://www.youtube.com/embed/eCHy58kRvVo"
            }, 
            {
            "word": "Confessional", 
            "synonym": "Kiosk, confession chair.", 
            "example": "He had stood there, indeed, from the moment of the girl's entrance into the confessional.", 
            "video": "https://www.youtube.com/embed/xIusz_LTj0c"
            }, 
            {
            "word": "Confessor", 
            "synonym": "Priest, bishop.", 
            "example": "She sent for her confessor because she was in mortal sin.", 
            "video": "https://www.youtube.com/embed/m1zseZwwTdA"
            }, 
            {
            "word": "Confetti", 
            "synonym": "Colored paper", 
            "example": "The winning team was showered with confetti.", 
            "video": "https://www.youtube.com/embed/oVD554Pfw00"
            }, 
            {
            "word": "Confidant", 
            "synonym": "Crony,  intimate.", 
            "example": "In London he became Pip's intimate confidant.", 
            "video": "https://www.youtube.com/embed/22yiUo_SMMU"
            }, 
            {
            "word": "Confide in sb", 
            "synonym": "", 
            "example": "He's nice, but I don't feel I can confide in her.", 
            "video": ""
            }, 
            {
            "word": "Confidence trick", 
            "synonym": "", 
            "example": "They were the innocent victims of an elaborate confidence trick.", 
            "video": "https://www.yoube.com/watch?v=WT6J_NQbx4Itu"
            }, 
            {
            "word": "Confidence", 
            "synonym": "Conviction, Credence.", 
            "example": "Lack of confidence makes a person look weak.", 
            "video": "https://www.youtube.com/embed/hXm9Hdxavag"
            }, 
            {
            "word": "Confidential", 
            "synonym": "Private, personal", 
            "example": "These documents are strictly confidential.", 
            "video": "https://www.youtube.com/embed/0QNTc"
            }, 
            {
            "word": "Confidentiality", 
            "synonym": "Private, secret.", 
            "example": "The lead bank's duty of confidentiality to the borrower.", 
            "video": "https://www.youtube.com/embed/2x2kdwFYJuI"
            }, 
            {
            "word": "Configuration", 
            "synonym": "Format, arrangement.", 
            "example": "We tried the furniture in different configurations to see which fit best.", 
            "video": "https://www.youtube.com/embed/2TMWE2WJFOU"
            }, 
            {
            "word": "Confines", 
            "synonym": "Limit, restrict.", 
            "example": "Within the confines of the hall escape was difficult.", 
            "video": "https://www.youtube.com/embed/NMUzNYxilOI up to 0:08"
            }, 
            {
            "word": "Confirmation", 
            "synonym": "Affirmation, avowal.", 
            "example": "The kind of joy mixed with tears one finds at weddings and confirmations, is really heart", 
            "video": "https://www.youtube.com/embed/uivBu0NMUdQ  from 0:16 second"
            }, 
            {
            "word": "Confirmation", 
            "synonym": "Verification, proof.", 
            "example": "High unemployment figures were further confirmation that the economy was in recession", 
            "video": "https://www.youtube.com/embed/uivBu0NMUdQ  up to 0:15 second"
            }, 
            {
            "word": "Confiscate", 
            "synonym": "Expropriate, seize.", 
            "example": "Miss Edwards confiscated my phone!", 
            "video": "https://www.youtube.com/embed/7l0mVifmmok"
            }, 
            {
            "word": "Confit", 
            "synonym": "", 
            "example": "In Spain and France, squab is also preserved as a confit.", 
            "video": "https://www.youtube.com/embed/V5qP4AFtg7E up to 0:43 second"
            }, 
            {
            "word": "Conflagration", 
            "synonym": "Inferno, blaze.", 
            "example": "Tinder", 
            "video": "https://www.youtube.com/embed/TfbXHRU50rI up to 0:13 second"
            }, 
            {
            "word": "Conflate", 
            "synonym": "Aggregate, amalgamate.", 
            "example": "She conflated the three plays to produce a fresh new work.", 
            "video": "https://www.youtube.com/embed/ziBuK9C8dBo from 0:11 second"
            }, 
            {
            "word": "Conflicted", 
            "synonym": "Uncertain, debatable.", 
            "example": "It seems that politicians like ordinary citizens are conflicted about gambling.", 
            "video": "https://www.youtube.com/embed/K2Pc4jSAgfU"
            }, 
            {
            "word": "Confluence", 
            "synonym": "Junction, convergence.", 
            "example": "The confluence of the Rivers Ouse and Foss.", 
            "video": "https://www.youtube.com/embed/Fh8V2unLJmg  up to 0:17 second"
            }, 
            {
            "word": "Conform to/ with sth", 
            "synonym": "", 
            "example": "Before buying the baby's car seat , make sure that it conforms to the official safety standards.", 
            "video": ""
            }, 
            {
            "word": "Conformity", 
            "synonym": "Conventionalism, traditionalism.", 
            "example": "It's depressing how much conformity there is in such young child.", 
            "video": "https://www.youtube.com/embed/u_WB_IV3iOA"
            }, 
            {
            "word": "Confound", 
            "synonym": "Surprise, startle.", 
            "example": "An  elderly man from Hull has confounded doctors by recovering after he was officially declared dead.", 
            "video": "https://www.youtube.com/embed/WeSc3Jq87XI"
            }, 
            {
            "word": "Confront sb with sth", 
            "synonym": "", 
            "example": "I know she's the one who made the error, but I don't want to confront her with it without having any hard evidence.", 
            "video": ""
            }, 
            {
            "word": "Confront", 
            "synonym": "Resist, tackle.", 
            "example": "As she left the court, she was confronted by angry crowds who tried to block her way.", 
            "video": "https://www.youtube.com/embed/Kkauc"
            }, 
            {
            "word": "Confusion marketing", 
            "synonym": "", 
            "example": "Unilever and P&G sometimes plays the game of confusion marketing.", 
            "video": ""
            }, 
            {
            "word": "Confute", 
            "synonym": "Contradict, refute", 
            "example": "Both of these confessions were drawn up to confute the teaching of a remarkable man who had been patriarch of Constantinople, Cyril Lucar.", 
            "video": "https://www.youtube.com/embed/5r1blkSWM4k up to 0:10 second"
            }, 
            {
            "word": "Conga", 
            "synonym": "Waltz, samba.", 
            "example": "He plays the conga drums to the heavy rock music from the huge house speakers.", 
            "video": "https://www.youtube.com/embed/9zZ_p4a8ZWc"
            }, 
            {
            "word": "Congeal", 
            "synonym": "Clot, coagulate.", 
            "example": "The blood had congealed in thick black clots.", 
            "video": "https://www.youtube.com/embed/kPrbFf0FCgA up to 0:14 second"
            }, 
            {
            "word": "Congenial", 
            "synonym": "Compatible, kindred.", 
            "example": "This expression was the result, no doubt, of his strenuous training and the comparative lack of congenial friendships.", 
            "video": "https://www.youtube.com/embed/cPYMl_a0QB8"
            }, 
            {
            "word": "Congenital", 
            "synonym": "Hereditary, inborn.", 
            "example": "In a congenital condition known as haemophylia, it is difficult to stop the flow of blood.", 
            "video": "https://www.youtube.com/embed/kggOLyDLy"
            }, 
            {
            "word": "Conger eel", 
            "synonym": "", 
            "example": "The life histories of most conger eels are poorly known.", 
            "video": "https://www.youtube.com/embed/BRWGa96SHl4"
            }, 
            {
            "word": "Congestion", 
            "synonym": "Crowding, overcrowding", 
            "example": "The traffic congestion in Belo Horizonte is an issue that can't be ignored.", 
            "video": "https://www.youtube.com/embed/agCtYArVHdI up to 0:22 second"
            }, 
            {
            "word": "Congestion", 
            "synonym": "Overcrowding,  crowding", 
            "example": "They called it acute congestion of the stomach and brain.", 
            "video": "https://www.youtube.com/embed/agCtYArVHdI  up to 0:11 second"
            }, 
            {
            "word": "Conglomerate", 
            "synonym": "Agglomerate, aggregate.", 
            "example": "A conglomerate at the base contains traces of gold.", 
            "video": "https://www.youtube.com/embed/NnGZ25UqaYA"
            }, 
            {
            "word": "Congregate", 
            "synonym": "Gather, assemble.", 
            "example": "Some 4,000 demonstrators had congregated at a border point.", 
            "video": "https://www.youtube.com/embed/gnvrqaGoJIM"
            }, 
            {
            "word": "Congressional", 
            "synonym": "Decreeing, senatorial.", 
            "example": "He called for a congressional investigation.", 
            "video": "https://www.youtube.com/embed/SvuYc14jssE"
            }, 
            {
            "word": "Congruent", 
            "synonym": "Consistency, compatibility.", 
            "example": "The rules may not be congruent with the requirements of the law.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Conical flask", 
            "synonym": "Erlenmeyer flask", 
            "example": "A solution chlorine spilled from the conical flask.", 
            "video": "https://www.youtube.com/embed/J1lkQL5WeF4"
            }, 
            {
            "word": "Conifer", 
            "synonym": "Pine, cedar.", 
            "example": "A mixed forest of deciduous and conifer trees formed a dense covering of mottled greens.", 
            "video": "https://www.youtube.com/embed/zLNNlcTdgAo"
            }, 
            {
            "word": "Conjecture", 
            "synonym": "Speculation, guess.", 
            "example": "Conjectures about the newcomer were many and varied.", 
            "video": "https://www.youtube.com/embed/fqALxbUtnyU up to 0:11 second"
            }, 
            {
            "word": "Conjoined twins", 
            "synonym": "Siamese twins", 
            "example": "", 
            "video": "https://www.youtube.com/embed/bm3RbjDyLRg"
            }, 
            {
            "word": "Conjunctivitis", 
            "synonym": "Inflammation, Pink eye.", 
            "example": "One of the common forms of allergy complication is conjunctivitis.", 
            "video": "https://www.youtube.com/embed/yfOk_ldiIUs"
            }, 
            {
            "word": "Conjure sb/ sth up", 
            "synonym": "", 
            "example": "Conjuring a dead spirit, and asking them question was a part of culture of some African tribes.", 
            "video": ""
            }, 
            {
            "word": "Conjure sth up", 
            "synonym": "", 
            "example": "How am I expected to conjure up a meal for six of his friends with almost nothing in the fridge?", 
            "video": ""
            }, 
            {
            "word": "Conjure sth up", 
            "synonym": "", 
            "example": "The glittering  conjured up images of Russia's imperial past.", 
            "video": ""
            }, 
            {
            "word": "Conjure", 
            "synonym": "Magic, materialize.", 
            "example": "The magician was able to conjure a rabbit out of his empty top hat.", 
            "video": "https://www.youtube.com/embed/Ln0UPGZsuzg"
            }, 
            {
            "word": "Conk out", 
            "synonym": "", 
            "example": "He was so tired after his long day at work that he conked out during the movie.", 
            "video": "https://www.youtube.com/embed/8N"
            }, 
            {
            "word": "Conk out", 
            "synonym": "Act, burn.", 
            "example": "After a six", 
            "video": "https://www.youtube.com/embed/8N"
            }, 
            {
            "word": "Conk", 
            "synonym": "Decease, hit.", 
            "example": "See the baby, then conk out on the stupid chair/cot.", 
            "video": ""
            }, 
            {
            "word": "Conk", 
            "synonym": "Nostril, nose.", 
            "example": "She had a hooked conk.", 
            "video": "https://www.youtube.com/embed/_w9_vli9ksE from 0:19"
            }, 
            {
            "word": "Conker", 
            "synonym": "Seed, horse chestnut.", 
            "example": "He put the conker in his pocket, dimly remembering.", 
            "video": "https://www.youtube.com/embed/PCh8hLyK"
            }, 
            {
            "word": "Conkers", 
            "synonym": "Catch, blind manís buff.", 
            "example": "Every year, since 1991, the French conkers championship is held in the village.", 
            "video": ""
            }, 
            {
            "word": "Connect", 
            "synonym": "Aggregate, conjunction.", 
            "example": "Your flight arrives at 12.30, when it connects with a bus service to your hotel.", 
            "video": "https://www.youtube.com/embed/KAaePEO8ysM"
            }, 
            {
            "word": "Connecting rod", 
            "synonym": "", 
            "example": "The connecting rods connect the piston to the crankshaft.", 
            "video": "https://www.youtube.com/embed/3Vk3MyqVkwQ"
            }, 
            {
            "word": "Connection", 
            "synonym": "Link, join.", 
            "example": "Yoga is an ancient health practice that focuses on the mind", 
            "video": "https://www.youtube.com/embed/VSnb0Crfha0 up to 0:12 second"
            }, 
            {
            "word": "Connections", 
            "synonym": "Association, network.", 
            "example": "What if the capability to see connections and even to have them detected was all there for us?", 
            "video": ""
            }, 
            {
            "word": "Connective tissue", 
            "synonym": "Combinatorial, conjoining.", 
            "example": "Does cancer destroys connective tissue even?", 
            "video": "https://www.youtube.com/embed/DAG0t3tDTh8"
            }, 
            {
            "word": "Connectivity", 
            "example": "Your paragraph misses connectivity among different lines.", 
            "video": ""
            }, 
            {
            "word": "Connivance", 
            "synonym": "Allow, permit.", 
            "example": "Their appalling treatment of their child could only have happened with the connivance of their neighbours.", 
            "video": "https://www.youtube.com/embed/jCCJK6mjlqI"
            }, 
            {
            "word": "Connoisseur", 
            "synonym": "Specialist, cognoscente.", 
            "example": "He was a well", 
            "video": "https://www.youtube.com/embed/2MFP4ukv5oA"
            }, 
            {
            "word": "Connote", 
            "synonym": "Suggest, imply.", 
            "example": "To me, chocolate connotes pleasure and indulgence.", 
            "video": "https://www.youtube.com/embed/6cH21XT2dSI"
            }, 
            {
            "word": "Connubial", 
            "synonym": "Married, conjugal.", 
            "example": "The new coupleís face showed connubial happiness.", 
            "video": "https://www.youtube.com/embed/4051AZ_RtJM"
            }, 
            {
            "word": "Conquer", 
            "synonym": "Beat, defeat", 
            "example": "You will conquer the worlds.", 
            "video": "https://www.youtube.com/embed/8J2bx2PXGv0"
            }, 
            {
            "word": "Conquer", 
            "synonym": "Defeat, beat", 
            "example": "The English were conquered by the Normans in 1066.", 
            "video": "https://www.youtube.com/embed/8J2bx2PXGv0 up to 0:15 second to 0:31 second"
            }, 
            {
            "word": "Conscience", 
            "synonym": "", 
            "example": "She was conscience", 
            "video": ""
            }, 
            {
            "word": "Conscience", 
            "synonym": "Moral, ethic.", 
            "example": "My conscience would really bother me if I wore a fur coat.", 
            "video": "https://www.youtube.com/embed/OZoQC1LFXK0"
            }, 
            {
            "word": "Conscientious", 
            "synonym": "Diligent, painstaking", 
            "example": "She is conscientious and hardworking.", 
            "video": "https://www.youtube.com/embed/nqMuY37ob8E"
            }, 
            {
            "word": "Conscientious", 
            "synonym": "Strenuous, painstaking.", 
            "example": "She is a conscientious student.", 
            "video": "https://www.youtube.com/embed/nqMuY37ob8E"
            }, 
            {
            "word": "Conscript", 
            "synonym": "Call ñup, commission.", 
            "example": "He was conscripted into the army at the age of 18.", 
            "video": "https://www.youtube.com/embed/nruT0Se4EgI"
            }, 
            {
            "word": "Consecrate", 
            "synonym": "Anoint, baptize.", 
            "example": "The new cathedral was completed and consecrated in 2002.", 
            "video": "https://www.youtube.com/embed/efP8XZuLA"
            }, 
            {
            "word": "Consecutive", 
            "example": "This is the fifth consecutive weekend that I've spent working.", 
            "video": "https://www.youtube.com/embed/imt5CxMjc3c"
            }, 
            {
            "word": "Consensual", 
            "synonym": "Assent, accept.", 
            "example": "The woman alleged rape, but Reeves insisted it was consensual.", 
            "video": "https://www.youtube.com/embed/iZU1jaG2APY up to 0:15 second"
            }, 
            {
            "word": "Consent", 
            "synonym": "Assent, agreement", 
            "example": "You can't come without your parents' consent.", 
            "video": "https://www.youtube.com/embed/zlHWjiBNbXQ"
            }, 
            {
            "word": "Consent", 
            "synonym": "Embrace, accept.", 
            "example": "They can't publish your name without your consent.", 
            "video": "https://www.youtube.com/embed/zlHWjiBNbXQ up to 0:09 second"
            }, 
            {
            "word": "Conservatism", 
            "synonym": "Traditionalism, orthodoxy.", 
            "example": "The conservatism of the group's fans even spread to the band members themselves.", 
            "video": "https://www.youtube.com/embed/pRByPYS2A48"
            }, 
            {
            "word": "Conservative", 
            "synonym": "Conventional, orthodox", 
            "example": "Older people tend to be very conservative.", 
            "video": "https://www.youtube.com/embed/lJRqIwNfJIA"
            }, 
            {
            "word": "Conservatory", 
            "synonym": "Convent,  coeducational.", 
            "example": "The conservatory is maintained by municipal appropriations.", 
            "video": ""
            }, 
            {
            "word": "Conservatory", 
            "synonym": "Double room, glass house.", 
            "example": "Great variety of design is admissible in the conservatory, but it ought always to be adapted to the style of the mansion of which it is a prominent appendage.", 
            "video": ""
            }, 
            {
            "word": "Consider it done", 
            "synonym": "", 
            "example": "'Could you give me a copy of this page, please?' 'Consider it done.'", 
            "video": ""
            }, 
            {
            "word": "Considerate", 
            "synonym": "Helpful, cooperative", 
            "example": "He is always a kind and considerate host.", 
            "video": "https://www.youtube.com/embed/xJWJ2Ymrv"
            }, 
            {
            "word": "Consideration", 
            "synonym": "", 
            "example": "His health has to be the prime consideration", 
            "video": ""
            }, 
            {
            "word": "Consideration", 
            "synonym": "", 
            "example": "It is time for companies to show more consideration for their public image.", 
            "video": ""
            }, 
            {
            "word": "Consideration", 
            "synonym": "", 
            "example": "You can buy the books for a small consideration", 
            "video": ""
            }, 
            {
            "word": "Consideration", 
            "synonym": "", 
            "example": "Your case needs very careful consideration.", 
            "video": ""
            }, 
            {
            "word": "Considered opinion/view/decision", 
            "synonym": "", 
            "example": "It is my considered opinion that tomatoes are not that great in pizzas.", 
            "video": ""
            }, 
            {
            "word": "Consign sb/sth to sth", 
            "synonym": "", 
            "example": "He consigned the document to the bin.", 
            "video": ""
            }, 
            {
            "word": "Consign", 
            "synonym": "", 
            "example": "She consigned four books to Lisaís.", 
            "video": "https://www.youtube.com/embed/R10lwGTooys"
            }, 
            {
            "word": "Consist in sth", 
            "synonym": "", 
            "example": "Her writing consisted in the use of cynical language.", 
            "video": ""
            }, 
            {
            "word": "Consist in", 
            "synonym": "Comprising and consisting of.", 
            "example": "The beauty of air travel consists in its speed and ease.", 
            "video": "https://www.youtube.com/embed/Dy85YtNX8Gc"
            }, 
            {
            "word": "Consist of sth", 
            "synonym": "", 
            "example": "The gang consists of 8 girls.", 
            "video": ""
            }, 
            {
            "word": "Consist of", 
            "synonym": "Comprising and consisting of.", 
            "example": "Breakfast, such as it was, consisted of a plain roll and a cup of coffee.", 
            "video": "https://www.youtube.com/embed/0I13xEV8PiE"
            }, 
            {
            "word": "Consistent", 
            "synonym": "", 
            "example": "The wounds are consistent with a knife cut.", 
            "video": ""
            }, 
            {
            "word": "Consistent", 
            "synonym": "", 
            "example": "There was consistent reminder of the exam duration.", 
            "video": ""
            }, 
            {
            "word": "Consolation", 
            "synonym": "", 
            "example": "There was consolation prize for all the children at the race.", 
            "video": ""
            }, 
            {
            "word": "Console", 
            "synonym": "", 
            "example": "Mary went to to console Linda after her father died.", 
            "video": ""
            }, 
            {
            "word": "Console", 
            "synonym": "", 
            "example": "Video game console are great for amateur gamers.", 
            "video": ""
            }, 
            {
            "word": "Consolidate", 
            "synonym": "", 
            "example": "The company consolidated its position after the merger.", 
            "video": ""
            }, 
            {
            "word": "ConsommÈ", 
            "synonym": "", 
            "example": "ConsommÈ is hard to make, it turns out watery easily.", 
            "video": "https://www.youtube.com/embed/N08TA3wET1U"
            }, 
            {
            "word": "Consort", 
            "synonym": "", 
            "example": "He consorted with the wrong type of people which lead to his demise.", 
            "video": ""
            }, 
            {
            "word": "Consort", 
            "synonym": "", 
            "example": "The queen consort of England is Prince Philip.", 
            "video": ""
            }, 
            {
            "word": "Consortium", 
            "synonym": "", 
            "example": "Most major industries are under a consortium.", 
            "video": ""
            }, 
            {
            "word": "Conspicuous consumption", 
            "synonym": "", 
            "example": "The hotels were seen as monuments to conspicuous consumption.", 
            "video": ""
            }, 
            {
            "word": "Conspicuous", 
            "synonym": "", 
            "example": "He tried to hide but he was quite conspicuous.", 
            "video": "https://www.youtube.com/embed/f01"
            }, 
            {
            "word": "Conspiracy of silence", 
            "synonym": "", 
            "example": "The government took part in a conspiracy of silence over population.", 
            "video": ""
            }, 
            {
            "word": "Conspiracy theorist", 
            "synonym": "", 
            "example": "Conspiracy theorist are usually mad people but some do get it right.", 
            "video": ""
            }, 
            {
            "word": "Conspiracy", 
            "synonym": "", 
            "example": "A conspiracy to overthrow the government is afoot.", 
            "video": ""
            }, 
            {
            "word": "Conspiratorial", 
            "synonym": "", 
            "example": "The KKK was charged with conspiratorial plot regarding the minorities.", 
            "video": ""
            }, 
            {
            "word": "Conspire against sth", 
            "synonym": "", 
            "example": "Brutus conspired to kill Cesar.", 
            "video": ""
            }, 
            {
            "word": "Constable", 
            "synonym": "", 
            "example": "The constable was a nice man and helped me find my missing bike.", 
            "video": ""
            }, 
            {
            "word": "Constabulary", 
            "synonym": "", 
            "example": "The constabulary in my area wear bright yellow uniforms.", 
            "video": "https://www.youtube.com/embed/3qcR0dbpn5c"
            }, 
            {
            "word": "Constancy", 
            "synonym": "", 
            "example": "Dogs have a constancy of always being energetic.", 
            "video": ""
            }, 
            {
            "word": "Constancy", 
            "synonym": "", 
            "example": "Olive was a big believer of constancy.", 
            "video": ""
            }, 
            {
            "word": "Constellation", 
            "synonym": "", 
            "example": "Zodiac sign are dependent on the constellations.", 
            "video": ""
            }, 
            {
            "word": "Consternation", 
            "synonym": "", 
            "example": "To her consternation her car would not start.", 
            "video": ""
            }, 
            {
            "word": "Constipation", 
            "synonym": "", 
            "example": "Constipation might sound silly but it can lead to death if not taken care of.", 
            "video": ""
            }, 
            {
            "word": "Constituency", 
            "synonym": "", 
            "example": "When an incompetent leader is chosen you can blame the constituency.", 
            "video": "https://www.youtube.com/embed/jaqLkmGhJQQ"
            }, 
            {
            "word": "Constitute", 
            "synonym": "Compose, comprise", 
            "example": "This defeat constitutes a real setback for their championship hopes.", 
            "video": "https://www.youtube.com/embed/UDUShTlne8Y"
            }, 
            {
            "word": "Constitution", 
            "synonym": "", 
            "example": "My grandfatherís constitution has deteriorated over the years.", 
            "video": ""
            }, 
            {
            "word": "Constitution", 
            "synonym": "", 
            "example": "The US constitution was among the first to leave out monarchy.", 
            "video": ""
            }, 
            {
            "word": "Constitution", 
            "synonym": "", 
            "example": "The genetic constitution of an ape is similar to that of a human.", 
            "video": ""
            }, 
            {
            "word": "Constitutional monarchy", 
            "synonym": "", 
            "example": "The UK runs on constitutional monarchy.", 
            "video": ""
            }, 
            {
            "word": "Constrained to do sth", 
            "synonym": "", 
            "example": "Richard felt constrained to explain himself.", 
            "video": ""
            }, 
            {
            "word": "Constrict", 
            "synonym": "", 
            "example": "Constricted food supply lead to the ration system.", 
            "video": ""
            }, 
            {
            "word": "Constrict", 
            "synonym": "", 
            "example": "The python constricted its prey before swallowing it.", 
            "video": ""
            }, 
            {
            "word": "Construct", 
            "synonym": "", 
            "example": "Helen constructed a massive art piece outside our building.", 
            "video": ""
            }, 
            {
            "word": "Constructive dismissal", 
            "synonym": "", 
            "example": "Constructive dismissal is very common in the modern workplace.", 
            "video": ""
            }, 
            {
            "word": "Constructive", 
            "synonym": "", 
            "example": "Johnís positive attitude was constructive and welcomed.", 
            "video": ""
            }, 
            {
            "word": "Construe sth as sth", 
            "synonym": "", 
            "example": "Hiring many women can also be construed as being sexist.", 
            "video": ""
            }, 
            {
            "word": "Consul", 
            "synonym": "", 
            "example": "The American consul was very nice to the residents around him.", 
            "video": ""
            }, 
            {
            "word": "Consultancy", 
            "synonym": "", 
            "example": "The consultancy solved our problems efficiently.", 
            "video": ""
            }, 
            {
            "word": "Consumables", 
            "synonym": "", 
            "example": "When you travel on holiday limit your consumables.", 
            "video": "https://www.youtube.com/embed/C57Hu3hJuYY"
            }, 
            {
            "word": "Consume", 
            "synonym": "", 
            "example": "The army consumes lot more budget compared to health and education.", 
            "video": ""
            }, 
            {
            "word": "Consume", 
            "synonym": "", 
            "example": "The lighthouse was consumed by the waves.", 
            "video": ""
            }, 
            {
            "word": "Consumer durables", 
            "synonym": "", 
            "example": "The Chinese are not known for their consumer durables as it is bad for business.", 
            "video": ""
            }, 
            {
            "word": "Consumer price index", 
            "synonym": "", 
            "example": "Having a consumer price index can really help with buying a rare item.", 
            "video": ""
            }, 
            {
            "word": "Consumerism", 
            "synonym": "", 
            "example": "Consumerism is a plague that is destroying societies around the world.", 
            "video": ""
            }, 
            {
            "word": "Consummate", 
            "synonym": "", 
            "example": "She dressed with consummate elegance.", 
            "video": ""
            }, 
            {
            "word": "Consumption", 
            "synonym": "", 
            "example": "Steveís father died of consumption.", 
            "video": ""
            }, 
            {
            "word": "Consumption", 
            "synonym": "", 
            "example": "The consumption of alcohol in restaurants are limited.", 
            "video": ""
            }, 
            {
            "word": "Contact lens", 
            "synonym": "", 
            "example": "Coloured contact lenses are all the rage in fashion now.", 
            "video": ""
            }, 
            {
            "word": "Contact sport", 
            "synonym": "", 
            "example": "Contact sport has a lot of injuries.", 
            "video": ""
            }, 
            {
            "word": "Contact", 
            "synonym": "", 
            "example": "Contact with West Germany was forbidden for East Germans.", 
            "video": ""
            }, 
            {
            "word": "Contact", 
            "synonym": "", 
            "example": "I have a contact in the UN who can get you to the country you want to go to.", 
            "video": ""
            }, 
            {
            "word": "Contact", 
            "synonym": "", 
            "example": "Ronald put the contacts to his friends car battery for a jump start.", 
            "video": ""
            }, 
            {
            "word": "Contagion", 
            "synonym": "", 
            "example": "The small pox was the worst contagion in human history.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Contain", 
            "synonym": "", 
            "example": "The police tried to contain the riot.", 
            "video": ""
            }, 
            {
            "word": "Contain", 
            "synonym": "", 
            "example": "The tin contains baked beans.", 
            "video": ""
            }, 
            {
            "word": "Containerise", 
            "synonym": "", 
            "example": "Most goods that travel by sea are containerised.", 
            "video": ""
            }, 
            {
            "word": "Containment", 
            "synonym": "", 
            "example": "The American CDC is responsible for containment of viral diseases.", 
            "video": ""
            }, 
            {
            "word": "Contaminant", 
            "synonym": "", 
            "example": "Contaminants in science labs can cause serious problems in experiments.", 
            "video": ""
            }, 
            {
            "word": "Contaminate", 
            "synonym": "", 
            "example": "The water was contaminated by the shoe factory.", 
            "video": ""
            }, 
            {
            "word": "Contemplate", 
            "synonym": "", 
            "example": "He could not even begin to contemplate the magnitude of his crime.", 
            "video": ""
            }, 
            {
            "word": "Contemporaneous", 
            "synonym": "", 
            "example": "Orwell was contemporaneous to the second World War.", 
            "video": "https://www.youtube.com/embed/i0txv4o4EFo"
            }, 
            {
            "word": "Contemporary", 
            "synonym": "", 
            "example": "Contemporary music is very complex compared to previous generations.", 
            "video": ""
            }, 
            {
            "word": "Contempt of court", 
            "synonym": "", 
            "example": "The judge jailed him for one night because of contempt of court.", 
            "video": ""
            }, 
            {
            "word": "Contempt", 
            "synonym": "", 
            "example": "I have nothing but contempt for criminals.", 
            "video": ""
            }, 
            {
            "word": "Contemptible", 
            "synonym": "", 
            "example": "Lying politicians are contemptible.", 
            "video": ""
            }, 
            {
            "word": "Contend with sth", 
            "synonym": "", 
            "example": "She had to contend with his massive debt.", 
            "video": ""
            }, 
            {
            "word": "Contend", 
            "synonym": "", 
            "example": "The basket ball team was contending for success over their competitors.", 
            "video": ""
            }, 
            {
            "word": "Contend", 
            "synonym": "", 
            "example": "The plaintiffs contended that their business plan was confidential.", 
            "video": ""
            }, 
            {
            "word": "Contender", 
            "synonym": "", 
            "example": "The contender in the gladiator fight was small and weak.", 
            "video": ""
            }, 
            {
            "word": "Content yourself with sth", 
            "synonym": "", 
            "example": "Sussie was contented herself with just the idea of a stable job.", 
            "video": ""
            }, 
            {
            "word": "Contention", 
            "synonym": "", 
            "example": "Richardís contention that all cows were watching him was just silly.", 
            "video": ""
            }, 
            {
            "word": "Contention", 
            "synonym": "", 
            "example": "The contention over the prize money lead a long law suite.", 
            "video": ""
            }, 
            {
            "word": "Contentment", 
            "synonym": "", 
            "example": "After eating the full pizza John had contentment written over his face.", 
            "video": ""
            }, 
            {
            "word": "Contest", 
            "synonym": "", 
            "example": "A laziness contest is paradoxical.", 
            "video": ""
            }, 
            {
            "word": "Contest", 
            "synonym": "", 
            "example": "Elizabeth contested that her way of rule was better.", 
            "video": ""
            }, 
            {
            "word": "Contest", 
            "synonym": "", 
            "example": "He tried to contest the throne over his older brother.", 
            "video": ""
            }, 
            {
            "word": "Context", 
            "synonym": "", 
            "example": "Without context the meaning changes in most situation.", 
            "video": ""
            }, 
            {
            "word": "Context", 
            "synonym": "Surroundings, circumstances", 
            "example": "In this exercise, a word is blanked out and you have to guess what it is by looking at the context.", 
            "video": "https://www.youtube.com/embed/DLgSi8Z6Q6A from 0:07 to 0:21 second"
            }, 
            {
            "word": "Contiguous", 
            "synonym": "", 
            "example": "America and Mexico are contiguous.", 
            "video": "https://www.youtube.com/embed/jgtm6pgcScQ"
            }, 
            {
            "word": "Continent n", 
            "synonym": "", 
            "example": "Asia is the largest continent.", 
            "video": ""
            }, 
            {
            "word": "Continental breakfast", 
            "synonym": "", 
            "example": "The continental breakfast served at the hotel was rather refreshing.", 
            "video": ""
            }, 
            {
            "word": "Continental crust", 
            "synonym": "", 
            "example": "Continental crust was the reason for land plants and animals.", 
            "video": ""
            }, 
            {
            "word": "Continental drift", 
            "synonym": "", 
            "example": "Continental drifts cause earthquakes.", 
            "video": ""
            }, 
            {
            "word": "Continental plate", 
            "synonym": "", 
            "example": "Himalayas was the product of two continental plates colliding.", 
            "video": ""
            }, 
            {
            "word": "Continental quilt", 
            "synonym": "", 
            "example": "Continental quilt are extremely nice to use during winter.", 
            "video": ""
            }, 
            {
            "word": "Continental shelf", 
            "synonym": "", 
            "example": "Continental shelf mark the start of oceans.", 
            "video": ""
            }, 
            {
            "word": "Contingency", 
            "synonym": "", 
            "example": "There are many contingency plans regarding succession of power in a government.", 
            "video": ""
            }, 
            {
            "word": "Contingent on /upon sth", 
            "synonym": "", 
            "example": "The fees were contingent on the success of the service.", 
            "video": ""
            }, 
            {
            "word": "Continuance", 
            "synonym": "", 
            "example": "The continuance of the negotiations is a positive sign.", 
            "video": ""
            }, 
            {
            "word": "Continuity", 
            "synonym": "", 
            "example": "Most movies have someone keeping tabs on the continuity of the plot.", 
            "video": "https://www.youtube.com/embed/Luob9fj9Knc"
            }, 
            {
            "word": "Continuum", 
            "synonym": "", 
            "example": "The continuum of the schools spending over a year is interesting.", 
            "video": "https://www.youtube.com/embed/IFDx5G_Wq2w"
            }, 
            {
            "word": "Contort", 
            "synonym": "", 
            "example": "His face contorted with laughter.", 
            "video": ""
            }, 
            {
            "word": "Contortionist", 
            "synonym": "", 
            "example": "Most contortionist have some sort of birth defect that allow them their flexibility.", 
            "video": ""
            }, 
            {
            "word": "Contour", 
            "synonym": "", 
            "example": "Rivers have shaped the contours of early civilisations.", 
            "video": ""
            }, 
            {
            "word": "Contraband", 
            "synonym": "", 
            "example": "Contraband in prisons is a common practice.", 
            "video": ""
            }, 
            {
            "word": "Contract in/out", 
            "synonym": "", 
            "example": "It is best to contract out of pyramid schemes.", 
            "video": ""
            }, 
            {
            "word": "Contract sth out", 
            "synonym": "", 
            "example": "Most companies contract out their customer services to developing countries.", 
            "video": ""
            }, 
            {
            "word": "Contract", 
            "synonym": "", 
            "example": "He contracted the bird flu and was hospitalised.", 
            "video": ""
            }, 
            {
            "word": "Contract", 
            "synonym": "", 
            "example": "The metal ring contracted when it cooled.", 
            "video": ""
            }, 
            {
            "word": "Contract", 
            "synonym": "", 
            "example": "They signed the contract and solidified the merger.", 
            "video": ""
            }, 
            {
            "word": "Contractile", 
            "synonym": "", 
            "example": "Contractile ability of muscles help us move.", 
            "video": ""
            }, 
            {
            "word": "Contractor", 
            "synonym": "", 
            "example": "My house was built using local contractors and they did a great job.", 
            "video": ""
            }, 
            {
            "word": "Contradict", 
            "synonym": "", 
            "example": "Jane: Be pa[t]ient with her, she is a lovely lady, although she doesn't like people to contradict her.", 
            "video": ""
            }, 
            {
            "word": "Contradiction", 
            "synonym": "", 
            "example": "Hypocritical people are always in contradiction with what they say and do.", 
            "video": ""
            }, 
            {
            "word": "Contraflow", 
            "synonym": "", 
            "example": "During road repairs it is common to see contraflow.", 
            "video": ""
            }, 
            {
            "word": "Contraindication", 
            "synonym": "", 
            "example": "The doctors contraindication toward surgery was a relief for everyone.", 
            "video": "https://www.youtube.com/embed/a0mUtk_"
            }, 
            {
            "word": "Contralto", 
            "synonym": "", 
            "example": "Contralto is really important in Italian opera.", 
            "video": ""
            }, 
            {
            "word": "Contraption", 
            "synonym": "", 
            "example": "Da Vinci was well know for his contraptions.", 
            "video": ""
            }, 
            {
            "word": "Contrapuntal", 
            "synonym": "", 
            "example": "The lawyer said the prosecutor was badgering his client as a contrapuntal.", 
            "video": ""
            }, 
            {
            "word": "Contrary to popular opinion", 
            "synonym": "", 
            "example": "To the contrary of popular belief the moon is not made of cheese.", 
            "video": ""
            }, 
            {
            "word": "Contrasting", 
            "synonym": "", 
            "example": "The quality of professional work was rather contrasting   to the work of an amateur.", 
            "video": ""
            }, 
            {
            "word": "Contravene", 
            "synonym": "", 
            "example": "He contravened the The Terrorist Act.", 
            "video": ""
            }, 
            {
            "word": "Contretemps", 
            "synonym": "", 
            "example": "Sarah had occasional contretemps with her husband.", 
            "video": "https://www.youtube.com/embed/x2aMpSSrd80"
            }, 
            {
            "word": "Contribute to sth", 
            "synonym": "", 
            "example": "The ice age contributed to the dinosaur extinction.", 
            "video": ""
            }, 
            {
            "word": "Contributory negligence", 
            "synonym": "", 
            "example": "Contributory negligence resulted in the defendant paying a minor penalty.", 
            "video": ""
            }, 
            {
            "word": "Contributory", 
            "synonym": "", 
            "example": "The donors were contributory to the expansion of the university.", 
            "video": ""
            }, 
            {
            "word": "Contrite", 
            "synonym": "", 
            "example": "My son told me in a contrite tone that he broke our TV.", 
            "video": ""
            }, 
            {
            "word": "Contrive", 
            "synonym": "", 
            "example": "You managed to contrive two failed mergers.", 
            "video": ""
            }, 
            {
            "word": "Control freak", 
            "synonym": "", 
            "example": "My mother is a control freak, it is really hard to work with her.", 
            "video": ""
            }, 
            {
            "word": "Control tower", 
            "synonym": "", 
            "example": "Control towers manage every aircraft that pass or land near the airport.", 
            "video": ""
            }, 
            {
            "word": "Control", 
            "synonym": "", 
            "example": "The controls on the new console are hard to use.", 
            "video": ""
            }, 
            {
            "word": "Control", 
            "synonym": "", 
            "example": "Whenever you conduct and experiment keep a control for reference.", 
            "video": ""
            }, 
            {
            "word": "Controversial", 
            "synonym": "", 
            "example": "Religion and politics are controversial topics.", 
            "video": ""
            }, 
            {
            "word": "Contusion", 
            "synonym": "", 
            "example": "After the accident Mary found contusions in her leg that prevent her from moving.", 
            "video": ""
            }, 
            {
            "word": "Conundrum", 
            "synonym": "", 
            "example": "The riddle was quite the conundrum.", 
            "video": ""
            }, 
            {
            "word": "Conurbation", 
            "synonym": "", 
            "example": "The major conurbations of London and Birmingham are heavily populated.", 
            "video": ""
            }, 
            {
            "word": "Convalesce", 
            "synonym": "", 
            "example": "The company was kind enough to fund Michealís convalesce after the accident.", 
            "video": ""
            }, 
            {
            "word": "Convector", 
            "synonym": "", 
            "example": "Convector are not always good for your health, best to just dress warm.", 
            "video": ""
            }, 
            {
            "word": "Convene", 
            "synonym": "Get together", 
            "example": "The council will be convening on the morning of the 25th.", 
            "video": "https://www.youtube.com/embed/uA33ulUdi5E"
            }, 
            {
            "word": "Convent", 
            "synonym": "Nunnery", 
            "example": "His memoirs led Campagnol to a convent at the church of Santa Maria degli Angeli on Murano, where Mr.Casanova had a lover.", 
            "video": "https://www.youtube.com/embed/8NrxvoFQfW8"
            }, 
            {
            "word": "Convention", 
            "synonym": "Conference", 
            "example": "The Governor of New York delivered a rousing speech to the national convention.", 
            "video": "https://www.youtube.com/embed/_BfHqlHay8s"
            }, 
            {
            "word": "Convention", 
            "synonym": "The new world order", 
            "example": "What do you expect from the upcoming party conventions?", 
            "video": "https://www.youtube.com/embed/PbWK"
            }, 
            {
            "word": "Convention", 
            "synonym": "Tradition & conformity.", 
            "example": "Convention dictates that it is the man who asks the woman to marry him and not the other way round.", 
            "video": "https://www.youtube.com/embed/KgPdjc8vscU"
            }, 
            {
            "word": "Converge", 
            "synonym": "Connecting and combining.", 
            "example": "The paths all converge at the main gate of the park.", 
            "video": "https://www.youtube.com/embed/vHTF7YmjWQE"
            }, 
            {
            "word": "Conversion", 
            "synonym": "Alteration.", 
            "example": "Solar power is the conversion of the sun's energy into heat and electricity.", 
            "video": "https://www.youtube.com/embed/AVuWhS5NMFc"
            }, 
            {
            "word": "Conversion", 
            "synonym": "Transformation", 
            "example": "In rugby, if a player makes or kicks a conversion, he scores points by kicking the ball over the goal after a try has been scored.", 
            "video": "https://www.youtube.com/embed/AMF"
            }, 
            {
            "word": "Converter", 
            "synonym": "Gadget", 
            "example": "This apparatus comprises transformers, converters, and certain minor auxiliaries.", 
            "video": "https://www.youtube.com/embed/09pZCh3ORis"
            }, 
            {
            "word": "Convertible", 
            "synonym": "Changing.", 
            "example": "A convertible sofa bed", 
            "video": "https://www.youtube.com/embed/mN1VT8KElBE"
            }, 
            {
            "word": "Convex", 
            "synonym": "Arched", 
            "example": "A convex lens/mirror.", 
            "video": "https://www.youtube.com/embed/becXPBK5t_U"
            }, 
            {
            "word": "Convey", 
            "synonym": "", 
            "example": "She always conveys a sense of enthusiasm for her work.", 
            "video": ""
            }, 
            {
            "word": "Conveyance", 
            "synonym": "Bus", 
            "example": "A horse", 
            "video": "https://www.youtube.com/embed/becXPBK5t_U"
            }, 
            {
            "word": "Conveyorbelt", 
            "synonym": "Power station", 
            "example": "A conveyor belt is the carrying medium of a belt conveyor system.", 
            "video": "https://www.youtube.com/embed/2mdn9Ay3ybk"
            }, 
            {
            "word": "Conviction", 
            "synonym": "Court cases.", 
            "example": "He has a long record of previous convictions for similar offences.", 
            "video": "https://www.youtube.com/embed/xL2hQVm9X84"
            }, 
            {
            "word": "Conviction", 
            "synonym": "Judgment", 
            "example": "It's my personal conviction that all rapists should be locked away for life.", 
            "video": "https://www.youtube.com/embed/79xWIVaeJ4E"
            }, 
            {
            "word": "Convivial", 
            "synonym": "Mate", 
            "example": "A convivial atmosphere/host", 
            "video": "https://www.youtube.com/embed/Bwr"
            }, 
            {
            "word": "Convocation", 
            "synonym": "Conference", 
            "example": "The arguments delayed the convocation of the first congress, planned for February 1992", 
            "video": "https://www.youtube.com/embed/V9nmhNGFpyA"
            }, 
            {
            "word": "Convoluted", 
            "synonym": "Meander", 
            "example": "His grammar explanations are terribly convoluted.", 
            "video": "https://www.youtube.com/embed/ZCmo0C5WCh0"
            }, 
            {
            "word": "Convoy", 
            "synonym": "Journeys.", 
            "example": "A convoy of trucks containing supplies was sent to the famine area.", 
            "video": "https://www.youtube.com/embed/iF2pceocW"
            }, 
            {
            "word": "Convulse", 
            "synonym": "Palpitate", 
            "example": "A racking cough convulsed her whole body.", 
            "video": "https://www.youtube.com/embed/VDwn08BqL9g"
            }, 
            {
            "word": "Cony", 
            "synonym": "Rodents & similar animals.", 
            "example": "The American cony lives on top of the world—on the crest of the continent.", 
            "video": "https://www.youtube.com/embed/lQRj4iH5yzI"
            }, 
            {
            "word": "Coo", 
            "synonym": "Oink", 
            "example": "The baby lay in his cot, cooing and gurgling.", 
            "video": "https://www.youtube.com/embed/6oBKlcIibWc"
            }, 
            {
            "word": "Cook someoneís goose", 
            "synonym": "", 
            "example": "When the burglar saw the police car arriving, he realised his goose was cooked!", 
            "video": ""
            }, 
            {
            "word": "Cook someone’s goose", 
            "synonym": "", 
            "example": "When the burglar saw the police car arriving, he realised his goose was cooked!", 
            "video": ""
            }, 
            {
            "word": "Cook sth up", 
            "synonym": "Cheating & tricking.", 
            "example": "I had to cook up an excuse about my car breaking down.", 
            "video": ""
            }, 
            {
            "word": "Cook the books", 
            "synonym": "Forensic accountant", 
            "example": "Falsify a company's financial records, as in An independent audit showed that they've been cooking the books for year.", 
            "video": "https://www.youtube.com/embed/jEL"
            }, 
            {
            "word": "Cookbook/ cookery book", 
            "synonym": "Preparing food.", 
            "example": "Chinese cookbooks are known from the Tang dynasty.", 
            "video": "https://www.youtube.com/embed/YZnEh3dgK1Y"
            }, 
            {
            "word": "Cooked ˈ breakfast", 
            "synonym": "Meals & parts of meals.", 
            "example": "50% of British families still started their day with a cooked breakfast.", 
            "video": ""
            }, 
            {
            "word": "Cookery", 
            "synonym": "spoonful", 
            "example": "A new cookery book by celebrity chef Jamie Oliver.", 
            "video": "https://www.youtube.com/embed/U2vP9FqTu2A"
            }, 
            {
            "word": "Cookie cutter n", 
            "synonym": "Kitchen utensils.", 
            "example": "She does not have her own style, she is cookie cutter. ", 
            "video": "https://www.youtube.com/embed/8F88KWCzs_c"
            }, 
            {
            "word": "Cookie", 
            "synonym": "Alike", 
            "example": "A row of cookie", 
            "video": "https://www.youtube.com/embed/hbDgtQf_oaM"
            }, 
            {
            "word": "Cooking  apple", 
            "synonym": "Types of fruit.", 
            "example": "Cooking apples are also known as culinary apples.", 
            "video": "https://www.youtube.com/embed/BJv5SG3o9Bw"
            }, 
            {
            "word": "Cookout", 
            "synonym": "Plate meal", 
            "example": "Many stay in touch through a private Facebook page, and several gathered last fall for a cookout.", 
            "video": "https://www.youtube.com/embed/oiT6zt05mUQ"
            }, 
            {
            "word": "Cool sb/sth down/off", 
            "synonym": "Fresh", 
            "example": "We went for a swim to cool off.", 
            "video": ""
            }, 
            {
            "word": "Cool bag.", 
            "synonym": "Cooler bag, Freezer pack.", 
            "example": "John forgot to bring the cooler bag with sodas for the picnic.", 
            "video": ""
            }, 
            {
            "word": "Cool box.", 
            "synonym": "Ice box, Ice bucket, Refrigerant.", 
            "example": "I suggest using the freezer itself as the 'cool box'.", 
            "video": ""
            }, 
            {
            "word": "Cool cat.", 
            "synonym": "Fashionable, Stylish, Trendy.", 
            "example": "Monty is a cool cat. I really like him.", 
            "video": ""
            }, 
            {
            "word": "Cool customer", 
            "synonym": "Peaceful", 
            "example": "They are the cool customer of this shop.", 
            "video": ""
            }, 
            {
            "word": "Cool it", 
            "synonym": "Calming and relaxing.", 
            "example": "Just cool it everyone, fighting won't solve anything.", 
            "video": "https://www.youtube.com/embed/4xLdtEJqJEk"
            }, 
            {
            "word": "Coolant", 
            "synonym": "Chemistry: types of chemical.", 
            "example": "It was discovered that the crash was due to the disconnection of some coolant hoses.", 
            "video": "https://www.youtube.com/embed/tLL_1lRYIjw"
            }, 
            {
            "word": "Cooler.", 
            "synonym": "Freezer, Fridge, Refrigerator.", 
            "example": "We brought a cooler full of beer with us.", 
            "video": "https://www.youtube.com/embed/dPHVDop2G"
            }, 
            {
            "word": "Coolheaded.", 
            "synonym": "Calm, Relaxed, Serene.", 
            "example": "She has a reputation for being calm and cool", 
            "video": "https://www.youtube.com/embed/LkRyAqxj5v4"
            }, 
            {
            "word": "Coolhunter.", 
            "synonym": "Swank, Hip, Modern.", 
            "example": "'Cool Hunters seek us out for our opinions then sell them right back to us'.", 
            "video": "https://www.youtube.com/embed/yX7EV2sm_"
            }, 
            {
            "word": "Coolie.", 
            "synonym": "Laborer, Cheaply employed.", 
            "example": "One coolie grabbed Karen's handbag from her shoulder and fled down the street.", 
            "video": "https://www.youtube.com/embed/jGKjb2S0ZJo"
            }, 
            {
            "word": "Cooling tower.", 
            "synonym": "Power station, Refinery, Mill.", 
            "example": "Around the small village the landscape is dominated by cooling towers and factory chimneys.", 
            "video": ""
            }, 
            {
            "word": "Cooling", 
            "synonym": "Stoppage, Wait, Postponement.", 
            "example": "There is a 20", 
            "video": ""
            }, 
            {
            "word": "Coolly.", 
            "synonym": "Unfriendly, Sour.", 
            "example": "Carmen eyed Katie coolly and responded in a dry tone.", 
            "video": "https://www.youtube.com/embed/UggudxICRao"
            }, 
            {
            "word": "Coon.", 
            "synonym": "Short for Raccoon.", 
            "example": "Later, I acquired a wonderful Maine coon cat we called Smudge.", 
            "video": "https://www.youtube.com/embed/J5g"
            }, 
            {
            "word": "Coon.", 
            "synonym": "Slang, Racist comment.", 
            "example": "I went to the R&B disco at DeNiro's last night and I was the only white person in there. It was full of coons.", 
            "video": "https://www.youtube.com/embed/J5g"
            }, 
            {
            "word": "Coop somebody/something up.", 
            "synonym": "Surround, Suffocate, Enclose.", 
            "example": "I feel like I've been cooped up in this flat for days.", 
            "video": ""
            }, 
            {
            "word": "Coop.", 
            "synonym": "Cage, Aviary, Birdhouse.", 
            "example": "The cat was caught in the night while trying to enter a chicken coop.", 
            "video": "https://www.youtube.com/embed/78L3q2315"
            }, 
            {
            "word": "Cooperation.", 
            "synonym": "Unity, Aid, Assist.", 
            "example": "There's very little cooperation between the two countries.", 
            "video": "https://www.youtube.com/embed/waD9JYvs2S0"
            }, 
            {
            "word": "Coordinated.", 
            "synonym": "Matched, Paired.", 
            "example": "The colour scheme of their living room is carefully coordinated.", 
            "video": "https://www.youtube.com/embed/TTgmeyr8qPQ"
            }, 
            {
            "word": "Coordinated.", 
            "synonym": "Organized, Orderly.", 
            "example": "The rebel troops have launched a coordinated attack on government soldiers.", 
            "video": "https://www.youtube.com/embed/TTgmeyr8qPQ"
            }, 
            {
            "word": "Coot.", 
            "synonym": "", 
            "example": "Let the old coot sleep", 
            "video": "https://www.youtube.com/embed/IzQIq5hTO5s"
            }, 
            {
            "word": "Coot.", 
            "synonym": "", 
            "example": "Texas has also the American coot or mud", 
            "video": "https://www.youtube.com/embed/IzQIq5hTO5s"
            }, 
            {
            "word": "Cop a plea.", 
            "synonym": "Admit sth, Concede, Surrender.", 
            "example": "If you don't want to go to jail, I think your best option here is to cop a plea.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Cop out.", 
            "synonym": "Back out, Cancel sth, Avoid.", 
            "example": "She copped out of the parachute jump at the last minute with some feeble excuse.", 
            "video": "https://www.youtube.com/embed/BxIpEMqQOlk"
            }, 
            {
            "word": "Cop.", 
            "synonym": "Arrest, Apprehend.", 
            "example": "He was copped for driving without a license last week.", 
            "video": "https://www.youtube.com/embed/QTtfmMfOPcE"
            }, 
            {
            "word": "Cop.", 
            "synonym": "Police officer, Deputy.", 
            "example": "Quick, run", 
            "video": "https://www.youtube.com/embed/QTtfmMfOPcE"
            }, 
            {
            "word": "Cop.", 
            "synonym": "To hold, To take.", 
            "example": "Cop hold of that, would you", 
            "video": "https://www.youtube.com/embed/QTtfmMfOPcE"
            }, 
            {
            "word": "Cop.", 
            "synonym": "Worthy, Quality.", 
            "example": "His last book wasn't much cop.", 
            "video": "https://www.youtube.com/embed/QTtfmMfOPcE"
            }, 
            {
            "word": "Copilot.", 
            "synonym": "A second pilot, Assistance.", 
            "example": "The co", 
            "video": "https://www.youtube.com/embed/iRgX99YplzY"
            }, 
            {
            "word": "Copious.", 
            "synonym": "Plenty, Large in amount.", 
            "example": "He took copious notes during the lecture.", 
            "video": "https://www.youtube.com/embed/az_yNXgd7gM"
            }, 
            {
            "word": "Copper beech.", 
            "synonym": "Tree with reddish", 
            "example": "His particular joy was the fine copper beech tree which dominated the scene.", 
            "video": ""
            }, 
            {
            "word": "Copper", 
            "synonym": "", 
            "example": "He signed a copper", 
            "video": "https://www.youtube.com/embed/uU0DJrKcPTI from 0:12 second"
            }, 
            {
            "word": "Copperplate.", 
            "synonym": "Penmanship, Font, Writing style.", 
            "example": "In 1700 Brancovan had a map of the country made and a copperplate engraving of it executed at Padua.", 
            "video": "https://www.youtube.com/embed/BMUNxijJip8"
            }, 
            {
            "word": "Coppice.", 
            "synonym": "Cut something down, Fell, Logjam.", 
            "example": "It is important as coppice", 
            "video": "https://www.youtube.com/embed/5SSwuZXaWQc"
            }, 
            {
            "word": "Copy cat", 
            "synonym": "", 
            "example": "My sister is such a copy cat. First she bought the same car as me, and now she is applying to my school.", 
            "video": ""
            }, 
            {
            "word": "Cork up something", 
            "synonym": "", 
            "example": "It would be better if she showed her grief and didn't cork up her feelings.", 
            "video": ""
            }, 
            {
            "word": "Corner the market", 
            "synonym": "", 
            "example": "By importing large quantities and selling at low prices, they have cornered the market.", 
            "video": "https://www.youtube.com/embed/ao85yOwNO4M up to 0:11 second"
            }, 
            {
            "word": "Corridors of power", 
            "synonym": "", 
            "example": "The matter is the subject of much discussion in the corridors of power at the present time.", 
            "video": "https://www.youtube.com/embed/9kubDjzDQ4Q"
            }, 
            {
            "word": "Cost an arm and a leg", 
            "synonym": "", 
            "example": "The new house cost us an arm and a leg, but we have no regrets.", 
            "video": "https://www.youtube.com/embed/PmeM1gPAKig"
            }, 
            {
            "word": "Cost an arm and a leg", 
            "synonym": "", 
            "example": "These cakes are delicious, but they cost me an arm and a leg.", 
            "video": ""
            }, 
            {
            "word": "Cost the earth", 
            "synonym": "", 
            "example": "She wears designer clothes that must cost the earth!", 
            "video": "https://www.youtube.com/embed/wV3UrB5HjXw from 0:50 second to 2:04 second"
            }, 
            {
            "word": "Couch potato", 
            "synonym": "", 
            "example": "Don't be such a couch potato. There are better ways of spending your time than in front of the TV.", 
            "video": "https://www.youtube.com/embed/gZ4iCbI4ADk"
            }, 
            {
            "word": "Couldn’t give a hoot", 
            "synonym": "", 
            "example": "She wears eccentric clothes but she couldn't give a hoot about what others think.", 
            "video": ""
            }, 
            {
            "word": "Count on", 
            "synonym": "Trusting and not trusting.", 
            "example": "You can always count on Michael in a crisis.", 
            "video": "https://www.youtube.com/embed/JgVSROco_VY"
            }, 
            {
            "word": "Cover your tracks", 
            "synonym": "", 
            "example": "Charlie was sorry he hadn't covered his tracks better when his wife discovered he had been unfaithful.", 
            "video": "https://www.youtube.com/embed/8HYexIwkpYA"
            }, 
            {
            "word": "Crack someone up", 
            "synonym": "", 
            "example": "There's something about that guy's face that just cracks me up.", 
            "video": "https://www.youtube.com/embed/MPbizr7QnD8"
            }, 
            {
            "word": "Crack the whip", 
            "synonym": "", 
            "example": "Every so often I'll crack the whip to make sure we meet the deadline.", 
            "video": "https://www.youtube.com/embed/QCTCDwUPpPU"
            }, 
            {
            "word": "Crack", 
            "synonym": "Fracture, Cleft", 
            "example": "A hairline crack down the middle of the glass", 
            "video": "https://www.youtube.com/embed/ORdq2TuWq8E"
            }, 
            {
            "word": "Crackdown", 
            "synonym": "", 
            "example": "A crackdown on crime and corruption", 
            "video": "https://www.youtube.com/embed/Oaxj1FUQOeA"
            }, 
            {
            "word": "Cracked", 
            "synonym": "Rude, Crabby", 
            "example": "The old pipes were cracked and leaking", 
            "video": "https://www.youtube.com/embed/t06"
            }, 
            {
            "word": "Cracker", 
            "synonym": "Bomb, Grenade", 
            "example": "He lived on crackers and water for three days.", 
            "video": "https://www.youtube.com/embed/kjJduUP9Ez4"
            }, 
            {
            "word": "Cracker", 
            "synonym": "Egg, Bun", 
            "example": "I often eat peanut butter on crackers.", 
            "video": "https://www.youtube.com/embed/kjJduUP9Ez4"
            }, 
            {
            "word": "Cracker", 
            "synonym": "Wafer, Cookies", 
            "example": "She grabbed a few crackers and cream cheese", 
            "video": "https://www.youtube.com/embed/kjJduUP9Ez4"
            }, 
            {
            "word": "Cracking", 
            "synonym": "", 
            "example": "He is in cracking form to win this race", 
            "video": "https://www.youtube.com/embed/t06"
            }, 
            {
            "word": "Crackling", 
            "synonym": "", 
            "example": "The skin crisps to crunchy crckling, and the meat melts with juicy tenderness", 
            "video": "https://www.youtube.com/embed/vtrVWBGXFyk"
            }, 
            {
            "word": "Crackling", 
            "synonym": "Hiss, Snap", 
            "example": "Carmen woke to a crackling sound and sat up, trying to identify it.", 
            "video": "https://www.youtube.com/embed/vtrVWBGXFyk"
            }, 
            {
            "word": "Crackpot", 
            "synonym": "Capricious Man, Eccentric", 
            "example": "It is a site dedicated to crackpots, kooks, loons on the web", 
            "video": "https://www.youtube.com/embed/0"
            }, 
            {
            "word": "Cradle", 
            "synonym": "Baby Bad, Moses Basket", 
            "example": "A baby is sleeping in the cradle.", 
            "video": "https://www.youtube.com/embed/_"
            }, 
            {
            "word": "Cradle", 
            "synonym": "Crib, Bassinet", 
            "example": "What is learned in the cradle is carried to the tomb.", 
            "video": "https://www.youtube.com/embed/_"
            }, 
            {
            "word": "Cradle", 
            "synonym": "Pannier, Turndle Bed", 
            "example": "Tom cradled the baby in his arms.", 
            "video": "https://www.youtube.com/embed/_"
            }, 
            {
            "word": "Cradle", 
            "synonym": "Spring, Fountain", 
            "example": "Cade kneeled beside the cradle and touched a blue crocheted bootie.", 
            "video": "https://www.youtube.com/embed/_"
            }, 
            {
            "word": "Craft", 
            "synonym": "", 
            "example": "the craft of furniture", 
            "video": ""
            }, 
            {
            "word": "Craft", 
            "synonym": "Appliance, Powerhouse", 
            "example": "She crafted a strategy to boost the company's earnings.", 
            "video": "https://www.youtube.com/embed/bvrfzUiMObQ"
            }, 
            {
            "word": "Craft", 
            "synonym": "Art, Cunning", 
            "example": "He is crafting a new sculpture.", 
            "video": "https://www.youtube.com/embed/bvrfzUiMObQ"
            }, 
            {
            "word": "Craftsmanship", 
            "synonym": "Artistry, Craft", 
            "example": "The building was a superb example of craftsmanship from an era when quality was meant to survive those skilled men who proudly worked it.", 
            "video": "https://www.youtube.com/embed/Dqz2"
            }, 
            {
            "word": "Crafty", 
            "synonym": "Sly,Wily", 
            "example": "The Austro", 
            "video": "https://www.youtube.com/embed/RDnlfYd9Vo0"
            }, 
            {
            "word": "Craggy", 
            "synonym": "Bumpy, Unever", 
            "example": "A craggy coastline", 
            "video": "https://www.youtube.com/embed/exs_5i"
            }, 
            {
            "word": "Craggy", 
            "synonym": "Rough, Broken", 
            "example": "From the railway from Moscow to Warsaw, on the high craggy banks of the Shchara", 
            "video": "https://www.youtube.com/embed/exs_5i"
            }, 
            {
            "word": "Craic", 
            "synonym": "Solve, Break", 
            "example": "The craic was good in Cricklewood.", 
            "video": "https://www.youtube.com/embed/LmeP4mEib6A"
            }, 
            {
            "word": "Cram", 
            "synonym": "Crowd,Load", 
            "example": "He barely had time to cram the papers in his pocket.", 
            "video": "https://www.youtube.com/embed/F7GAo7hYoIQ"
            }, 
            {
            "word": "Cram", 
            "synonym": "Force,overfill", 
            "example": "She couldnít cram the bread into her mouth quick.", 
            "video": "https://www.youtube.com/embed/F7GAo7hYoIQ"
            }, 
            {
            "word": "Cram", 
            "synonym": "Overeat, Thurst", 
            "example": "I really do have to cram for my history final.", 
            "video": "https://www.youtube.com/embed/F7GAo7hYoIQ"
            }, 
            {
            "word": "Crammed", 
            "synonym": "Wedge, Overfilled", 
            "example": "https://www.shutterstock.com/image", 
            "video": "https://www.youtube.com/embed/F7GAo7hYoIQ"
            }, 
            {
            "word": "Cramp", 
            "synonym": "Kink, Ache", 
            "example": "That awful cramp in Lad lane.", 
            "video": "https://www.youtube.com/embed/InHikSQzEQk"
            }, 
            {
            "word": "Cramp", 
            "synonym": "Pain, Stiffness", 
            "example": "If your ladyship knew the creature as well as I do, you'd call her Sally Cramp.", 
            "video": "https://www.youtube.com/embed/InHikSQzEQk"
            }, 
            {
            "word": "Cramped", 
            "synonym": "Confident, Pent", 
            "example": "The staff had to work in cramped conditions.", 
            "video": "https://www.youtube.com/embed/OK2j31K6FFc"
            }, 
            {
            "word": "Crampon", 
            "synonym": "A metal plate with spikes fixed to a boot fpr walking on ice or rock climbing.", 
            "example": "Some companies that currently produce saxophones are Buffet Crampon, Yanagisawa.", 
            "video": "https://www.youtube.com/embed/"
            }, 
            {
            "word": "Cranberry", 
            "synonym": "Cloudberry, Cowberry", 
            "example": "It is likely to apply to canbarries and cranberry sauce as well as juice.", 
            "video": "https://www.youtube.com/embed/Mnp6nV6skZA"
            }, 
            {
            "word": "Crane fly", 
            "synonym": "", 
            "example": "Except for observations of a longh", 
            "video": "https://www.youtube.com/embed/VXZFqmYAyRA"
            }, 
            {
            "word": "Crane", 
            "synonym": "Derick, Winch", 
            "example": "Tom can operate a crane.", 
            "video": "https://www.youtube.com/embed/F4VjZVbJbS8"
            }, 
            {
            "word": "Crane", 
            "synonym": "Hoist, Davit", 
            "example": "Cranes are big beautiful birds.", 
            "video": "https://www.youtube.com/embed/F4VjZVbJbS8"
            }, 
            {
            "word": "Crane", 
            "synonym": "Pulley, Elevator", 
            "example": "Giant cranes were lifting large, mangled steel beams and depositing then onto 18", 
            "video": "https://www.youtube.com/embed/F4VjZVbJbS8"
            }, 
            {
            "word": "Cranium", 
            "synonym": "Skull, Cranium", 
            "example": "The cranium, pronounced by Huxley to be the most ape", 
            "video": "https://www.youtube.com/embed/bqrjonQsKRY"
            }, 
            {
            "word": "Crank", 
            "synonym": "Freak, Eccentric", 
            "example": "Katie turned the crank at the base of the bed", 
            "video": "https://www.youtube.com/embed/Qj6WMwKTaXY"
            }, 
            {
            "word": "Crank", 
            "synonym": "Oddity, Caprice", 
            "example": "Next time, crank this up all the way.", 
            "video": "https://www.youtube.com/embed/Qj6WMwKTaXY"
            }, 
            {
            "word": "Crank", 
            "synonym": "Slack, Loose", 
            "example": "The situation of the Ranger's crew, with a top", 
            "video": "https://www.youtube.com/embed/Qj6WMwKTaXY"
            }, 
            {
            "word": "Crankshaft", 
            "synonym": "", 
            "example": "The uses of medium carbon", 
            "video": "https://www.youtube.com/embed/qhIWGLfAoAg"
            }, 
            {
            "word": "Cranky", 
            "synonym": "Limp, Wonky", 
            "example": "He was bored and cranky after eight hours of working", 
            "video": "https://www.youtube.com/embed/8yi"
            }, 
            {
            "word": "Cranky", 
            "synonym": "Shaky, Tottering", 
            "example": "He's been cranky all night.", 
            "video": "https://www.youtube.com/embed/8yi"
            }, 
            {
            "word": "Cranny", 
            "synonym": "Fracture, Nook", 
            "example": "You could spend several hours exploring the elegant, wide streets and narrow nooks and crannies.", 
            "video": "https://www.youtube.com/embed/5dBFMzJ3iZc"
            }, 
            {
            "word": "Crap", 
            "synonym": "Foolishness,Claptrap", 
            "example": "The articles in that magazine are totally ridiculous. I don't know how anybody can believe that crap.", 
            "video": "https://www.youtube.com/embed/YEHKkAyBuFg"
            }, 
            {
            "word": "Crap", 
            "synonym": "Shit, Defecation", 
            "example": "The movie was very amateurish looking, with really crappy special effects", 
            "video": "https://www.youtube.com/embed/YEHKkAyBuFg"
            }, 
            {
            "word": "Crape Myrtle", 
            "synonym": "", 
            "example": "We plated verbena around our crape myrtle", 
            "video": "https://www.youtube.com/embed/aCfSwk0pDLE"
            }, 
            {
            "word": "Crappy", 
            "synonym": "Nasty, Fulsome", 
            "example": "Crappy Wine", 
            "video": "https://www.youtube.com/embed/qExt9qftTD8"
            }, 
            {
            "word": "Crash Out", 
            "synonym": "Sleep, Doze off, Drift off", 
            "example": "I crashed out around ten in front of the TV.", 
            "video": ""
            }, 
            {
            "word": "Crash Out", 
            "synonym": "Submit, Surrender, Appease", 
            "example": "England crashed out of the European Cup again today.", 
            "video": ""
            }, 
            {
            "word": "Crash and burn", 
            "synonym": "Accident, Bang, Collapse", 
            "example": "A car crash.", 
            "video": ""
            }, 
            {
            "word": "Crash barrier", 
            "synonym": "Abuttals, Balustrade, Barbed wire", 
            "example": "They drove ahead of him on the other side of the crash barrier and flashed their lights to warn oncoming cars.", 
            "video": ""
            }, 
            {
            "word": "Crash helmet", 
            "synonym": "Helmet, Construction helmet, Hard Hat", 
            "example": "Neither were wearing protective clothing or crash helmets.", 
            "video": ""
            }, 
            {
            "word": "Crash", 
            "synonym": "Accident, Bang, Collapse, Smash", 
            "example": "A plane crash.", 
            "video": ""
            }, 
            {
            "word": "Crash", 
            "synonym": "Bang, Blast, Boom, Clap", 
            "example": "The crash of cymbals", 
            "video": ""
            }, 
            {
            "word": "Crash", 
            "synonym": "Bed, Retire, Turn in", 
            "example": "I'm so exhausted that I'm just going to crash as soon as we get home.", 
            "video": ""
            }, 
            {
            "word": "Crash", 
            "synonym": "Collapse, Cropper, Defeat, Failure", 
            "example": "She refused to be discouraged by the crash of her first business venture.", 
            "video": ""
            }, 
            {
            "word": "Crash", 
            "synonym": "Creak, Bankrupt", 
            "example": "A cra crash", 
            "video": "https://www.youtube.com/embed/mLEjVFrrf4o"
            }, 
            {
            "word": "Crash", 
            "synonym": "Decline, Descend, Dip, Dive", 
            "example": "Sales of that phone have crashed since the competing version came out.", 
            "video": ""
            }, 
            {
            "word": "Crashing", 
            "synonym": "Complete, Total, Smash into, Collide with, Hit, Strike,", 
            "example": "The stolen car she was riding in crashed into a tree.", 
            "video": ""
            }, 
            {
            "word": "Crass", 
            "synonym": "Stupid, Insensitive, Mindless, Thoughtless", 
            "example": "The crass assumptions that men make about women.", 
            "video": ""
            }, 
            {
            "word": "Crate", 
            "synonym": "Case, Packing case, Chest, Box, Container,", 
            "example": "A crate of bananas.", 
            "video": ""
            }, 
            {
            "word": "Crater", 
            "synonym": "Hollow, Bowl, Basin, Hole, Cavity,", 
            "example": "As a result, the ground is littered with craters from asteroid impacts.", 
            "video": ""
            }, 
            {
            "word": "Cravat", 
            "synonym": "Tie, Ascot, Band", 
            "example": "The bridegroom is able to hire his choice of morning suit or dinner suit, tuxedo, shirt and cravat or bow tie.", 
            "video": ""
            }, 
            {
            "word": "Crave", 
            "synonym": "Long for, Yearn for, Desire, Want, Wish for", 
            "example": "A program to give the infants the human touch they crave.", 
            "video": ""
            }, 
            {
            "word": "Craven", 
            "synonym": "Cowardly,Lily", 
            "example": "A craven abdication of his moral duty.", 
            "video": ""
            }, 
            {
            "word": "Crawl back to sb", 
            "synonym": "Back, Crawl", 
            "example": "Maybe if you went crawling back to your boss, you could get your job back.", 
            "video": ""
            }, 
            {
            "word": "Crawl", 
            "synonym": "Creep, Worm one's way, Go on all fours.", 
            "example": "They began the crawl back to their own lines.", 
            "video": ""
            }, 
            {
            "word": "Crawl", 
            "synonym": "Wriggle, Slither, Ssquirm", 
            "example": "The crawl stroke, with flutter kick, had been introduced into competitive swimming a few years earlier by another Aussie.", 
            "video": ""
            }, 
            {
            "word": "Crayfish", 
            "synonym": "Crawdad, Crawfish, Spiny lobster", 
            "example": "Looking that way, he saw a pair of raccoons dunking their paws in the river, obviously after crayfish.", 
            "video": ""
            }, 
            {
            "word": "Crayon", 
            "synonym": "Wax crayon, Pencil crayon.", 
            "example": "Jeff crayoned a picture on a legal pad.", 
            "video": ""
            }, 
            {
            "word": "Crazed", 
            "synonym": "Mad, Insane, Psychotic, Out of one's mind", 
            "example": "A crazed killer.", 
            "video": ""
            }, 
            {
            "word": "Crazy paving", 
            "synonym": "Asphalt, Bitumen, Blacktop.", 
            "example": "", 
            "video": ""
            }, 
            {
            "word": "Creak", 
            "synonym": "Scrape, Scratch, Sound, Creaking", 
            "example": "The creak of a floorboard broke the silence.", 
            "video": ""
            }, 
            {
            "word": "Cream Cheese", 
            "synonym": "Ice cream, Sour cream, Whipped cream, Cream cheese.", 
            "example": "She loves cream cheese, so maybe I'll make something with goat cream cheese.", 
            "video": ""
            }, 
            {
            "word": "Cream Crackers", 
            "synonym": "Biscuits, Food", 
            "example": "Cream crackers are crisp dry biscuits which are eaten with cheese.", 
            "video": ""
            }, 
            {
            "word": "Cream of mushroom/tomato, etc.", 
            "synonym": "Cream of mushroom soup is a simple type of soup where a basic roux is thinned with cream or milk and then mushrooms and/or mushroom broth are added.  Definition ", 
            "example": "", 
            "video": ""
            }, 
            {
            "word": "Cream of the crop", 
            "synonym": "", 
            "example": "As usual, the cream of the crop of this year's graduates were offered the best jobs.", 
            "video": ""
            }, 
            {
            "word": "Cream", 
            "synonym": "Lotion, Ointment, Moisturizer, Emollient", 
            "example": "Shaving cream.", 
            "video": ""
            }, 
            {
            "word": "Creamer", 
            "synonym": "Choice, fat, Cream, Pick, Top", 
            "example": "Alex prayed that Dan hadn't used the milk for creamer in his coffee.", 
            "video": ""
            }, 
            {
            "word": "Crease sb up", 
            "synonym": "Burst out, Crack up, Dissolve into.", 
            "example": "You really crease me up!", 
            "video": ""
            }, 
            {
            "word": "Crease", 
            "synonym": "Fold, Wrinkle, Kris, Crimp, Line", 
            "example": "khaki trousers with knife", 
            "video": ""
            }, 
            {
            "word": "Crease", 
            "synonym": "line, Bowling crease, Popping crease, Return crease", 
            "example": "One of the lines in cricket marking off the positions of the bowler and batter or the space between two of these lines.", 
            "video": ""
            }, 
            {
            "word": "Creationist", 
            "synonym": "Fundamentalist, Adventist, Muslim, Hindu", 
            "example": "The belief that the universe was created exactly as the Bible describes it.", 
            "video": ""
            }, 
            {
            "word": "Creative accounting", 
            "synonym": "", 
            "example": "It was suggested that some creative accounting might help to attract investors.", 
            "video": "https://www.youtube.com/embed/YTxLI4jOagI"
            }, 
            {
            "word": "Creature Comforts", 
            "synonym": "Conveniences, Amenities, Comforts", 
            "example": "What are the creature comfort you have on the bus?", 
            "video": ""
            }, 
            {
            "word": "Creature of habit", 
            "synonym": "Habit, Creature", 
            "example": "He's a creature of habit—he keeps to the places he knows.", 
            "video": ""
            }, 
            {
            "word": "Creche", 
            "synonym": "Child Care, Day Care", 
            "example": "A nursery where babies and young children are cared for during the working day.", 
            "video": ""
            }, 
            {
            "word": "Creche", 
            "synonym": "Infirmary, Hospital", 
            "example": "a representation of Christ's nativity in the stable at Bethlehem", 
            "video": ""
            }, 
            {
            "word": "Credentials", 
            "synonym": "Documents, Documentation, Papers, Identity papers, Bona fides, ID, ID card, Passport", 
            "example": "Recruitment is based mainly on academic credentials.", 
            "video": ""
            }, 
            {
            "word": "Credibility", 
            "synonym": "Trustworthiness, Reliability, Dependability, Integrity, Reputation, Status", 
            "example": "The government's loss of credibility.", 
            "video": ""
            }, 
            {
            "word": "Credit card", 
            "synonym": "ATM card, baksheesh.", 
            "example": "What is the expiry date on your credit card ?", 
            "video": "https://www.youtube.com/embed/_CDIAX7FDJo"
            }, 
            {
            "word": "Credit sb with sth", 
            "synonym": "Analysing and evaluating.", 
            "example": "She is credited with making the business a success.", 
            "video": ""
            }, 
            {
            "word": "Credit squeeze / credit crunch", 
            "synonym": "Borrowing & lending.", 
            "example": "The severe credit squeeze is producing some ghastly results.", 
            "video": "https://www.youtube.com/embed/Vn_jFcJmp2g"
            }, 
            {
            "word": "Credit where credit's due", 
            "synonym": "Well done, Good boy/girl, Bravo", 
            "example": "Used for saying that someone deserves praise for something that they have done.", 
            "video": ""
            }, 
            {
            "word": "Creditor", 
            "synonym": "Borrowers & lenders.", 
            "example": "The company couldn't pay its creditors.", 
            "video": "https://www.youtube.com/embed/EM3LtbYwkPo"
            }, 
            {
            "word": "Credulous", 
            "synonym": "Stupid and silly.", 
            "example": "The credulous approach can allow proving both something and its contrary.", 
            "video": "https://www.youtube.com/embed/lpdQ08O4SsA"
            }, 
            {
            "word": "Creek", 
            "synonym": "Watercourses & waterfalls.", 
            "example": "The next sedimentation cycle starts with development of new creeks and gullies.", 
            "video": "https://www.youtube.com/embed/olOgiyRMyGo"
            }, 
            {
            "word": "Creep in/creep into sth", 
            "synonym": "Faults and mistakes.", 
            "example": "A few mistakes always creep in during the editing process.", 
            "video": ""
            }, 
            {
            "word": "Creep over sb", 
            "synonym": "Experiencing and suffering.", 
            "example": "A dangerous tiredness crept over her as she drove.", 
            "video": ""
            }, 
            {
            "word": "Creep up on sb", 
            "synonym": "Experiencing and suffering.", 
            "example": "It was only after I turned 60 that old age began to creep up on me.", 
            "video": ""
            }, 
            {
            "word": "Creep up on/behind sb", 
            "synonym": "Surprising and shocking.", 
            "example": "Don't creep up on me like that!", 
            "video": ""
            }, 
            {
            "word": "Creep up", 
            "synonym": "Increasing and intensifying.", 
            "example": "Over the last year, the rate of inflation has crept up to almost seven percent.", 
            "video": "https://www.youtube.com/embed/VNBmIRu_Hp4"
            }, 
            {
            "word": "Creep", 
            "synonym": "Slow and moving slowly.", 
            "example": "The traffic was creeping along at a snail's pace.", 
            "video": "https://www.youtube.com/embed/r3H7jn_OFfs"
            }, 
            {
            "word": "Creeper PLANT", 
            "synonym": "Bindweed, bougainvillea.", 
            "example": "The caterpillars are known to feed on virginia creeper.", 
            "video": "https://www.youtube.com/embed/Nsf1SdZI"
            }, 
            {
            "word": "Creepy                            CRAWLY", 
            "synonym": "Anopheles, ant.", 
            "example": "", 
            "video": "https://www.youtube.com/embed/BH10Qqegjk0"
            }, 
            {
            "word": "Creepy", 
            "synonym": "Awesome, bloodcurdling.", 
            "example": "She got pestered by a creepy cab driver.", 
            "video": "https://www.youtube.com/embed/BH10Qqegjk0"
            }, 
            {
            "word": "Cremate", 
            "synonym": "Burying, cremating and preserving bodies.", 
            "example": "In acute penury, she could not even pay the taxes needed to cremate him.", 
            "video": "https://www.youtube.com/embed/GEPxPepoTTo"
            }, 
            {
            "word": "Crenellations", 
            "synonym": "Acropolis, barricade.", 
            "example": "Dawn was breaking over the crenellations of the tower.", 
            "video": "https://www.youtube.com/embed/rkRSZPObHV0"
            }, 
            {
            "word": "Creole                            PERSON", 
            "synonym": "Albanian, american English.", 
            "example": "Creole is one of the official languages of Haiti.", 
            "video": "https://www.youtube.com/embed/lXzryuQZ0Ds"
            }, 
            {
            "word": "Creosote", 
            "synonym": "Airbrick, asbestos.", 
            "example": "There is, in the first place, creosote, the product of the high temperature distillation of coal.", 
            "video": "https://www.youtube.com/embed/HLBbx9dqsls"
            }, 
            {
            "word": "Crepe                              CLOTH", 
            "synonym": "Burlap, calico.", 
            "example": "The use of rayon in elastic adhesive dressings, elastic bandages and cotton crepe bandages is already authorised.", 
            "video": "https://www.youtube.com/embed/3YDrKA"
            }, 
            {
            "word": "Crepe                              FOOD", 
            "synonym": "Pancakes & batter.", 
            "example": "How to make crepe paper frills for decorating food displays of cod liver oil.", 
            "video": "https://www.youtube.com/embed/3YDrKA"
            }, 
            {
            "word": "Crepe                              RUBBER", 
            "synonym": "Ankle boot, ballet shoe.", 
            "example": "He wanted the soldier to be wearing a black crepe mourning armband, with the sweetheart of the young soldier sewing it around his arm.", 
            "video": "https://www.youtube.com/embed/3YDrKA"
            }, 
            {
            "word": "Crepe paper", 
            "synonym": "Publishing: paper & stationery.", 
            "example": "The paper is usually newspaper, wrapping paper or crepe paper in various colors.", 
            "video": "https://www.youtube.com/embed/2kDQfMHcDm4"
            }, 
            {
            "word": "Crepuscular", 
            "synonym": "Days & times of day.", 
            "example": "Deer are crepuscular, meaning that they are most active at dawn and at dusk.", 
            "video": "https://www.youtube.com/embed/TXrdJzV1c3c"
            }
          
      ]
    }
  },

  
  computed: {
      filterVocabularies: function(){

          var mainData = this.vocabularies.filter((vocabulary)=>{

              if(this.value)
                  return vocabulary.word[0].match(this.value);

              else
                  return vocabulary.word.match(this.search);

              
          })

          this.value = null;

          return mainData;
      }

  }
};
</script>

<style scoped>

    .paginate{
        margin: 20px;
    }

</style>