<template>
  <div class="home">
    <div class="container">
      <div class="paginate">

            <nav aria-label="Page navigation" v-if="!search">
                <ul class="pagination justify-content-center">
                    
                    <li class="page-item active"><a class="page-link bg-dark text-white" href="#">A</a></li>
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

       
        
        
       
        <div class="active-cyan-3 active-cyan-4 mb-4 sticky-top">
             
             <input class="form-control" aria-label="Search" type="text" v-model="search" placeholder="search">
       
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
          "word": "passing   lane", 
          "synonym": "", 
          "example": "The northern section of the highway features the occasional passing lane in both directions.", 
          "video": ""
          }, 
          {
          "word": "Prepare the ground", 
          "synonym": "", 
          "example": "The meeting was to prepare the ground for next weekís peace talks.", 
          "video": ""
          }, 
          {
          "word": "fall foul of sb", 
          "synonym": "", 
          "example": "Things were going well for her till she fell foul of the director.", 
          "video": ""
          }, 
          {
          "word": "passing   shot", 
          "synonym": "", 
          "example": "Nadal is an expert in passing shots.", 
          "video": ""
          }, 
          {
          "word": "Sign on dotted line", 
          "synonym": "", 
          "example": "A financial adviser can suggest questions you should ask before signing on the dotted line.", 
          "video": "https://www.youtube.com/embed/HzZep7673hI"
          }, 
          {
          "word": "a passion for  sth", 
          "synonym": "", 
          "example": "Anton has a consuming passion for science fiction.", 
          "video": ""
          }, 
          {
          "word": "fall in love", 
          "synonym": "", 
          "example": "I was 20 when I first fell in love.", 
          "video": "https://www.youtube.com/embed/5XJVv2lFPRE"
          }, 
          {
          "word": "Sticking point", 
          "synonym": "", 
          "example": "Exactly how the land is to be divided up is the main sticking point of the peace talks.", 
          "video": "https://www.youtube.com/embed/ujs_tn2s0j8"
          }, 
          {
          "word": "fall prey/victim to sth/sb", 
          "synonym": "", 
          "example": "Police fear that more senior citizens could fall prey to the thieves.", 
          "video": ""
          }, 
          {
          "word": "passions", 
          "synonym": "", 
          "example": "Touch a man's property and his passions are immediately aroused.", 
          "video": "https://www.youtube.com/embed/svyAubXEde4"
          }, 
          {
          "word": "Take stock of the situation", 
          "synonym": "", 
          "example": "He takes stock of the situation to understand the situation.", 
          "video": ""
          }, 
          {
          "word": "fall short", 
          "synonym": "", 
          "example": "They needed 60 votes to pass the bill, but they fell short by 12 votes.", 
          "video": ""
          }, 
          {
          "word": "passions run high", 
          "synonym": "", 
          "example": "Passions run very high at election time.", 
          "video": ""
          }, 
          {
          "word": "Turn on/ up the heat", 
          "synonym": "", 
          "example": "The Democrats turned up the heat on their candidate to concede the election", 
          "video": ""
          }, 
          {
          "word": "nearly/almost fall off your chair", 
          "synonym": "", 
          "example": "She nearly fell off her chair when she heard the news.", 
          "video": ""
          }, 
          {
          "word": "passion   flower", 
          "synonym": "", 
          "example": "The unusual domed ceiling represents a passion flower surrounded by lotuses.", 
          "video": "https://www.youtube.com/embed/Mn8oVvwUtpY"
          }, 
          {
          "word": "All told", 
          "synonym": "", 
          "example": "There were 550 people at the festival all told.", 
          "video": "https://www.youtube.com/embed/6Ax4m3xRwf8"
          }, 
          {
          "word": "fall about laughing", 
          "synonym": "", 
          "example": "We fell about when we heard her reply.", 
          "video": ""
          }, 
          {
          "word": "passion   fruit", 
          "synonym": "", 
          "example": "The tropical syrup flavors vary from lemon and strawberry to passion fruit and guava.", 
          "video": "https://www.youtube.com/embed/iGZgr81cWm0"
          }, 
          {
          "word": "In dribs and drabs", 
          "synonym": "Bites and pieces, odds and ends.", 
          "example": "There will be a greater tendency for companies to act together, rather than in dribs and drabs.", 
          "video": "https://www.youtube.com/embed/Kvcp59TWFDg"
          }, 
          {
          "word": "fall apart", 
          "synonym": "Fall to pieces, come to pieces, fall to bits.", 
          "example": "My poor old boots are falling apart.", 
          "video": "https://www.youtube.com/embed/i3UqaUQl8rA"
          }, 
          {
          "word": "passionless", 
          "synonym": "", 
          "example": "This music is passionless.", 
          "video": "https://www.youtube.com/embed/3w4_yMS0VsQ"
          }, 
          {
          "word": "Have one over the eight", 
          "synonym": "", 
          "example": "I think someone should drive Jerry home, he's one over the eight.", 
          "video": ""
          }, 
          {
          "word": "fall apart", 
          "synonym": "Break down", 
          "example": "The deal fell apart because of a lack of financing.", 
          "video": "https://www.youtube.com/embed/i3UqaUQl8rA"
          }, 
          {
          "word": "passive", 
          "synonym": "", 
          "example": "He's very passive in the relationship.", 
          "video": "https://www.youtube.com/embed/a7PboqbFqWc"
          }, 
          {
          "word": "Fiddling while Rome burns", 
          "synonym": "", 
          "example": "Environmentalists claimed governments were fiddling while Rome burned.", 
          "video": "https://www.youtube.com/embed/01QjRMgDsI4"
          }, 
          {
          "word": "fairy bread", 
          "synonym": "", 
          "example": "Fairy bread is very tasty.", 
          "video": "https://www.youtube.com/embed/gBGkdsYi9fs"
          }, 
          {
          "word": "pass  sth  out", 
          "synonym": "", 
          "example": "The teacher passed out the test booklets.", 
          "video": ""
          }, 
          {
          "word": "At the eleventh hour", 
          "synonym": "", 
          "example": "I was shocked that they reached an agreement at the eleventh hour after weeks of squabbling.", 
          "video": "https://www.youtube.com/embed/NzUuXi40QWk"
          }, 
          {
          "word": "fall apart", 
          "synonym": "", 
          "example": "After his wife died, he began to fall apart.", 
          "video": "https://www.youtube.com/embed/i3UqaUQl8rA"
          }, 
          {
          "word": "passive resistance", 
          "synonym": "", 
          "example": "The Mahatma instigated several campaigns of passive resistance against the British government in India.", 
          "video": ""
          }, 
          {
          "word": "Fifth wheel", 
          "synonym": "", 
          "example": "I didn't realize that the party was for couples only, so when I showed up alone, I felt like a fifth wheel.", 
          "video": "https://www.youtube.com/embed/yfIc_nJYUds"
          }, 
          {
          "word": "fall away", 
          "synonym": "", 
          "example": "The rear sections of the rocket fell away.", 
          "video": "https://www.youtube.com/embed/gawx6aR2Pqg"
          }, 
          {
          "word": "passive   smoking", 
          "synonym": "", 
          "example": "Doctors say passive smoking has caused his lung cancer.", 
          "video": "https://www.youtube.com/embed/btq902z3_"
          }, 
          {
          "word": "First and foremost", 
          "synonym": "", 
          "example": "In spite of being elected to office, she remains first and foremost a writer.", 
          "video": "https://www.youtube.com/embed/lmnkDWR5JUM"
          }, 
          {
          "word": "fall away", 
          "synonym": "", 
          "example": "As she looked at him, the years fell away, and she saw him again as a young boy.", 
          "video": "https://www.youtube.com/embed/gawx6aR2Pqg"
          }, 
          {
          "word": "passkey", 
          "synonym": "", 
          "example": "Getting no answer, they entered her room with a pass key.", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "First base", 
          "synonym": "", 
          "example": "Mattingly played first base for the Yankees.", 
          "video": "https://www.youtube.com/embed/2vznr4yuHpI"
          }, 
          {
          "word": "fall away", 
          "synonym": "", 
          "example": "On the other side of the hill, the land falls away sharply", 
          "video": "https://www.youtube.com/embed/gawx6aR2Pqg"
          }, 
          {
          "word": "passport", 
          "synonym": "", 
          "example": "Many refugees have arrived at the border without passports.", 
          "video": "https://www.youtube.com/embed/_wdqdaQgxqw"
          }, 
          {
          "word": "First come first served", 
          "synonym": "", 
          "example": "Free tickets will be given out on a first come, first served basis.", 
          "video": "https://www.youtube.com/embed/j7jT7O1LNJY"
          }, 
          {
          "word": "a passport to  sth", 
          "synonym": "", 
          "example": "Beauty alone can be a passport to success.", 
          "video": ""
          }, 
          {
          "word": "fall away/off", 
          "synonym": "", 
          "example": "Sales have been falling off recently.", 
          "video": "https://www.youtube.com/embed/Wtt4rWEGAmQ"
          }, 
          {
          "word": "at first hand", 
          "synonym": "", 
          "example": "Scientists observed the process at first hand.", 
          "video": "https://www.youtube.com/embed/AmJqym30LIM"
          }, 
          {
          "word": "fall back", 
          "synonym": "", 
          "example": "She fell back in horror/disgust.", 
          "video": "https://www.youtube.com/embed/cP3iCSQGFuA"
          }, 
          {
          "word": "password", 
          "synonym": "", 
          "example": "I can't let you in unless you give the password.", 
          "video": "https://www.youtube.com/embed/zmlUUrpekIQ"
          }, 
          {
          "word": "First out of the gate", 
          "synonym": "Out of the gate running", 
          "example": "My favorite horse was the first out of the gate when the race began.", 
          "video": ""
          }, 
          {
          "word": "be past it", 
          "synonym": "", 
          "example": "Don't ask Andy to enter the race", 
          "video": ""
          }, 
          {
          "word": "fall back on sth", 
          "synonym": "", 
          "example": "We had to fall back on our personal savings to pay our business overheads.", 
          "video": ""
          }, 
          {
          "word": "In the first place", 
          "synonym": "", 
          "example": "The trousers shrank when I washed them, but they weren't really big enough in the first place.", 
          "video": ""
          }, 
          {
          "word": "be past  your  sell", 
          "synonym": "", 
          "example": "There's plenty of time to have a baby. I'm not past my sell", 
          "video": ""
          }, 
          {
          "word": "fall behind", 
          "synonym": "", 
          "example": "He was ill for six weeks and fell behind with his schoolwork.", 
          "video": "https://www.youtube.com/embed/ORvaKPH2fu4"
          }, 
          {
          "word": "First water", 
          "synonym": "", 
          "example": "He is a fool of the first water.", 
          "video": "https://www.youtube.com/embed/NO63gsJD50g"
          }, 
          {
          "word": "fall down", 
          "example": "Our apple tree fell down in the storm.", 
          "video": "https://www.youtube.com/embed/06Kfck7AtLQ"
          }, 
          {
          "word": "not put it past  sb  to do  sth", 
          "synonym": "", 
          "example": "Perhaps Helena told him", 
          "video": ""
          }, 
          {
          "word": "Five finger discount", 
          "synonym": "Theft or pilferage, shoplifting.", 
          "example": "Whenever I walk past the candy rack, I give myself a five", 
          "video": "https://www.youtube.com/embed/NO63gsJD50g"
          }, 
          {
          "word": "fall down", 
          "synonym": "Failing, doing badly", 
          "example": "The deal fell down because there were a lot of unanswered questions", 
          "video": "https://www.youtube.com/embed/06Kfck7AtLQ"
          }, 
          {
          "word": "past", 
          "synonym": "", 
          "example": "The average temperature worldwide has risen by about one degree Fahrenheit in the past 100 years.", 
          "video": "https://www.youtube.com/embed/Q6jK8Rl3niQ"
          }, 
          {
          "word": "Jazz something up", 
          "synonym": "", 
          "example": "He jazzed up the food with a spicy sauce.", 
          "video": ""
          }, 
          {
          "word": "fairy cake", 
          "synonym": "Cupcake", 
          "example": "This fairy cake look so delicious.", 
          "video": "https://www.youtube.com/embed/Hb4apCIjUiQ"
          }, 
          {
          "word": "pass  sb/sth  over", 
          "synonym": "", 
          "example": "The woman alleges that her employers passed her over for promotion because she was pregnant.", 
          "video": ""
          }, 
          {
          "word": "Five oíclock shadow", 
          "synonym": "", 
          "example": "What made you want to look up five", 
          "video": "https://www.youtube.com/embed/eLIAP848Ax4"
          }, 
          {
          "word": "fall down on sth", 
          "synonym": "", 
          "example": "I'm quite good at speaking Chinese, but I fall down on the written work.", 
          "video": ""
          }, 
          {
          "word": "pasta", 
          "synonym": "", 
          "example": "Spaghetti, lasagne, ravioli, and cannelloni are all types of pasta.", 
          "video": "https://www.youtube.com/embed/1ElW26ZWBIs"
          }, 
          {
          "word": "All that jazz", 
          "synonym": "All that stuff; all that nonsense.", 
          "example": "She told me I was selfish, hateful, rude, ugly, and all that jazz.", 
          "video": "https://www.youtube.com/embed/M0lBQ9aXc1k"
          }, 
          {
          "word": "fairy godmother", 
          "synonym": "", 
          "example": "Cinderella's fairy godmother helped her go to the ball.", 
          "video": "https://www.youtube.com/embed/XXcRaY1wpIk"
          }, 
          {
          "word": "pass  sth  round", 
          "synonym": "", 
          "example": "Could you do me a favour and pass these sandwiches around?", 
          "video": ""
          }, 
          {
          "word": "Face the music", 
          "synonym": "", 
          "example": "Be a man and face the music.", 
          "video": "https://www.youtube.com/embed/qtdGg"
          }, 
          {
          "word": "fairyland", 
          "synonym": "", 
          "example": "It had snowed heavily during the night and in the morning the city was a white fairyland.", 
          "video": "https://www.youtube.com/embed/sMbflcozGSw"
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