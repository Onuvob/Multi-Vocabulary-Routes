<template>
  <div class="home">
    <div class="container">
      <Vocabularies v-bind:vocabularies="vocabularies"/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Vocabularies from '../components/Vocabularies.vue' 

export default {
  name: "home",
  components: {
    Vocabularies
  },

  data() {
    
    return{

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
          }, 
          {
          "word": "pass  sth  up", 
          "synonym": "", 
          "example": "He's never one to pass up a free meal.", 
          "video": ""
          }, 
          {
          "word": "Strike a false note", 
          "synonym": "", 
          "example": "I know she apologized, but it struck a false note with me I don't believe she meant what she said.", 
          "video": ""
          }, 
          {
          "word": "fairy lights", 
          "synonym": "", 
          "example": "Fairy lights add a touch of whimsy to any space.", 
          "video": "https://www.youtube.com/embed/deOFUZECYUk"
          }, 
          {
          "word": "pass", 
          "synonym": "", 
          "example": "I got a pass in my Literature course.", 
          "video": "https://www.youtube.com/embed/vz4t0CchIrM"
          }, 
          {
          "word": "Strike or hit the right note", 
          "synonym": "", 
          "example": "The commercial hit the right note with its target audience, and was one of the most highly rated spots of the year.", 
          "video": ""
          }, 
          {
          "word": "fairytale", 
          "synonym": "", 
          "example": "They had a fairy", 
          "video": "https://www.youtube.com/embed/ko2X"
          }, 
          {
          "word": "pass", 
          "synonym": "", 
          "example": "Messi pass the ball to Neymar.", 
          "video": "https://www.youtube.com/embed/vz4t0CchIrM"
          }, 
          {
          "word": "A done deal", 
          "synonym": "", 
          "example": "You  don’t have to worry about  the  merger it is a done  deal.", 
          "video": ""
          }, 
          {
          "word": "A heavy cross to bear", 
          "synonym": "", 
          "example": "When Nancy's husband passed away, she was left with quite a cross to bear having to raise four children on her own.", 
          "video": ""
          }, 
          {
          "word": "A bad workman blames his tools", 
          "synonym": "Accusing", 
          "example": "When Mary blamed the oven for burning the turkey on Thanksgiving, her husband jokingly replied, 'a bad workman always blames his tools.'", 
          "video": "https://www.youtube.com/embed/XlS8HYCrjLc"
          }, 
          {
          "word": "A baptism by fire", 
          "synonym": "", 
          "example": "I was given a million", 
          "video": "https://www.youtube.com/embed/jNOgdCiPquA"
          }, 
          {
          "word": "A big/great girl's blouse coward", 
          "synonym": "Baby, Girl, Adventurer", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "A bitter pill to swallow", 
          "synonym": "Diificult things.", 
          "example": "Losing to a younger player was a bitter pill to swallow.", 
          "video": "https://www.youtube.com/embed/lJfVcAibhCg"
          }, 
          {
          "word": "A black sheep.", 
          "synonym": "", 
          "example": "My oldest brother was the black sheep in our family. He dropped out of school at fifteen.", 
          "video": ""
          }, 
          {
          "word": "A blast from the past", 
          "synonym": "Reminding", 
          "example": "Bumping into my old high school sweetheart in the grocery store was a real blast from the past.", 
          "video": "https://www.youtube.com/embed/aHRiQFdlLds"
          }, 
          {
          "word": "A blinding flash", 
          "synonym": "", 
          "example": "The answer came to her in a blinding flash.", 
          "video": ""
          }, 
          {
          "word": "A blitz on something", 
          "synonym": "Go to great lengths", 
          "example": "We had a blitz on the house at the weekend and cleaned it completely.", 
          "video": ""
          }, 
          {
          "word": "A blot on somebodyís character", 
          "synonym": "Black mark", 
          "example": "A blot on somebodyís character ruins that person, no matter how much money he has.", 
          "video": ""
          }, 
          {
          "word": "A blot on the landscape", 
          "synonym": "Inelegant", 
          "example": "Although many people say that they want clean energy, they argue  that miles of turbines on wind farms are a blot on the landscape.", 
          "video": ""
          }, 
          {
          "word": "A bolt from the blue.", 
          "synonym": "", 
          "example": "The resignation of the chairman came like a bolt from the blue.", 
          "video": ""
          }, 
          {
          "word": "A bolt out of the blue", 
          "synonym": "Surprise", 
          "example": "The resignation of the chairman came like a bolt from the blue.", 
          "video": "https://www.youtube.com/embed/hUzB5auYRI0"
          }, 
          {
          "word": "A bone of contention.", 
          "synonym": "", 
          "example": "Money is a common bone of contention in many marriages.", 
          "video": ""
          }, 
          {
          "word": "A boot up the backside", 
          "synonym": "", 
          "example": "She's so lazy", 
          "video": ""
          }, 
          {
          "word": "A bottleneck", 
          "synonym": "", 
          "example": "Micromanaging cause bottlenecking and we never get any work done.", 
          "video": ""
          }, 
          {
          "word": "A change is as good as a rest", 
          "synonym": "", 
          "example": "You need to change jobs to prevent exhaustion, a change is as good as a rest.", 
          "video": ""
          }, 
          {
          "word": "A cheap shot", 
          "synonym": "", 
          "example": "Bringing up his disability in the argument was a cheap shot.", 
          "video": ""
          }, 
          {
          "word": "A chicken and egg situation", 
          "synonym": "", 
          "example": "The patent office has to deal with hundreds of chicken and egg situations daily.", 
          "video": ""
          }, 
          {
          "word": "A chip off the old block", 
          "synonym": "", 
          "example": "After meeting you son I can see that he is a chip off the old block.", 
          "video": ""
          }, 
          {
          "word": "A contradiction in terms", 
          "synonym": "", 
          "example": "Most oxymoron are a contradiction in terms.", 
          "video": ""
          }, 
          {
          "word": "A convincing win/victory", 
          "synonym": "Believable", 
          "example": "They won a convincing victory.", 
          "video": ""
          }, 
          {
          "word": "A crock of shit", 
          "synonym": "", 
          "example": "'I'm really sorry!' 'What a crock'", 
          "video": "https://www.youtube.com/embed/acalHM06eF4"
          }, 
          {
          "word": "A cut above", 
          "synonym": "", 
          "example": "She thinks she's a cut above her neighbours.", 
          "video": "https://www.youtube.com/embed/EaSA439ZkFM  from 0:09 second"
          }, 
          {
          "word": "A damsel in distress", 
          "synonym": "Housewife, domestic goddess.", 
          "example": "When I got a flat tyre I had to wait for my boyfriend to come and help me, like a true damsel in distress!", 
          "video": "https://www.youtube.com/embed/T__yr5ksDs0"
          }, 
          {
          "word": "A dark horse", 
          "synonym": "", 
          "example": "He might be famous now but Usain Bolt was a dark horse in his debut run.", 
          "video": ""
          }, 
          {
          "word": "A dash", 
          "synonym": "Clipping,  chip.", 
          "example": "Add some butter and a dash of salt.", 
          "video": "https://www.youtube.com/embed/nqluA"
          }, 
          {
          "word": "A doss", 
          "synonym": "Easy, Does not need hard work", 
          "example": "Aye, and a chip cob, Wasim said, stretching out for a kip in a doss.", 
          "video": ""
          }, 
          {
          "word": "A fact of life", 
          "synonym": "Unpalatable fact", 
          "example": "Death is a fact of life everyone should accustom themselves with.", 
          "video": ""
          }, 
          {
          "word": "A fair crack of the whip", 
          "synonym": "impartial", 
          "example": "If I get a fair crack of the whip at the job interview I can get it.", 
          "video": ""
          }, 
          {
          "word": "A fair hearing", 
          "synonym": "impartial", 
          "example": "Both the defendant and prosecutor thought it was a fair hearing.", 
          "video": ""
          }, 
          {
          "word": "A feather in one’s cap", 
          "synonym": "", 
          "example": "Learning how to speak German was a nice feather on my cap.", 
          "video": ""
          }, 
          {
          "word": "A field day", 
          "synonym": "", 
          "example": "The kids had a field day at the water slide park.", 
          "video": ""
          }, 
          {
          "word": "A fish out of water", 
          "synonym": "", 
          "example": "When someone goes abroad they always feel like a fish out of water.", 
          "video": ""
          }, 
          {
          "word": "A foolís paradise.", 
          "synonym": "", 
          "example": "Joan lived in a fool's paradise, looking forward to a promotion she would never get.", 
          "video": ""
          }, 
          {
          "word": "A gala day.", 
          "synonym": "", 
          "example": "Republic Day is a gala day for the whole of India.", 
          "video": ""
          }, 
          {
          "word": "A gift from the gods", 
          "synonym": "", 
          "example": "He is a gift from the gods.", 
          "video": ""
          }, 
          {
          "word": "A hail of something", 
          "synonym": "praise, congratulate, compliment", 
          "example": "The courtís ruling was immediately hailed as a victory for freedom.", 
          "video": "https://www.youtube.com/embed/DsLuMCyP5"
          }, 
          {
          "word": "A hair", 
          "synonym": "become angry easily, reacting, baclash", 
          "example": "A hair", 
          "video": "https://www.youtube.com/embed/lD2QphUOwNE"
          }, 
          {
          "word": "A hair's breadth", 
          "synonym": "smallest possible distance, depth, climb", 
          "example": "The car only missed us by a hairís breadth.", 
          "video": "https://www.youtube.com/embed/MOvAxI"
          }, 
          {
          "word": "A hard nut to crack.", 
          "synonym": "", 
          "example": "This algebra equation sure is a hard nut to crack.", 
          "video": ""
          }, 
          {
          "word": "A henpecked husband", 
          "synonym": "", 
          "example": "Tom has a miserable family life as he is a henpecked husband.", 
          "video": ""
          }, 
          {
          "word": "A herculean task", 
          "synonym": "", 
          "example": "An extremely difficult or dangerous task.", 
          "video": ""
          }, 
          {
          "word": "A jobbing actor/builder/gardener, etc.", 
          "synonym": "Freelancer, Honorary, Off", 
          "example": "He gradually establishes himself as a photographer and jobbing journalist reporting the war.", 
          "video": ""
          }, 
          {
          "word": "A kickback", 
          "synonym": "", 
          "example": "The property developers were accused of giving kickbacks to the local authorities.", 
          "video": "https://www.youtube.com/embed/6LYNE6Nm0OE&pbjreload=10 from 0:08 to 0:13 second"
          }, 
          {
          "word": "A laundry list.", 
          "synonym": "", 
          "example": "It wasn't much of a speech", 
          "video": "https://www.youtube.com/embed/Gsj9aMfOfm0"
          }, 
          {
          "word": "A leap in the dark", 
          "synonym": "", 
          "example": "You can’t calculate love you have to take a leap in the dark.", 
          "video": ""
          }, 
          {
          "word": "A level playing field", 
          "synonym": "Similar, Same, Equal, Even, Akin, Alike", 
          "example": "If the tax systems are different in each European country, how can industries start on a level playing field?", 
          "video": "https://www.youtube.com/embed/BdFuZR22cJI"
          }, 
          {
          "word": "A lick and a promise", 
          "synonym": "", 
          "example": "My maid washes all the utensils by a lick and a promise.", 
          "video": "https://www.youtube.com/embed/zUeeFIEmDew"
          }, 
          {
          "word": "A light", 
          "synonym": "", 
          "example": "Have you got a light, please?", 
          "video": "https://www.youtube.com/embed/c4HY5UoiQVo"
          }, 
          {
          "word": "A long line of.", 
          "synonym": "Queue, Single file, String of people, things etc.", 
          "example": "She is the latest in a long line of controversial leaders.", 
          "video": ""
          }, 
          {
          "word": "A long row to hoe", 
          "synonym": "", 
          "example": "Dealing with parent as a teacher is a long row to hoe.", 
          "video": ""
          }, 
          {
          "word": "A love/hate relationship", 
          "synonym": "A relationship in which you have feelings of love and hate for someone or something", 
          "example": "The father and son share a loving relationship.", 
          "video": "https://www.youtube.com/embed/gbb"
          }, 
          {
          "word": "A man of action", 
          "synonym": "", 
          "example": "Most leaders talk a lot but few are men of action.", 
          "video": ""
          }, 
          {
          "word": "A man/woman of means.", 
          "synonym": "", 
          "example": "His extravagant spending habits led everyone to believe that he was a man of means.", 
          "video": ""
          }, 
          {
          "word": "A matter of form", 
          "synonym": "", 
          "example": "Marx wasn’t too keen on doing the paper work but it was a matter of form.", 
          "video": ""
          }, 
          {
          "word": "A means to an end.", 
          "synonym": "", 
          "example": "I didn't particularly like the job", 
          "video": ""
          }, 
          {
          "word": "A meeting of minds.", 
          "synonym": "", 
          "example": "After debating for hours, we finally came to a meeting of minds and decided on a name for our band.", 
          "video": ""
          }, 
          {
          "word": "A nod's as good as a wink.", 
          "synonym": "", 
          "example": "", 
          "video": "https://www.youtube.com/embed/8ZKjEXcx_po"
          }, 
          {
          "word": "A pair of scales", 
          "synonym": "Weighing machine, Balance,", 
          "example": "A large drinking container for beer or other alcoholic drink.", 
          "video": ""
          }, 
          {
          "word": "A pearl of great price", 
          "synonym": "", 
          "example": "Inexhaustible patience is a pearl of great price.", 
          "video": ""
          }, 
          {
          "word": "A penny saved is a penny earned.", 
          "synonym": "Cut, cut back.", 
          "example": "I'd advise anyone to put aside a proportion of their earnings", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "A piece / slice of the action", 
          "synonym": "", 
          "example": "When it comes to lawsuits, everyone seems to wanta piece of the action.", 
          "video": ""
          }, 
          {
          "word": "A reach of the imagination", 
          "synonym": "Imagining and conceiving.", 
          "example": "It takes quite a reach of the imagination to believe that story.", 
          "video": ""
          }, 
          {
          "word": "A red letter day", 
          "synonym": "", 
          "example": "The day I graduated was a red letter day.", 
          "video": ""
          }, 
          {
          "word": "A reflection on  sb/sth", 
          "synonym": "", 
          "example": "Low test scores are a sad reflection on our school system.", 
          "video": ""
          }, 
          {
          "word": "A scintilla of  sth", 
          "synonym": "", 
          "example": "There's not a scintilla of truth in what he says.", 
          "video": ""
          }, 
          {
          "word": "A screw loose", 
          "synonym": "", 
          "example": "She wears a fur coat in the summer", 
          "video": "https://www.youtube.com/embed/6xSfsK_Y31w"
          }, 
          {
          "word": "A second bite of the cherry", 
          "synonym": "Opportunity", 
          "example": "He missed a medal in the 100 meters, but will get a second bite of the cherry in the 400 meters.", 
          "video": "https://www.youtube.com/embed/AOrr_s0V2_g?t=18s"
          }, 
          {
          "word": "A square deal", 
          "synonym": "", 
          "example": "The mugger getting 10 years in prison for assaulted robbery was a square deal.", 
          "video": ""
          }, 
          {
          "word": "A sweet tooth", 
          "synonym": "", 
          "example": "Charles has a sweet tooth so we have to always keep some sweets at home.", 
          "video": ""
          }, 
          {
          "word": "A tad", 
          "synonym": "A little, slightly.", 
          "example": "The fish was OK, but the chips were a tad greasy.", 
          "video": "https://www.youtube.com/embed/6oRy5G7oH6E"
          }, 
          {
          "word": "A thorn in one’s side", 
          "synonym": "", 
          "example": "My younger cousin is really a thorn in my side as he requires constant attention.", 
          "video": ""
          }, 
          {
          "word": "A thousand times", 
          "synonym": "", 
          "example": "This poison is a thousand", 
          "video": "https://www.youtube.com/embed/FzWb1B96"
          }, 
          {
          "word": "A turn coat.", 
          "synonym": "", 
          "example": "He was a turncoat, changing sides for advantage.", 
          "video": ""
          }, 
          {
          "word": "A wet blanket", 
          "synonym": "", 
          "example": "I would like to invite Russell over for the party but he is a wet blanket and he will ruin the mood of the party.", 
          "video": ""
          }, 
          {
          "word": "Abandon yourself to something", 
          "synonym": "", 
          "example": "He began to cry in earnest, abandoning himself to a storm of weeping, sobbing against his folded arms.", 
          "video": ""
          }, 
          {
          "word": "Abase yourself", 
          "synonym": "", 
          "example": "The members of the Political Executive Committee abased themselves once more.", 
          "video": ""
          }, 
          {
          "word": "Abashed", 
          "synonym": "", 
          "example": "Both girls fixed their eyes on the ground, abashed.", 
          "video": ""
          }, 
          {
          "word": "Abate", 
          "synonym": "", 
          "example": "The storm/wind/rain has started to abate.", 
          "video": ""
          }, 
          {
          "word": "Abbey", 
          "synonym": "", 
          "example": "We glimpsed the ruined abbey from the windows of the train.", 
          "video": ""
          }, 
          {
          "word": "Abbreviated piece of nothing", 
          "synonym": "", 
          "example": "Bob doesn't think much of his new colleague. He calls him an abbreviated piece of nothing.", 
          "video": ""
          }, 
          {
          "word": "Abdomen Human body", 
          "synonym": "", 
          "example": "Abdomens need to warm all the time or you will have trouble digesting", 
          "video": ""
          }, 
          {
          "word": "Abduct", 
          "synonym": "", 
          "example": "the millionaire who disappeared may have been abductedí", 
          "video": ""
          }, 
          {
          "word": "Abet", 
          "synonym": "", 
          "example": "ëhe was not guilty of murder but was guilty of aiding and abetting othersí", 
          "video": ""
          }, 
          {
          "word": "Abhor", 
          "synonym": "", 
          "example": "ëhe abhorred sexism in every formí", 
          "video": ""
          }, 
          {
          "word": "Abide by something", 
          "synonym": "", 
          "example": "I said I would abide by their decisioní", 
          "video": ""
          }, 
          {
          "word": "Abide by", 
          "synonym": "", 
          "example": "If you want to stay at this school, you must abide by the rules.", 
          "video": "https://www.youtube.com/embed/AtdBpXnO0KM"
          }, 
          {
          "word": "Abide", 
          "synonym": "", 
          "example": "ëat least one memory will abideí", 
          "video": ""
          }, 
          {
          "word": "Abjure", 
          "synonym": "", 
          "example": "MPs were urged to abjure their Jacobite allegianceí", 
          "video": ""
          }, 
          {
          "word": "Ablaze", 
          "synonym": "", 
          "example": "his clothes were ablazeí", 
          "video": ""
          }, 
          {
          "word": "Ablution", 
          "synonym": "", 
          "example": "the women performed their ablutionsí", 
          "video": ""
          }, 
          {
          "word": "Abnormal", 
          "synonym": "", 
          "example": "They found abnormal levels of lead in the water.", 
          "video": "https://www.youtube.com/embed/BQWGUNqTlto?t=1s"
          }, 
          {
          "word": "Abode", 
          "synonym": "", 
          "example": "ëmy humble abodeí", 
          "video": ""
          }, 
          {
          "word": "Abominate", 
          "synonym": "", 
          "example": "they abominated the very idea of monarchyí", 
          "video": ""
          }, 
          {
          "word": "Aboriginal", 
          "synonym": "", 
          "example": "Relating to the Australian Aborigines or their languages.", 
          "video": ""
          }, 
          {
          "word": "Abortive stop", 
          "synonym": "", 
          "example": "ëthe rebel officers who led the abortive coup were shotí", 
          "video": ""
          }, 
          {
          "word": "Abound in/with something", 
          "synonym": "", 
          "example": "this area abounds with caravan sitesí", 
          "video": ""
          }, 
          {
          "word": "Abound", 
          "synonym": "", 
          "example": "rumors of a further scandal aboundí", 
          "video": ""
          }, 
          {
          "word": "About turn", 
          "synonym": "", 
          "example": "ëhe did an about", 
          "video": ""
          }, 
          {
          "word": "Above and beyond the call of duty", 
          "synonym": "", 
          "example": "The fire", 
          "video": ""
          }, 
          {
          "word": "Above board", 
          "synonym": "", 
          "example": "There are not secret negotiations.  Our dealings have always been above board.", 
          "video": "https://www.youtube.com/embed/OqkwcfuP"
          }, 
          {
          "word": "Above mention", 
          "synonym": "", 
          "example": "ëthe above", 
          "video": ""
          }, 
          {
          "word": "Above the call of duty", 
          "synonym": "", 
          "example": "The fire", 
          "video": ""
          }, 
          {
          "word": "Abrasive cleaning substance", 
          "synonym": "", 
          "example": "ëthe wood should be rubbed down with fine abrasive paperí", 
          "video": ""
          }, 
          {
          "word": "Abrasive rude", 
          "synonym": "", 
          "example": "ëher abrasive and arrogant personal style won her few friendsí", 
          "video": ""
          }, 
          {
          "word": "Abreast", 
          "synonym": "", 
          "example": "ëthe path was wide enough for two people to walk abreastí", 
          "video": ""
          }, 
          {
          "word": "Abridge", 
          "synonym": "", 
          "example": "an abridged text of his speechí", 
          "video": ""
          }, 
          {
          "word": "Abroad", 
          "synonym": "", 
          "example": "ëwe usually go abroad for a week in Mayí", 
          "video": ""
          }, 
          {
          "word": "Abrogate", 
          "synonym": "", 
          "example": "ëa proposal to abrogate temporarily the right to strikeí", 
          "video": ""
          }, 
          {
          "word": "Abrupt sudden", 
          "synonym": "", 
          "example": "ëI was surprised by the abrupt change of subjectí", 
          "video": ""
          }, 
          {
          "word": "Abrupt unfriendly", 
          "synonym": "", 
          "example": "ëyou were rather abrupt with that young maní", 
          "video": ""
          }, 
          {
          "word": "Abscond Skill", 
          "synonym": "", 
          "example": "ëcharges of absconding while on bailí", 
          "video": ""
          }, 
          {
          "word": "Abscond escape", 
          "synonym": "", 
          "example": "ëthe barman absconded with a week's takingsí", 
          "video": ""
          }, 
          {
          "word": "Abseil", 
          "synonym": "", 
          "example": "ëteam members had to abseil down sheer cliffs to reach the coupleí", 
          "video": ""
          }, 
          {
          "word": "Absent", 
          "synonym": "", 
          "example": "ëan absent", 
          "video": ""
          }, 
          {
          "word": "Absentee", 
          "synonym": "", 
          "example": "ëan absentee from the matchí", 
          "video": ""
          }, 
          {
          "word": "Abstain  not to do something", 
          "synonym": "", 
          "example": "ëshe intends to abstain from sex before marriageí", 
          "video": ""
          }, 
          {
          "word": "Abstain  not vote", 
          "synonym": "", 
          "example": "ëforty", 
          "video": ""
          }, 
          {
          "word": "Abstemious", 
          "synonym": "", 
          "example": "ëëWe only had a bottle.í ëVery abstemious of you.íí", 
          "video": ""
          }, 
          {
          "word": "Abstruse", 
          "synonym": "", 
          "example": "ëan abstruse philosophical inquiryí", 
          "video": ""
          }, 
          {
          "word": "Abundance", 
          "synonym": "", 
          "example": "ëthe tropical island boasts an abundance of wildlifeí", 
          "video": ""
          }, 
          {
          "word": "Abuzz", 
          "synonym": "", 
          "example": "ëthe room was abuzz with mosquitoesí", 
          "video": ""
          }, 
          {
          "word": "Abysmal", 
          "synonym": "", 
          "example": "ëthe quality of her work is abysmal", 
          "video": ""
          }, 
          {
          "word": "Abyss", 
          "synonym": "", 
          "example": "ëteetering on the edge of the abyss of a total political wipeoutí", 
          "video": ""
          }, 
          {
          "word": "Acacia tree", 
          "synonym": "", 
          "example": "Australia is littered with Acacia.", 
          "video": ""
          }, 
          {
          "word": "Academe", 
          "synonym": "", 
          "example": "ëbridging the gap between industry and academeí", 
          "video": ""
          }, 
          {
          "word": "Academia", 
          "synonym": "", 
          "example": "ëhe spent his working life in academiaí", 
          "video": ""
          }, 
          {
          "word": "Accelerate", 
          "synonym": "", 
          "example": "Inflation is likely to accelerate this year.", 
          "video": "https://www.youtube.com/embed/NKB0YwREWAE?t=2s"
          }, 
          {
          "word": "Accentuate", 
          "synonym": "", 
          "example": "ëhis jacket unfortunately accentuated his paunchí", 
          "video": ""
          }, 
          {
          "word": "Accept/take sth on faith", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Accessory after the fact", 
          "synonym": "", 
          "example": "Donít mingle with your criminal cousin he will make you an accessory after the fact.", 
          "video": ""
          }, 
          {
          "word": "Accessory before the fact", 
          "synonym": "", 
          "example": "Donít mingle with your criminal cousin he will make you an accessory after the fact.", 
          "video": ""
          }, 
          {
          "word": "Accessory", 
          "synonym": "", 
          "example": "They find pleasure in looking at different clothes, shoes, accessories, gadgets and home furnishings.", 
          "video": "https://www.youtube.com/embed/Jq4fut6QC88"
          }, 
          {
          "word": "Accident prone", 
          "synonym": "", 
          "example": "ëhe's always been accident", 
          "video": ""
          }, 
          {
          "word": "Accident waiting to happen", 
          "synonym": "", 
          "example": "An ageing nuclear reactor is an accident waiting to happen.", 
          "video": ""
          }, 
          {
          "word": "Accident", 
          "synonym": "", 
          "example": "ëhe had an accident at the factoryí", 
          "video": ""
          }, 
          {
          "word": "Accidental", 
          "synonym": "", 
          "example": "When old people die it is better to confirm accidental death with an autopsy.", 
          "video": ""
          }, 
          {
          "word": "Accidentally on purpose", 
          "synonym": "", 
          "example": "I've never liked these glasses of Peter's. I might drop them one day ", 
          "video": ""
          }, 
          {
          "word": "Accidents will happen", 
          "synonym": "", 
          "example": "I donít blame my students if they break something, accidents will happen.", 
          "video": ""
          }, 
          {
          "word": "Acclaimed", 
          "synonym": "", 
          "example": "In order to avoid embarrassing inconsistency in the next meeting, I suggest inviting Colin Briggs, the acclaimed footballer, to talk to his fans.", 
          "video": "https://www.youtube.com/embed/xTL9NPPPAtU"
          }, 
          {
          "word": "Acclimatize", 
          "synonym": "", 
          "example": "ëit's unknown whether people will acclimatize to increasingly warm weatherí", 
          "video": ""
          }, 
          {
          "word": "Accolade", 
          "synonym": "", 
          "example": "ëthe hotel has won numerous accoladesí", 
          "video": ""
          }, 
          {
          "word": "Accommodation", 
          "synonym": "", 
          "example": "She arranged an accommodation for her daughter/", 
          "video": "https://www.youtube.com/embed/tzNvs61ZMZw from 0:32 second to 0:47 second"
          }, 
          {
          "word": "Accompany", 
          "synonym": "", 
          "example": "The two sisters were to accompany us to London.", 
          "video": "https://www.youtube.com/embed/izM6TqQElmI up to 0:12 second"
          }, 
          {
          "word": "Accomplice", 
          "synonym": "", 
          "example": "ëan accomplice in the murderí", 
          "video": ""
          }, 
          {
          "word": "Accomplish", 
          "synonym": "", 
          "example": "I feel as if I've accomplished nothing all day.", 
          "video": "https://www.youtube.com/embed/_9U6_4Qon5Y"
          }, 
          {
          "word": "Accord v", 
          "synonym": "", 
          "example": "ëthe powers accorded to the head of stateí", 
          "video": ""
          }, 
          {
          "word": "Accord with something", 
          "synonym": "", 
          "example": "ëhis views accorded well with those of Merivaleí", 
          "video": ""
          }, 
          {
          "word": "Accord", 
          "synonym": "", 
          "example": "ëopposition groups refused to sign the accordí", 
          "video": ""
          }, 
          {
          "word": "Accordion", 
          "synonym": "", 
          "example": "The Accordion is popular in Europe.", 
          "video": ""
          }, 
          {
          "word": "Accost", 
          "synonym": "", 
          "example": "ëreporters accosted him in the streetí", 
          "video": ""
          }, 
          {
          "word": "Account for", 
          "synonym": "", 
          "example": "I hope you can account for all the money you spent!", 
          "video": "https://www.youtube.com/embed/ZJm8UpMTpCk?t=5s"
          }, 
          {
          "word": "Accumulate", 
          "synonym": "", 
          "example": "The chemicals accumulate in your body.", 
          "video": "https://www.youtube.com/embed/oBuKQ7dLUeI?t=10s"
          }, 
          {
          "word": "Accurate", 
          "synonym": "", 
          "example": "Accurate information about the illness is essential.", 
          "video": "https://www.youtube.com/embed/OO9pEwTnCMU"
          }, 
          {
          "word": "Accursed", 
          "synonym": "", 
          "example": "ëthe Angel of Death walks this accursed houseí", 
          "video": ""
          }, 
          {
          "word": "Accustom yourself to something", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Accustomed", 
          "synonym": "", 
          "example": "I've worked nights for years now so I've grown accustomed to it.", 
          "video": "https://www.youtube.com/embed/nKYgFROSloo"
          }, 
          {
          "word": "Ace v", 
          "synonym": "", 
          "example": "I aced the test today since it was so easy.", 
          "video": ""
          }, 
          {
          "word": "Ace a test", 
          "synonym": "", 
          "example": "Maria's parents said she could go to the party if she aced her English test.", 
          "video": ""
          }, 
          {
          "word": "Ace a test", 
          "synonym": "", 
          "example": "Maria's parents said she could go to the party if she aced her English test.", 
          "video": ""
          }, 
          {
          "word": "Ace in the hole", 
          "synonym": "", 
          "example": "Our candidate has an ace in the hole that will ensure victory ... you'll see!", 
          "video": ""
          }, 
          {
          "word": "Ace in the hole", 
          "synonym": "", 
          "example": "Our candidate has an ace in the hole that will ensure victory ... you'll see!", 
          "video": ""
          }, 
          {
          "word": "Ace up your sleeve", 
          "synonym": "", 
          "example": "I am not worried about Steveís competition as I have a ace up my sleeve.", 
          "video": ""
          }, 
          {
          "word": "Ace up your sleeve", 
          "synonym": "", 
          "example": "Our new product is an ace up our sleeve.", 
          "video": "https://www.youtube.com/embed/H6ZlwqHxOGw&list=PLoIr30tNT8CYMKdJlVbaF"
          }, 
          {
          "word": "Ace", 
          "synonym": "", 
          "example": "Best tennis players can ace any novice easily.", 
          "video": ""
          }, 
          {
          "word": "Ace", 
          "synonym": "", 
          "example": "You are likely to win if you have more aces in your hand.", 
          "video": ""
          }, 
          {
          "word": "Ace", 
          "synonym": "", 
          "example": "You should take Jimmy he is an ace pilot.", 
          "video": ""
          }, 
          {
          "word": "Ache for something", 
          "synonym": "", 
          "example": "I ached for a cold drink in the hot summer day.", 
          "video": ""
          }, 
          {
          "word": "Ache for", 
          "synonym": "", 
          "example": "He was so lonely he ached for the sound of a human voice.", 
          "video": ""
          }, 
          {
          "word": "Ache", 
          "synonym": "", 
          "example": "The ache in her head worsened", 
          "video": "https://www.youtube.com/embed/yb0knjYtEaE"
          }, 
          {
          "word": "Achilles heel", 
          "synonym": "", 
          "example": "ëthe Achilles heel of the case for nuclear power remains the issue of the disposal of wasteí", 
          "video": ""
          }, 
          {
          "word": "Achilles heel.", 
          "synonym": "", 
          "example": "He's extremely intelligent, but his inability to speak in public is his Achilles heel.", 
          "video": "https://www.youtube.com/embed/MkyrNHKh6Uc"
          }, 
          {
          "word": "Achilles tendon human body", 
          "synonym": "", 
          "example": "Achilles tendon are easy to get damaged, so better to stretch before running.", 
          "video": ""
          }, 
          {
          "word": "Acid rain", 
          "synonym": "", 
          "example": "Acid rain is ruining the Taj Mahal.", 
          "video": ""
          }, 
          {
          "word": "Acid test", 
          "synonym": "", 
          "example": "The training course was very interesting but the acid test will come when I start my new job.", 
          "video": ""
          }, 
          {
          "word": "Acid test", 
          "synonym": "", 
          "example": "ëgritstone is the acid test of a climber's abilityí", 
          "video": ""
          }, 
          {
          "word": "Acknowledge", 
          "synonym": "", 
          "example": "He acknowledged that there was a problem.", 
          "video": "https://www.youtube.com/embed/NncPe9"
          }, 
          {
          "word": "Acne", 
          "synonym": "", 
          "example": "ëhe was clean", 
          "video": ""
          }, 
          {
          "word": "Acolyte", 
          "synonym": "", 
          "example": "ëshe runs the department through a small group of acolytesí", 
          "video": ""
          }, 
          {
          "word": "Acorn", 
          "synonym": "", 
          "example": "Acorns are surprisingly hard, I wonder how squirrels eat them.", 
          "video": ""
          }, 
          {
          "word": "Acoustic", 
          "synonym": "", 
          "example": "ëdogs have a much greater acoustic range than humansí", 
          "video": ""
          }, 
          {
          "word": "Acquaint somebody to something", 
          "synonym": "", 
          "example": "Take time to acquaint yourself with the rules.", 
          "video": ""
          }, 
          {
          "word": "Acquaintance", 
          "synonym": "", 
          "example": "He's just a business acquaintance.", 
          "video": "https://www.youtube.com/embed/M6THze1B6NI"
          }, 
          {
          "word": "Acquisition", 
          "synonym": "", 
          "example": "ëthe legacy will be used for new acquisitionsí", 
          "video": ""
          }, 
          {
          "word": "Acrid", 
          "synonym": "", 
          "example": "ëan acrid smellí", 
          "video": ""
          }, 
          {
          "word": "Acrimonious", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Acrobat", 
          "synonym": "", 
          "example": "Acrobat are a lot of fun to watch at circuses.", 
          "video": ""
          }, 
          {
          "word": "Acrobatics", 
          "synonym": "", 
          "example": "ëshe sealed the title with a powerful display of acrobatics and tumblingí", 
          "video": ""
          }, 
          {
          "word": "Acrostic", 
          "synonym": "", 
          "example": "As English is my second language I have trouble playing acrostic games.", 
          "video": ""
          }, 
          {
          "word": "Acrylic", 
          "synonym": "", 
          "example": "ëa red acrylic jumperí", 
          "video": ""
          }, 
          {
          "word": "Act on", 
          "synonym": "", 
          "example": "The police decided to act on the anonymous call they received.", 
          "video": "https://www.youtube.com/embed/bwU7L0KSFj4"
          }, 
          {
          "word": "Act out", 
          "synonym": "", 
          "example": "The children acted out the scene in the classroom.", 
          "video": "https://www.youtube.com/embed/bFTIJXn7SAg?t=2s 0:02"
          }, 
          {
          "word": "Act the fool", 
          "synonym": "", 
          "example": "Tommy always acts the fool but he is a smart man.", 
          "video": ""
          }, 
          {
          "word": "Act up", 
          "synonym": "", 
          "example": "Dad's poor knee is acting up again.", 
          "video": "https://www.youtube.com/embed/X2uwQPu_bvk"
          }, 
          {
          "word": "Act/do  sth  on  your  own responsibility", 
          "synonym": "", 
          "example": "In critical situation, we expext our employess to act/ do sth on their own responsibilty.", 
          "video": ""
          }, 
          {
          "word": "Acting chairman/manager", 
          "synonym": "", 
          "example": "He'll be the acting director until they can appoint a permanent one.", 
          "video": ""
          }, 
          {
          "word": "Action packed", 
          "synonym": "", 
          "example": "an action", 
          "video": ""
          }, 
          {
          "word": "Action replay", 
          "synonym": "", 
          "example": "They showed an action replay of the goal.", 
          "video": ""
          }, 
          {
          "word": "Action stations", 
          "synonym": "", 
          "example": "The whole school was at action stations for the inspectors' visit.", 
          "video": ""
          }, 
          {
          "word": "Action", 
          "synonym": "", 
          "example": "Ending child labour will require action on many levels.", 
          "video": "https://www.youtube.com/embed/SU3UEVWgpww"
          }, 
          {
          "word": "Actions speaks louder than words", 
          "synonym": "", 
          "example": "I like to talk less and work more as I believe actions speaks louder than words.", 
          "video": ""
          }, 
          {
          "word": "Activism", 
          "synonym": "", 
          "example": "ëgrowing activism on the abortion issueí", 
          "video": ""
          }, 
          {
          "word": "Activity holiday", 
          "synonym": "", 
          "example": "Camping is a great activity holiday.", 
          "video": ""
          }, 
          {
          "word": "Acuity", 
          "synonym": "", 
          "example": "ëintellectual acuityí", 
          "video": ""
          }, 
          {
          "word": "Acumen", 
          "synonym": "", 
          "example": "ëshe hides a shrewd business acumení", 
          "video": ""
          }, 
          {
          "word": "Acupuncture", 
          "synonym": "", 
          "example": "Chinese still prefer acupuncture over modern medicine.", 
          "video": ""
          }, 
          {
          "word": "Ad hoc", 
          "synonym": "", 
          "example": "ëthe discussions were on an ad hoc basisí", 
          "video": ""
          }, 
          {
          "word": "Adage", 
          "synonym": "", 
          "example": "ëthe old adage ëout of sight out of mindíí", 
          "video": ""
          }, 
          {
          "word": "Adagio", 
          "synonym": "", 
          "example": "Barber's Adagio for Strings", 
          "video": ""
          }, 
          {
          "word": "Adamant", 
          "synonym": "", 
          "example": "ëhe is adamant that he is not going to resigní", 
          "video": ""
          }, 
          {
          "word": "Adamís apple", 
          "synonym": "", 
          "example": "I got hit on the Adamís apple once and it hurt a lot.", 
          "video": ""
          }, 
          {
          "word": "Add up", 
          "synonym": "", 
          "example": "She explained what happened but the details she gave just don't add up.", 
          "video": "https://www.youtube.com/embed/JYBocT7gxtE?t=2s"
          }, 
          {
          "word": "Add", 
          "synonym": "", 
          "example": "ëcars with add", 
          "video": ""
          }, 
          {
          "word": "Added value", 
          "synonym": "", 
          "example": "The printer's added value makes it worth the extracost.", 
          "video": ""
          }, 
          {
          "word": "Adder", 
          "synonym": "", 
          "example": "Britain is known for having a lot of adders.", 
          "video": ""
          }, 
          {
          "word": "Addiction", 
          "synonym": "", 
          "example": "His addiction to computer games means he is spending far too much time indoors.", 
          "video": "https://www.youtube.com/embed/dKPxTVAABwM"
          }, 
          {
          "word": "Addition", 
          "synonym": "", 
          "example": "The hotel has been extended with the addition of more rooms.", 
          "video": "https://www.youtube.com/embed/vYMEzz2c2aE"
          }, 
          {
          "word": "Addle", 
          "synonym": "", 
          "example": "ëbeing in love must have addled your brainí", 
          "video": ""
          }, 
          {
          "word": "Adenoids", 
          "synonym": "", 
          "example": "My adenoids are acting up again.", 
          "video": ""
          }, 
          {
          "word": "Adept", 
          "synonym": "", 
          "example": "ëshe is adept at cutting through red tapeí", 
          "video": ""
          }, 
          {
          "word": "Adhere to", 
          "synonym": "", 
          "example": "All contestants must adhere to the rules.", 
          "video": "https://www.youtube.com/embed/TLy0z3C_hdo?t=1m59s"
          }, 
          {
          "word": "Adherent", 
          "synonym": "", 
          "example": "ëhe was a strong adherent of monetarismí", 
          "video": ""
          }, 
          {
          "word": "Adherent", 
          "synonym": "", 
          "example": "ëthe eggs have thick sticky shells to which debris is often adherentí", 
          "video": ""
          }, 
          {
          "word": "Adios", 
          "synonym": "", 
          "example": "My Spanish friend always uses Adios instead of goodbye", 
          "video": ""
          }, 
          {
          "word": "Adjacent", 
          "synonym": "", 
          "example": "ëadjacent roomsí", 
          "video": ""
          }, 
          {
          "word": "Adjoin", 
          "synonym": "", 
          "example": "ëthe dining room adjoins a conservatoryí", 
          "video": ""
          }, 
          {
          "word": "Adjourn to somewhere", 
          "synonym": "", 
          "example": "ëthey adjourned to a local pubí", 
          "video": ""
          }, 
          {
          "word": "Adjourn", 
          "synonym": "", 
          "example": "ëthe meeting was adjourned until December 4í", 
          "video": ""
          }, 
          {
          "word": "Adjunct", 
          "synonym": "", 
          "example": "ëcomputer technology is an adjunct to learningí", 
          "video": ""
          }, 
          {
          "word": "Adjure", 
          "synonym": "", 
          "example": "ëI adjure you to tell me the truthí", 
          "video": ""
          }, 
          {
          "word": "Adjutant", 
          "synonym": "", 
          "example": "ëhe eventually became adjutant to the commander of the tactical air forceí", 
          "video": ""
          }, 
          {
          "word": "Adman", 
          "synonym": "", 
          "example": "Admen do a lot of research to find what people want to see.", 
          "video": ""
          }, 
          {
          "word": "Administrative", 
          "synonym": "", 
          "example": "The work is largely administrative.", 
          "video": "https://www.youtube.com/embed/uvwF7eh2_fk?t=4s"
          }, 
          {
          "word": "Admiration", 
          "synonym": "", 
          "example": "I have the greatest admiration for all those are involved in the project.", 
          "video": "https://www.youtube.com/embed/diyI"
          }, 
          {
          "word": "Admit defeat", 
          "synonym": "", 
          "example": "I admit defeat! Burger King is better than White Castle.", 
          "video": ""
          }, 
          {
          "word": "Admit", 
          "synonym": "", 
          "example": "You know you're wrong! Admit it!", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Adult", 
          "synonym": "", 
          "example": "My brother is now grown up as an adult.", 
          "video": "https://www.youtube.com/embed/z3kvE4AiO4g?t=5s"
          }, 
          {
          "word": "Advanced", 
          "synonym": "", 
          "example": "The team advanced the ball steadily down the field.", 
          "video": "https://www.youtube.com/embed/3I7dCMEyhmc from 0:16 second"
          }, 
          {
          "word": "Advantage", 
          "synonym": "", 
          "example": "Companies with a computerized database are at an advantage.", 
          "video": "https://www.youtube.com/embed/uGPLP5OdLx8"
          }, 
          {
          "word": "Advise against", 
          "synonym": "", 
          "example": "The doctor advised him against carrying heavy loads.", 
          "video": ""
          }, 
          {
          "word": "Adviser", 
          "synonym": "", 
          "example": "Some of our financial advisers could provide your students [with] the latest methods used in Accounting and in developing new business projects.", 
          "video": "https://www.youtube.com/embed/JK1INfTABp0"
          }, 
          {
          "word": "Affluent", 
          "synonym": "", 
          "example": "Children who come from poor families are more mature and responsible than those children coming from affluent families.", 
          "video": "https://www.youtube.com/embed/uasEcmjyWJY"
          }, 
          {
          "word": "Afford", 
          "synonym": "", 
          "example": "The best that I could afford was a first", 
          "video": "https://www.youtube.com/embed/en_whbxYiNk"
          }, 
          {
          "word": "Affordale", 
          "synonym": "", 
          "example": "We need more affordable housing in this area.", 
          "video": "https://www.youtube.com/embed/d9Jx2YRfFtQ?t=4s"
          }, 
          {
          "word": "After a fashion.", 
          "synonym": "", 
          "example": "I can cook, after a fashion.", 
          "video": ""
          }, 
          {
          "word": "Against all the odds/against all odds", 
          "synonym": "Not expected or planned.", 
          "example": "Against all the odds, he recovered.", 
          "video": "https://www.youtube.com/embed/v7OZ5NiJBbU"
          }, 
          {
          "word": "Agency", 
          "synonym": "", 
          "example": "Tom works for a translation agency.", 
          "video": "https://www.youtube.com/embed/HtHtAT_5Y_I  from 0:27 second"
          }, 
          {
          "word": "Agenda", 
          "synonym": "", 
          "example": "There are several items on the agenda.", 
          "video": "https://www.youtube.com/embed/peC5cPuJ78U?t=6s"
          }, 
          {
          "word": "Agree with", 
          "synonym": "", 
          "example": "I agree with you. I think she deserves the award too.", 
          "video": "https://www.youtube.com/embed/aLX92tpsMfI?t=10s"
          }, 
          {
          "word": "Agree", 
          "synonym": "", 
          "example": "Does the information in the two reports agree?", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Ahead of schedule", 
          "synonym": "Early", 
          "example": "We expect the building work to be completed ahead of schedule.", 
          "video": ""
          }, 
          {
          "word": "Ahead of the pack", 
          "synonym": "", 
          "example": "Our products will have to be more innovative if we want to stay ahead of the pack. ", 
          "video": ""
          }, 
          {
          "word": "Ahead of the pack", 
          "synonym": "", 
          "example": "Our products will have to be more innovative if we want to stay ahead of the pack. ", 
          "video": ""
          }, 
          {
          "word": "Ahead of the pack", 
          "synonym": "", 
          "example": "Our products will have to be more innovative if we want to stay ahead of the pack. ", 
          "video": ""
          }, 
          {
          "word": "Ahead", 
          "synonym": "", 
          "example": "Shaila walked ahead of her.", 
          "video": "https://www.youtube.com/embed/lnz8AufJsT4"
          }, 
          {
          "word": "Aid", 
          "synonym": "", 
          "example": "Emergency aid was sent to the flood victims.", 
          "video": "https://www.youtube.com/embed/K05TeKxEAXI?t=5s"
          }, 
          {
          "word": "Aim at", 
          "synonym": "", 
          "example": "The policeman aimed his gun at the hijacker.", 
          "video": "https://www.youtube.com/embed/Su4d4aExp7k?t=6s"
          }, 
          {
          "word": "Alarm bells ringing.", 
          "synonym": "", 
          "example": "Alarm bells started to ring when my old neighbour didn't open his shutters all day and didn't answer his phone.", 
          "video": ""
          }, 
          {
          "word": "Alarm", 
          "synonym": "", 
          "example": "I don't want to alarm you but he really should be here by now.", 
          "video": "https://www.youtube.com/embed/CAGBqx_i1r0"
          }, 
          {
          "word": "Alarm", 
          "synonym": "", 
          "example": "The boat tilted and the boatmen cried out in alarm.", 
          "video": "https://www.youtube.com/embed/mi8PGY8S"
          }, 
          {
          "word": "Alert", 
          "synonym": "", 
          "example": "A young dog should be alert and playful.", 
          "video": "https://www.youtube.com/embed/TFfPORoSKzs"
          }, 
          {
          "word": "All along the line.", 
          "synonym": "", 
          "example": "The project's been plagued with financial problems all along the line.", 
          "video": ""
          }, 
          {
          "word": "All brawn and no brain", 
          "synonym": "", 
          "example": "He's an impressive player to watch, but he's all brawn and no brain.", 
          "video": ""
          }, 
          {
          "word": "All credit to sb.", 
          "synonym": "Explain, Argue, Excuse", 
          "example": "The team credited their victory to hard work.", 
          "video": ""
          }, 
          {
          "word": "All downhill/ downhill all the way", 
          "synonym": "", 
          "example": "The hardest part for the burglars was turning off the alarm system.  After that it was all downhill.", 
          "video": ""
          }, 
          {
          "word": "All downhill/ downhill all the way", 
          "synonym": "", 
          "example": "The hardest part for the burglars was turning off the alarm system.  After that it was all downhill.", 
          "video": ""
          }, 
          {
          "word": "All ears", 
          "synonym": "", 
          "example": "Give me a minute to finish my work and then I’ll be all ears to hear about your project.", 
          "video": ""
          }, 
          {
          "word": "All mouth and no trousers", 
          "synonym": "", 
          "example": "He keeps saying he's going to resign and travel around the world, but he's all mouth and no trousers.", 
          "video": "https://www.youtube.com/embed/ozGY4_jqjDU"
          }, 
          {
          "word": "All sizzle and no steak", 
          "synonym": "", 
          "example": "Because of the electoral promises he made, which so far he has failed to keep, many people call the new president 'all sizzle and no steak'.", 
          "video": "https://www.youtube.com/embed/sRHbQTOJ5Eg"
          }, 
          {
          "word": "All skin and bone", 
          "synonym": "", 
          "example": "After trekking in the Himalayas, he was all skin and bone.", 
          "video": "https://www.youtube.com/embed/eaShxTDCjQA"
          }, 
          {
          "word": "All things to all people", 
          "synonym": "", 
          "example": "She's exhausted tying to be a good wife,  a good mother and a good teacher,  but she can't be all things to all people.", 
          "video": ""
          }, 
          {
          "word": "All's fair in love and war", 
          "synonym": "", 
          "example": "I will try any trick to win, you know all's fair in love and war.", 
          "video": ""
          }, 
          {
          "word": "Allegation", 
          "synonym": "", 
          "example": "He denied allegations that he had cheated.", 
          "video": "https://www.youtube.com/embed/DXRkBGFrIng"
          }, 
          {
          "word": "Allocate", 
          "synonym": "", 
          "example": "The government has promised to allocate extra money for health care.", 
          "video": "https://www.youtube.com/embed/lCwu7wVj"
          }, 
          {
          "word": "Allow for", 
          "synonym": "", 
          "example": "It will take longer. You have to allow for heavy traffic at rush hour.", 
          "video": "https://www.youtube.com/embed/uPeiWLOYDlQ"
          }, 
          {
          "word": "Allowance", 
          "synonym": "", 
          "example": "She spends most of her allowance quickly and is then without money for the rest of the month.", 
          "video": "https://www.youtube.com/embed/x0OSFAe"
          }, 
          {
          "word": "Allude to", 
          "synonym": "", 
          "example": "I don't understand. What problem is she alluding to?", 
          "video": "https://www.youtube.com/embed/PrWoGq24EzA"
          }, 
          {
          "word": "Ally", 
          "synonym": "", 
          "example": "He is generally considered to be the Prime Minister's closest political ally.", 
          "video": "https://www.youtube.com/embed/GSs4zwMg6lI"
          }, 
          {
          "word": "Along the lines of something / Along those lines.", 
          "synonym": "Similar to, Akin, Alike.", 
          "example": "I was thinking of doing a meal along the lines of that dinner I did for Annie and Dave.", 
          "video": ""
          }, 
          {
          "word": "Aloud", 
          "synonym": "", 
          "example": "He read the letter aloud.", 
          "video": "https://www.youtube.com/embed/fERCyS"
          }, 
          {
          "word": "Also", 
          "synonym": "", 
          "example": "He entered the contest hoping that he wouldn't end up as an ëalso", 
          "video": ""
          }, 
          {
          "word": "Also", 
          "synonym": "", 
          "example": "He entered the contest hoping that he wouldn't end up as an ‘also", 
          "video": ""
          }, 
          {
          "word": "Alter ego", 
          "synonym": "", 
          "example": "Superman is Clark Kent's alter ego.", 
          "video": "https://www.youtube.com/embed/LSY0XEzSc8A from 0:11 second"
          }, 
          {
          "word": "Amateur", 
          "synonym": "", 
          "example": "Finally I would like to mention that I feel very confident in front of cameras, since I am an amateur actor.", 
          "video": "https://www.youtube.com/embed/McJJSha37NE"
          }, 
          {
          "word": "Amazed", 
          "synonym": "", 
          "example": "Alex stared in amazed appreciation.", 
          "video": "https://www.youtube.com/embed/0BFyfv"
          }, 
          {
          "word": "Ambition", 
          "synonym": "", 
          "example": "Her ambition was to become a pilot.", 
          "video": "https://www.youtube.com/embed/5VemUbcGFTE"
          }, 
          {
          "word": "Ambulance chaser", 
          "synonym": "", 
          "example": "Rahad and Sharif are well", 
          "video": "https://www.youtube.com/embed/7c_P_FzRJlo up to 0:20 second"
          }, 
          {
          "word": "Amend", 
          "synonym": "", 
          "example": "MPs were urged to amend the law to prevent another oil tanker disaster.", 
          "video": "https://www.youtube.com/embed/nq4Bq1SAvWk?t=6s"
          }, 
          {
          "word": "Amount to", 
          "synonym": "", 
          "example": "The total repair work will amount to 1200Ä.", 
          "video": "https://www.youtube.com/embed/u1N"
          }, 
          {
          "word": "Ample", 
          "synonym": "", 
          "example": "She's had ample time to get the work done.", 
          "video": "https://www.youtube.com/embed/QJgAAnPpgdk?t=5s"
          }, 
          {
          "word": "Amusing", 
          "synonym": "", 
          "example": "So, he found her questions amusing, did he?", 
          "video": "https://www.youtube.com/embed/8Hib5dZj5IU from 0:19 second to 0:39 second"
          }, 
          {
          "word": "An Englishman's home is his castle", 
          "synonym": "domestic, address.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/PyPWyATZIh0"
          }, 
          {
          "word": "An artist/poet/writer manquÈ", 
          "synonym": "Opportunity, Chance, Break", 
          "example": "Politician manquÈ", 
          "video": "https://www.youtube.com/embed/WVWcwXltmrE"
          }, 
          {
          "word": "An element of sth", 
          "synonym": "", 
          "example": "There was certainly an element of truth in what she said.", 
          "video": ""
          }, 
          {
          "word": "An elephant in the room", 
          "synonym": "", 
          "example": "I think, thereís an elephant in the room right now.", 
          "video": "https://www.youtube.com/embed/ezgjbwJ44qA"
          }, 
          {
          "word": "An embarrassment of riches", 
          "synonym": "", 
          "example": "There are so many stellar applicants for the job that we can't choose between them it's truly an embarrassment of riches.", 
          "video": "https://www.youtube.com/embed/0BBHjCgXb48"
          }, 
          {
          "word": "Ancient", 
          "synonym": "", 
          "example": "In ancient times, it was thought that the world was flat.", 
          "video": "https://www.youtube.com/embed/U1IxTEN6nY4"
          }, 
          {
          "word": "And all that jazz", 
          "synonym": "Also, extra, and in addition.", 
          "example": "They sell televisions and radios and all that jazz.", 
          "video": "https://www.youtube.com/embed/M0lBQ9aXc1k"
          }, 
          {
          "word": "Angle for", 
          "synonym": "Acquisitive, ambitious.", 
          "example": "He's clearly angling for a job/an invitation.", 
          "video": "https://www.youtube.com/embed/tgFKNLSLMvo"
          }, 
          {
          "word": "Angle", 
          "synonym": "", 
          "example": "The interior angles of a square are right angles.", 
          "video": "https://www.youtube.com/embed/MMB"
          }, 
          {
          "word": "Animation", 
          "synonym": "", 
          "example": "The animation for the film took over two years to complete.", 
          "video": "https://www.youtube.com/embed/pan_YaQo6lU up to 0:17 second"
          }, 
          {
          "word": "Ankle", 
          "synonym": "", 
          "example": "Jennie fell downstairs, breaking her ankle.", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Announce/Announcement", 
          "synonym": "", 
          "example": "The government announced a cut in taxes.", 
          "video": "https://www.youtube.com/embed/99URH_Cj4I4"
          }, 
          {
          "word": "Annoyed", 
          "synonym": "", 
          "example": "Kelly was annoyed with him.", 
          "video": "https://www.youtube.com/embed/kfyD756Spzc up to 0:19 second"
          }, 
          {
          "word": "Answer back", 
          "synonym": "Answering & responding.", 
          "example": "The company criticized in the documentary was given the opportunity to answer back.", 
          "video": "https://www.youtube.com/embed/kKy0lk9xvLo"
          }, 
          {
          "word": "Answer for", 
          "synonym": "Duty, obligation and responsibility.", 
          "example": "I expect parents to answer for their children's behaviour.", 
          "video": "https://www.youtube.com/embed/yTiMZppNrEk"
          }, 
          {
          "word": "Answer to", 
          "synonym": "Obedient and compliant.", 
          "example": "The great thing about working for yourself is that you don't have to answer to anyone.", 
          "video": "https://www.youtube.com/embed/aboZctrHfK8"
          }, 
          {
          "word": "Antic", 
          "synonym": "", 
          "example": "She has a hobby of collecting antic furniture.", 
          "video": "https://www.youtube.com/embed/YQjaFITyjbM"
          }, 
          {
          "word": "Anticipate", 
          "synonym": "", 
          "example": "We anticipate that prices will fall next year.", 
          "video": "https://www.youtube.com/embed/LIGoYoYLhGw"
          }, 
          {
          "word": "Antisocial", 
          "synonym": "", 
          "example": "Increasingly, smoking is regarded as an anti", 
          "video": "https://www.youtube.com/embed/HXv3oEg3nhg?t=5s"
          }, 
          {
          "word": "Ants in one's pants.", 
          "synonym": "", 
          "example": "I wish he'd relax. He's got ants in his pants about something today.", 
          "video": "https://www.youtube.com/embed/i_UVhTUBdXI"
          }, 
          {
          "word": "Ants in one’s pants", 
          "synonym": "", 
          "example": "Lisa had ants in her pants the day before her interview.", 
          "video": ""
          }, 
          {
          "word": "Anxious", 
          "synonym": "", 
          "example": "She was extremely anxious about her exams.", 
          "video": "https://www.youtube.com/embed/OD2p1dosfjU  up to 0:27 second"
          }, 
          {
          "word": "Any minute/moment/second/time now.", 
          "synonym": "", 
          "example": "The guests are coming any minute now, and the house is still a mess.", 
          "video": ""
          }, 
          {
          "word": "Any port in a storm", 
          "synonym": "", 
          "example": "The hotel was substandard, but it was a case of any port in a storm; all the others were full.", 
          "video": ""
          }, 
          {
          "word": "Apologize", 
          "synonym": "", 
          "example": "I must apologize for disturbing you like this.", 
          "video": "https://www.youtube.com/embed/vGCAladDhzM"
          }, 
          {
          "word": "Appalling", 
          "synonym": "", 
          "example": "The film was absolutely appalling!", 
          "video": "https://www.youtube.com/embed/JDWPI_eN11w?t=5s"
          }, 
          {
          "word": "Apparent", 
          "synonym": "", 
          "example": "I was a little surprised by her apparent lack of interest.", 
          "video": "https://www.youtube.com/embed/5beh8EA6hl8"
          }, 
          {
          "word": "Appeal to", 
          "synonym": "", 
          "example": "The organisers appealed to the crowd to stay calm.", 
          "video": "https://www.youtube.com/embed/3PDrnZoM3nA"
          }, 
          {
          "word": "Appearance", 
          "synonym": "", 
          "example": "She checked her appearance in the mirror.", 
          "video": "https://www.youtube.com/embed/PtiiRrbbtFw up to 0:15 second"
          }, 
          {
          "word": "Appetite", 
          "synonym": "", 
          "example": "All that walking has given me an appetite.", 
          "video": "https://www.youtube.com/embed/ANfJjJhteH4"
          }, 
          {
          "word": "Applaud", 
          "synonym": "", 
          "example": "The audience applauded loudly.", 
          "video": "https://www.youtube.com/embed/U1KYJP3feQk?t=5s"
          }, 
          {
          "word": "Appliance", 
          "synonym": "", 
          "example": "The fair was well organized and structured into specific sections from clothing and sportswear to household appliances and electronic.", 
          "video": "https://www.youtube.com/embed/sxjS_59Nnz4"
          }, 
          {
          "word": "Apply for", 
          "synonym": "", 
          "example": "When he saw the advertisement he decided to apply for the job.", 
          "video": "https://www.youtube.com/embed/ZOdVNSh_9Mk"
          }, 
          {
          "word": "Appoint", 
          "synonym": "", 
          "example": "He was appointed as company director last year.", 
          "video": "https://www.youtube.com/embed/MmINeCD5noU"
          }, 
          {
          "word": "Approach", 
          "synonym": "", 
          "example": "The train approached the main line.", 
          "video": "https://www.youtube.com/embed/U7OtsjqliNc"
          }, 
          {
          "word": "Approval", 
          "synonym": "", 
          "example": "The road schemes have been given approval.", 
          "video": "https://www.youtube.com/embed/4joLsnYkpE4 up to0:21 second"
          }, 
          {
          "word": "Archeologist", 
          "synonym": "", 
          "example": "Archaeologists believe the remains date back to the 5th century.", 
          "video": "https://www.youtube.com/embed/wpFLUrHqIHg"
          }, 
          {
          "word": "Argument", 
          "synonym": "", 
          "example": "I've had an argument with my father.", 
          "video": "https://www.youtube.com/embed/uZBntZ4"
          }, 
          {
          "word": "Arise", 
          "synonym": "", 
          "example": "The whole problem arose from a lack of communication.", 
          "video": "https://www.youtube.com/embed/mnELZWBMQvI"
          }, 
          {
          "word": "Armchair critic", 
          "synonym": "", 
          "example": "That guy is such an armchair critic", 
          "video": "https://www.youtube.com/embed/22vC67H_GUs"
          }, 
          {
          "word": "Armchair traveler", 
          "synonym": "", 
          "example": "A surprising number of adventure books are bought by armchair travelers. ", 
          "video": ""
          }, 
          {
          "word": "Arrangement", 
          "synonym": "", 
          "example": "All the arrangements for the wedding were made.", 
          "video": "https://www.youtube.com/embed/pu8_lrKxb2s"
          }, 
          {
          "word": "Arrival", 
          "synonym": "", 
          "example": "Hotel staff greeted the late arrivals.", 
          "video": "https://www.youtube.com/embed/UmII_vVKfPw from 0:32 to 0:49 second"
          }, 
          {
          "word": "Arrive at", 
          "synonym": "Accepting & agreeing.", 
          "example": "We all argued about it for hours and eventually arrived at a decision.", 
          "video": "https://www.youtube.com/embed/CPXUDS"
          }, 
          {
          "word": "Artistic/poetic licence", 
          "synonym": "", 
          "example": "She used a fair amount of poetic licence when describing her life in rural France.", 
          "video": "https://www.youtube.com/embed/6ghLglfoCog"
          }, 
          {
          "word": "As a last resort", 
          "synonym": "", 
          "example": "Nuclear weapons should be used only as a last resort.", 
          "video": "https://www.youtube.com/embed/uvMlZKB7QhY"
          }, 
          {
          "word": "As a matter of course", 
          "synonym": "Habitual and customary.", 
          "example": "Safety precautions are observed as a matter of course.", 
          "video": ""
          }, 
          {
          "word": "As a matter of fact/in actual fact", 
          "synonym": "Actually", 
          "example": "I love gaming, as a matter of fact I am currently carrying my gaming laptop.", 
          "video": ""
          }, 
          {
          "word": "As blind as a bat", 
          "synonym": "Sightless", 
          "example": "I'm as blind as a bat without my glasses.", 
          "video": "https://www.youtube.com/embed/DzDC7b4zxHU"
          }, 
          {
          "word": "As blind as a bat.", 
          "synonym": "", 
          "example": "Without his glasses, the old man is as blind as a bat.", 
          "video": "https://www.youtube.com/embed/DzDC7b4zxHU"
          }, 
          {
          "word": "As bold as brass", 
          "synonym": "Impertinent", 
          "example": "She  marched into the store, as bold as brass, and demanded her money back.", 
          "video": ""
          }, 
          {
          "word": "As broad as it's long.", 
          "synonym": "", 
          "example": "Take the high", 
          "video": ""
          }, 
          {
          "word": "As clean as a whistle.", 
          "synonym": "", 
          "example": "Bob spent the afternoon washing and shining his car until it was as clean as a whistle.", 
          "video": "https://www.youtube.com/embed/1uBZcU7kU3U"
          }, 
          {
          "word": "As close / as dumb as an oyster.", 
          "synonym": "", 
          "example": "Sophie will never repeat what you tell her. She's as dumb as an oyster.", 
          "video": ""
          }, 
          {
          "word": "As different as chalk and cheese.", 
          "synonym": "", 
          "example": "I'm surprised they get on so well.  They're as different as chalk and cheese.", 
          "video": "https://www.youtube.com/embed/HVQQcHHp7eA"
          }, 
          {
          "word": "As different as night and day.", 
          "synonym": "", 
          "example": "Although they are twins they are as different as night and day.", 
          "video": ""
          }, 
          {
          "word": "As dry as dust.", 
          "synonym": "", 
          "example": "His speech was as dry as dust.", 
          "video": "https://www.youtube.com/embed/7pcEbMHmcic"
          }, 
          {
          "word": "As dull as ditchwater.", 
          "synonym": "", 
          "example": "The film was as dull as ditchwater.  I nearly fell asleep.", 
          "video": ""
          }, 
          {
          "word": "As easy as pie.", 
          "synonym": "", 
          "example": "'How did the English test go?' 'No problem,  it was as easy as pie!'", 
          "video": ""
          }, 
          {
          "word": "As every schoolboy/schoolchild knows", 
          "synonym": "", 
          "example": "As every schoolboy knows, the earth revolves around the sun.", 
          "video": ""
          }, 
          {
          "word": "As far as it goes.", 
          "synonym": "okay, average, satisfactory.", 
          "example": "It's a good essay as far as it goes.", 
          "video": ""
          }, 
          {
          "word": "As far as somebody is concerned", 
          "synonym": "Matter, Issue, Referent", 
          "example": "Thereís no reason to wait, as far as Iím concerned.", 
          "video": "https://www.youtube.com/embed/K_TZYNVGpa0"
          }, 
          {
          "word": "As far as something is concerned", 
          "synonym": "Subject, Theme, Topic, Item", 
          "example": "I make the decisions as far as finance is concerned.", 
          "video": "https://www.youtube.com/embed/K_TZYNVGpa0"
          }, 
          {
          "word": "As fit as a fiddle.", 
          "synonym": "", 
          "example": "My grandfather is nearly ninety but he's as fit as a fiddle.", 
          "video": "https://www.youtube.com/embed/FES"
          }, 
          {
          "word": "As free as a bird.", 
          "synonym": "", 
          "example": "My dad's very happy", 
          "video": ""
          }, 
          {
          "word": "As fresh as a daisy.", 
          "synonym": "", 
          "example": "So you got the job", 
          "video": ""
          }, 
          {
          "word": "As full as a tick.", 
          "synonym": "", 
          "example": "The little boy ate biscuits and drank lemonade until he was as full as a tick.", 
          "video": ""
          }, 
          {
          "word": "As good as gold.", 
          "synonym": "", 
          "example": "Your children are always as good as gold when I look after them.", 
          "video": "https://www.youtube.com/embed/5OpTStnf9xU"
          }, 
          {
          "word": "As happy as Larry.", 
          "synonym": "", 
          "example": "My dad's as happy as Larry at the week", 
          "video": "https://www.youtube.com/embed/7UYdVubP6H0"
          }, 
          {
          "word": "As happy as a flea in a doghouse.", 
          "synonym": "", 
          "example": "Since she moved to a smaller apartment, my mother is as happy as a flea in a doghouse!", 
          "video": ""
          }, 
          {
          "word": "As hard as nails.", 
          "synonym": "", 
          "example": "Don't expect any sympathy from him.  He's as hard as nails.", 
          "video": "https://www.youtube.com/embed/YEHz5eQcjRs"
          }, 
          {
          "word": "As mad as a hatter.", 
          "synonym": "", 
          "example": "The old lady next door is as mad as a hatter.  She says the strangest things!", 
          "video": "https://www.youtube.com/embed/WLV4vy6wIQI"
          }, 
          {
          "word": "As much use as a handbrake on a canoe.", 
          "synonym": "", 
          "example": "With no electricity, a refrigerator would be as much use as a handbrake on a canoe!", 
          "video": ""
          }, 
          {
          "word": "As nice as pie.", 
          "synonym": "", 
          "example": "After our argument, she was as nice as pie!", 
          "video": ""
          }, 
          {
          "word": "As nutty as a fruitcake.", 
          "synonym": "", 
          "example": "Don't pay attention to what the old man says; he's as nutty as a fruitcake!", 
          "video": "https://www.youtube.com/embed/PXc5uQyl7n4"
          }, 
          {
          "word": "As often as not  /  more often than not", 
          "synonym": "Habitual and customary.", 
          "example": "More often than not, a student will come up with the right answer.", 
          "video": "https://www.youtube.com/embed/NvKWyKumZ24"
          }, 
          {
          "word": "As proud as a peacock.", 
          "synonym": "", 
          "example": "When his son won first prize, Bill was as proud as a peacock.", 
          "video": ""
          }, 
          {
          "word": "As quick as a dog can lick a dish.", 
          "synonym": "", 
          "example": "He packed his bag as quick as a dog can lick a dish.", 
          "video": ""
          }, 
          {
          "word": "As quiet as a mouse.", 
          "synonym": "", 
          "example": "The burglar was a quiet as a mouse as he moved around the house.", 
          "video": "https://www.youtube.com/embed/Z4dcwI_qp6w"
          }, 
          {
          "word": "As regards", 
          "synonym": "", 
          "example": "There is no problem as regards the financial arrangements.", 
          "video": ""
          }, 
          {
          "word": "As scarce as hens' teeth.", 
          "synonym": "", 
          "example": "Take enough supplies.  Water is as scarce as hens' teeth where you're going!", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "As sharp as a tack.", 
          "synonym": "", 
          "example": "You won't have to explain it to him twice. He's as sharp as a tack.", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "As slippery as an eel.", 
          "synonym": "", 
          "example": "The man was as slippery as an eel.  He was arrested for theft several times but was never convicted.", 
          "video": ""
          }, 
          {
          "word": "As sly as a fox.", 
          "synonym": "", 
          "example": "Be wary of that insurance salesman.  He's as sly as a fox.", 
          "video": "https://www.youtube.com/embed/wUwf7qqCKPs"
          }, 
          {
          "word": "As the crow flies", 
          "synonym": "", 
          "example": "Easingwold was 22 miles away as the crow flies.", 
          "video": "https://www.youtube.com/embed/3m2Bo2GGLYc"
          }, 
          {
          "word": "As/so far as I can tell.", 
          "synonym": "", 
          "example": "There's been no change, as far as I can tell.", 
          "video": ""
          }, 
          {
          "word": "As/so far as I know.", 
          "synonym": "", 
          "example": "He isn't coming today, as far as I know.", 
          "video": ""
          }, 
          {
          "word": "As/so far as I'm concerned.", 
          "synonym": "", 
          "example": "She can come whenever she likes, as far as I'm concerned.", 
          "video": ""
          }, 
          {
          "word": "Ashamed", 
          "synonym": "", 
          "example": "You should be ashamed of yourself.", 
          "video": "https://www.youtube.com/embed/Tr35"
          }, 
          {
          "word": "Ask after", 
          "synonym": "Questioning people & asking questions in general.", 
          "example": "Tell your father I was asking after him.", 
          "video": "https://www.youtube.com/embed/o7ubK98I06g"
          }, 
          {
          "word": "Ask around", 
          "synonym": "Questioning people & asking questions in general.", 
          "example": "Our babysitter's just moved away, so we're asking around for a replacement.", 
          "video": "https://www.youtube.com/embed/NjV3wzbPhQ0"
          }, 
          {
          "word": "Ask in", 
          "synonym": "Inviting & summoning.", 
          "example": "I'd ask you in for a coffee but I have to get up early for work in the morning.", 
          "video": "https://www.youtube.com/embed/2vopEwz7bK8"
          }, 
          {
          "word": "Ask out", 
          "synonym": "Inviting & summoning.", 
          "example": "She's asked Steve out to the cinema this evening.", 
          "video": "https://www.youtube.com/embed/8_yFMmcrp5Q"
          }, 
          {
          "word": "Asking for trouble.", 
          "synonym": "", 
          "example": "Driving fast on these roads is really asking for trouble!", 
          "video": ""
          }, 
          {
          "word": "Asleep", 
          "synonym": "", 
          "example": "She had been asleep for over three hours.", 
          "video": "https://www.youtube.com/embed/55S"
          }, 
          {
          "word": "Assert", 
          "synonym": "", 
          "example": "He asserts that she stole money from him.", 
          "video": "https://www.youtube.com/embed/17H71BIK9jA"
          }, 
          {
          "word": "Asset", 
          "synonym": "", 
          "example": "He'll be a great asset to the team.", 
          "video": "https://www.youtube.com/embed/32AQb1l2Gew"
          }, 
          {
          "word": "Assign", 
          "synonym": "", 
          "example": "UN forces were assigned the task of rebuilding the hospital.", 
          "video": "https://www.youtube.com/embed/JQlZ0wSfe0U"
          }, 
          {
          "word": "At long last", 
          "synonym": "Finally.", 
          "example": "At long last the government is starting to listen to our problems.", 
          "video": "https://www.youtube.com/embed/SWaRyeOdu"
          }, 
          {
          "word": "At a disadvantage", 
          "synonym": "", 
          "example": "He's at a disadvantage being so shy.", 
          "video": ""
          }, 
          {
          "word": "At a disadvantage", 
          "synonym": "", 
          "example": "The storm had me at a disadvantage.", 
          "video": ""
          }, 
          {
          "word": "At a hell of lick", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "At a low ebb", 
          "synonym": "", 
          "example": "The recent political crisis has left the country at a low ebb.", 
          "video": ""
          }, 
          {
          "word": "At a low ebb", 
          "synonym": "", 
          "example": "The recent political crisis has left the country at a low ebb.", 
          "video": ""
          }, 
          {
          "word": "At all costs", 
          "synonym": "", 
          "example": "The journalist was determined at all costs to get a report from the war zone. ", 
          "video": ""
          }, 
          {
          "word": "At all costs", 
          "synonym": "", 
          "example": "The merger must go through at all costs.", 
          "video": ""
          }, 
          {
          "word": "At cross purposes", 
          "synonym": "", 
          "example": "We had been talking at cross purposes.", 
          "video": "https://www.youtube.com/embed/VI5C_WWrZmM"
          }, 
          {
          "word": "At daggers drawn.", 
          "synonym": "", 
          "example": "The two sides have been at daggers drawn for some months now with no sign of improvement in relations.", 
          "video": ""
          }, 
          {
          "word": "At hand", 
          "synonym": "brew, come up.", 
          "example": "We want to ensure that help is at hand = easily available for all children suffering abuse.", 
          "video": "https://www.youtube.com/embed/3FCYzxxCiH4"
          }, 
          {
          "word": "At large", 
          "synonym": "Large, largely.", 
          "example": "This group is not representative of the population at large.", 
          "video": "https://www.youtube.com/embed/LHrGjjzwNF4"
          }, 
          {
          "word": "At local/national level", 
          "synonym": "", 
          "example": "These changes are taking place at regional level.", 
          "video": "https://www.youtube.com/embed/qgzl_oLK8tE"
          }, 
          {
          "word": "At loggerheads", 
          "synonym": "Arguing & disagreeing.", 
          "example": "The party is at loggerheads with the president over public spending.", 
          "video": "https://www.youtube.com/embed/BLudYDZtwrI"
          }, 
          {
          "word": "At peace", 
          "synonym": "", 
          "example": "Now she is at peace and her suffering is over.", 
          "video": ""
          }, 
          {
          "word": "At sbís elbow", 
          "synonym": "", 
          "example": "During the visit, the interpreter was always at her elbow.", 
          "video": ""
          }, 
          {
          "word": "At short notice.", 
          "synonym": "", 
          "example": "It is not possible to get a replacement at such short notice.", 
          "video": ""
          }, 
          {
          "word": "At sixes and sevens", 
          "synonym": "Confusion, confusing and feeling confused.", 
          "example": "We've been at sixes and sevens in the office this week.", 
          "video": "https://www.youtube.com/embed/y7JUbTSthUg"
          }, 
          {
          "word": "At somebody's beck and call.", 
          "synonym": "", 
          "example": "Go and get it yourself! I'm not at your beck and call, you know.", 
          "video": "https://www.youtube.com/embed/KRd6bJs1Ckk"
          }, 
          {
          "word": "At stake", 
          "synonym": "Unsafe and insecure.", 
          "example": "Thousands of lives will be at stake if emergency aid does not arrive in the city soon.", 
          "video": "https://www.youtube.com/embed/qGvJdc5kpDM"
          }, 
          {
          "word": "At the back of your mind", 
          "synonym": "", 
          "example": "At the back of my mind is the fear of failing the test.", 
          "video": ""
          }, 
          {
          "word": "At the drop of a hat", 
          "synonym": "", 
          "example": "Fire fighters are always ready so they can leave at the drop of a hat.", 
          "video": ""
          }, 
          {
          "word": "At the drop of a hat", 
          "synonym": "", 
          "example": "I've got great friends. They're ready to help out at the drop of a hat.", 
          "video": "https://www.youtube.com/embed/z4X0d0H1QbM"
          }, 
          {
          "word": "At the end of the day", 
          "synonym": "eventually, final.", 
          "example": "Of course I'll listen to what she has to say but at the end of the day, it's my decision.", 
          "video": "https://www.youtube.com/embed/b6YpHAW76WM"
          }, 
          {
          "word": "At the hands of  sb", 
          "synonym": "Treating people or animals badly, abuser.", 
          "example": "How many people have died at the hands of terrorist organizations?", 
          "video": ""
          }, 
          {
          "word": "At the push of a button", 
          "synonym": "Easiness, Simplicity, Very easily", 
          "example": "You can't expect to get everything you need at the push of a button.", 
          "video": "https://www.youtube.com/embed/IVSsddUvXxg"
          }, 
          {
          "word": "At the ready", 
          "synonym": "Ready and willing.", 
          "example": "He stood by the phone, pencil at the ready.", 
          "video": "https://www.youtube.com/embed/GWjSLJXXsLA"
          }, 
          {
          "word": "At the very latest", 
          "synonym": "", 
          "example": "You've got to be there by nine o'clock in the morning at the latest.", 
          "video": ""
          }, 
          {
          "word": "At this stage of the game", 
          "synonym": "", 
          "example": "At this stage of the game I think any further intervention would be unwise.  Let's wait and see how things develop.", 
          "video": ""
          }, 
          {
          "word": "At this stage of the game", 
          "synonym": "", 
          "example": "At this stage of the game I think any further intervention would be unwise.  Let's wait and see how things develop.", 
          "video": ""
          }, 
          {
          "word": "At your convenience", 
          "synonym": "Acceptable", 
          "example": "The goods will be delivered at your convenience.", 
          "video": "https://www.youtube.com/embed/hg6yYD"
          }, 
          {
          "word": "At your earliest convenience", 
          "synonym": "Quickly", 
          "example": "We should be grateful if you would reply at your earliest convenience.", 
          "video": "https://www.youtube.com/embed/9UZOTpq8To8"
          }, 
          {
          "word": "At/on the double", 
          "synonym": "Very quickly, Without any delay, Accelerate", 
          "example": "Two soldiers entered at the double and saluted.", 
          "video": ""
          }, 
          {
          "word": "Athlete", 
          "synonym": "", 
          "example": "He had the broad", 
          "video": "https://www.youtube.com/embed/O_obhwTb5Q4&spfreload=10 up to 0:24 second"
          }, 
          {
          "word": "Atmosphere", 
          "synonym": "", 
          "example": "The atmosphere of earth is mainly made up of nitrogen.", 
          "video": "https://www.youtube.com/embed/8SQj7BqtmFA up to 0:13 second"
          }, 
          {
          "word": "Attach", 
          "synonym": "", 
          "example": "Use this cable to attach the printer to the computer.", 
          "video": "https://www.youtube.com/embed/GhmbLnsSpGM"
          }, 
          {
          "word": "Attack", 
          "synonym": "", 
          "example": "He attacked the government's defence policy.", 
          "video": "https://www.youtube.com/embed/H2m1OJZ6frAup to 0:24 second"
          }, 
          {
          "word": "Attend", 
          "synonym": "", 
          "example": "The whole sales force attended the conference.", 
          "video": "https://www.youtube.com/embed/2_NDhZaGOL8"
          }, 
          {
          "word": "Attest to", 
          "synonym": "", 
          "example": "The number of visitors attest to the popularity of the website.", 
          "video": "https://www.youtube.com/embed/aO9yRGD4Yck"
          }, 
          {
          "word": "Attitude", 
          "synonym": "", 
          "example": "He was questioned on his attitude to South Africa.", 
          "video": "https://www.youtube.com/embed/1MOndSrpIok"
          }, 
          {
          "word": "Attract", 
          "synonym": "", 
          "example": "I did not want to attract attention.", 
          "video": "https://www.youtube.com/embed/Ivx4iwcmYtM"
          }, 
          {
          "word": "Auction", 
          "synonym": "", 
          "example": "The furniture was sold at auction.", 
          "video": "https://www.youtube.com/embed/Gf75ybjyimQ"
          }, 
          {
          "word": "Audience", 
          "synonym": "", 
          "example": "He asked for questions from members of the audience.", 
          "video": "https://www.youtube.com/embed/Xvx8CPvhEcY from 0:11 second"
          }, 
          {
          "word": "Authentic", 
          "synonym": "", 
          "example": "I am also nostalgic for authentic Thai culture which has subtly and gradually been replaced by American and European culture.", 
          "video": "https://www.youtube.com/embed/bKLpXEk_keM"
          }, 
          {
          "word": "Avail oneself of", 
          "synonym": "Using and misusing.", 
          "example": "Employees should avail themselves of the opportunity to buy cheap shares in the company.", 
          "video": "https://www.youtube.com/embed/OAf2M1uQPBg"
          }, 
          {
          "word": "Avenue", 
          "synonym": "", 
          "example": "The demonstrators just spread litter all over the largest and finest avenue.", 
          "video": "https://www.youtube.com/embed/s4lWVoALVVY"
          }, 
          {
          "word": "Average out at", 
          "synonym": "Average, average out.", 
          "example": "My annual holiday varies, but it averages out at five weeks a year.", 
          "video": "https://www.youtube.com/embed/v"
          }, 
          {
          "word": "Average", 
          "synonym": "", 
          "example": "The meal was pretty average.", 
          "video": "https://www.youtube.com/embed/18uBVzOsRWE?t=5s"
          }, 
          {
          "word": "Avoid", 
          "synonym": "", 
          "example": "Avoid excessive exposure to the sun.", 
          "video": "https://www.youtube.com/embed/8LusT8ce1nI up to 0:12 second"
          }, 
          {
          "word": "Avowed intent", 
          "synonym": "", 
          "example": "Even though politicians give out avowed intent they rarely follow through.", 
          "video": ""
          }, 
          {
          "word": "Awake", 
          "synonym": "", 
          "example": "To awake timely in the morning, we should set the alarm before going to sleep.", 
          "video": "https://www.youtube.com/embed/U8JZpNTgyDs"
          }, 
          {
          "word": "Away with the fairies", 
          "synonym": "", 
          "example": "It's no use trying to explain the problem to her", 
          "video": "https://www.youtube.com/embed/7KIpFtIBD1o"
          }, 
          {
          "word": "Awful", 
          "synonym": "", 
          "example": "I've made an awful fool of myself.", 
          "video": "https://www.youtube.com/embed/kH6jahB5l5I"
          }, 
          {
          "word": "Back ache", 
          "synonym": "", 
          "example": "Gardening gives me such backache.", 
          "video": "https://www.youtube.com/embed/OER41XRsQbo"
          }, 
          {
          "word": "Back away", 
          "synonym": "Running away and escaping.", 
          "example": "The government has backed away from plans to increase taxes.", 
          "video": "https://www.youtube.com/embed/EK"
          }, 
          {
          "word": "Back breaking", 
          "synonym": "", 
          "example": "Digging the vegetable garden was backbreaking work.", 
          "video": "https://www.youtube.com/embed/Nd29HzFYq54"
          }, 
          {
          "word": "Back chat", 
          "synonym": "", 
          "example": "That's enough backchat! You do as you're told.", 
          "video": "https://www.youtube.com/embed/rFBJoB9uONY"
          }, 
          {
          "word": "Back comb", 
          "synonym": "", 
          "example": "You can achieve a sixties feel by gently backcombing hair at the crown.", 
          "video": "https://www.youtube.com/embed/7TEb3MZdFpo"
          }, 
          {
          "word": "Back down", 
          "synonym": "Admitting & confessing.", 
          "example": "Eventually, Roberto backed down and apologized.", 
          "video": "https://www.youtube.com/embed/dsj8VaP_bnY"
          }, 
          {
          "word": "Back into", 
          "synonym": "", 
          "example": "He backed his car into a parking space.", 
          "video": "https://www.youtube.com/embed/SdtKDRn1S9E"
          }, 
          {
          "word": "Back of the envelope calculation", 
          "synonym": "", 
          "example": "I don't need the exact amount.  Just give me a back", 
          "video": "https://www.youtube.com/embed/_ygJ"
          }, 
          {
          "word": "Back off", 
          "synonym": "", 
          "example": "The thugs backed off when they saw the police.", 
          "video": "https://www.youtube.com/embed/En16vmGB2y8"
          }, 
          {
          "word": "Back out", 
          "synonym": "Back away, backpedal.", 
          "example": "You agreed to come. You can't back out now!", 
          "video": "https://www.youtube.com/embed/FIH3D3J5UxM"
          }, 
          {
          "word": "Back out", 
          "synonym": "Climbdown, cold.", 
          "example": "You agreed to come. You can't back out now!", 
          "video": "https://www.youtube.com/embed/FIH3D3J5UxM"
          }, 
          {
          "word": "Back payment", 
          "synonym": "Balance due, debit", 
          "example": "She will get a back payment, as her salary is increased by  five thousand.", 
          "video": ""
          }, 
          {
          "word": "Back pedal", 
          "synonym": "Change opinion", 
          "example": "As soon as I said I thought she was wrong, she started backpedalling.", 
          "video": "https://www.youtube.com/embed/DqSkf"
          }, 
          {
          "word": "Back slapping", 
          "synonym": "", 
          "example": "There was a party after the ceremony where much drinking and backslapping went on.", 
          "video": "https://www.youtube.com/embed/ZHXMwEes3bY"
          }, 
          {
          "word": "Back slide", 
          "synonym": "", 
          "example": "My diet was going well, but I've been backsliding a little recently.", 
          "video": "https://www.youtube.com/embed/9xaiNS_vesE"
          }, 
          {
          "word": "Back stabber", 
          "synonym": "", 
          "example": "Trust No one!! life's full of backstabbers.", 
          "video": "https://www.youtube.com/embed/Ol7cYEv9WB0"
          }, 
          {
          "word": "Back the wrong horse", 
          "synonym": "", 
          "example": "When I voted for him I was convinced he would win, but I backed the wrong horse!", 
          "video": "https://www.youtube.com/embed/sbRD41OSw8Y"
          }, 
          {
          "word": "Back to back", 
          "synonym": "Close together", 
          "example": "Uk back", 
          "video": "https://www.youtube.com/embed/Pzutre_jtD0"
          }, 
          {
          "word": "Back to back", 
          "synonym": "Continuous", 
          "example": "Hamilton is celebrating back", 
          "video": "https://www.youtube.com/embed/Pzutre_jtD0"
          }, 
          {
          "word": "Back to basics", 
          "synonym": "", 
          "example": "This is all part of a new back", 
          "video": "https://www.youtube.com/embed/ILvRZR2A0Vc"
          }, 
          {
          "word": "Back to square one", 
          "synonym": "", 
          "example": "When the plans were refused, it was 'back to square one' for the architect.", 
          "video": ""
          }, 
          {
          "word": "Back to square one", 
          "synonym": "", 
          "example": "When the plans were refused, it was 'back to square one' for the architect.", 
          "video": ""
          }, 
          {
          "word": "Back to the salt mines", 
          "synonym": "", 
          "example": "We get two days off at Christmas and then it's back to the salt mines!", 
          "video": ""
          }, 
          {
          "word": "Back to the wall.", 
          "synonym": "", 
          "example": "With his back to the wall, the supplier had to accept the deal.", 
          "video": ""
          }, 
          {
          "word": "Back up", 
          "synonym": "Helpers and accomplices.", 
          "example": "If we run out of sandwiches I've got some pizzas in the kitchen as backup.", 
          "video": "https://www.youtube.com/embed/SdtKDRn1S9E"
          }, 
          {
          "word": "Back water", 
          "synonym": "", 
          "example": "He grew up in a rural backwater.", 
          "video": "https://www.youtube.com/embed/pO1oIThbEeY"
          }, 
          {
          "word": "Back", 
          "synonym": "", 
          "example": "Back", 
          "video": ""
          }, 
          {
          "word": "Backbench", 
          "synonym": "", 
          "example": "The prime minister expects strong support from the Labor backbenches.", 
          "video": "https://www.youtube.com/embed/AGOritum_tA"
          }, 
          {
          "word": "Backbiting", 
          "synonym": "", 
          "example": "A lot of backbiting goes on in our office.", 
          "video": "https://www.youtube.com/embed/kGbqrJ4JbA0"
          }, 
          {
          "word": "Backfire", 
          "synonym": "Bad result", 
          "example": "Her plans to make him jealous backfired on her when he started dating her best friend.", 
          "video": "https://www.youtube.com/embed/bsw_IgxWMj0"
          }, 
          {
          "word": "Backfire", 
          "synonym": "Engine", 
          "example": "I was woken by the sound of a truck backfiring.", 
          "video": "https://www.youtube.com/embed/bsw_IgxWMj0"
          }, 
          {
          "word": "Backlash", 
          "synonym": "", 
          "example": "The 60s backlash against bourgeois materialism.", 
          "video": "https://www.youtube.com/embed/d2ZFmfzIVP0?t=6s"
          }, 
          {
          "word": "Backlit", 
          "synonym": "", 
          "example": "His trophies were proudly displayed in a backlit cabinet.", 
          "video": "https://www.youtube.com/embed/6_pWFTqP8r8"
          }, 
          {
          "word": "Backlog", 
          "synonym": "", 
          "example": "I've got a huge backlog of work to do.", 
          "video": "https://www.youtube.com/embed/lHoEhGBFfAk?t=6s"
          }, 
          {
          "word": "Backpack", 
          "synonym": "", 
          "example": "It's a frame backpack with a belt and padded shoulder straps.", 
          "video": "https://www.youtube.com/embed/y_qAfek8cGk?t=6s"
          }, 
          {
          "word": "Backseat driver", 
          "synonym": "", 
          "example": "I can't stand backseat drivers like my mother", 
          "video": "https://www.youtube.com/embed/o"
          }, 
          {
          "word": "Backstage", 
          "synonym": "", 
          "example": "We went backstage after the show to meet the actors.", 
          "video": "https://www.youtube.com/embed/FOiMB0ca3_o?t=6s"
          }, 
          {
          "word": "Backstroke", 
          "synonym": "", 
          "example": "Can you do backstroke?", 
          "video": "https://www.youtube.com/embed/Ci8QaazDZRA"
          }, 
          {
          "word": "Backyard", 
          "synonym": "", 
          "example": "The kids were playing in the backyard.", 
          "video": "https://www.youtube.com/embed/08XS6zvhMGI"
          }, 
          {
          "word": "Bacon", 
          "synonym": "", 
          "example": "The scent of bacon reached her from the kitchen.", 
          "video": "https://www.youtube.com/embed/D3emowxArLk up to 0:14 second"
          }, 
          {
          "word": "Bad blood", 
          "synonym": "", 
          "example": "There has been bad blood between the two families for years.", 
          "video": "https://www.youtube.com/embed/zrE2O6ri"
          }, 
          {
          "word": "Bad debt", 
          "synonym": "", 
          "example": "The bank expects to lose £703 million of last year's profits as a result of bad debts.", 
          "video": "https://www.youtube.com/embed/AfFS2rMplF0"
          }, 
          {
          "word": "Bad egg", 
          "synonym": "", 
          "example": "I don't want my son to be friends with Bobby Smith. Bobby's a bad egg.", 
          "video": "https://www.youtube.com/embed/J8qgGG2SppE"
          }, 
          {
          "word": "Bad temper", 
          "synonym": "", 
          "example": "She's very bad", 
          "video": "https://www.youtube.com/embed/2T5JShs11Cg"
          }, 
          {
          "word": "Baffle", 
          "synonym": "", 
          "example": "She was completely baffled by his strange behavior.", 
          "video": "https://www.youtube.com/embed/9Fuevvrkodo"
          }, 
          {
          "word": "Bag and baggage", 
          "synonym": "", 
          "example": "I was pleasantly surprised when I saw my cousin appear at my door with all his bag and baggages.", 
          "video": ""
          }, 
          {
          "word": "Bagel", 
          "synonym": "Food", 
          "example": "An onion bagel.", 
          "video": "https://www.youtube.com/embed/CFsnoN0FKUA?t=7s"
          }, 
          {
          "word": "Baggage", 
          "synonym": "", 
          "example": "We collected our baggage before clearing customs.", 
          "video": "https://www.youtube.com/embed/M"
          }, 
          {
          "word": "Baguette", 
          "synonym": "Food", 
          "example": "A ham and cheese baguette.", 
          "video": "https://www.youtube.com/embed/5UWAJBeOhcI?t=6s"
          }, 
          {
          "word": "Bail out", 
          "synonym": "Running away and escaping.", 
          "example": "The plane's engine failed and the pilot was forced to bail out.", 
          "video": "https://www.youtube.com/embed/OynRYXKMbsI"
          }, 
          {
          "word": "Bail somebody out", 
          "synonym": "", 
          "example": "She keeps running up huge debts and asking friends to bail her out.", 
          "video": "https://www.youtube.com/embed/OynRYXKMbsI"
          }, 
          {
          "word": "Bail something out", 
          "synonym": "", 
          "example": "After all that rain, my dad and I have been bailing out our basement all day. We'll sink if we don't bail out the boat now!", 
          "video": "https://www.youtube.com/embed/OynRYXKMbsI"
          }, 
          {
          "word": "Bait and switch", 
          "synonym": "", 
          "example": "This store is famous for its bait and switch tactics.", 
          "video": "https://www.youtube.com/embed/VRkBg5fWreY up to 0:23 second"
          }, 
          {
          "word": "Bait", 
          "synonym": "Make angry", 
          "example": "Ignore him", 
          "video": "https://www.youtube.com/embed/uWd0lhjkodo"
          }, 
          {
          "word": "Baize", 
          "synonym": "", 
          "example": "'a baize apron'", 
          "video": "https://www.youtube.com/embed/z9KCBt48TFM"
          }, 
          {
          "word": "Bald", 
          "synonym": "", 
          "example": "He was starting to go bald.", 
          "video": "https://www.youtube.com/embed/vvmVHdbA9hM  up to 0:10 second"
          }, 
          {
          "word": "Ball and chain.", 
          "synonym": "", 
          "example": "Our holiday home has become a ball and chain", 
          "video": "https://www.dailymotion.com/video/x3vkidg"
          }, 
          {
          "word": "Ball gown", 
          "synonym": "", 
          "example": "It was light, like a hatbox or a gift box containing a ball gown, and it bore her own name in small printed capitals.", 
          "video": "https://www.youtube.com/embed/MTT6iuQi_Vk"
          }, 
          {
          "word": "Ballet", 
          "synonym": "", 
          "example": "By the age of 15 he had already composed his first ballet.", 
          "video": "https://www.youtube.com/embed/cOE_Eh6LLNU"
          }, 
          {
          "word": "Ballet", 
          "synonym": "", 
          "example": "She invited me to the ballet.", 
          "video": "https://www.youtube.com/embed/43hniD"
          }, 
          {
          "word": "Ballot", 
          "synonym": "", 
          "example": "Representatives were elected by ballot.", 
          "video": "https://www.youtube.com/embed/kMYX4"
          }, 
          {
          "word": "Ballot", 
          "synonym": "", 
          "example": "Rumours of ballot rigging discouraged from voting.", 
          "video": ""
          }, 
          {
          "word": "Ballpark figure", 
          "synonym": "", 
          "example": "I don't know exactly how much it will cost, but a ballpark figure would be around $100 000.", 
          "video": "https://www.youtube.com/embed/FCDmLc59EBQ up to 1:10 second"
          }, 
          {
          "word": "Banana skin", 
          "synonym": "", 
          "example": "The new tax has proved to be a banana skin for the government.", 
          "video": ""
          }, 
          {
          "word": "Banana split", 
          "synonym": "", 
          "example": "A banana split is a popular summer treat.", 
          "video": ""
          }, 
          {
          "word": "Band together", 
          "synonym": "Helping and co", 
          "example": "We decided to band together and organize a protest.", 
          "video": "https://www.youtube.com/embed/7DRxCP3gx7s"
          }, 
          {
          "word": "Bandage", 
          "synonym": "", 
          "example": "Her leg was swathed in bandage.", 
          "video": "https://www.youtube.com/embed/x36gvFxtUhs"
          }, 
          {
          "word": "Bandit territory", 
          "synonym": "", 
          "example": "There are a certain number of bandit territories in the world where travellers are advised not to go. ", 
          "video": ""
          }, 
          {
          "word": "Bane of one's life.", 
          "synonym": "", 
          "example": "The heating system is always breaking down. It's the bane of my life!", 
          "video": ""
          }, 
          {
          "word": "Banjo", 
          "synonym": "", 
          "example": "I hear you're good at playing the banjo.", 
          "video": "https://www.youtube.com/embed/nqpp7vPH8OU up to 0:13 second"
          }, 
          {
          "word": "Bank holiday", 
          "synonym": "", 
          "example": "Hot weather and bank holidays helped  high street sales to recover in  April.", 
          "video": "https://www.youtube.com/embed/oogw"
          }, 
          {
          "word": "Bank on sb/sth", 
          "synonym": "", 
          "example": "Can I  bank on your support?", 
          "video": ""
          }, 
          {
          "word": "Bank on", 
          "synonym": "", 
          "example": "Don't forget the date. I'm banking on your help.", 
          "video": "https://www.youtube.com/embed/PWT9"
          }, 
          {
          "word": "Bankable", 
          "synonym": "", 
          "example": "She is currently Hollywood's most bankable actress = her movies make large profits.", 
          "video": "https://www.youtube.com/embed/ROdmuYqayZQ up to 0: 14 second"
          }, 
          {
          "word": "Bankroll", 
          "synonym": "", 
          "example": "A  joint project bankrolled by the US space agency.", 
          "video": "https://www.youtube.com/embed/NDuklbSUN98  from 0:11 second"
          }, 
          {
          "word": "Bankrupt", 
          "synonym": "", 
          "example": "He went bankrupt after only a year in business.", 
          "video": "https://www.youtube.com/embed/whyJrKy_qKM"
          }, 
          {
          "word": "Bankrupt", 
          "synonym": "", 
          "example": "He went bankrupt after only a year in business.", 
          "video": "https://www.youtube.com/embed/6s60Xiy6o5c"
          }, 
          {
          "word": "Bannock", 
          "synonym": "", 
          "example": "Did you ever tasted bannock?", 
          "video": "https://www.youtube.com/embed/z3NUxWHYnwQ"
          }, 
          {
          "word": "Banter", 
          "synonym": "", 
          "example": "He considered himself a master of witty banter.", 
          "video": "https://www.youtube.com/embed/qJAFiFsJvws"
          }, 
          {
          "word": "Banyan", 
          "synonym": "", 
          "example": "We were hiding amid the roots of a great banyan tree, and could see well.", 
          "video": ""
          }, 
          {
          "word": "Barb", 
          "synonym": "", 
          "example": "I tried to ignore their barbs about my new jacket.", 
          "video": "https://www.youtube.com/embed/yxbxet8GkVk  from 0:20 to 0:23 second"
          }, 
          {
          "word": "Barb", 
          "synonym": "", 
          "example": "Sharp metal barbs clustered around one tip of the arrow.", 
          "video": "https://www.youtube.com/embed/yxbxet8GkVkup to 0:18 second"
          }, 
          {
          "word": "Barbarian", 
          "synonym": "", 
          "example": "The walled city  was  attacked by barbarian hordes.", 
          "video": "https://www.youtube.com/embed/WKyWg4LgtGY"
          }, 
          {
          "word": "Barbaric", 
          "synonym": "", 
          "example": "She found the idea of killing animals for pleasure barbaric.", 
          "video": "https://www.youtube.com/embed/Da_kIpoVcYg"
          }, 
          {
          "word": "Barbecue", 
          "synonym": "", 
          "example": "In the evening there was a barbecue.", 
          "video": "https://www.youtube.com/embed/a1nYuKJPe"
          }, 
          {
          "word": "Bare your heart or soul to someone", 
          "synonym": "", 
          "example": "Mike couldn't keep things to himself any longer. He decided to bare his soul to his best friend.", 
          "video": ""
          }, 
          {
          "word": "Bare your heart/soul", 
          "synonym": "", 
          "example": "We don't know each other that well. I  certainly wouldn't bare my soul to her.", 
          "video": ""
          }, 
          {
          "word": "Bareback", 
          "synonym": "", 
          "example": "Is it difficult riding bareback?", 
          "video": "https://www.youtube.com/embed/fIU3dM00HW8  up to 0:08 second"
          }, 
          {
          "word": "Barefaced", 
          "synonym": "", 
          "example": "That's a barefaced lie.", 
          "video": "https://www.youtube.com/embed/g8WwAkx0ZnU"
          }, 
          {
          "word": "Barefoot", 
          "synonym": "", 
          "example": "We took off our shoes and socks and  walked barefoot along the beach.", 
          "video": "https://www.youtube.com/embed/XrfIcGxt"
          }, 
          {
          "word": "Bareheaded", 
          "synonym": "", 
          "example": "In all weathers they are bareheaded.", 
          "video": "https://www.youtube.com/embed/h1Uk3J5_IAo"
          }, 
          {
          "word": "Bargain for", 
          "synonym": "Planning, expecting and arranging.", 
          "example": "We hadn't bargained on such a long wait.", 
          "video": "https://www.youtube.com/embed/v17fDq575os"
          }, 
          {
          "word": "Bargain for/on sth", 
          "synonym": "", 
          "example": "We hadn't bargained on such a long wait.", 
          "video": ""
          }, 
          {
          "word": "Bargain sth away", 
          "synonym": "", 
          "example": "I realized  that by trying to gain security I had bargained  away my freedom.", 
          "video": ""
          }, 
          {
          "word": "Barge in", 
          "synonym": "", 
          "example": "I wish he'd knock instead of just barging in.", 
          "video": "https://www.youtube.com/embed/pbqeroD4Yo0"
          }, 
          {
          "word": "Barge", 
          "synonym": "", 
          "example": "Carrying goods by train costs nearly three times more than carrying them by barge.", 
          "video": "https://www.youtube.com/embed/1la7vlh5Vdc up to 0:14 second"
          }, 
          {
          "word": "Barista", 
          "synonym": "", 
          "example": "'On the house,' a barista said, placing a drink before her.", 
          "video": "https://www.youtube.com/embed/oMMPwh8YyUU"
          }, 
          {
          "word": "Baroque", 
          "synonym": "", 
          "example": "The present church is baroque in style, but contains some works of art of earlier periods.", 
          "video": "https://www.youtube.com/embed/BHM"
          }, 
          {
          "word": "Barrack for sb", 
          "synonym": "", 
          "example": "The coach barracked for his players from the gallery.", 
          "video": ""
          }, 
          {
          "word": "Barrack", 
          "synonym": "", 
          "example": "Every time the minister got up to speak  he was barracked mercilessly.", 
          "video": ""
          }, 
          {
          "word": "Barracuda", 
          "synonym": "", 
          "example": "In the world  of high finance, you have to keep an eye on the barracudas.", 
          "video": "https://www.youtube.com/embed/RYFtdzDmQ68 from 0:16 second"
          }, 
          {
          "word": "Barracuda", 
          "synonym": "", 
          "example": "When the sun rises, the place is peaceful, as the lagoon laps at its mangrove forest and barracuda, snapper and grouper enjoy the solitude.", 
          "video": "https://www.youtube.com/embed/RYFtdzDmQ68 up to 0:14 second"
          }, 
          {
          "word": "Barrage", 
          "synonym": "", 
          "example": "The proposed tidal barrage would generate enough electricity to  supply 80,000 homes.", 
          "video": "https://www.youtube.com/embed/fAEd5ZFx2_g up to 0:20 second"
          }, 
          {
          "word": "Barren", 
          "synonym": "", 
          "example": "We drove through a barren, rocky landscape.", 
          "video": "https://www.youtube.com/embed/2nSsdC2OmOs  up to 0:15 second"
          }, 
          {
          "word": "Barricade", 
          "synonym": "", 
          "example": "Inmates erected a barricade between themselves and the prison guards.", 
          "video": "https://www.youtube.com/embed/2lbDxUuIp3Q up to 0:13 second"
          }, 
          {
          "word": "Barrow", 
          "synonym": "", 
          "example": "ëPete had a lovely barrow, everything at chest height.í", 
          "video": ""
          }, 
          {
          "word": "Barter", 
          "synonym": "Buying & selling", 
          "example": "He bartered his stamp collection for her comics.", 
          "video": "https://www.youtube.com/embed/83gkEHzlCFc"
          }, 
          {
          "word": "Basalt", 
          "synonym": "Bedrock, bioclastic.", 
          "example": "The hills which bound the valley of the creek are basalt, sandstone, and schist.", 
          "video": "https://www.youtube.com/embed/_ots26QzOyA"
          }, 
          {
          "word": "Base jumping", 
          "synonym": "Glide, gliding.", 
          "example": "K is confused, but escapes from the base jumping into water and ends up in a ragged room from which he sees himself staring out from a hospital room.", 
          "video": "https://www.youtube.com/embed/hj"
          }, 
          {
          "word": "Bash on", 
          "synonym": "Continue & last.", 
          "example": "Oh well, that's enough chatting. I suppose I'd better bash on with this essay.", 
          "video": "https://www.youtube.com/embed/JoQK6dWq0D4"
          }, 
          {
          "word": "Bash", 
          "synonym": "Disapproving & criticizing.", 
          "example": "He kept bashing local government officials.", 
          "video": "https://www.youtube.com/embed/KhRj3Z0dOsY"
          }, 
          {
          "word": "Bash", 
          "synonym": "Hitting and beating.", 
          "example": "He bashed his arm against a shelf.", 
          "video": "https://www.youtube.com/embed/j2q4TZz0"
          }, 
          {
          "word": "Bask in sth", 
          "synonym": "Ecstasy, glory.", 
          "example": "He basked in his moment of glory, holding the trophy up to the crowd.", 
          "video": "https://www.youtube.com/embed/2BVrzWqdAdg"
          }, 
          {
          "word": "Bask", 
          "synonym": "Calming and relaxing.", 
          "example": "We could see seals on the rocks, basking in the sun.", 
          "video": "https://www.youtube.com/embed/jyK83HSQMRY"
          }, 
          {
          "word": "Basset", 
          "synonym": "Alsatian, beagle.", 
          "example": "Basset hounds are occasionally referred to as hush puppies for that reason.", 
          "video": "https://www.youtube.com/embed/O"
          }, 
          {
          "word": "Bassoon", 
          "synonym": "Accordion, acoustically.", 
          "example": "The name of the instrument is a portmanteau word of trombone and bassoon.", 
          "video": "https://www.youtube.com/embed/kCWXcbwdIB4"
          }, 
          {
          "word": "Bats in the belfry", 
          "synonym": "", 
          "example": "He comes up with the craziest ideas", 
          "video": "https://www.youtube.com/embed/eeWtPyBQxZs"
          }, 
          {
          "word": "Batten down the hatches", 
          "synonym": "Closing and blocking.", 
          "example": "When you're coming down with flu all you can do is batten down the hatches and wait for it to pass.", 
          "video": "https://www.youtube.com/embed/5cpA35r1J3o"
          }, 
          {
          "word": "Batten on somebody", 
          "synonym": "Treating people or animals badly.", 
          "example": "He's spent these last five years battening on a rich aunt of his.", 
          "video": ""
          }, 
          {
          "word": "Battle of wits", 
          "synonym": "Thinking and contemplating.", 
          "example": "A good mystery story is a battle of wits between author and reader.", 
          "video": "https://www.youtube.com/embed/m66xPzu9vj4"
          }, 
          {
          "word": "Bawl", 
          "synonym": "Shouting & screaming.", 
          "example": "She bawled at me to sit down.", 
          "video": "https://www.youtube.com/embed/n45bsRH4ZcE"
          }, 
          {
          "word": "Bawl", 
          "synonym": "Weeping and crying.", 
          "example": "He was bawling his eyes out.", 
          "video": "https://www.youtube.com/embed/P156dbke5RI"
          }, 
          {
          "word": "Bay leaf", 
          "synonym": "Herbs & spices.", 
          "example": "Put into boiling salt water, add bay leaf, parsley, seasonings and cook till tender.", 
          "video": "https://www.youtube.com/embed/0_FRj7wjChY"
          }, 
          {
          "word": "Bayou", 
          "synonym": "Watercourses & waterfalls.", 
          "example": "About five in the afternoon we gathered on the bank of the bayou.", 
          "video": "https://www.youtube.com/embed/lxq3MEkCRe4"
          }, 
          {
          "word": "Be  much obliged", 
          "synonym": "Satisfied, Pleased", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be all downhill", 
          "synonym": "Easiness ,simplicity.", 
          "example": "Once we get the preparation done, it'll be downhill all the way.", 
          "video": "https://www.youtube.com/embed/iHxpqebW3qU"
          }, 
          {
          "word": "Be all part of life's rich tapestry/pageant", 
          "synonym": "", 
          "example": "Traffic jam of Dhaka is part of life's rich tapestry of the city people, who enjoys all the modern facilities of the capital.", 
          "video": ""
          }, 
          {
          "word": "Be all the rage", 
          "synonym": "Sharp, Latest, Happening, High", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be as daft as a brush", 
          "synonym": "", 
          "example": "He's a nice enough boy, but he's as daft as a brush.", 
          "video": "https://www.youtube.com/embed/g"
          }, 
          {
          "word": "Be as old as the hills", 
          "synonym": "Old or old", 
          "example": "As vales are as old as the hills, so loughs and rivers must be as old as they.", 
          "video": "https://www.youtube.com/embed/p6m"
          }, 
          {
          "word": "Be only a matter of time", 
          "synonym": "Relentless, remorseless.", 
          "example": "It's only a matter of time before he's forced to resign.", 
          "video": "https://www.youtube.com/embed/3ugbNN0BKDI"
          }, 
          {
          "word": "Be right under  your  nose", 
          "synonym": "", 
          "example": "I spent all morning looking for the book, and it was right under my nose the whole time.", 
          "video": ""
          }, 
          {
          "word": "Be Descended", 
          "synonym": "Dive, Roll Down", 
          "example": "She claims to be descended from royalty.", 
          "video": "https://www.youtube.com/embed/CylT6U0Oz1Y"
          }, 
          {
          "word": "Be a badge of something", 
          "synonym": "", 
          "example": "For Tony, owning a big car was a badge of success.", 
          "video": ""
          }, 
          {
          "word": "Be a barrel of laughs/fun", 
          "synonym": "", 
          "example": "'He's a bit serious, isn't he?' 'Yeah, not exactly a barrel of laughs.'", 
          "video": "https://www.youtube.com/embed/o_BEggKk"
          }, 
          {
          "word": "Be a chapter of accidents", 
          "synonym": "", 
          "example": "Lately with my bad health and financial condition it has been a chapter of accidents.", 
          "video": ""
          }, 
          {
          "word": "Be a credit to sb/sth", 
          "synonym": "Pride yourself on something, Congratulate yourself, Be a credit to someone.", 
          "example": "Our fans are a credit to the club.", 
          "video": ""
          }, 
          {
          "word": "Be a disaster", 
          "synonym": "", 
          "example": "My personal life has been a disaster last few months.", 
          "video": ""
          }, 
          {
          "word": "Be a disaster", 
          "synonym": "", 
          "example": "The evening was a complete disaster.", 
          "video": ""
          }, 
          {
          "word": "Be a disgrace to sb/ sth", 
          "synonym": "", 
          "example": "You're a disgrace to the family", 
          "video": ""
          }, 
          {
          "word": "Be a disgrace to sb/sth", 
          "synonym": "", 
          "example": "Omar was a disgrace to his family.", 
          "video": ""
          }, 
          {
          "word": "Be a disgrace", 
          "synonym": "", 
          "example": "The conduct of the player was a disgrace.", 
          "video": ""
          }, 
          {
          "word": "Be a disgrace", 
          "synonym": "", 
          "example": "Three families living in one room", 
          "video": "https://www.youtube.com/embed/t9vNP5iyw3U"
          }, 
          {
          "word": "Be a drag on sb/sth", 
          "synonym": "Preventing, impeding.", 
          "example": "She didn't want a husband who would be a drag on her career.", 
          "video": ""
          }, 
          {
          "word": "Be a faff", 
          "synonym": "loiter n", 
          "example": "Don't be a faff and help us out.", 
          "video": ""
          }, 
          {
          "word": "Be a fag", 
          "synonym": "", 
          "example": "Doing chores can be a fag.", 
          "video": ""
          }, 
          {
          "word": "Be a far cry from something.", 
          "synonym": "differ, another way.", 
          "example": "This flat is a far cry from the house they had before.", 
          "video": ""
          }, 
          {
          "word": "Be a hard or tough act to follow", 
          "synonym": "", 
          "example": "His presidency was very successful ", 
          "video": ""
          }, 
          {
          "word": "Be a heather", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be a licence to print money", 
          "synonym": "", 
          "example": "I wonder where he gets such amount of money, he has become a licence to print money.", 
          "video": "https://www.youtube.com/embed/lmHmqJn"
          }, 
          {
          "word": "Be a martyr to  sth", 
          "synonym": "Sicken, relapse", 
          "example": "She's a martyr to migraines!", 
          "video": ""
          }, 
          {
          "word": "Be a matter of confidence/luck/waiting, etc.", 
          "synonym": "", 
          "example": "Baking a cake isn't difficult", 
          "video": ""
          }, 
          {
          "word": "Be a matter of life and/or death", 
          "synonym": "Very important or urgent.", 
          "example": "And if you miss the bus, well, it's not a matter of life and death.", 
          "video": ""
          }, 
          {
          "word": "Be a matter of opinion", 
          "synonym": "Opinions, beliefs and points of view.", 
          "example": "Both performances were excellent; it's simply a matter of opinion as to whose was better.", 
          "video": ""
          }, 
          {
          "word": "Be a matter of record", 
          "synonym": "True, real, false, and unreal.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/0ycQeD5PfU8"
          }, 
          {
          "word": "Be a pack of lies / be a tissue of lies", 
          "synonym": "", 
          "example": "The whole report is a pack of lies.", 
          "video": ""
          }, 
          {
          "word": "Be after somebodyís blood", 
          "synonym": "Lose your temper", 
          "example": "Lisa is looking for you, and sheís after your blood.", 
          "video": ""
          }, 
          {
          "word": "Be ahead of the game", 
          "synonym": "", 
          "example": "Our research and development program ensures that we're ahead of the game.", 
          "video": ""
          }, 
          {
          "word": "Be an item", 
          "synonym": "Marriage, cohabitation & other relationships.", 
          "example": "I saw Darren and Emma there. Are they an item?", 
          "video": "https://www.youtube.com/embed/hA4X90"
          }, 
          {
          "word": "Be as busy as a bee.", 
          "synonym": "", 
          "example": "She is as busy as a bee in the morning.", 
          "video": "https://www.youtube.com/embed/XA9_CE0SMBs"
          }, 
          {
          "word": "Be at a crossroads", 
          "synonym": "", 
          "example": "By 1998 I was at the crossroads.", 
          "video": ""
          }, 
          {
          "word": "Be at large", 
          "synonym": "Running away and escaping.", 
          "example": "Twelve prisoners are at large following a series of escapes.", 
          "video": ""
          }, 
          {
          "word": "Be at liberty to do  sth", 
          "synonym": "", 
          "example": "I'm not at liberty to reveal any names.", 
          "video": ""
          }, 
          {
          "word": "Be at odds", 
          "synonym": "Arguing & disagreeing.", 
          "example": "They're at odds over the funding of the project.", 
          "video": "https://www.youtube.com/embed/n6mkRIMuB"
          }, 
          {
          "word": "Be at peace with the world", 
          "synonym": "", 
          "example": "Mental satisfaction along with financial security makes a person to be at peace with the world.", 
          "video": ""
          }, 
          {
          "word": "Be away with the fairies", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be backward in coming forward", 
          "synonym": "", 
          "example": "I'm sure Matt will tell you what he thinks of the idea", 
          "video": ""
          }, 
          {
          "word": "Be bang on", 
          "synonym": "", 
          "example": "What was your answer? 76? That's absolutely bang on!", 
          "video": "https://www.youtube.com/embed/DVjhMpJPOxk"
          }, 
          {
          "word": "Be barking up the wrong tree", 
          "synonym": "", 
          "example": "She thinks it'll solve the problem, but I think she's barking up the wrong tree.", 
          "video": "https://www.youtube.com/embed/7HYjay9PpC0"
          }, 
          {
          "word": "Be bound and determined", 
          "synonym": "Assuredly", 
          "example": "They are bound and determined to build their own house someday.", 
          "video": ""
          }, 
          {
          "word": "Be carpeted with something", 
          "synonym": "Matting", 
          "example": "In spring this area is carpeted with bluebells.", 
          "video": ""
          }, 
          {
          "word": "Be cast in the same mould", 
          "synonym": "", 
          "example": "All the members of the family are cast in the same mold and they all had success as entertainers.", 
          "video": ""
          }, 
          {
          "word": "Be chasing your tail", 
          "synonym": "", 
          "example": "Watching you try to fix the problem is kind of silly, it is like chasing your tail.", 
          "video": ""
          }, 
          {
          "word": "Be childís play", 
          "synonym": "", 
          "example": "Working out that problem is childís play.", 
          "video": ""
          }, 
          {
          "word": "Be chilled/frozen to the marrow", 
          "synonym": "", 
          "example": "Such a weather, I am almost freezing to the cold.", 
          "video": ""
          }, 
          {
          "word": "Be concerned with sth/ sb", 
          "synonym": "Worried,feeling care for something/someone", 
          "example": "Today's lesson is concerned with punctuation.", 
          "video": ""
          }, 
          {
          "word": "Be confined to somewhere/ sth", 
          "synonym": "", 
          "example": "Everyone knows that the illness is not confined to any one group in society.", 
          "video": ""
          }, 
          {
          "word": "Be conscious of sth/sb", 
          "synonym": "", 
          "example": "He is elegant, sensual, conscious of his body.", 
          "video": ""
          }, 
          {
          "word": "Be conspicuous by your absence", 
          "synonym": "", 
          "example": "The football players got angry that the police were conspicuous by their absence.", 
          "video": ""
          }, 
          {
          "word": "Be consumed by/with sth", 
          "synonym": "", 
          "example": "In Moby Dick the captain was consumed with the white whale.", 
          "video": ""
          }, 
          {
          "word": "Be conversant with sth", 
          "synonym": "Aware.", 
          "example": "I'm not conversant with the rules of chess.", 
          "video": ""
          }, 
          {
          "word": "Be convulsed with laughter/rage, etc.", 
          "synonym": "Strong feelings.", 
          "example": "All of us were convulsed with laughter.", 
          "video": ""
          }, 
          {
          "word": "Be cooking", 
          "synonym": "Betterment", 
          "example": "The battery's recharged, give it a little more gas. Now we're cooking!", 
          "video": ""
          }, 
          {
          "word": "Be cool with sth", 
          "synonym": "Calm and relaxed.", 
          "example": "", 
          "video": "Yeah, we could leave later "
          }, 
          {
          "word": "Be crawling with sth", 
          "synonym": "Brim, Abound, Jam", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be crazy about sb/sth", 
          "synonym": "Admire, Care for, Worship", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be curtains for sb", 
          "synonym": "", 
          "example": "It'll be curtains for him if he doesn't do what I tell him!", 
          "video": ""
          }, 
          {
          "word": "Be cut up", 
          "synonym": "", 
          "example": "Philip was very cut up about his grandmother's death.", 
          "video": "https://www.youtube.com/embed/DtALNCfs1Ng from 0:19 second"
          }, 
          {
          "word": "Be damned if you do and damned if you don't", 
          "synonym": "", 
          "example": "He's damned if he does and damned if he doesn't.", 
          "video": ""
          }, 
          {
          "word": "Be dancing in the streets", 
          "synonym": "Breezy,  delighted.", 
          "example": "Not many people will be dancing in the streets about a two percent pay rise.", 
          "video": ""
          }, 
          {
          "word": "Be devoid of sth", 
          "synonym": "Wasted, Drained, Reduced , Vacant", 
          "example": "When he finally lifted his head and spoke to Adrienne, his voice was devoid of any emotion.", 
          "video": ""
          }, 
          {
          "word": "Be devoured by sth.", 
          "synonym": "Absorb, nag, Brood, Fix", 
          "example": "He was devoured by jealousy/hatred.", 
          "video": ""
          }, 
          {
          "word": "Be dotty about somebody/something", 
          "synonym": "Crazy, Stupid, Silly, Absurd", 
          "example": "Joyaís absolutely dotty about cats.", 
          "video": ""
          }, 
          {
          "word": "Be down in black and white", 
          "synonym": "", 
          "example": "I couldn't believe it was true, but there it was, in black and white.", 
          "video": "https://www.youtube.com/embed/v5xFT4vjysg"
          }, 
          {
          "word": "Be draped in/with sth", 
          "synonym": "Flow, hang.", 
          "example": "The coffins were all draped with the national flag.", 
          "video": ""
          }, 
          {
          "word": "Be elevated to sth", 
          "synonym": "", 
          "example": "He has been elevated to deputy manager.", 
          "video": ""
          }, 
          {
          "word": "Be endowed with sth", 
          "synonym": "claim, endow.", 
          "example": "Sardinia is generously endowed with prehistoric sites.", 
          "video": ""
          }, 
          {
          "word": "Be engraved on your memory/mind", 
          "synonym": "Remembering, reminding and reminders.", 
          "example": "That last conversation we had is engraved on my memory forever.", 
          "video": ""
          }, 
          {
          "word": "Be enshrined in sth", 
          "synonym": "lay, maintain.", 
          "example": "The right of freedom of speech is enshrined in law/in the constitution.", 
          "video": ""
          }, 
          {
          "word": "Be fading away/fast", 
          "synonym": "disappearing", 
          "example": "The coast line is fading away fast.", 
          "video": ""
          }, 
          {
          "word": "Be familiar with something/somebody.", 
          "synonym": "Aware of something/somebody. To know.", 
          "example": "I'm sorry, I'm not familiar with your poetry.", 
          "video": ""
          }, 
          {
          "word": "Be gagging for it", 
          "synonym": "crave, desire, want", 
          "example": "Oh, where is that 'gagging for it' peanut butter isle!", 
          "video": "https://www.youtube.com/embed/pZsHjEBqxwk"
          }, 
          {
          "word": "Be gagging for/to do  sth", 
          "synonym": "be desperate for, thirst for, yearn for", 
          "example": "Men everywhere are gagging for a car like this.", 
          "video": "https://www.youtube.com/embed/pZsHjEBqxwk"
          }, 
          {
          "word": "Be getting on", 
          "synonym": "latecomer, latest.", 
          "example": "It's getting on", 
          "video": ""
          }, 
          {
          "word": "Be getting on", 
          "synonym": "midlife crisis, old age.", 
          "example": "He's getting on a bit", 
          "video": ""
          }, 
          {
          "word": "Be green about the gills", 
          "synonym": "Be green around the gills.", 
          "example": "Some of the passengers looked kind of green around the gills after the trip!", 
          "video": "https://www.youtube.com/embed/2oTjEQkuO4A"
          }, 
          {
          "word": "Be had", 
          "synonym": "trick, ploy, dodge, ruse", 
          "example": "If your customer thinks he's been had, you have to make him happy.", 
          "video": ""
          }, 
          {
          "word": "Be half the battle", 
          "synonym": "", 
          "example": "For a lot of jobs, getting an interview is half the battle.", 
          "video": ""
          }, 
          {
          "word": "Be half the dancer/writer, etc. you used to be", 
          "synonym": "", 
          "example": "She's half the tennis player she used to be.", 
          "video": ""
          }, 
          {
          "word": "Be highly/ well considered", 
          "synonym": "", 
          "example": "I don't like her books, but I know she's very highly considered.", 
          "video": ""
          }, 
          {
          "word": "Be in a bad way", 
          "synonym": "", 
          "example": "She was thin and tired", 
          "video": "https://www.youtube.com/embed/njgq4fqbtpI?t=16s"
          }, 
          {
          "word": "Be in a lather", 
          "synonym": "Flustered;", 
          "example": "Now, calm down. Don't be in a lather.", 
          "video": ""
          }, 
          {
          "word": "Be in bed with.", 
          "synonym": "", 
          "example": "The newspaper editor is obviously in bed with the president.", 
          "video": ""
          }, 
          {
          "word": "Be in bondage to sth", 
          "synonym": "Be locked in sth", 
          "example": "Masters sometimes allowed their slaves to buy their way out of bondage.", 
          "video": ""
          }, 
          {
          "word": "Be in conference", 
          "synonym": "", 
          "example": "Mr. David  isn't available at the moment. He's in conference.", 
          "video": ""
          }, 
          {
          "word": "Be in convulsions", 
          "synonym": "Giggle", 
          "example": "Hearing the joke I was in convulsions.", 
          "video": ""
          }, 
          {
          "word": "Be in deep water/get into deep water", 
          "synonym": "", 
          "example": "With the war looming over us we are in deep water now.", 
          "video": ""
          }, 
          {
          "word": "Be in its infancy", 
          "synonym": "", 
          "example": "The system is still in its infancy.", 
          "video": ""
          }, 
          {
          "word": "Be in line for something.", 
          "synonym": "Possibility, Likely, Probably.", 
          "example": "If anyone's in line for promotion, I should think it's Helen.", 
          "video": ""
          }, 
          {
          "word": "Be in line to do something.", 
          "synonym": "Likelihood, Maybe, Arguably.", 
          "example": "Kim Bailey is next in line to replace Chris Finlay as CEO.", 
          "video": ""
          }, 
          {
          "word": "Be in line to the throne.", 
          "synonym": "", 
          "example": "Prince Charles is first in line to the British throne.", 
          "video": ""
          }, 
          {
          "word": "Be in line with something.", 
          "synonym": "", 
          "example": "Just get in line and wait your turn like everyone else.", 
          "video": ""
          }, 
          {
          "word": "Be in sb's employ", 
          "synonym": "", 
          "example": "Mr. Rashed is currently in our employ.", 
          "video": ""
          }, 
          {
          "word": "Be in sbís bad book", 
          "synonym": "", 
          "example": "He's in Melanie's bad books because he arrived two hours late.", 
          "video": "https://www.youtube.com/embed/YjTpLsGf5j4up to  0:40 second"
          }, 
          {
          "word": "Be in sbís good book", 
          "synonym": "", 
          "example": "He's in Melanie's good book because he arrived two hours late.", 
          "video": "https://www.youtube.com/embed/SzoIOfRoFR0"
          }, 
          {
          "word": "Be in the blood", 
          "synonym": "Ancestor", 
          "example": "His father and grandmother were painters too, so it's obviously in the blood.", 
          "video": ""
          }, 
          {
          "word": "Be in the dark", 
          "synonym": "Unaware,  unconscious.", 
          "example": "Somehow, everyone knew that Alicia had quit school except for me I was totally in the dark.", 
          "video": ""
          }, 
          {
          "word": "Be in the family way.", 
          "synonym": "to be pregnant, pregnancy.", 
          "example": "He would disgrace them by getting a girl in the family way.", 
          "video": ""
          }, 
          {
          "word": "Be in the know", 
          "synonym": "To have information, To be familiar with", 
          "example": "'Where did he go?' 'I don't know.'", 
          "video": ""
          }, 
          {
          "word": "Be in the land of nod", 
          "synonym": "", 
          "example": "Jamie's in the land of nod at last.", 
          "video": ""
          }, 
          {
          "word": "Be in the land of the living", 
          "synonym": "", 
          "example": "She was partying till the early hours, so I don't imagine she'll be in the land of the living before lunchtime.", 
          "video": ""
          }, 
          {
          "word": "Be in the pay of  sb", 
          "synonym": "", 
          "example": "Why are you talking in the support of that criminal? Are you in pay of him?", 
          "video": ""
          }, 
          {
          "word": "Be in your element", 
          "synonym": "", 
          "example": "Maria, of course , was in her element, making all the arrangements", 
          "video": ""
          }, 
          {
          "word": "Be in your face", 
          "synonym": "Aggressive", 
          "example": "Why has your boss been in your face all day.", 
          "video": ""
          }, 
          {
          "word": "Be in/out of contention of sth", 
          "synonym": "", 
          "example": "Sanders was in the contention of winning the primaries.", 
          "video": ""
          }, 
          {
          "word": "Be joined in marriage/matrimony.", 
          "synonym": "", 
          "example": "They were joined together in holy matrimony .", 
          "video": ""
          }, 
          {
          "word": "Be jonesing for something.", 
          "synonym": "", 
          "example": "I'm jonesing for a coffee", 
          "video": ""
          }, 
          {
          "word": "Be lacking in sth", 
          "synonym": "", 
          "example": "He's totally lacking in charm.", 
          "video": ""
          }, 
          {
          "word": "Be lacking", 
          "synonym": "", 
          "example": "Enthusiasm has been sadly lacking these past months at work.", 
          "video": ""
          }, 
          {
          "word": "Be laid up", 
          "synonym": "", 
          "example": "She's been laid up in bed with flu for a week.", 
          "video": "https://www.youtube.com/embed/UGBtefVxxFM up to 0:11 second"
          }, 
          {
          "word": "Be laughed out of court", 
          "synonym": "", 
          "example": "The proposal will be laughed out of court.", 
          "video": ""
          }, 
          {
          "word": "Be laughing all the way to the bank.", 
          "synonym": "", 
          "example": "We'll be laughing all the way to the bank if this deal works out.", 
          "video": ""
          }, 
          {
          "word": "Be laughing on the other side of your face.", 
          "synonym": "", 
          "example": "She's pleased with her promotion but she'll be laughing on the other side of her face when she sees the extra work.", 
          "video": ""
          }, 
          {
          "word": "Be laughing.", 
          "synonym": "", 
          "example": "If the loan's approved, you're laughing.", 
          "video": ""
          }, 
          {
          "word": "Be like a bear with a sore head", 
          "synonym": "Argumentative, bad", 
          "example": "You're like a bear with a sore head this morning. What's wrong with you?", 
          "video": "https://www.youtube.com/embed/_NKzdSZc9qE"
          }, 
          {
          "word": "Be like a red flag to a bull", 
          "synonym": "", 
          "example": "John’s gone to gloat about his success over his brother, which is like a red flag to a bull, if you ask me.", 
          "video": ""
          }, 
          {
          "word": "Be marked out as something", 
          "synonym": "Unique, Unusal", 
          "example": "I can't speak a word of French so I'm marked out as a foreigner as soon as I arrive in France.", 
          "video": ""
          }, 
          {
          "word": "Be meant for each other.", 
          "synonym": "", 
          "example": "I'm not surprised that they have such a happy marriage. I always knew that they were meant for each other.", 
          "video": ""
          }, 
          {
          "word": "Be meat and drink to somebody.", 
          "synonym": "Self", 
          "example": "Working on complex pension calculations would put me to sleep, but it's meat and drink to my brother.", 
          "video": ""
          }, 
          {
          "word": "Be mentioned in dispatches", 
          "synonym": "", 
          "example": "He was a war hero according since he was mentioned in dispatches.", 
          "video": ""
          }, 
          {
          "word": "Be mentioned in dispatches", 
          "synonym": "", 
          "example": "Sergeant Havers was mentioned in dispatches for his courage.", 
          "video": ""
          }, 
          {
          "word": "Be more to this than meets the eye.", 
          "synonym": "", 
          "example": "This whole business is very puzzling. There is a lot more to it than meets the eye.", 
          "video": ""
          }, 
          {
          "word": "Be new to this game", 
          "synonym": "", 
          "example": "I am new to this game of transcibing conversations.", 
          "video": ""
          }, 
          {
          "word": "Be no laughing matter", 
          "synonym": "", 
          "example": "Being arrested by the police is no laughing matter.", 
          "video": ""
          }, 
          {
          "word": "Be no laughing matter.", 
          "synonym": "", 
          "example": "Being arrested by the police is no laughing matter.", 
          "video": ""
          }, 
          {
          "word": "Be no match for  sth/sb", 
          "synonym": "", 
          "example": "Gibson ran well but was no match for the young Italian.", 
          "video": ""
          }, 
          {
          "word": "Be no oil painting", 
          "synonym": "Ghoulish, hideously.", 
          "example": "She's no oil painting but she's got an attractive personality.", 
          "video": ""
          }, 
          {
          "word": "Be no respecter of sth", 
          "synonym": "", 
          "example": "Air pollution is no respecter of national frontiers.", 
          "video": ""
          }, 
          {
          "word": "Be obliged if", 
          "synonym": "Acknowledge Enjoy , Welcome", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Be obliged if", 
          "synonym": "Relief, relieved.", 
          "example": "I'd be obliged if you would complete and return the form as soon as possible.", 
          "video": ""
          }, 
          {
          "word": "Be of concern", 
          "synonym": "Deal with, Cover, Treat", 
          "example": "The report concerns global warming.", 
          "video": ""
          }, 
          {
          "word": "Be of little account", 
          "synonym": "", 
          "example": "The colour of someoneís skin should be of no account.", 
          "video": ""
          }, 
          {
          "word": "Be off the mark", 
          "synonym": "Unreal, Fake", 
          "example": "His criticisms are way off the mark.", 
          "video": "https://www.youtube.com/embed/rlRSytdQ_"
          }, 
          {
          "word": "Be on  sb's  tail", 
          "synonym": "", 
          "example": "That driver's been on my tail for miles.", 
          "video": ""
          }, 
          {
          "word": "Be on familiar terms.", 
          "synonym": "friendly, amiable, familiarity.", 
          "example": "We had met before, but we were hardly on familiar terms.", 
          "video": ""
          }, 
          {
          "word": "Be on the cards", 
          "synonym": "", 
          "example": "'So you think they'll get married next year?' 'I think it's on the cards.'", 
          "video": ""
          }, 
          {
          "word": "Be on the carpet", 
          "synonym": "Chastising & rebuking.", 
          "example": "When my team lost that big client, the boss called me on the carpet.", 
          "video": ""
          }, 
          {
          "word": "Be on the level", 
          "synonym": "Genuine, Straight, Honest, Above board, Fair, True, Legitimate, Sincere", 
          "example": "Eddie said my story was on the level.", 
          "video": ""
          }, 
          {
          "word": "Be on the line.", 
          "synonym": "Unsafe, Threatened, Jeopardy.", 
          "example": "Almost 3,000 jobs have been lost recently, and a further 3,000 are on the line.", 
          "video": ""
          }, 
          {
          "word": "Be on the scene", 
          "synonym": "To arrive, Arriving, Entering, Invading", 
          "example": "I called the police and they were on the scene within minutes.", 
          "video": "https://www.youtube.com/embed/NnbDNCqdgVM"
          }, 
          {
          "word": "Be on/off the danger list", 
          "synonym": "Infirmity, organic.", 
          "example": "Heís been extremely sick, but thankfully heís off the danger list now.", 
          "video": ""
          }, 
          {
          "word": "Be one/another of life's great mysteries", 
          "synonym": "", 
          "example": "It really is one of life's greatest mysteries why that awful restaurant is busy every night.", 
          "video": ""
          }, 
          {
          "word": "Be out for/after  sb's  scalp", 
          "synonym": "Acrimonious, Aggrieved, Amused, Annoyed, Apoplectic", 
          "example": "He's made one mistake too many, and now they're out for his scalp.", 
          "video": ""
          }, 
          {
          "word": "Be out of line with something.", 
          "synonym": "Conflict, Depart, Diverge.", 
          "example": "Their predictions were hopelessly out of line with the actual results.", 
          "video": ""
          }, 
          {
          "word": "Be out of your element", 
          "synonym": "", 
          "example": "Most students are out of their element during their exams.", 
          "video": ""
          }, 
          {
          "word": "Be par for the course", 
          "synonym": "", 
          "example": "The school budget is going to be cut again this year, but then that's par for the course.", 
          "video": ""
          }, 
          {
          "word": "Be penny", 
          "synonym": "Ante, chargeable.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/n8eTfI5pp9A"
          }, 
          {
          "word": "Be quick/slow off the mark", 
          "synonym": "Intelligence, Acuity", 
          "example": "The police were certainly quick off the mark in reaching the scene of the accident.", 
          "video": "https://www.youtube.com/embed/rlRSytdQ_"
          }, 
          {
          "word": "Be ready to do  sth", 
          "synonym": "Ready and willing.", 
          "example": "These men are ready to die for their country.", 
          "video": ""
          }, 
          {
          "word": "Be ready to roll", 
          "synonym": "Corner, horizon.", 
          "example": "The new TV series from the West Wing team is ready to roll.", 
          "video": ""
          }, 
          {
          "word": "Be respectful of  sth", 
          "synonym": "", 
          "example": "He taught his children to be respectful of other cultures.", 
          "video": ""
          }, 
          {
          "word": "Be responsible for  your  actions", 
          "synonym": "", 
          "example": "Although he was ill at the time, he was still responsible for his actions.", 
          "video": ""
          }, 
          {
          "word": "Be responsible for sb/sth/doing sth", 
          "synonym": "", 
          "example": "Who is responsible for this terrible mess?", 
          "video": ""
          }, 
          {
          "word": "Be responsible for sth/doing sth", 
          "synonym": "", 
          "example": "Last month's bad weather was responsible for the crop failure.", 
          "video": ""
          }, 
          {
          "word": "Be responsible to  sth", 
          "synonym": "", 
          "example": "Only our elected representatives, responsible to us, can make these big decisions.", 
          "video": ""
          }, 
          {
          "word": "Be resting", 
          "synonym": "", 
          "example": "Over 90 percent of professional actors are resting at any given time.", 
          "video": ""
          }, 
          {
          "word": "Be riding/on the crest of a wave", 
          "synonym": "Ascendant, chart.", 
          "example": "Mrs Singh is still riding the crest of a wave of popularity.", 
          "video": ""
          }, 
          {
          "word": "Be sacked/get the sack", 
          "synonym": "", 
          "example": "Charlie got the sack when his boss caught him stealing.", 
          "video": ""
          }, 
          {
          "word": "Be scattered to the four winds", 
          "synonym": "Removing, Getting rid of things", 
          "example": "It was the finest collection of paintings in Denmark, but during the last war it was broken up and scattered to the four winds.", 
          "video": ""
          }, 
          {
          "word": "Be tailor", 
          "synonym": "", 
          "example": "It sounds as though you're tailor", 
          "video": ""
          }, 
          {
          "word": "Be that as it may.", 
          "synonym": "Nevertheless, However, Though.", 
          "example": "Building a new children's home will cost a lot of money but, be that as it may, there is an urgent need for the facility.", 
          "video": "https://www.youtube.com/embed/nvYEpJavQtw"
          }, 
          {
          "word": "Be the creature of sb/sth", 
          "synonym": "Life, Animal, living thing, Mortal, Soul, Man", 
          "example": "We must try to be kind to our fellow creatures.", 
          "video": ""
          }, 
          {
          "word": "Be the last word in sth", 
          "synonym": "", 
          "example": "It's a nice enough restaurant and it's very reasonably priced but it's not exactly the last word in style.", 
          "video": ""
          }, 
          {
          "word": "Be to blame", 
          "synonym": "Guilt", 
          "example": "The hot weather is partly to blame for the water shortage.", 
          "video": ""
          }, 
          {
          "word": "Be two/ten a penny", 
          "synonym": "Buck, C", 
          "example": "A dime is paid for two papers.", 
          "video": "https://www.youtube.com/embed/SKMgrqjkGM4"
          }, 
          {
          "word": "Be under contract", 
          "synonym": "", 
          "example": "Richard was under contract and was unable to disclose much information.", 
          "video": ""
          }, 
          {
          "word": "Be up in arms", 
          "synonym": "", 
          "example": "The entire population is up in arms.", 
          "video": ""
          }, 
          {
          "word": "Be up to par", 
          "synonym": "", 
          "example": "Her work hasn't been up to par lately.", 
          "video": ""
          }, 
          {
          "word": "Be up to the mark", 
          "synonym": "To be good enough", 
          "example": "Her latest batch of work just isn't up to the mark.", 
          "video": "https://www.youtube.com/embed/rlRSytdQ_"
          }, 
          {
          "word": "Be up with the lark", 
          "synonym": "Ahead, ahead of.", 
          "example": "Normally she was up with the lark, but today she had nothing on till late morning and had arranged to drop Mother off at Cherry's at ten.", 
          "video": "https://www.youtube.com/embed/5QMsFKDdg2c"
          }, 
          {
          "word": "Be wearing blinkers", 
          "synonym": "Narrow", 
          "example": "Always wearing blinkers brings only negativity in life.", 
          "video": ""
          }, 
          {
          "word": "Be within hailing distance of somewhere", 
          "synonym": "to be near someone, closeness in distance and time", 
          "example": "When the boat came within hailing distance, I asked if I could borrow some gasoline.", 
          "video": "https://www.youtube.com/embed/iEXzQdIHn2Y"
          }, 
          {
          "word": "Be your  own master", 
          "synonym": "", 
          "example": "Every woman should earn theit living by themselves, so that they can be their own master.", 
          "video": ""
          }, 
          {
          "word": "Be/ feel disinclined to do sth", 
          "synonym": "", 
          "example": "I am/feel disinclined to offer him a job if he doesn't have a degree.", 
          "video": "https://www.youtube.com/embed/JP_GfeHFzSk"
          }, 
          {
          "word": "Be/ weigh on your conscience", 
          "synonym": "", 
          "example": "Yesterday I ignored an old woman who asked me for money in the street, and it's been on my conscience ever since.", 
          "video": ""
          }, 
          {
          "word": "Be/feel  etc.  obliged", 
          "synonym": "Duty, obligation and responsibility.", 
          "example": "She feels obligated to be nice to Jack because he's her boss.", 
          "video": ""
          }, 
          {
          "word": "Be/feel disinclined to do sth", 
          "synonym": "", 
          "example": "Jamal was disinclined to ride the roller coaster.", 
          "video": ""
          }, 
          {
          "word": "Be/feel etc. obliged", 
          "synonym": "chillax, calm down, relax...", 
          "example": "Doing something you feel obligated to do is not bad.", 
          "video": ""
          }, 
          {
          "word": "Be/go at it hammer and tongs", 
          "synonym": "Energetic and lively.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/wwbaAFiuPCE"
          }, 
          {
          "word": "Be/go into ecstasies about/over something", 
          "synonym": "effusive, enthuse, rave", 
          "example": "They went into ecstasies over the beauty of the countryside.", 
          "video": ""
          }, 
          {
          "word": "Be/go off on one", 
          "synonym": "Berate, bite.", 
          "example": "He went off on one and started accusing me of stealing his girlfriend.", 
          "video": ""
          }, 
          {
          "word": "Be/live in la", 
          "synonym": "", 
          "example": "Even after not studying seriously, you dream of being a topper in the board exam, you are just living in la", 
          "video": ""
          }, 
          {
          "word": "Beacon", 
          "synonym": "Fire & flame.", 
          "example": "She was a beacon of hope in troubled times.", 
          "video": "https://www.youtube.com/embed/2QpPiOVpsVE"
          }, 
          {
          "word": "Bead", 
          "synonym": "badge, beaded.", 
          "example": "She wore a necklace of brightly coloured wooden beads.", 
          "video": "https://www.youtube.com/embed/Dp5gwxVQT24"
          }, 
          {
          "word": "Beagle", 
          "synonym": "Bloodhound, doggy.", 
          "example": "Snoopy is the world's most famous beagle.", 
          "video": "https://www.youtube.com/embed/oqmpepNNkw0"
          }, 
          {
          "word": "Beak", 
          "synonym": "", 
          "example": "It carried a huge stick in its beak.", 
          "video": "https://www.youtube.com/embed/i0p1p8TWztE"
          }, 
          {
          "word": "Beam", 
          "synonym": "Arch,architrave.", 
          "example": "The sitting room had exposed wooden beams.", 
          "video": "https://www.youtube.com/embed/euto2vgiHys"
          }, 
          {
          "word": "Beam", 
          "synonym": "Quantities & units of light.", 
          "example": "We could just pick out the trail in the weak beam of the flashlight.", 
          "video": "https://www.youtube.com/embed/wA_A0vjQbaU"
          }, 
          {
          "word": "Beanbag", 
          "synonym": "Chairs & seats.", 
          "example": "The beanbags are only retrieved after all six are thrown.", 
          "video": "https://www.youtube.com/embed/7TDY2_jHHRk"
          }, 
          {
          "word": "Beanie", 
          "synonym": "Hats & scarves.", 
          "example": "He was a recognizable character, with chubby cheeks and a trademark beanie cap.", 
          "video": "https://www.youtube.com/embed/oXQcIpDDSUI"
          }, 
          {
          "word": "Bear down on sb/sth", 
          "synonym": "Heel, hot.", 
          "example": "I looked up to see the car bearing down on me.", 
          "video": "https://www.youtube.com/embed/SBdAAZ17X"
          }, 
          {
          "word": "Bear fruit", 
          "synonym": "", 
          "example": "After years of hard work, his research finally began to bear fruit.  ", 
          "video": ""
          }, 
          {
          "word": "Bear fruit", 
          "synonym": "", 
          "example": "After years of hard work, his research finally began to bear fruit.  ", 
          "video": ""
          }, 
          {
          "word": "Bear in on/upon", 
          "synonym": "Understanding and comprehending", 
          "example": "Suddenly it was borne in on him that he was becoming too old to start a new career.", 
          "video": "https://www.youtube.com/embed/ahoNDZQxFws"
          }, 
          {
          "word": "Bear on sth", 
          "synonym": "Affecting and influencing.", 
          "example": "I don't see how that information bears on this case.", 
          "video": ""
          }, 
          {
          "word": "Bear out", 
          "synonym": "Proving and disproving.", 
          "example": "His version of events just isn't borne out by the facts.", 
          "video": "https://www.youtube.com/embed/CSbzoHxnYyI"
          }, 
          {
          "word": "Bear sb/sth out", 
          "synonym": "Proving and disproving.", 
          "example": "His version of events just isn't borne out by the facts.", 
          "video": ""
          }, 
          {
          "word": "Bear the brunt", 
          "synonym": "", 
          "example": "When things go wrong, his assistant always has to bear the brunt of his anger.", 
          "video": ""
          }, 
          {
          "word": "Bear up", 
          "synonym": "Coping and not coping.", 
          "example": "'How has she been since the funeral?' 'Oh, she's bearing up.'", 
          "video": "https://www.youtube.com/embed/I8JQt_w1pbc"
          }, 
          {
          "word": "Bear with a sore head", 
          "synonym": "", 
          "example": "I wouldn’t try to start a conversation with Nancy she is a like a bear with a sore head.", 
          "video": ""
          }, 
          {
          "word": "Bear with sb", 
          "synonym": "Tolerating and enduring.", 
          "example": "If you'll just bear with me for a moment, I'll find you a copy of the drawings.", 
          "video": "https://www.youtube.com/embed/cVItOMcgRvA"
          }, 
          {
          "word": "Bear with", 
          "synonym": "Tolerating and enduring.", 
          "example": "If you'll just bear with me for a moment, I'll find you a copy of the drawings.", 
          "video": "https://www.youtube.com/embed/kG_855QabwQ"
          }, 
          {
          "word": "Bear/ keep in mind", 
          "synonym": "", 
          "example": "Bear in mind  that no food will be served on board.", 
          "video": "https://www.youtube.com/embed/kngJQ9DpAgs?t=5s"
          }, 
          {
          "word": "Beard the lion in his den", 
          "synonym": "", 
          "example": "A risk very often doesn’t turn out well, but if you don’t face it and beard the lion in his den, you will never achieve the success you truly desire.", 
          "video": ""
          }, 
          {
          "word": "Beat a path to sbís door", 
          "synonym": "Acquisitive, ambitious.", 
          "example": "She was a successful lawyer and had clients beating a path to her door.", 
          "video": ""
          }, 
          {
          "word": "Beat a retreat", 
          "synonym": "Running away and escaping.", 
          "example": "When we saw the police arriving we beat a hasty retreat.", 
          "video": "https://www.youtube.com/embed/Th6ZF5I0DlQ"
          }, 
          {
          "word": "Beat a retreat.", 
          "synonym": "", 
          "example": "When we saw the police arriving we beat a hasty retreat.", 
          "video": ""
          }, 
          {
          "word": "Beat black and blue", 
          "synonym": "", 
          "example": "The passenger was beaten black and blue by a gang of thugs.", 
          "video": ""
          }, 
          {
          "word": "Beat down.", 
          "synonym": "", 
          "example": "The tropical sun beat down on them mercilessly.", 
          "video": "https://www.youtube.com/embed/LUadW5siovU"
          }, 
          {
          "word": "Beat off.", 
          "synonym": "", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Beat sb at their own game", 
          "synonym": "Winning and defeating.", 
          "example": "Jean knew that if she matched the new store's discount she would keep all her customers and beat the new competitors at their own game .", 
          "video": ""
          }, 
          {
          "word": "Beat sb hollow", 
          "synonym": "Winning and defeating.", 
          "example": "We played my brother's school at basketball and beat them hollow.", 
          "video": "https://www.youtube.com/embed/yj3eB6h_22A"
          }, 
          {
          "word": "Beat sb to a jelly", 
          "synonym": "Hitting and beating.", 
          "example": "They've threatened to beat him to a jelly if he doesn't repay the money.", 
          "video": ""
          }, 
          {
          "word": "Beat sb to it", 
          "synonym": "", 
          "example": "Paul beat me by three games to two .", 
          "video": ""
          }, 
          {
          "word": "Beat sbís brain out", 
          "synonym": "Hitting and beating.", 
          "example": "She threatened to beat my brains out.", 
          "video": "https://www.youtube.com/embed/TTFQKisUJY4"
          }, 
          {
          "word": "Beat somebody down.", 
          "synonym": "", 
          "example": "They tried to beat us down on the price, but we remained firm.", 
          "video": "https://www.youtube.com/embed/LUadW5siovU"
          }, 
          {
          "word": "Beat somebody off.", 
          "synonym": "", 
          "example": "She beat off her attacker by hitting him with her handbag.", 
          "video": ""
          }, 
          {
          "word": "Beat somebody/something back.", 
          "synonym": "", 
          "example": "Riot police beat back the crowds of demonstrators.", 
          "video": ""
          }, 
          {
          "word": "Beat the rap", 
          "synonym": "Accuse, acquit.", 
          "example": "With the right lawyer, you can definitely beat the rap and avoid any jail time.", 
          "video": "https://www.youtube.com/embed/HKr"
          }, 
          {
          "word": "Beat your chest", 
          "synonym": "Expressing and showing feelings.", 
          "example": "There's no point in beating your breast about losing the money", 
          "video": "https://www.youtube.com/embed/b2YL7xr"
          }, 
          {
          "word": "Beat.", 
          "synonym": "", 
          "example": "'I'm beat I need an hour or so to rest.î", 
          "video": "https://www.youtube.com/embed/iIYZrgsYQK0"
          }, 
          {
          "word": "Beat/knock the living daylights", 
          "synonym": "", 
          "example": "If I catch you stealing again I'll beat the daylights out of you!", 
          "video": "https://www.youtube.com/embed/GLxFh9WBDrY up to 0:16 second"
          }, 
          {
          "word": "Beatific.", 
          "synonym": "", 
          "example": "The angels in the painting have beatific smiles.", 
          "video": "https://www.youtube.com/embed/ST9ehggP0Mo"
          }, 
          {
          "word": "Beauteous.", 
          "synonym": "", 
          "example": "She is very powerful, with a beauteous appearance masking a fearsome treelike form.", 
          "video": "https://www.youtube.com/embed/PS6P8QQaWD4"
          }, 
          {
          "word": "Beauty is in the eye of the beholder.", 
          "synonym": "", 
          "example": "I canít believe he finally settled for that ugly little car. And he loves it too! Beauty is in the eye of the beholder.", 
          "video": "https://www.youtube.com/embed/FBOdZ9P72pY"
          }, 
          {
          "word": "Beauty is only skin deep.", 
          "synonym": "", 
          "example": "Of course that gorgeous model didn't tip you beauty is only skin deep, after all.", 
          "video": "https://www.youtube.com/embed/WqdAQ"
          }, 
          {
          "word": "Beaver away.", 
          "synonym": "", 
          "example": "She has been beavering away at that essay for hours.", 
          "video": "https://www.youtube.com/embed/vrIxysZ1tM4"
          }, 
          {
          "word": "Beaver.", 
          "synonym": "", 
          "example": "Beavers build dams walls of sticks and earth across rivers.", 
          "video": "https://www.youtube.com/embed/Q"
          }, 
          {
          "word": "Becalmed.", 
          "synonym": "", 
          "example": "We mustn't show more lights than we can help, when becalmed at night so near the land.", 
          "video": "https://www.youtube.com/embed/1VErvZ9ox_c"
          }, 
          {
          "word": "Beck.", 
          "synonym": "", 
          "example": "Here we found the beck running deeply and swiftly along a channel which appeared to have been hewn out expressly for it, but on closer inspection we found it quite a natural formation.", 
          "video": "https://www.youtube.com/embed/vmwMEycLZmI"
          }, 
          {
          "word": "Beckon.", 
          "synonym": "", 
          "example": "The customs official beckoned the woman to his counter.", 
          "video": "https://www.youtube.com/embed/NE8Rm4fuQDc"
          }, 
          {
          "word": "Bed and breakfast.", 
          "synonym": "", 
          "example": "There are several bed and breakfast places near the station.", 
          "video": "https://www.youtube.com/embed/6Tg9ae9Ew4E"
          }, 
          {
          "word": "Bed down.", 
          "synonym": "", 
          "example": "I bedded down on the couch for the night.", 
          "video": "https://www.youtube.com/embed/IRuYG68XEh4"
          }, 
          {
          "word": "Bed down.", 
          "synonym": "", 
          "example": "It did not take the procedure long to bed down.", 
          "video": "https://www.youtube.com/embed/IRuYG68XEh4"
          }, 
          {
          "word": "Bed of nails.", 
          "synonym": "", 
          "example": "Taking care of her sick brother all these years has been a bed of nails for her.", 
          "video": ""
          }, 
          {
          "word": "Bed of roses.", 
          "synonym": "", 
          "example": "Making money is not a bed of roses, so wake up early and go to work.", 
          "video": ""
          }, 
          {
          "word": "Bedaub.", 
          "synonym": "", 
          "example": "The child's face was bedaubed with chocolate.", 
          "video": "https://www.youtube.com/embed/UCasJx_Y7fI"
          }, 
          {
          "word": "Bedeck.", 
          "synonym": "", 
          "example": "The room was bedecked with flowers.", 
          "video": "https://www.youtube.com/embed/di90VU0WBr4"
          }, 
          {
          "word": "Bedevil.", 
          "synonym": "", 
          "example": "Ever since I started playing tennis, I've been bedeviled by back pains.", 
          "video": "https://www.youtube.com/embed/NmF3OR"
          }, 
          {
          "word": "Bedfellow.", 
          "synonym": "", 
          "example": "The priest and the politician made strange/odd/unlikely bedfellows in their campaign for peace.", 
          "video": "https://www.youtube.com/embed/U4vcoUsyJNk"
          }, 
          {
          "word": "Bedlam.", 
          "synonym": "", 
          "example": "It was bedlam at the football stadium after the match was suspended.", 
          "video": "https://www.youtube.com/embed/QoUAB235yPY"
          }, 
          {
          "word": "Bedpost.", 
          "synonym": "", 
          "example": "I dream about it nights and wake up with my arms around the bedpost.", 
          "video": "https://www.youtube.com/embed/P8ttxIt4z"
          }, 
          {
          "word": "Bedraggled.", 
          "synonym": "Wet, Dirty, and Untidy.", 
          "example": "On his way he met an old woman with a shawl around her, a bedraggled dress and wet feet.", 
          "video": "https://www.youtube.com/embed/RbUEEI3BPNA"
          }, 
          {
          "word": "Bedridden.", 
          "synonym": "", 
          "example": "His aunt was 93 and bedridden.", 
          "video": "https://www.youtube.com/embed/Zf38"
          }, 
          {
          "word": "Bedside manner.", 
          "synonym": "", 
          "example": "He has a very good bedside manner.", 
          "video": "https://www.youtube.com/embed/ubGt_X17KOs"
          }, 
          {
          "word": "Bedsore.", 
          "synonym": "", 
          "example": "After several difficult days, Isaacís bedsores began healing.", 
          "video": "https://www.youtube.com/embed/3IZEsfXnr5o"
          }, 
          {
          "word": "Bedspread.", 
          "synonym": "", 
          "example": "Sheets and bedspreads edged with lace!", 
          "video": "https://www.youtube.com/embed/WEHQ"
          }, 
          {
          "word": "Bedstead.", 
          "synonym": "", 
          "example": "A bed had been made on a bedstead for the countess only.", 
          "video": "https://www.youtube.com/embed/ZvvLhVFiG18"
          }, 
          {
          "word": "Bee in one’s bonnet", 
          "synonym": "", 
          "example": "Michelle can’t stand the new neighbour as she has a bee in her bonnet about their lifestyle.", 
          "video": ""
          }, 
          {
          "word": "Beef something up.", 
          "synonym": "", 
          "example": "We need to find some new players to beef up the team.", 
          "video": "https://www.youtube.com/embed/AkZbcOX1iY0"
          }, 
          {
          "word": "Beef up", 
          "synonym": "Augmenting and supplementing.", 
          "example": "The company has plans to beef up its production.", 
          "video": "https://www.youtube.com/embed/EPMIFMIXF4g"
          }, 
          {
          "word": "Beef.", 
          "synonym": "", 
          "example": "My main beef about the job is that I have to work on Saturdays.", 
          "video": "https://www.youtube.com/embed/YcfXtRt9JP0"
          }, 
          {
          "word": "Beef.", 
          "synonym": "Strength, Power, or Force.", 
          "example": "https://www.youtube.com/embed/YcfXtRt9JP0", 
          "video": ""
          }, 
          {
          "word": "Beefy.", 
          "synonym": "", 
          "example": "A beefy football player.", 
          "video": "https://www.youtube.com/embed/wqcvlhINcs0"
          }, 
          {
          "word": "Beetle", 
          "synonym": "", 
          "example": "A knock brought a black", 
          "video": "https://www.youtube.com/embed/ReRvLboi1lE"
          }, 
          {
          "word": "Before you can/could say Jack Robinson", 
          "synonym": "", 
          "example": "I put the dish of food on the floor, and before you could say Jack Robinson, the dog had eaten it.", 
          "video": ""
          }, 
          {
          "word": "Before/after dark", 
          "synonym": "Darkness , becoming dark.", 
          "example": "It isn't safe to leave the house after dark.", 
          "video": "https://www.youtube.com/embed/1nz8xRN4azE"
          }, 
          {
          "word": "Behind bars", 
          "synonym": "", 
          "example": "He's  spent most of his  life  behind  bars.", 
          "video": "https://www.youtube.com/embed/W0DH4U4NJmI"
          }, 
          {
          "word": "Behind closed doors", 
          "synonym": "", 
          "example": "The matter was discussed behind closed doors.", 
          "video": "https://www.youtube.com/embed/UCWLTW1VOTI"
          }, 
          {
          "word": "Behind the scenes", 
          "synonym": "Secrecy, Privacy", 
          "example": "A lot of hard work has been going on behind the scenes.", 
          "video": "https://thumb7.shutterstock.com/display_pic_with_logo/167744610/1042050787/stock"
          }, 
          {
          "word": "Behind the times", 
          "synonym": "", 
          "example": "Jane doesn't have a mobile phone.  She's completely behind the times.", 
          "video": "https://www.youtube.com/embed/yYByQBmvo8"
          }, 
          {
          "word": "Below decks", 
          "synonym": "", 
          "example": "When the storm hit us we all went below decks for safety.", 
          "video": ""
          }, 
          {
          "word": "Below the belt", 
          "synonym": "", 
          "example": "His comment about Manfred’s handicap was below the belt.", 
          "video": ""
          }, 
          {
          "word": "Below the belt", 
          "synonym": "", 
          "example": "Politicians sometimes use personal information to hit their rivals below the belt.", 
          "video": "https://www.youtube.com/embed/k89MdLONeOw"
          }, 
          {
          "word": "Below/under par", 
          "synonym": "", 
          "example": "I was feeling under par.", 
          "video": ""
          }, 
          {
          "word": "Bend over backwards", 
          "synonym": "", 
          "example": "Mann insisted that he bent over backwards to be objective in presenting the story.", 
          "video": "https://www.youtube.com/embed/HYbiOhxpatg?t=3s"
          }, 
          {
          "word": "Bent out of shape", 
          "synonym": "", 
          "example": "Don't get bent out of shape if you're delayed.  We'll wait for you.", 
          "video": ""
          }, 
          {
          "word": "Beside yourself with emotion", 
          "synonym": "", 
          "example": "He was beside himself with grief when he lost his son.", 
          "video": ""
          }, 
          {
          "word": "Bet your bottom dollar", 
          "synonym": "", 
          "example": "Jack is very punctual.  You can bet your bottom dollar he'll be here at 9 o'clock on the dot.", 
          "video": "https://www.youtube.com/embed/FzsL8JuGGzk"
          }, 
          {
          "word": "Between a rock and a hard place", 
          "synonym": "bind, difficulty, no", 
          "example": "I canít make up my mind whose side I am on; Iím caught between a rock and a hard place.", 
          "video": "https://www.youtube.com/embed/Ju1N14SXrjM"
          }, 
          {
          "word": "Between the devil and the deep sea", 
          "synonym": "", 
          "example": "Taking the train at night or the bus is like choosing between the devil and the deep sea.", 
          "video": ""
          }, 
          {
          "word": "Between you, me, and the bedpost.", 
          "synonym": "", 
          "example": "I overheard the boss talking to her secretary last night and just between you, me, and the bedpost she's giving the promotion to George after all.", 
          "video": ""
          }, 
          {
          "word": "Beware", 
          "synonym": "", 
          "example": "Beware of the dog.", 
          "video": "https://www.youtube.com/embed/7T"
          }, 
          {
          "word": "Beyond Description", 
          "synonym": "painting, Depiction", 
          "example": "The death and destruction were beyond description.", 
          "video": "https://www.youtube.com/embed/hYhlpPP"
          }, 
          {
          "word": "Beyond the ball", 
          "synonym": "", 
          "example": "I didn't sleep well last night and I'm not really on the ball today.", 
          "video": ""
          }, 
          {
          "word": "Beyond wildest dream", 
          "synonym": "", 
          "example": "Sarah is beyond my wildest dMarrying ream but here we are getting hitched.", 
          "video": ""
          }, 
          {
          "word": "Bias", 
          "synonym": "", 
          "example": "Reporters must be impartial and not show political bias.", 
          "video": "https://www.youtube.com/embed/Y_HtcDhWY9g"
          }, 
          {
          "word": "Big cheese", 
          "synonym": "", 
          "example": "Tom's father is a big cheese in the oil industry.", 
          "video": "https://www.youtube.com/embed/tacoPZotG3Q"
          }, 
          {
          "word": "Big fish in a small pond", 
          "synonym": "", 
          "example": "Example: He could get a job with a big company but he enjoys being a big fish in a small pond.", 
          "video": "https://www.youtube.com/embed/vTnVo351"
          }, 
          {
          "word": "Bilingual", 
          "synonym": "Multilingual, polyglot", 
          "example": "The staff also seem reluctant to help travelers with their children and it would help if the staff were bilingual.", 
          "video": "https://www.youtube.com/embed/TZMO"
          }, 
          {
          "word": "Bird brain", 
          "synonym": "Airhead", 
          "example": "Her brother's a real birdbrain.", 
          "video": "https://www.youtube.com/embed/QPiexEs04Cs"
          }, 
          {
          "word": "Bisect", 
          "synonym": "Disunite.", 
          "example": "The new road will bisect the town.", 
          "video": "https://www.youtube.com/embed/uh5JT4c2SEI"
          }, 
          {
          "word": "Bishop", 
          "synonym": "Priest.", 
          "example": "The bishop's speech has prompted an angry response from both political parties.", 
          "video": "https://www.youtube.com/embed/F5eonb_JjE8?t=6s"
          }, 
          {
          "word": "Bison", 
          "synonym": "Buffalo", 
          "example": "When the white men came they hunted the bison with guns, and soon killed them off.", 
          "video": "https://www.youtube.com/embed/xsfWmwDU17Y"
          }, 
          {
          "word": "Bite head off", 
          "synonym": "", 
          "example": "I don’t know why he bit my head off over such a trivial thing.", 
          "video": ""
          }, 
          {
          "word": "Bite into something", 
          "synonym": "Subside.", 
          "example": "People are worried about inflation biting into their savings and investments.", 
          "video": "https://www.youtube.com/embed/eQQwbSjx"
          }, 
          {
          "word": "Bite off more than you can chew", 
          "synonym": "go to extremes, go to far, overdo", 
          "example": "We bit off more than we could chew in our original reform proposals.", 
          "video": "https://www.youtube.com/embed/0ofELc83fAA"
          }, 
          {
          "word": "Bite sized", 
          "synonym": "Mini", 
          "example": "Cut the cheese into bite", 
          "video": "https://www.youtube.com/embed/P2GYsF2xuO0"
          }, 
          {
          "word": "Bite something back", 
          "synonym": "Gob", 
          "example": "Susan bit back the words she would like to have said.", 
          "video": ""
          }, 
          {
          "word": "Bite the bullet", 
          "synonym": "Courageous.", 
          "example": "I hate going to the dentist, but I'll just have to bite the bullet.", 
          "video": "https://www.youtube.com/embed/wVvssFCQOlQ"
          }, 
          {
          "word": "Bite the dust", 
          "synonym": "To die", 
          "example": "The soldier bit the dust after a very long fight and even at that he managed to take many enemy soldiers with him.", 
          "video": "https://www.youtube.com/embed/qz3"
          }, 
          {
          "word": "Bite your tongue", 
          "synonym": "", 
          "example": "I wanted to tell him exactly what I thought of him, but I had to bite my tongue.", 
          "video": "https://www.youtube.com/embed/3OHu45yXpo0"
          }, 
          {
          "word": "Black and white.", 
          "synonym": "", 
          "example": "The press has been presenting the conflict in black", 
          "video": ""
          }, 
          {
          "word": "Black eye", 
          "synonym": "Blemishes.", 
          "example": "He had a fight at school and came home with a black eye.", 
          "video": "https://www.youtube.com/embed/4gMRa"
          }, 
          {
          "word": "Black humor", 
          "synonym": "", 
          "example": "Sorry indeed would be anyone's plight who should encounter you in this black humor.", 
          "video": "https://www.youtube.com/embed/34cW7O9PQSE"
          }, 
          {
          "word": "Black mood", 
          "synonym": "", 
          "example": "Try cheering up Nancy as she is in a black mood.", 
          "video": ""
          }, 
          {
          "word": "Black something out", 
          "synonym": "Hide, Cover", 
          "example": "In the TV interview, they blacked out the victim's face.", 
          "video": "https://www.youtube.com/embed/5w6QSe9AvB8"
          }, 
          {
          "word": "Black tie event.", 
          "synonym": "", 
          "example": "I need to know if it's going to be a casual get", 
          "video": "https://www.youtube.com/embed/ecudxDHv1uk"
          }, 
          {
          "word": "Black widow", 
          "synonym": "Arachnids.", 
          "example": "She got out the same costume she wore last year, which is a black widow spider.", 
          "video": "https://www.youtube.com/embed/R_aDj"
          }, 
          {
          "word": "Blame worthy", 
          "synonym": "Guilty", 
          "example": "But I doubt not you are both blameworthy.", 
          "video": "https://www.youtube.com/embed/L59e0Pb7U_Q"
          }, 
          {
          "word": "Blanch", 
          "synonym": "To boil", 
          "example": "Blanched almonds", 
          "video": "https://www.youtube.com/embed/p8Zs_gc0DWc"
          }, 
          {
          "word": "Bland", 
          "synonym": "Tasteless", 
          "example": "I find chicken a little bland.", 
          "video": "https://www.youtube.com/embed/sKPLMiP8frw"
          }, 
          {
          "word": "Blandishments", 
          "synonym": "Reassuring", 
          "example": "She was impervious to his blandishments.", 
          "video": "https://www.youtube.com/embed/MbilldBeBbI"
          }, 
          {
          "word": "Blank cheque", 
          "synonym": "", 
          "example": "Tom was given a blank cheque and told to negotiate the best deal possible.", 
          "video": "https://www.youtube.com/embed/J36GG6cu07A from 0:14 second"
          }, 
          {
          "word": "Blare", 
          "synonym": "Noisy", 
          "example": "The loudspeakers blared across the square.", 
          "video": "https://www.youtube.com/embed/rvvYM5iiCCk"
          }, 
          {
          "word": "Blarney", 
          "synonym": "Flattery", 
          "example": "Don't listen to any of his blarney!", 
          "video": "https://www.youtube.com/embed/8o"
          }, 
          {
          "word": "Blaspheme", 
          "synonym": "Swearing", 
          "example": "He did not curse or blaspheme.", 
          "video": "https://www.youtube.com/embed/8"
          }, 
          {
          "word": "Blast", 
          "synonym": "Launch", 
          "example": "Five seconds to blast", 
          "video": "https://www.youtube.com/embed/TiR99qmU_x0"
          }, 
          {
          "word": "Blatant", 
          "synonym": "Apparent.", 
          "example": "The whole episode was a blatant attempt to gain publicity.", 
          "video": "https://www.youtube.com/embed/PX5HNLpDaxQ"
          }, 
          {
          "word": "Blather", 
          "synonym": "Blable", 
          "example": "What on earth are you blathering on about?", 
          "video": "https://www.youtube.com/embed/vcMcvuLMOyc"
          }, 
          {
          "word": "Blaze a trail", 
          "synonym": "Surreal", 
          "example": "Le Corbusier blazed a trail in architecture.", 
          "video": "https://www.youtube.com/embed/W2cPY0CIlkk"
          }, 
          {
          "word": "Blaze", 
          "synonym": "Burning", 
          "example": "The sun was blazing down that afternoon.", 
          "video": "https://www.youtube.com/embed/1YtC8"
          }, 
          {
          "word": "Bleak", 
          "synonym": "Harsh", 
          "example": "The house stands on a bleak, windswept hilltop.", 
          "video": "https://www.youtube.com/embed/xfD"
          }, 
          {
          "word": "Bleary", 
          "synonym": "Blurry", 
          "example": "To be bleary", 
          "video": "https://www.youtube.com/embed/A6c8qaBsrxU"
          }, 
          {
          "word": "Bleat", 
          "synonym": "Whimper", 
          "example": "The lamb bleated as I approached.", 
          "video": "https://www.youtube.com/embed/Ywu_TbPik_g"
          }, 
          {
          "word": "Bleed somebody dry", 
          "synonym": "Bankrupt", 
          "example": "The West is bleeding poorer countries dry through interest payments on their debts.", 
          "video": "https://www.youtube.com/embed/QLO1QlFO1eY"
          }, 
          {
          "word": "Blemish", 
          "synonym": "Freckles", 
          "example": "The cream is supposed to prevent blemishes on the skin.", 
          "video": "https://www.youtube.com/embed/lBWn_yF2DKY"
          }, 
          {
          "word": "Blench", 
          "synonym": "Shock", 
          "example": "At the sight of the dead animal, Diana blenched.", 
          "video": "https://www.youtube.com/embed/IyvSQJvu5LM"
          }, 
          {
          "word": "Blend in/into something", 
          "synonym": "Mix", 
          "example": "We tried to blend into the crowd.", 
          "video": "We tried to blend into the crowd."
          }, 
          {
          "word": "Blend into the scenery", 
          "synonym": "Custom, Tradition, Conformity", 
          "example": "On the following day's journey, he was enthusiastic in blending into the scenery.", 
          "video": ""
          }, 
          {
          "word": "Blight", 
          "synonym": "Infestation", 
          "example": "The vines suffered blight and disease.", 
          "video": "https://www.youtube.com/embed/FtEv52KP76A"
          }, 
          {
          "word": "Blind manís buff", 
          "synonym": "Blind manís bluff", 
          "example": "I had always known the childrenís game as blind manís bluff and so was surprised to find a chapter in a book Iím reading titled blind manís buff", 
          "video": "https://www.youtube.com/embed/39SZYZfkjbY"
          }, 
          {
          "word": "Blind side", 
          "synonym": "Attack by surprise.", 
          "example": "A punch delivered on the referee's blind side.", 
          "video": "https://www.youtube.com/embed/7AdofW6h"
          }, 
          {
          "word": "Blind somebody with science", 
          "synonym": "Puzzle", 
          "example": "As you plan your talk, be careful not to blind the audience with science.", 
          "video": "https://www.youtube.com/embed/lnGVxfKXu94"
          }, 
          {
          "word": "Blind spot", 
          "synonym": "Dead spot, unseen area.", 
          "example": "The rear", 
          "video": "https://www.youtube.com/embed/nhJLQH4goj8 up to 0:17 second"
          }, 
          {
          "word": "Blind", 
          "synonym": "Unsighted, sightless", 
          "example": "He went to a school for the blind.", 
          "video": "https://www.youtube.com/embed/U3ZRum098QM"
          }, 
          {
          "word": "Blindfold", 
          "synonym": "Screen, covering", 
          "example": "The report says prisoners were often kept blindfolded.", 
          "video": "https://www.youtube.com/embed/EMC8jtExlK8"
          }, 
          {
          "word": "Bliss", 
          "synonym": "Pleasure", 
          "example": "Lying on a  sunny beach is my idea of sheer bliss.", 
          "video": "https://www.youtube.com/embed/g8CbZ3tye9o"
          }, 
          {
          "word": "Blister", 
          "synonym": "Blemishes", 
          "example": "New shoes always give me blisters.", 
          "video": "https://www.youtube.com/embed/3uegsDwithU up to 0:16 second"
          }, 
          {
          "word": "Blistering", 
          "synonym": "Annoyed", 
          "example": "No one likes to hear blistering remarks.", 
          "video": ""
          }, 
          {
          "word": "Blistering", 
          "synonym": "Burning", 
          "example": "We went out in the blistering heat.", 
          "video": ""
          }, 
          {
          "word": "Blistering", 
          "synonym": "Fleet", 
          "example": "The runners set off at a blistering pace.", 
          "video": ""
          }, 
          {
          "word": "Blitz", 
          "synonym": "Bombardment", 
          "example": "The German air raids that occurred during the war in the 1940's were an example of a blitz.", 
          "video": "https://www.youtube.com/embed/1Iv9VhWaSz8  up to 0:11 second"
          }, 
          {
          "word": "Blitz", 
          "synonym": "Momentarily", 
          "example": "The car was launched with a massive media/advertising blitz, involving newspapers, magazines, television and radio.", 
          "video": ""
          }, 
          {
          "word": "Blizzard", 
          "synonym": "Snowstorm", 
          "example": "We once got struck in a blizzard for six hours.", 
          "video": "https://www.youtube.com/embed/UkuAEfACFCQ up to 0:11 second"
          }, 
          {
          "word": "Bloat", 
          "synonym": "", 
          "example": "If I eat it, my stomach bloats up.", 
          "video": "https://www.youtube.com/embed/3vyuiYXURqQ from 0:15 second"
          }, 
          {
          "word": "Blob", 
          "synonym": "Bubble", 
          "example": "While drawing, a blob of paint fall on the paper.", 
          "video": "https://www.youtube.com/embed/IoObqHHeVdo up to 0:15 second"
          }, 
          {
          "word": "Block and tackle", 
          "synonym": "Machine", 
          "example": "Block and tackle is a coomon device that we can find in construction sites.", 
          "video": "https://www.youtube.com/embed/ErJFiCis1MEup to 0:13 second"
          }, 
          {
          "word": "Block off", 
          "synonym": "Closing and blocking.", 
          "example": "The area was blocked off during the demonstration.", 
          "video": "https://www.youtube.com/embed/oVTfyCyB74Q"
          }, 
          {
          "word": "Block sth in", 
          "synonym": "Parked", 
          "example": "Another car had parked behind me and blocked me in.", 
          "video": ""
          }, 
          {
          "word": "Block sth off", 
          "synonym": "Barricade", 
          "example": "All the roads out of the town had been blocked off by the police.", 
          "video": ""
          }, 
          {
          "word": "Block sth out", 
          "synonym": "Impede", 
          "example": "The tree outside  the window blocks out the sun.", 
          "video": ""
          }, 
          {
          "word": "Block sth up", 
          "synonym": "Jam", 
          "example": "In autumn, leaves block the drains up.", 
          "video": ""
          }, 
          {
          "word": "Blockade", 
          "synonym": "Invade", 
          "example": "The Soviet blockade of Berlin was lifted in May 1949.", 
          "video": "https://www.youtube.com/embed/NId25a7WKok up to 0:15 second"
          }, 
          {
          "word": "Blockage", 
          "synonym": "Barricade", 
          "example": "His death was caused by a blockage in one of his arteries.", 
          "video": "https://www.youtube.com/embed/x60UTsgJEpo"
          }, 
          {
          "word": "Blockbuster", 
          "synonym": "", 
          "example": "The TV series was a blockbuster.", 
          "video": ""
          }, 
          {
          "word": "Blockbuster", 
          "synonym": "", 
          "example": "The TV series was a blockbuster.", 
          "video": ""
          }, 
          {
          "word": "Blood and guts", 
          "synonym": "Aggressive", 
          "example": "There was too much blood and guts in the movie for my liking.", 
          "video": "https://www.youtube.com/embed/IRCn9R4lxJo"
          }, 
          {
          "word": "Blood is thicker than water", 
          "synonym": "", 
          "example": "When you get into trouble, usually your family will be the ones to bail you out, not your friends. After all, blood is thicker than water.", 
          "video": "https://www.youtube.com/embed/hNZJpA2_gw0"
          }, 
          {
          "word": "Blood, sweat and tears", 
          "synonym": "", 
          "example": "My father made this company from the ground up with his blood, sweat and tears.", 
          "video": ""
          }, 
          {
          "word": "Bloodbath", 
          "synonym": "Violent", 
          "example": "Is there nothing that the outside world can do to prevent a bloodbath?", 
          "video": "https://www.youtube.com/embed/F0ZntEXX2R4 up to 0:15 second"
          }, 
          {
          "word": "Bloodcurdling", 
          "synonym": "Frightening", 
          "example": "The mother told a bloodcurdling story to her son.", 
          "video": "https://www.youtube.com/embed/y2VoodxeIC8"
          }, 
          {
          "word": "Bloodhound", 
          "synonym": "Canines", 
          "example": "My brother once had a bloodhound as his pet.", 
          "video": ""
          }, 
          {
          "word": "Bloodless", 
          "synonym": "Expressionless", 
          "example": "He is a bloodless person.", 
          "video": "https://www.youtube.com/embed/afh_BREEHqQ from 0:13 second"
          }, 
          {
          "word": "Bloodshed", 
          "synonym": "Violent", 
          "example": "The army was brought in to try to prevent further bloodshed.", 
          "video": "https://www.youtube.com/embed/j8Z6O71H0fo up to 0:13 second"
          }, 
          {
          "word": "Bloodshot", 
          "synonym": "Reddish", 
          "example": "Dulce's eyes were bloodshot and her cheeks were covered with tears", 
          "video": "https://www.youtube.com/embed/HRnOJZG8MG4"
          }, 
          {
          "word": "Bloodstain", 
          "synonym": "Blood", 
          "example": "He had seen Lydia's bloodstained apartment and witnessed its disrupted condition.", 
          "video": "https://www.youtube.com/embed/K_KQB3Tpv4E"
          }, 
          {
          "word": "Blot your copybook", 
          "synonym": "Damaging reputation", 
          "example": "I really blotted my copybook by missing the meeting.", 
          "video": "https://www.youtube.com/embed/3H8klcCphvQ"
          }, 
          {
          "word": "Blotch", 
          "synonym": "Blemishes", 
          "example": "Her face was covered in purple blotches.", 
          "video": "https://www.youtube.com/embed/eH37PSzt9EM"
          }, 
          {
          "word": "Blow a fuse", 
          "synonym": "", 
          "example": "I wouldn’t touch or move things in his room, if he finds out he will blow a fuse.", 
          "video": ""
          }, 
          {
          "word": "Blow a gasket", 
          "synonym": "", 
          "example": "When I meddled with his day planner he blew a gasket!", 
          "video": ""
          }, 
          {
          "word": "Blow by blow", 
          "synonym": "Granular", 
          "example": "You'll have to tell me about your night out with Sam ñ I want a blow", 
          "video": "https://www.youtube.com/embed/CDNiD_"
          }, 
          {
          "word": "Blow hot and cold", 
          "synonym": "Ambivalent", 
          "example": "He's been blowing hot and cold about the trip to Brazil.", 
          "video": "https://www.youtube.com/embed/VOIOfsvoBvA"
          }, 
          {
          "word": "Blow over", 
          "synonym": "Blow up", 
          "example": "The storm raged all night but by morning it had blown over.", 
          "video": "https://www.youtube.com/embed/SlUWQllVwk0 from 0:10 to 0:12 second"
          }, 
          {
          "word": "Blow over", 
          "synonym": "Dim", 
          "example": "I thought that after a few days the argument would blow over.", 
          "video": "https://www.youtube.com/embed/SlUWQllVwk0 from 0:13 second"
          }, 
          {
          "word": "Blow sbís cover", 
          "synonym": "Revealing secrets", 
          "example": "One mistake could blow our agentís cover and ruin years of careful investigation.", 
          "video": ""
          }, 
          {
          "word": "Blow sbís lid", 
          "synonym": "Tempers get frayed", 
          "example": "My father will blow his lid when he sees what happened to the car.", 
          "video": ""
          }, 
          {
          "word": "Blow something/somebody out of the water", 
          "synonym": "Outscore", 
          "example": "They came to court with  fresh evidence that would, they said, blow the prosecution's case completely out of the water.", 
          "video": "https://www.youtube.com/embed/wahf0XPIjqw"
          }, 
          {
          "word": "Blow sth up", 
          "synonym": "Explode", 
          "example": "They blew the plane up on the ground with dynamite.", 
          "video": "https://www.youtube.com/embed/bhTMtCdhLPM up to 0:17 second"
          }, 
          {
          "word": "Blow sth up", 
          "synonym": "Inflate", 
          "example": "He asked for a small pump for blowing up balloons, while decorating the stage.", 
          "video": "https://www.youtube.com/embed/bhTMtCdhLPM from 0:19 second"
          }, 
          {
          "word": "Blow the cobwebs away", 
          "synonym": "High", 
          "example": "We went for a five", 
          "video": "https://www.youtube.com/embed/NG10HYf_k3I up to 1:01 second"
          }, 
          {
          "word": "Blow the whistle on sb/sth away", 
          "synonym": "Let the cat out of the bag.", 
          "example": "If you keep coming in late, I'm going to have to blow the whistle and report you to the department head.", 
          "video": ""
          }, 
          {
          "word": "Blow up in face", 
          "synonym": "", 
          "example": "The trip was difficult to organise, but it blew up in his face when the airline company went on strike.", 
          "video": ""
          }, 
          {
          "word": "Blow up in face", 
          "synonym": "", 
          "example": "The trip was difficult to organise, but it blew up in his face when the airline company went on strike.", 
          "video": ""
          }, 
          {
          "word": "Blow up", 
          "synonym": "Bolt, derecho.", 
          "example": "The expected blow", 
          "video": "https://www.youtube.com/embed/fXxzyRyHuZM"
          }, 
          {
          "word": "Blow up", 
          "synonym": "Go nuts.", 
          "example": "My dad blew up at me when he saw the bill.", 
          "video": ""
          }, 
          {
          "word": "Blow your mind", 
          "synonym": "", 
          "example": "The concert was so good, it blew my mind.", 
          "video": ""
          }, 
          {
          "word": "Blow your own trumpet", 
          "synonym": "Boasting", 
          "example": "Hollywood cameramen have good reason to blow their own trumpets.", 
          "video": "https://www.youtube.com/embed/ORMRtEwFalA up to 0:44 second"
          }, 
          {
          "word": "Blow your top", 
          "synonym": "", 
          "example": "Oh man, dad is going to blow his top when he sees that I wrecked his car!", 
          "video": ""
          }, 
          {
          "word": "Blow", 
          "synonym": "", 
          "example": "She used to blow dry her hair everyday in the morning, after bathing.", 
          "video": "https://www.youtube.com/embed/b238GfibYkY"
          }, 
          {
          "word": "Blow/bomb/wipe, something off the map", 
          "synonym": "Destroying, Demolishing", 
          "example": "A nuclear bomb could wipe the whole country off the map.", 
          "video": ""
          }, 
          {
          "word": "Blow/take the lid off  sth  / lift the lid on  sth", 
          "synonym": "", 
          "example": "In 1989 they started an investigation that was to blow the lid off corruption in the police force.", 
          "video": ""
          }, 
          {
          "word": "Blowfly", 
          "synonym": "Aphid", 
          "example": "The effect of blowflies on birds is a current research issue", 
          "video": "https://www.youtube.com/embed/lZV57B6jwMs"
          }, 
          {
          "word": "Blowsy", 
          "synonym": "Inelegant", 
          "example": "After racking his imagination, it occurred to him to bribe the blowsy waiting", 
          "video": "https://www.youtube.com/embed/xQt9lGf3TFo"
          }, 
          {
          "word": "Blowtorch", 
          "synonym": "Blowlamp", 
          "example": "A lot of cable to fit, and no blowtorch, and you tell me we can manage!", 
          "video": "https://www.youtube.com/embed/64odHz0ro5s"
          }, 
          {
          "word": "Blowy", 
          "synonym": "Windy", 
          "example": "Yesterday it was a blowy day.", 
          "video": "https://www.youtube.com/embed/VfPZpggGtp0"
          }, 
          {
          "word": "Blubber", 
          "synonym": "Adipose tissue", 
          "example": "Get some exercise and get rid of some of that blubber!", 
          "video": "https://www.youtube.com/embed/gN1z_tGwpQQ"
          }, 
          {
          "word": "Bludgeon", 
          "synonym": "Beat", 
          "example": "The two boys had been mercilessly bludgeoned to death.", 
          "video": "https://www.youtube.com/embed/mtVQr0pZ0SQ from 0:27 second to 0:37 second"
          }, 
          {
          "word": "Bludgeon", 
          "synonym": "Coerce", 
          "example": "The managers bludgeoned us into agreeing to the changes.", 
          "video": ""
          }, 
          {
          "word": "Bludgeon", 
          "synonym": "Cudgel", 
          "example": "Maces and spiked bludgeons were found in the hotel.", 
          "video": ""
          }, 
          {
          "word": "Blue chip company", 
          "synonym": "", 
          "example": "It's usually safe to invest in a blue chip company.", 
          "video": "https://www.youtube.com/embed/cIrbBR6kWLw from 0:08 second"
          }, 
          {
          "word": "Blue moon", 
          "synonym": "", 
          "example": "My sister lives in Alaska, so I only see her once in a blue moon.", 
          "video": "https://www.youtube.com/embed/FSkJvKzP4pA"
          }, 
          {
          "word": "Blue", 
          "synonym": "Impractical", 
          "example": "Stop your blue", 
          "video": "https://www.youtube.com/embed/I85MQEGleQI up to 0:10 second"
          }, 
          {
          "word": "Bluebell", 
          "synonym": "Harebell", 
          "example": "I would like to plant bluebell in my garden.", 
          "video": "https://www.youtube.com/embed/RvqMvXgR7EM"
          }, 
          {
          "word": "Blueprint", 
          "synonym": "Plan", 
          "example": "Their blueprint for economic reform has been finalized yesterday.", 
          "video": "https://www.youtube.com/embed/QyrxIeiV5"
          }, 
          {
          "word": "Bluff", 
          "synonym": "Deceit", 
          "example": "Tony seems to know  a lot about music, but sometimes I think he's only bluffing.", 
          "video": "https://www.youtube.com/embed/rKKpUPEiFfc"
          }, 
          {
          "word": "Blunder", 
          "synonym": "Error", 
          "example": "I made a blunder by getting his name wrong.", 
          "video": "https://www.youtube.com/embed/0SgWjBaFjLU"
          }, 
          {
          "word": "Blunt", 
          "synonym": "Dull", 
          "example": "Donít write with a blunt pencil at the exam hall.", 
          "video": "https://www.youtube.com/embed/crYZZp1j9NU up to 0:10 second"
          }, 
          {
          "word": "Blunt", 
          "synonym": "Straightforward", 
          "example": "I'll be blunt", 
          "video": ""
          }, 
          {
          "word": "Blur", 
          "synonym": "Unfocused", 
          "example": "If I don't wear my glasses, everything is just a blur.", 
          "video": "https://www.youtube.com/embed/KktAY_vyLDc"
          }, 
          {
          "word": "Blurb", 
          "synonym": "Brief", 
          "example": "The blurb on the back of the book says that it 'will touch your heart'.", 
          "video": "https://www.youtube.com/embed/BxzUi8ZA5lU"
          }, 
          {
          "word": "Blurt sth out", 
          "synonym": "Interrupt", 
          "example": "He blurted everything out about the baby, though we'd agreed to keep it a secret for a while.", 
          "video": "https://www.youtube.com/embed/zcM0fZVtXb4  up to 0:44 second"
          }, 
          {
          "word": "Bluster", 
          "synonym": "Rant", 
          "example": "You had no right to do it, no right at all,' he blustered.", 
          "video": "https://www.youtube.com/embed/_TGVy_lk_pw"
          }, 
          {
          "word": "Blustery", 
          "synonym": "Breeze", 
          "example": "Yesterday it was a blustery day.", 
          "video": "https://www.youtube.com/embed/Mh8Tw2MjLNY"
          }, 
          {
          "word": "Boar", 
          "synonym": "Swine", 
          "example": "Ever since that date, for five hundred years, a boar's head has graced the college table at Christmas", 
          "video": "https://www.youtube.com/embed/4PSuuT1Ed3I"
          }, 
          {
          "word": "Boast", 
          "synonym": "", 
          "example": "He didn't talk about his exam results in case people thought he was boasting.", 
          "video": "https://www.youtube.com/embed/izwnbwlZZkQ  up to 0:09 second"
          }, 
          {
          "word": "Boatyard", 
          "synonym": "Boathouse", 
          "example": "The yacht now lies in a boatyard at Lymington.", 
          "video": ""
          }, 
          {
          "word": "Bob", 
          "synonym": "Penny", 
          "example": "That coat cost me ten bob in 1956.", 
          "video": ""
          }, 
          {
          "word": "Bobble", 
          "synonym": "Frayed", 
          "example": "I've only worn this jumper twice, and it's already begun to bobble.", 
          "video": ""
          }, 
          {
          "word": "Bog down", 
          "synonym": "", 
          "example": "He's a big", 
          "video": "https://www.youtube.com/embed/he1mAqVpbqY"
          }, 
          {
          "word": "Boggle", 
          "synonym": "Confused", 
          "example": "My mind boggles at the amount of money they spend on food.", 
          "video": "https://www.youtube.com/embed/bs"
          }, 
          {
          "word": "Boggy", 
          "synonym": "Wetland", 
          "example": "All these places were boggy and impassable for horses.", 
          "video": "https://www.youtube.com/embed/ztPcbgrX_So"
          }, 
          {
          "word": "Bohemian", 
          "synonym": "Nomadic", 
          "example": "Marry soon, and settle down, we don't expect a life of Bohemian from you.", 
          "video": "https://www.youtube.com/embed/CQLM8e9WxKU"
          }, 
          {
          "word": "Boil down to sth", 
          "synonym": "Basis", 
          "example": "The problem boils down to one thing", 
          "video": ""
          }, 
          {
          "word": "Boil down to", 
          "synonym": "Being based on or depending on something.", 
          "example": "The problem boils down to one thing", 
          "video": "https://www.youtube.com/embed/7Mrub0jhYnk"
          }, 
          {
          "word": "Boil over", 
          "synonym": "Burn up", 
          "example": "That saucepan is boiling over.", 
          "video": "https://www.youtube.com/embed/UBJaK5r7nQs"
          }, 
          {
          "word": "Boil sth down", 
          "synonym": "Stripped down", 
          "example": "He had boiled down a lengthy report to just a few paragraphs.", 
          "video": ""
          }, 
          {
          "word": "Boil the ocean", 
          "synonym": "", 
          "example": "I expect you to do the job well but donít try to boil the ocean!", 
          "video": ""
          }, 
          {
          "word": "Boil the ocean", 
          "synonym": "", 
          "example": "I expect you to do the job well but don’t try to boil the ocean!", 
          "video": ""
          }, 
          {
          "word": "Boisterous", 
          "synonym": "Cacophony", 
          "example": "Boisterous children were playing in the field.", 
          "video": "https://www.youtube.com/embed/2bxSTTsG6tU up to 0:15 second "
          }, 
          {
          "word": "Bold", 
          "synonym": "Apparent", 
          "example": "They painted the kitchen in bold colors.", 
          "video": ""
          }, 
          {
          "word": "Bold", 
          "synonym": "Brave", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Bologna", 
          "synonym": "Mortadella", 
          "example": "She cooks bologna well.", 
          "video": ""
          }, 
          {
          "word": "Bolster", 
          "synonym": "Backbone", 
          "example": "More money is needed to bolster the industry.", 
          "video": "https://www.youtube.com/embed/LQ3w"
          }, 
          {
          "word": "Bolt from the blue", 
          "synonym": "", 
          "example": "The chairman's resignation came as a bolt from the blue.", 
          "video": "https://www.youtube.com/embed/dkAH3"
          }, 
          {
          "word": "Bolt", 
          "synonym": "Rush", 
          "example": "The thief tried to make a bolt for the exit.", 
          "video": ""
          }, 
          {
          "word": "Bomb", 
          "synonym": "Lost cause", 
          "example": "The play was a real bomb.", 
          "video": "https://www.youtube.com/embed/6tn2BiA5qcs from 0:15 second to up to 0:20 second"
          }, 
          {
          "word": "Bombard someone with something", 
          "synonym": "Cross", 
          "example": "The children bombarded her with questions.", 
          "video": ""
          }, 
          {
          "word": "Bombast", 
          "synonym": "Condescend", 
          "example": "His bombastic rant made her rethink her decision to go on a date with him.", 
          "video": "https://www.youtube.com/embed/9dR4fMHmLmI  from 0: 21 second"
          }, 
          {
          "word": "Bonanza", 
          "synonym": "Capital gains", 
          "example": "The rise  in house  prices meant that those who were selling enjoyed a bonanza.", 
          "video": "https://www.youtube.com/embed/7GfuM4cNmH0 from 0:10 second"
          }, 
          {
          "word": "Bone china", 
          "synonym": "Ceramics", 
          "example": "Linda was presented a boal china dinner set by her husband.", 
          "video": "https://www.youtube.com/embed/ih0Cx2kHcQ4"
          }, 
          {
          "word": "Bone dry", 
          "synonym": "Arid", 
          "example": "Bone dry lands are not preferable for cultivating crops.", 
          "video": "https://www.youtube.com/embed/X2SHxNY92Go"
          }, 
          {
          "word": "Bone idle", 
          "synonym": "Lazy", 
          "example": "He never does any exercise", 
          "video": "https://www.youtube.com/embed/4ro6Ub4RqQw up to 1:02"
          }, 
          {
          "word": "Bonfire", 
          "synonym": "Fire pit", 
          "example": "A bonfire was set up in the winter camp.", 
          "video": "https://www.youtube.com/embed/lyfh2BMeA9o from 0:12 second"
          }, 
          {
          "word": "Bongo", 
          "synonym": "Drums", 
          "example": "Joseph is an excellent bongo player.", 
          "video": ""
          }, 
          {
          "word": "Bonhomie", 
          "synonym": "Amiable", 
          "example": "There was a lot of cheerful bonhomie amongst  the people  on the trip.", 
          "video": "https://www.youtube.com/embed/HIfiXaXvCc0"
          }, 
          {
          "word": "Bonnet", 
          "synonym": "Hat", 
          "example": "Wearing bonnet was a style of 18th century.", 
          "video": "https://www.youtube.com/embed/H3RCjeLnVyo"
          }, 
          {
          "word": "Bonnet", 
          "synonym": "Inner tube", 
          "example": "I looked under the bonnet and clouds of smoke poured out.", 
          "video": ""
          }, 
          {
          "word": "Bony", 
          "synonym": "Anorexic", 
          "example": "She once had bony fingers.", 
          "video": "https://www.youtube.com/embed/DNaSWECIYrs"
          }, 
          {
          "word": "Boon companion", 
          "synonym": "Friend", 
          "example": "Raima is my boon companion.", 
          "video": ""
          }, 
          {
          "word": "Boon", 
          "synonym": "Advantage", 
          "example": "Guide dogs are a great boon to the partially sighted.", 
          "video": "https://www.youtube.com/embed/G8h1ENOUbW0 from 0:09"
          }, 
          {
          "word": "Boor", 
          "synonym": "Undesirables", 
          "example": "My mother often acts like a boor.", 
          "video": ""
          }, 
          {
          "word": "Boost", 
          "synonym": "Increase", 
          "example": "The theatre managed to boost its audiences by cutting ticket price.", 
          "video": ""
          }, 
          {
          "word": "Boot up", 
          "synonym": "", 
          "example": "Just give me a few minutes to boot up the computer.", 
          "video": "https://www.youtube.com/embed/YVMOjuLTzmk"
          }, 
          {
          "word": "Bored to tears", 
          "synonym": "", 
          "example": "I could see that my son was bored to tears by the historical documentary.", 
          "video": ""
          }, 
          {
          "word": "Born and bred", 
          "synonym": "Congenital", 
          "example": "He's a Parisian born and bred.", 
          "video": ""
          }, 
          {
          "word": "Borrow", 
          "synonym": "Take as a loan, use temporarily", 
          "example": "We had to borrow heavily to set up the business.", 
          "video": "https://www.youtube.com/embed/n7P9YDRAn4Y up to 0:10 second"
          }, 
          {
          "word": "Botch up/ make a botch of", 
          "synonym": "", 
          "example": "Sharif tried to assemble the new desk, but he made a botch of it.", 
          "video": "https://www.youtube.com/embed/SK_oY5MsS80"
          }, 
          {
          "word": "Bottle sth up", 
          "synonym": "Harden your heart", 
          "example": "His anger and frustration had been bottled up for years.", 
          "video": ""
          }, 
          {
          "word": "Bottom fell out", 
          "synonym": "", 
          "example": "When heavy rain was announced, the bottom fell out of their plans for a beach party.", 
          "video": ""
          }, 
          {
          "word": "Bottom fell out", 
          "synonym": "", 
          "example": "When heavy rain was announced, the bottom fell out of their plans for a beach party.", 
          "video": ""
          }, 
          {
          "word": "Bottom line", 
          "synonym": "Capital gains", 
          "example": "How will the  rise in interest  rates affect our bottom line?", 
          "video": "https://www.youtube.com/embed/DEZSvRyThEo"
          }, 
          {
          "word": "Bottomless", 
          "synonym": "Unlimited", 
          "example": "The generosity of the local people is bottomless.", 
          "video": "https://www.youtube.com/embed/bkCI5cYGizE"
          }, 
          {
          "word": "Bouffant", 
          "synonym": "Blowout", 
          "example": "She turned her incredible bouffant hairdo towards us.", 
          "video": "https://www.youtube.com/embed/zv8Jx"
          }, 
          {
          "word": "Boulder", 
          "synonym": "Haematite", 
          "example": "At dawn on the second day, he decided to try and use his climbing gear to lift the boulder off his arm.", 
          "video": "https://www.youtube.com/embed/HHvbvmAeB4Q"
          }, 
          {
          "word": "Boulevard", 
          "synonym": "Lane", 
          "example": "We strolled along the boulevard.", 
          "video": "https://www.youtube.com/embed/ljiJETzn9qc"
          }, 
          {
          "word": "Bounce back", 
          "synonym": "Come round", 
          "example": "Stock prices bounced back after a steep plunge earlier this  week.", 
          "video": "https://www.youtube.com/embed/GcenjUz1hRs"
          }, 
          {
          "word": "Bounce off the walls", 
          "synonym": "", 
          "example": "Danny can't wait to start his new job.  He's bouncing off the walls.", 
          "video": ""
          }, 
          {
          "word": "Bounce sb into sth", 
          "synonym": "", 
          "example": "The opposition hopes to bounce the prime minister into calling an early election.", 
          "video": "https://www.youtube.com/embed/GcenjUz1hRs"
          }, 
          {
          "word": "Bounce sth off sb", 
          "synonym": "", 
          "example": "Can I bounce  a couple of ideas off you?", 
          "video": ""
          }, 
          {
          "word": "Bountiful", 
          "synonym": "Aample", 
          "example": "We found a bountiful supply of coconuts on the island.", 
          "video": "https://www.youtube.com/embed/h"
          }, 
          {
          "word": "Bounty.", 
          "synonym": "Commission.", 
          "example": "A bounty of $10,000 has been offered for the capture of his murderer.", 
          "video": "https://www.youtube.com/embed/7H"
          }, 
          {
          "word": "Bow and scrape.", 
          "synonym": "", 
          "example": "The President was greeted with much bowing and scraping.", 
          "video": "https://www.youtube.com/embed/iUXOIpTB4Zc"
          }, 
          {
          "word": "Bow down to somebody.", 
          "synonym": "surrender.", 
          "example": "He expects me to bow down to him and do everything he tells me.", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Bow out.", 
          "synonym": "Retire, Resign.", 
          "example": "She'll be bowing out at the end of the month, after hosting the programme for eight years.", 
          "video": ""
          }, 
          {
          "word": "Bowl down/Along something.", 
          "synonym": "Rush, Scurry.", 
          "example": "They bowled down the street on their new bicycles.", 
          "video": ""
          }, 
          {
          "word": "Bowl somebody out.", 
          "synonym": "", 
          "example": "India were bowled out for 209.", 
          "video": ""
          }, 
          {
          "word": "Boxed in.", 
          "synonym": "Stuck, Blocked.", 
          "example": "I was boxed in, and had to wait for the driver of the other car to get back.", 
          "video": ""
          }, 
          {
          "word": "Brain drain", 
          "synonym": "", 
          "example": "Developing countries are struggling more because of the brain drain.", 
          "video": ""
          }, 
          {
          "word": "Brain drain.", 
          "synonym": "Emigrants.", 
          "example": "Britain has suffered a huge brain drain in recent years.", 
          "video": "https://www.youtube.com/embed/mQJkw_m7l08"
          }, 
          {
          "word": "Brain training.", 
          "synonym": "", 
          "example": "He runs a course in brain training for older people.", 
          "video": ""
          }, 
          {
          "word": "Brain trust.", 
          "synonym": "Advisors.", 
          "example": "The candidate's brain trust is gathering this weekend to plan strategy for the primary election.", 
          "video": ""
          }, 
          {
          "word": "Brain", 
          "synonym": "Exhausted", 
          "example": "By the time I leave work I'm completely brain", 
          "video": ""
          }, 
          {
          "word": "Brainchild.", 
          "synonym": "Conceptualize.", 
          "example": "The project was the brainchild of one of the students.", 
          "video": "https://www.youtube.com/embed/lC2sA_dl8ho"
          }, 
          {
          "word": "Brainstorm.", 
          "synonym": "Plan, Analyze.", 
          "example": "The team got together to brainstorm the project.", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Brainteaser.", 
          "synonym": "Riddle", 
          "example": "The paper publishes two brainteasers every Saturday.", 
          "video": "https://www.youtube.com/embed/r5wqrwn8guA"
          }, 
          {
          "word": "Brainwash.", 
          "synonym": "Convert.", 
          "example": "Their government is trying to brainwash them into thinking that war cannot be avoided.", 
          "video": "https://www.youtube.com/embed/DnItkG1yauQ"
          }, 
          {
          "word": "Brainwave.", 
          "synonym": "Theorize", 
          "example": "I couldn't see how I could get home from the station", 
          "video": "https://www.youtube.com/embed/RKPJlB80hRA"
          }, 
          {
          "word": "Brainy.", 
          "synonym": "Brilliant.", 
          "example": "Sarah was beautiful and brainy.", 
          "video": "https://www.youtube.com/embed/gbU7UXXiR10"
          }, 
          {
          "word": "Braise.", 
          "synonym": "Broil.", 
          "example": "Braise the lamb in wine.", 
          "video": "https://www.youtube.com/embed/dnYDRvh88k8"
          }, 
          {
          "word": "Bran.", 
          "synonym": "", 
          "example": "Both these breakfast cereals have added bran.", 
          "video": "https://www.youtube.com/embed/ou"
          }, 
          {
          "word": "Branch off something.", 
          "synonym": "", 
          "example": "We branched off the main route and went through the countryside.", 
          "video": ""
          }, 
          {
          "word": "Branch off.", 
          "synonym": "Diversify.", 
          "example": "We drove down a narrow track that branched off from the main road.", 
          "video": ""
          }, 
          {
          "word": "Branch out.", 
          "synonym": "Multiply.", 
          "example": "This designer has recently branched out into children's wear.", 
          "video": ""
          }, 
          {
          "word": "Brand", 
          "synonym": "", 
          "example": "Children are becoming more and more brand", 
          "video": "https://www.youtube.com/embed/p62JDg1veD8"
          }, 
          {
          "word": "Brass", 
          "synonym": "Yellow metal, copper base alloy", 
          "example": "The dark marble is easy to keep clean and the solid brass handles look luxurious.", 
          "video": "https://www.youtube.com/embed/y_F4liFMcZQ up to 0:11 second"
          }, 
          {
          "word": "Bravado.", 
          "synonym": "Heroic", 
          "example": "It was an act of bravado that made him ask his boss to resign.", 
          "video": "https://www.youtube.com/embed/5v2mDR"
          }, 
          {
          "word": "Brawl.", 
          "synonym": "Fight.", 
          "example": "A drunken brawl", 
          "video": "https://www.youtube.com/embed/4W_2KVSeikI"
          }, 
          {
          "word": "Brawn.", 
          "synonym": "Toughness.", 
          "example": "She said she preferred brawn to brains = a person who is physically attractive rather than an intelligent one.", 
          "video": "https://www.youtube.com/embed/6R5Z7uQJVjc"
          }, 
          {
          "word": "Bray.", 
          "synonym": "Bellow.", 
          "example": "The mules suddenly started braying.", 
          "video": "https://www.youtube.com/embed/ifzLv35bFf8"
          }, 
          {
          "word": "Brazen something out.", 
          "synonym": "Assured.", 
          "example": "I decided to brazen it out and hoped they wouldn't notice the scratch on the car.", 
          "video": ""
          }, 
          {
          "word": "Brazen.", 
          "synonym": "Bold.", 
          "example": "He told me a brazen lie.", 
          "video": "https://www.youtube.com/embed/hhA1TQiupUY"
          }, 
          {
          "word": "Breach.", 
          "synonym": "Violate.", 
          "example": "The theatre was in breach of the safety laws for having no fire doors.", 
          "video": "https://www.youtube.com/embed/B23d4zP512I"
          }, 
          {
          "word": "Bread and butter", 
          "synonym": "", 
          "example": "Teaching children math is my bread and butter.", 
          "video": ""
          }, 
          {
          "word": "Breadwinner.", 
          "synonym": "Jobholder.", 
          "example": "Men are often expected to be the breadwinner in a family.", 
          "video": "https://www.youtube.com/embed/nyUTwVZFX1I"
          }, 
          {
          "word": "Break sth off.", 
          "synonym": "Split.", 
          "example": "He broke off a piece of chocolate.", 
          "video": ""
          }, 
          {
          "word": "Break a leg", 
          "synonym": "", 
          "example": "'Break a leg!' shouted the stage director to his actors before the beginning of the play", 
          "video": "https://www.youtube.com/embed/O3asBV_lkKE"
          }, 
          {
          "word": "Break a leg", 
          "synonym": "", 
          "example": "Today’s the big game, eh? Break a leg!", 
          "video": ""
          }, 
          {
          "word": "Break down barriers.", 
          "synonym": "Mediate.", 
          "example": "The talks were meant to break down barriers between the two", 
          "video": ""
          }, 
          {
          "word": "Break fresh/new ground.", 
          "synonym": "Discover.", 
          "example": "This recovery technique breaks new ground.", 
          "video": "https://www.youtube.com/embed/d89ItgqJ"
          }, 
          {
          "word": "Break in.", 
          "synonym": "Barge.", 
          "example": "As she was talking, he suddenly broke in, saying, 'That's a lie.?'", 
          "video": "https://www.youtube.com/embed/mq8Wm6B3e8Q"
          }, 
          {
          "word": "Break into something.", 
          "synonym": "Trigger.", 
          "example": "He felt so happy that he broke into song = suddenly began to sing.", 
          "video": ""
          }, 
          {
          "word": "Break out.", 
          "synonym": "Arise.", 
          "example": "Fighting has broken out all over the city.", 
          "video": "https://www.youtube.com/embed/5aaB"
          }, 
          {
          "word": "Break the back of the beast.", 
          "synonym": "", 
          "example": "After hours of effort, the technicians finally broke the back of the beast and turned the electricity back on again.", 
          "video": ""
          }, 
          {
          "word": "Break the news.", 
          "synonym": "Declare.", 
          "example": "I was devastated when the doctor broke the news to me.", 
          "video": ""
          }, 
          {
          "word": "Break through something.", 
          "synonym": "Trespass.", 
          "example": "High waves broke through the barrier beach.", 
          "video": "https://www.youtube.com/embed/KoEpUuvcm_c"
          }, 
          {
          "word": "Break your back", 
          "synonym": "", 
          "example": "If you want the job done well, you should accept to pay more.  He's not going to break his back for such a low price!", 
          "video": ""
          }, 
          {
          "word": "Break your back.", 
          "synonym": "Labor.", 
          "example": "He broke his back to get the project done on time.", 
          "video": ""
          }, 
          {
          "word": "Breakeven.", 
          "synonym": "", 
          "example": "The business has grow from breakeven six years ago to seven", 
          "video": "https://www.youtube.com/embed/IOrG6y2sWw0"
          }, 
          {
          "word": "Breaking and entering.", 
          "synonym": "Break", 
          "example": "The thief was arrested and charged with breaking and entering.", 
          "video": "https://www.youtube.com/embed/gtYWVe9A8rQ"
          }, 
          {
          "word": "Breakneck.", 
          "synonym": "Rapid.", 
          "example": "They were riding along at breakneck speed/at a breakneck pace.", 
          "video": "https://www.youtube.com/embed/OfqdvpSW128"
          }, 
          {
          "word": "Breakwater.", 
          "synonym": "Barrier.", 
          "example": "There were boys bathing still from the breakwater of the rocks.", 
          "video": "https://www.youtube.com/embed/xbYrEXnWQHI"
          }, 
          {
          "word": "Bribe", 
          "synonym": "Inducement, Incentive", 
          "example": "The politician was accused of accepting bribes from businessmen.", 
          "video": "https://www.youtube.com/embed/VlnG8brfLU0"
          }, 
          {
          "word": "Bricks and mortar/ bricks and clicks", 
          "synonym": "", 
          "example": "Click businesses are usually more flexible than brick", 
          "video": "https://www.youtube.com/embed/ZUxWKHb8xIc"
          }, 
          {
          "word": "Bridge a/the gap", 
          "synonym": "", 
          "example": "The president singled out education as a vital tool in bridging the gap between rich and poor.", 
          "video": ""
          }, 
          {
          "word": "Bright", 
          "synonym": "", 
          "example": "Gary was fantastic. He arrived bright", 
          "video": ""
          }, 
          {
          "word": "Bring  sth  to life / come to life", 
          "synonym": "", 
          "example": "It's always been an interesting period in history and this film really brought it to life.", 
          "video": ""
          }, 
          {
          "word": "Bring about", 
          "synonym": "Activation, actuate.", 
          "example": "Ten years of incompetent government had brought about the virtual collapse of the country's economy.", 
          "video": "https://www.youtube.com/embed/y0RYamIZ5QI"
          }, 
          {
          "word": "Bring off", 
          "synonym": "Succeeding, achieving and fulfilling.", 
          "example": "It was an important event, and she's managed to bring it off wonderfully.", 
          "video": "https://www.youtube.com/embed/yS1rk40bSgs"
          }, 
          {
          "word": "Bring the house down", 
          "synonym": "", 
          "example": "f he sings like that on Saturday, he'll bring the house down.", 
          "video": ""
          }, 
          {
          "word": "Bring the house down", 
          "synonym": "", 
          "video": ""
          }, 
          {
          "word": "Bring to heel", 
          "synonym": "", 
          "example": "The boy had always behaved badly, but the new headmaster managed to bring him to heel.", 
          "video": "https://www.youtube.com/embed/OQcQAPPWT"
          }, 
          {
          "word": "Bring to mind", 
          "synonym": "", 
          "example": "Fish and chip shops bring to mind  my holidays in Britain.", 
          "video": "https://www.youtube.com/embed/qCs2NXVvAIA"
          }, 
          {
          "word": "Bring up", 
          "synonym": "Quoting & making references.", 
          "example": "It was neither the time nor place to bring up the issue of religion.", 
          "video": "https://www.youtube.com/embed/Ns3Yz1GtNfI"
          }, 
          {
          "word": "Broaden", 
          "synonym": "Widen, expand", 
          "example": "Travel broadens your mind.", 
          "video": "https://www.youtube.com/embed/VmXIE4cv5BU"
          }, 
          {
          "word": "Broadens the mind", 
          "synonym": "", 
          "example": "Travel broadens the mind.", 
          "video": ""
          }, 
          {
          "word": "Bronze", 
          "synonym": "Bronze medal, third prize", 
          "example": "He won a bronze in the 200m.", 
          "video": "https://www.youtube.com/embed/HERzrfSwB2U"
          }, 
          {
          "word": "Brush up on", 
          "synonym": "Relieve, salve.", 
          "example": "I thought I'd brush up on my French before going to Paris.", 
          "video": "https://www.youtube.com/embed/hw6hE_GW6r0"
          }, 
          {
          "word": "Brutal", 
          "synonym": "Cruel, vicious", 
          "example": "Soccer has nothing to do with contemporary soccer, which is brutal, aggressive, and emotional.", 
          "video": "https://www.youtube.com/embed/uGYarfPcx5Q"
          }, 
          {
          "word": "Bubble", 
          "synonym": "Globule, bead", 
          "example": "As a consequence the sea became polluted, and its deep blue colour turned into a dirty green, covered with bubbles.", 
          "video": "https://www.youtube.com/embed/LvSvM1fEx40 up to 0:10 second"
          }, 
          {
          "word": "Buckle down", 
          "synonym": "", 
          "example": "If you don’t buckle down to your job, you’ll be fired.", 
          "video": ""
          }, 
          {
          "word": "Buckle down", 
          "synonym": "", 
          "example": "It’s almost exam time, so I need to buckle down this weekend.", 
          "video": ""
          }, 
          {
          "word": "Bugger/Sod, etc. this for a lark!", 
          "synonym": "Complaining, protest.", 
          "example": "I'd been waiting for him for an hour and I thought, sod this for a lark", 
          "video": ""
          }, 
          {
          "word": "Built", 
          "synonym": "Incalescence, Obsolescent, Incalescence", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Built", 
          "synonym": "Old or old", 
          "example": "", 
          "video": "https://www.youtube.com/embed/hfHH8BqcEak"
          }, 
          {
          "word": "Buldoze into doing", 
          "synonym": "", 
          "example": "The immigrants we bulldozed into accepting the work.", 
          "video": "https://www.youtube.com/embed/68mQbAbw6Xw"
          }, 
          {
          "word": "Bulk", 
          "synonym": "Loads, heaps", 
          "example": "I suggest that you buy food in bulk so that you not only save money but also save time.", 
          "video": "https://www.youtube.com/embed/V9nB5bF6yp4 up to 0:13 second"
          }, 
          {
          "word": "Bully", 
          "synonym": "Tyrant, tormentor", 
          "example": "Nowadays, due to active bullying prevention by the schools, the children are exposed to the bad effects of bullying and how to stand up if anybody tries to bully them.", 
          "video": "https://www.youtube.com/embed/uY_cdYR0vLg up to 0:19 second"
          }, 
          {
          "word": "Bump into", 
          "synonym": "Assignation, conclave.", 
          "example": "We bumped into Amy when we were in town last week.", 
          "video": "https://www.youtube.com/embed/78t8TqtLQSI"
          }, 
          {
          "word": "Bunk", 
          "synonym": "Berth, cot", 
          "example": "The skipper slept in a bunk in the forward cabin.", 
          "video": "https://www.youtube.com/embed/5BZgEvItJxY"
          }, 
          {
          "word": "Burble", 
          "synonym": "", 
          "example": "If you mumble or burble, give up all thought of advocacy.", 
          "video": "https://www.youtube.com/embed/v"
          }, 
          {
          "word": "Burden", 
          "synonym": "Load, weight", 
          "example": "I'd hate to be a burden to you when I'm older.", 
          "video": "https://www.youtube.com/embed/B0Hj4KMwQjE"
          }, 
          {
          "word": "Burdensome", 
          "synonym": "Complicated, Difficult to do", 
          "example": "Some agents however do not favour a delegation and consider the power of making a decision rather burdensome.", 
          "video": "https://www.youtube.com/embed/Z4ICpIhcyos"
          }, 
          {
          "word": "Burgeon", 
          "synonym": "Making progress, Advancing", 
          "example": "Love burgeoned between them.", 
          "video": "https://www.youtube.com/embed/BcbdTSRimUk"
          }, 
          {
          "word": "Burgle", 
          "synonym": "Robery, Theft", 
          "example": "When they got back from their holiday they found that their home had been burgled.", 
          "video": "https://www.youtube.com/embed/Hu500FrxelQ"
          }, 
          {
          "word": "Burial at sea", 
          "synonym": "Burying, Cremating, Preserving bodies", 
          "example": "As the Captain passed away in his ship, he was given a proper burial at the sea.", 
          "video": "https://www.youtube.com/embed/iHNqd"
          }, 
          {
          "word": "Burly", 
          "synonym": "Big, Husky, Quite big", 
          "example": "Emmett is tall, burly, extremely muscular, and, to most humans, the most intimidating of his adoptive siblings.", 
          "video": "https://www.youtube.com/embed/2C4eY4AmhSo"
          }, 
          {
          "word": "Burn a hole in one’s pocket", 
          "synonym": "", 
          "example": "Let’s go to the mall after school. There’s a hundred dollar bill burning a hole in my pocket.", 
          "video": ""
          }, 
          {
          "word": "Burn one’s finger", 
          "synonym": "", 
          "example": "I don’t like little Johnny’s new friend as he burns his finger.", 
          "video": ""
          }, 
          {
          "word": "Burn out", 
          "synonym": "Burning, Burnt, On fire", 
          "example": "It looks like the starter motor on the car has burned out.", 
          "video": "https://www.youtube.com/embed/iKchlQM4fyQ"
          }, 
          {
          "word": "Burn out", 
          "synonym": "Burning, burnt & on fire.", 
          "example": "The relentless pressure to make money means traders burn out fast.", 
          "video": "https://www.youtube.com/embed/W91cUefNb2Q"
          }, 
          {
          "word": "Burn something down", 
          "synonym": "", 
          "example": "He tried to burn down the school by setting fire to a pile of papers.", 
          "video": "https://www.youtube.com/embed/HOCaxxPtzdw"
          }, 
          {
          "word": "Burn something off", 
          "synonym": "Exercising, Training, Workout", 
          "example": "Running is an excellent way to burn off excess calories.", 
          "video": "https://www.youtube.com/embed/HOCaxxPtzdw"
          }, 
          {
          "word": "Burn the candle at both ends", 
          "synonym": "", 
          "example": "Lizzy took two jobs and it is not good for her health to burn the candle at both ends.", 
          "video": ""
          }, 
          {
          "word": "Burn up with something", 
          "synonym": "Strong feelings", 
          "example": "He was burned up with jealousy and suspicion.", 
          "video": "https://www.youtube.com/embed/A8yF2rnmdTs"
          }, 
          {
          "word": "Burn your boats", 
          "synonym": "", 
          "example": "There is no going back to her now, you have burnt your boats.", 
          "video": "https://www.youtube.com/embed/37rRApH5dfs"
          }, 
          {
          "word": "Burn your fingers", 
          "synonym": "", 
          "example": "Jack got his fingers burnt playing on the stock market.", 
          "video": "https://www.youtube.com/embed/BKdQRFK5kPw"
          }, 
          {
          "word": "Burn", 
          "synonym": "Burning, Burnt, On fire", 
          "example": "The relentless pressure to make money means traders burn out fast.", 
          "video": "https://www.youtube.com/embed/iKchlQM4fyQ"
          }, 
          {
          "word": "Burner", 
          "synonym": "Heaters, Burners, Stove", 
          "example": "Image incense burners prompt an entirely different series of speculations.", 
          "video": "https://www.youtube.com/embed/eqkzSmgyYTo"
          }, 
          {
          "word": "Burning issue", 
          "synonym": "Strong desire", 
          "example": "He spoke of his burning desire to play for his country.", 
          "video": "https://www.youtube.com/embed/9jFuBzO5idQ"
          }, 
          {
          "word": "Burp", 
          "synonym": "Noises made by the body", 
          "example": "The baby gave a contented burp.", 
          "video": "https://www.youtube.com/embed/TZPnxE96nnI"
          }, 
          {
          "word": "Burrow", 
          "synonym": "", 
          "example": "Squirrels were captured, by chasing them from their burrows.", 
          "video": "https://www.youtube.com/embed/ubcH24Eoxfc"
          }, 
          {
          "word": "Bursary", 
          "synonym": "Grants, Allowances", 
          "example": "There are two types of bursary awarded by institutions such as universities.", 
          "video": "https://www.youtube.com/embed/Cj1VPUnOIyc"
          }, 
          {
          "word": "Burst at the seams", 
          "synonym": "", 
          "example": "I ate too much. I am bursting at the seams in these jeans.", 
          "video": ""
          }, 
          {
          "word": "Burst in on somebody/something", 
          "synonym": "Exploding, Erupting", 
          "example": "Katya burst in on him without warning.", 
          "video": "https://www.youtube.com/embed/Uzh9arv5hhE"
          }, 
          {
          "word": "Burst in", 
          "synonym": "Exploding, Erupting", 
          "example": "The side door of the bar flew open and three men burst in.", 
          "video": "https://www.youtube.com/embed/Uzh9arv5hhE"
          }, 
          {
          "word": "Burst into flames", 
          "synonym": "", 
          "example": "Smoke started pouring out from underneath, then the truck burst into flames.", 
          "video": ""
          }, 
          {
          "word": "Burst into laughter", 
          "synonym": "To suddenly begin to laugh.", 
          "example": "Much to my surprise, Caleb suddenly burst into laughter.", 
          "video": "https://www.youtube.com/embed/ke2qajU3TWk"
          }, 
          {
          "word": "Burst into tears", 
          "synonym": "To suddenly start to cry.", 
          "example": "I saw her burst into tears in her room.", 
          "video": ""
          }, 
          {
          "word": "Burst out", 
          "synonym": "Shouting, Screaming", 
          "example": "'Don't go!' he burst out.", 
          "video": "https://www.youtube.com/embed/Uzh9arv5hhE"
          }, 
          {
          "word": "Bury the hatchet.", 
          "synonym": "", 
          "example": "Letís bury the hatchet and be friends.", 
          "video": ""
          }, 
          {
          "word": "Busby", 
          "synonym": "Fur hats , Scarves", 
          "example": "The tall black", 
          "video": "https://www.youtube.com/embed/tOzw69v1tYw"
          }, 
          {
          "word": "Bushfire", 
          "synonym": "Fire, Flame", 
          "example": "The news spread like bushfire.", 
          "video": "https://www.youtube.com/embed/N2l7UdM_ZS4"
          }, 
          {
          "word": "Bushman", 
          "synonym": "", 
          "example": "Naturalist Wyn Jones is an expert bushman.", 
          "video": "https://www.youtube.com/embed/ba8vsf"
          }, 
          {
          "word": "Bushranger", 
          "synonym": "Miscellaneous criminals", 
          "example": "The bag was stolen by a bushranger.", 
          "video": "https://www.youtube.com/embed/7oTfkf2Wkrc"
          }, 
          {
          "word": "Business as usual", 
          "synonym": "", 
          "example": "It was business as usual at the supermarket the day after the hold", 
          "video": "https://www.youtube.com/embed/Fc4NtngefJU up to 0:12 second"
          }, 
          {
          "word": "Business before pleasure", 
          "synonym": "", 
          "example": "I'd love to have lunch with you  but I've got a report to finish", 
          "video": "https://www.youtube.com/embed/p9azXwAV5_c"
          }, 
          {
          "word": "Business is business", 
          "synonym": "", 
          "example": "I'll hire your brother only if he is the best candidate. I'm sorry but business is business!", 
          "video": ""
          }, 
          {
          "word": "Busk", 
          "synonym": "Playing music in public for money", 
          "example": "Busk took his theories into the air and tried them out in practice.", 
          "video": "https://www.youtube.com/embed/nzFc24vHEpk"
          }, 
          {
          "word": "Busker", 
          "synonym": "", 
          "example": "The busker intended to provide an inherently stable aeroplane.", 
          "video": "https://www.youtube.com/embed/kgYjHy1zJvI"
          }, 
          {
          "word": "Busman’s holiday", 
          "synonym": "", 
          "example": "My husband is a chef, so for him time off with the family is often a busman's holiday!", 
          "video": ""
          }, 
          {
          "word": "Bustle", 
          "synonym": "Busy activity, Hustle", 
          "example": "Thora bustled around the house, getting everything ready.", 
          "video": "https://www.youtube.com/embed/Ik1uI6UB3FU"
          }, 
          {
          "word": "Bustling", 
          "synonym": "Hurrying, Doing things quickly", 
          "example": "Thora bustled around the house, getting everything ready.", 
          "video": "https://www.youtube.com/embed/oNShEtGA5zI"
          }, 
          {
          "word": "Butt in on", 
          "synonym": "Interrupting & preventing from speaking.", 
          "example": "He kept on butting in with silly comments.", 
          "video": "https://www.youtube.com/embed/a75TnPXN"
          }, 
          {
          "word": "Butter wouldn't melt in your mouth", 
          "synonym": "", 
          "example": "The boy who stole the purse looked as if butter wouldn't melt in his mouth.", 
          "video": "https://www.youtube.com/embed/z8MV9j7rWcg"
          }, 
          {
          "word": "Buttercup", 
          "synonym": "A small, bright yellow wild flower", 
          "example": "Flowering plants within the grassland areas include: birdsfoot trefoil, buttercup, clover, flax, ox", 
          "video": "https://www.youtube.com/embed/ANw5RuZOJiE"
          }, 
          {
          "word": "Buy a lemon", 
          "synonym": "", 
          "example": "The used car I bought is not very good, I think that I bought a lemon.", 
          "video": "https://www.youtube.com/embed/H5bDZUUaOcA?t=1s"
          }, 
          {
          "word": "Buy somebody's silence", 
          "synonym": "", 
          "example": "What will we have to do to buy her silence?", 
          "video": ""
          }, 
          {
          "word": "Buy time", 
          "synonym": "", 
          "example": "He tried to buy time by saying he hadn't been well.", 
          "video": ""
          }, 
          {
          "word": "Buzz", 
          "synonym": "Active, Full of energy", 
          "example": "He predicts that Logan Airport will be buzzing as usual", 
          "video": "https://www.youtube.com/embed/tSyLbuHDbUs"
          }, 
          {
          "word": "By a factor of", 
          "synonym": "Influential element", 
          "example": "The election was lost by a factor of indiscipline.", 
          "video": ""
          }, 
          {
          "word": "By a hairís breadth", 
          "synonym": "", 
          "example": "A slate fell off the roof and missed the child by a hair's breadth.", 
          "video": "https://www.youtube.com/embed/MOvAxI"
          }, 
          {
          "word": "By a nose", 
          "synonym": "", 
          "example": "It was a very exciting race. My horse won but only by a nose.", 
          "video": ""
          }, 
          {
          "word": "By a process of elimination", 
          "synonym": "", 
          "example": "We eventually found the answer by a process of elimination.", 
          "video": ""
          }, 
          {
          "word": "By accident", 
          "synonym": "", 
          "example": "I met Sally at the mall by accident.", 
          "video": ""
          }, 
          {
          "word": "By all means.", 
          "synonym": "", 
          "example": "'May I borrow this book?' 'By all means.'", 
          "video": "https://www.youtube.com/embed/Hql9GBzgv"
          }, 
          {
          "word": "By and large", 
          "synonym": "Abstract, abstraction.", 
          "example": "There are a few small things that I don't like about my job, but by and large it's very enjoyable.", 
          "video": "https://www.youtube.com/embed/cipj1gGfJi8"
          }, 
          {
          "word": "By common consent", 
          "synonym": "", 
          "example": "Her latest novel, by common consent, is her best yet.", 
          "video": ""
          }, 
          {
          "word": "By definition", 
          "synonym": "", 
          "example": "By definition war is the most unjustifiable human creation.", 
          "video": ""
          }, 
          {
          "word": "By dint of sth", 
          "synonym": "", 
          "example": "They got the building finished on time by dint of hard work and good organization.", 
          "video": ""
          }, 
          {
          "word": "By fair means or foul", 
          "synonym": "", 
          "example": "I will get the win by fair means or foul.", 
          "video": ""
          }, 
          {
          "word": "By far and away.", 
          "synonym": "great extent, large amount, immense.", 
          "example": "He is by far and away the most accomplished player", 
          "video": ""
          }, 
          {
          "word": "By far.", 
          "synonym": "by huge amount, abundantly, majorly.", 
          "example": "They are by far the best students in the class.", 
          "video": "0:05"
          }, 
          {
          "word": "By fits and starts.", 
          "synonym": "", 
          "example": "He did his work by fits and starts.", 
          "video": ""
          }, 
          {
          "word": "By hook or by crook.", 
          "synonym": "", 
          "example": "Iíll get her to marry me, by hook or by crook.", 
          "video": ""
          }, 
          {
          "word": "By leaps and bounds.", 
          "synonym": "", 
          "example": "The company is growing by leaps and bounds this year.", 
          "video": ""
          }, 
          {
          "word": "By no means / not by any means.", 
          "synonym": "", 
          "example": "It is by no means certain that we'll finish the project by June.", 
          "video": "https://www.youtube.com/embed/BjzGhMPowu4"
          }, 
          {
          "word": "By", 
          "synonym": "Outcomes, Consequences", 
          "example": "Buttermilk is a by", 
          "video": "https://www.youtube.com/embed/tSyLbuHDbUs"
          }, 
          {
          "word": "Bystander", 
          "synonym": "Audiences, Spectators", 
          "example": "Many innocent bystanders were injured by the explosion.", 
          "video": "https://www.youtube.com/embed/evQ27QfbGJs"
          }, 
          {
          "word": "Cabaret", 
          "synonym": "Musical performances", 
          "example": "In the early 1930s she turned to cabaret.", 
          "video": "https://www.youtube.com/embed/BNc2KFMx"
          }, 
          {
          "word": "Cabin crew", 
          "synonym": "Workers on aircraft & spacecraft", 
          "example": "Responsibility for the health of cabin crews rests with the airlines.", 
          "video": "https://www.youtube.com/embed/379dG4lr1fA"
          }, 
          {
          "word": "Cabin cruiser", 
          "synonym": "Boats, Sailing craft", 
          "example": "The river is large enough to support small barges, and medium", 
          "video": "https://www.youtube.com/embed/jrbwJZfN"
          }, 
          {
          "word": "Cacao", 
          "synonym": "", 
          "example": "Much of the land went for the production of corn, cacao and bananas.", 
          "video": "https://www.youtube.com/embed/kVSIkXL_Nmo"
          }, 
          {
          "word": "Cache", 
          "synonym": "Groups, Hidden collections of things", 
          "example": "A cache of explosives.", 
          "video": "https://www.youtube.com/embed/mm2VPpcl6Eo"
          }, 
          {
          "word": "Cachet", 
          "synonym": "Quality, Standard", 
          "example": "This type of jacket used to have a certain cachet.", 
          "video": "https://www.youtube.com/embed/yhxhJQwrzII"
          }, 
          {
          "word": "Cackle", 
          "synonym": "Alarming sound, Unpleasant sound", 
          "example": "The hens cackled in alarm.", 
          "video": "https://www.youtube.com/embed/dPOjkGsnwr8"
          }, 
          {
          "word": "Cacophony", 
          "synonym": "Noise, discord", 
          "example": "As we entered the farmyard we were met with a cacophony of animal sounds.", 
          "video": "https://www.youtube.com/embed/fE7JLJ7pnvc"
          }, 
          {
          "word": "Cadaverous", 
          "synonym": "Pallid, white", 
          "example": "The opportunity for them to contaminate their hands with cadaverous particles was thereby greatly reduced.", 
          "video": "https://www.youtube.com/embed/JZFx8IwKk"
          }, 
          {
          "word": "Caddy", 
          "synonym": "Jar, container", 
          "example": "The tea caddy is on the kitchen table.", 
          "video": ""
          }, 
          {
          "word": "Cadence", 
          "synonym": "Accent, inflection", 
          "example": "A sentence may look correct on paper but its cadence may be jarring.", 
          "video": "https://www.youtube.com/embed/V0DKXEjvNSM from 0:10 second"
          }, 
          {
          "word": "Cadge", 
          "synonym": "", 
          "example": "He's always cadging free meals and free trips from/off his clients.", 
          "video": ""
          }, 
          {
          "word": "Cagey", 
          "synonym": "Crafty, secretive", 
          "example": "He was very cagey about what happened at the meeting.", 
          "video": "https://www.youtube.com/embed/8R0k2z0eacI from 0:12 second"
          }, 
          {
          "word": "Cajole", 
          "synonym": "Tempt, persuade", 
          "example": "He really knows how to cajole people into doing what he wants.", 
          "video": "https://www.youtube.com/embed/NwJGf6dbduY"
          }, 
          {
          "word": "Cake not worth the candle", 
          "synonym": "", 
          "example": "He recorded an album but sold very few copies; the cake wasn't worth the candle.", 
          "video": ""
          }, 
          {
          "word": "Cake not worth the candle", 
          "synonym": "", 
          "example": "He recorded an album but sold very few copies; the cake wasn't worth the candle.", 
          "video": ""
          }, 
          {
          "word": "Cakewalk", 
          "synonym": "", 
          "example": "The Superbowl was a cakewalk for the Forty", 
          "video": "https://www.youtube.com/embed/JNZAgFjogJU"
          }, 
          {
          "word": "Calculate on sth", 
          "synonym": "", 
          "example": "We're calculating on about 30 guests.", 
          "video": ""
          }, 
          {
          "word": "Calculated risk", 
          "synonym": "Dangers and threats.", 
          "example": "The director took a calculated risk in giving the film's main role to an unknown actor.", 
          "video": "https://www.youtube.com/embed/I5U9jWtsCdg"
          }, 
          {
          "word": "Call a halt to  sth", 
          "synonym": "Staying and remaining.", 
          "example": "How many more people will have to die before they call a halt to the fighting?", 
          "video": ""
          }, 
          {
          "word": "Call a spade a spade", 
          "synonym": "", 
          "example": "What I like about the new manager is that he calls a spade a spade ", 
          "video": "https://www.youtube.com/embed/ogZp_61sp8I"
          }, 
          {
          "word": "Call for sth", 
          "synonym": "", 
          "example": "It's the sort of work that calls for a high level of concentration.", 
          "video": ""
          }, 
          {
          "word": "Call forth sth", 
          "synonym": "", 
          "example": "The proposed shopping centre has called forth an angry response from local residents.", 
          "video": ""
          }, 
          {
          "word": "Call in on sb", 
          "synonym": "", 
          "example": "I thought we might call in on your mother on our way", 
          "video": ""
          }, 
          {
          "word": "Call sb in", 
          "synonym": "", 
          "example": "A new team of detectives were called in to conduct a fresh inquiry.", 
          "video": ""
          }, 
          {
          "word": "Call sth off", 
          "synonym": "", 
          "example": "Tomorrow's match has been called off because of the icy weather.", 
          "video": ""
          }, 
          {
          "word": "Call the shots/the tune", 
          "synonym": "", 
          "example": "He shows a lot of authority but in fact it's his wife who calls the tune.", 
          "video": "https://www.youtube.com/embed/hrYdMrjq3gA"
          }, 
          {
          "word": "Callous", 
          "synonym": "Heartless, apathetic", 
          "example": "It might sound callous, but I don't care if he's homeless. He's not living with me!", 
          "video": "https://www.youtube.com/embed/a2d8f7tTCps up to 0:11 second"
          }, 
          {
          "word": "Callus", 
          "synonym": "", 
          "example": "He had workman's hands which were rough and covered with calluses.", 
          "video": "https://www.youtube.com/embed/E82"
          }, 
          {
          "word": "Calm down", 
          "synonym": "Calming and relaxing.", 
          "example": "When she calmed down, she was more coherent .", 
          "video": "https://www.youtube.com/embed/hBeJ"
          }, 
          {
          "word": "Calypso", 
          "synonym": "", 
          "example": "Have you heard any calypso?", 
          "video": "https://www.youtube.com/embed/5qmK9h3oWJI"
          }, 
          {
          "word": "Camber", 
          "synonym": "Leaning, cant", 
          "example": "Rigid chairs also have the option for their rear wheels to have a camber.", 
          "video": "https://www.youtube.com/embed/Cwb9"
          }, 
          {
          "word": "Camouflage", 
          "synonym": "Disguise, faking", 
          "example": "The troops had camouflaged themselves so effectively that the enemy didn't notice them approaching.", 
          "video": "https://www.youtube.com/embed/FhZmRO6Y6Eo"
          }, 
          {
          "word": "Campaign", 
          "synonym": "Push, movement", 
          "example": "In order to solve problems caused by traffic congestion, perhaps the City Council should consider launching a publicity campaign to show people in Baden the alternative means of transport and the advantages of using them.", 
          "video": "https://www.youtube.com/embed/ZEdrz6WBtp8 up to 0:10 second"
          }, 
          {
          "word": "Campfire", 
          "synonym": "", 
          "example": "Each unit also has its own water spigot, outhouse, and campfire ring.", 
          "video": "https://www.youtube.com/embed/3osVQRM3f7o"
          }, 
          {
          "word": "Can of worms.", 
          "synonym": "", 
          "example": "The discovery of the transfer of funds turned out to be a real can of worms.", 
          "video": "https://www.youtube.com/embed/otWuCKynN7A"
          }, 
          {
          "word": "Can't be fagged", 
          "synonym": "bothered", 
          "example": "I can't be fagged to do the peeling and cooking.", 
          "video": ""
          }, 
          {
          "word": "Can't cut the mustard / can't cut it", 
          "synonym": "", 
          "example": "If he can't cut it, then we'll get someone else to do the job.", 
          "video": "https://www.youtube.com/embed/C654XiiAT_8"
          }, 
          {
          "word": "Can't face sth/doing sth", 
          "synonym": "", 
          "example": "I can't face doing the work right now after all that has happened.", 
          "video": ""
          }, 
          {
          "word": "Can't see the wood for the trees.", 
          "synonym": "", 
          "example": "The new manager found the situation so complicated that he couldn't see the wood for the trees.", 
          "video": ""
          }, 
          {
          "word": "Can't take  sth", 
          "synonym": "", 
          "example": "I can't take it any more. I'm leaving.", 
          "video": ""
          }, 
          {
          "word": "Can't wait", 
          "synonym": "Be unable to endure, Be very impatient", 
          "example": "He can’t wait to buy a house.", 
          "video": ""
          }, 
          {
          "word": "Canary", 
          "synonym": "", 
          "example": "The canary in the green cage that hung in the window put its head on one side and tweaked a seed husk out into Philip's face, then twittered defiantly.", 
          "video": "https://www.youtube.com/embed/uDJdxfJGq0w up to 0:18 second"
          }, 
          {
          "word": "Candour", 
          "synonym": "", 
          "example": "'We really don't know what to do about it,' she said with surprising candour.", 
          "video": ""
          }, 
          {
          "word": "Candyfloss", 
          "synonym": "Fairyfloss, spun sugar", 
          "example": "My son wanted to buy a candyfloss at the fair, but I did not allow him as he had stomach issues that time.", 
          "video": "https://www.youtube.com/embed/uhKtRT6Gsrc"
          }, 
          {
          "word": "Cane", 
          "synonym": "", 
          "example": "Chair seats are often woven out of cane.", 
          "video": "https://www.youtube.com/embed/eI5DduuU_as up to 0:44 second"
          }, 
          {
          "word": "Canker", 
          "synonym": "", 
          "example": "Poverty is a canker eating away at the heart of society.", 
          "video": "https://www.youtube.com/embed/as1eDdS0UZc from 0:22 second"
          }, 
          {
          "word": "Cannibal", 
          "synonym": "Aborigine, brute", 
          "example": "It is fortunate that these cannibal devils are too stupid and too anxious for human flesh to exercise patience.", 
          "video": "https://www.youtube.com/embed/OMVwo1pZ_SU"
          }, 
          {
          "word": "Cannon", 
          "synonym": "Mortar, ordnance", 
          "example": "Beside the cannon a cart was standing to which two horses were harnessed.", 
          "video": "https://www.youtube.com/embed/xI_Y7Tjaws0 up to 0:18 second"
          }, 
          {
          "word": "Cannonade", 
          "synonym": "Battery, bomb", 
          "example": "Some of the houses seemed to have been ruined by a cannonade.", 
          "video": "https://www.youtube.com/embed/CBp_"
          }, 
          {
          "word": "Canny", 
          "synonym": "Clever, artful", 
          "example": "These salesmen are a canny lot.", 
          "video": "https://www.youtube.com/embed/13PalPJxx3M"
          }, 
          {
          "word": "Canon", 
          "synonym": "Priest", 
          "example": "For a time he served as canon and treasurer of Salisbury Cathedral, having been ordained a priest several years before.", 
          "video": ""
          }, 
          {
          "word": "Canopy", 
          "synonym": "Shade, roof", 
          "example": "Trees arched over the road, forming a canopy of leaves.", 
          "video": "https://www.youtube.com/embed/Rws1icmaGGQ from 0:21 second"
          }, 
          {
          "word": "Canyon", 
          "synonym": "Dale, valley", 
          "example": "Night had fallen and the canyon was turning cold.", 
          "video": "https://www.youtube.com/embed/ZqhHpbmbBlk"
          }, 
          {
          "word": "Canít  stand the pace", 
          "synonym": "", 
          "example": "She once worked for a famous fashion designer but she couldn't stand the pace.", 
          "video": ""
          }, 
          {
          "word": "Canít boil an egg", 
          "synonym": "Inability", 
          "example": "Her daughter even canít boil an egg.", 
          "video": ""
          }, 
          {
          "word": "Canít cut the mustard", 
          "synonym": "", 
          "example": "That guy looks like he's 110 years old I'm sure he can't cut the mustard stocking shelves all day!", 
          "video": "https://www.youtube.com/embed/_Z_RM9ogLoo?t=8s"
          }, 
          {
          "word": "Cap", 
          "synonym": "Limit, restrict", 
          "example": "The interest rate has been capped at 5%.", 
          "video": "https://www.youtube.com/embed/oRBITg5j8SU from 2:20 second to 2:47 second"
          }, 
          {
          "word": "Capacious", 
          "synonym": "Spacious, captious", 
          "example": "Upstairs there is a capacious conference room and three apartments.", 
          "video": "https://www.youtube.com/embed/MNTvxXDxGGI"
          }, 
          {
          "word": "Capital punishment.", 
          "synonym": "", 
          "example": "Capital punishment was regarded as inhuman and immoral.", 
          "video": ""
          }, 
          {
          "word": "Capitalize on sth", 
          "synonym": "", 
          "example": "She capitalized on her knowledge and experience to get a better job.", 
          "video": ""
          }, 
          {
          "word": "Capitulate", 
          "synonym": "Submit, surrender", 
          "example": "Their forces capitulated five hours after the bombardment of the city began.", 
          "video": "https://www.youtube.com/embed/i"
          }, 
          {
          "word": "Capricious", 
          "synonym": "Fickle, unpredictable", 
          "example": "He was a cruel and capricious tyrant.", 
          "video": "https://www.youtube.com/embed/LlHdQq27Ulc"
          }, 
          {
          "word": "Captious", 
          "synonym": "Hypercritical, nit", 
          "example": "Amid such splendor it seems captious to point out the flaw.", 
          "video": "https://www.youtube.com/embed/0uNIvz2ihVI from 0:17 second"
          }, 
          {
          "word": "Captivate", 
          "synonym": "Attract, enchant", 
          "example": "With her beauty and charm, she captivated film audiences everywhere.", 
          "video": "https://www.youtube.com/embed/7DO5wQNBqLM up to 0:10 second"
          }, 
          {
          "word": "Captive", 
          "synonym": "Imprisoned, enslaved", 
          "example": "When the town was recaptured, we found soldiers who had been captives for several years.", 
          "video": "https://www.youtube.com/embed/yuYzU2JTjco up to 0:13 second"
          }, 
          {
          "word": "Car pool", 
          "synonym": "", 
          "example": "Its easier to car", 
          "video": "https://www.youtube.com/embed/xuaX1eyj1Ew"
          }, 
          {
          "word": "Caramel", 
          "synonym": "HOneyed, flaxen", 
          "example": "The sugar glaze that melts to become caramel forms a continuous coat, also adds to firmness of cake.", 
          "video": "https://www.youtube.com/embed/T5iOoLmWC9k"
          }, 
          {
          "word": "Carcass", 
          "synonym": "Corpse, skeleton", 
          "example": "Vultures flew around in the sky waiting to pick at the rotting carcass of the deer.", 
          "video": "https://www.youtube.com/embed/08vn8Nc4Frw up to 0:12 second"
          }, 
          {
          "word": "Carcinogenic", 
          "synonym": "Mutagen, toxin", 
          "example": "If there are doubts as to the carcinogenic effect of a substance, we should apply the precautionary principle.", 
          "video": "https://www.youtube.com/embed/50KcPJQTSoA"
          }, 
          {
          "word": "Career woman", 
          "synonym": "Associate", 
          "example": "Afterwards, so many successful career women came up to me wanting advice.", 
          "video": ""
          }, 
          {
          "word": "Careerist", 
          "synonym": "Stubborn and determined people.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/l"
          }, 
          {
          "word": "Careworn", 
          "synonym": "Mournful", 
          "example": "Her mother, who couldn't have been much more than 30, looked old and careworn.", 
          "video": "https://www.youtube.com/embed/DN6csbAWWJw"
          }, 
          {
          "word": "Cargo", 
          "synonym": "Transportation", 
          "example": "The ship was carrying a cargo of wood.", 
          "video": "https://www.youtube.com/embed/V"
          }, 
          {
          "word": "Carmine", 
          "synonym": "Maroon", 
          "example": "To avoid any renderings too literal or ironic, Robbie traded carmine lips for a swipe of rose, the hue also applied along cheekbones.", 
          "video": "https://www.youtube.com/embed/IjXfjzQxXE4"
          }, 
          {
          "word": "Carnage", 
          "synonym": "Fatal", 
          "example": "The Battle of the Somme was a scene of dreadful carnage.", 
          "video": ""
          }, 
          {
          "word": "Carnival", 
          "synonym": "Amusement arcade", 
          "example": "There's a real carnival atmosphere in the streets.", 
          "video": "https://www.youtube.com/embed/Jo"
          }, 
          {
          "word": "Carnivore", 
          "synonym": "Omnivore", 
          "example": "Lions and tigers are carnivores.", 
          "video": "https://www.youtube.com/embed/pr7Wu05H8no"
          }, 
          {
          "word": "Carol", 
          "synonym": "Singing", 
          "example": "'Silent Night' is my favorite Christmas carol.", 
          "video": "https://www.youtube.com/embed/Z0Z3QHmciU8"
          }, 
          {
          "word": "Carp", 
          "synonym": "Prosecute", 
          "example": "He always craps against her.", 
          "video": "https://www.youtube.com/embed/WxlsLCQ"
          }, 
          {
          "word": "Carriage", 
          "synonym": "Cart", 
          "example": "The Queen's carriage headed the procession.", 
          "video": "https://www.youtube.com/embed/oBZjK5ON2o8"
          }, 
          {
          "word": "Carriage", 
          "synonym": "Coach,bogie", 
          "example": "The front carriage of the train is for first", 
          "video": "https://www.youtube.com/embed/oBZjK5ON2o8"
          }, 
          {
          "word": "Carrion", 
          "synonym": "Meat", 
          "example": "A crow wheeled over the hills in search of carrion.", 
          "video": "https://www.youtube.com/embed/qUN6VFYPsN0"
          }, 
          {
          "word": "Carry a torch for sb", 
          "synonym": "Infatuation", 
          "example": "Terry has been carrying a torch for Liz for years, but she seems not to notice.", 
          "video": "https://www.youtube.com/embed/COyDP9dJXM4"
          }, 
          {
          "word": "Carry on", 
          "synonym": "Behaving, interacting and behaviour.", 
          "example": "The children have been carrying on all day.", 
          "video": "https://www.youtube.com/embed/3ovY8h58MoA"
          }, 
          {
          "word": "Carry out", 
          "synonym": "Succeeding, achieving and fulfilling.", 
          "example": "According to witnesses, the robbery was carried out by two teenage boys.", 
          "video": "https://www.youtube.com/embed/8K7YNbobngM"
          }, 
          {
          "word": "Carry over", 
          "synonym": "Delaying and wasting time.", 
          "example": "The performance has had to be carried over to/till next week because the repairs to the theatre aren't finished yet.", 
          "video": "https://www.youtube.com/embed/EGDlpaVLV7o"
          }, 
          {
          "word": "Carry sb through sth", 
          "synonym": "", 
          "example": "He was a real friend to see me through my long illness.", 
          "video": ""
          }, 
          {
          "word": "Carry sth forward", 
          "synonym": "Core.", 
          "example": "The players are relaxing now in the restrooms, who are the nucleus of the cricket team.", 
          "video": ""
          }, 
          {
          "word": "Carry sth off", 
          "synonym": "", 
          "example": "My sister failed to carry off the gold medal.", 
          "video": ""
          }, 
          {
          "word": "Carry sth on", 
          "synonym": "Engage in, Conduct, Undertake.", 
          "example": "He could not carry on a logical conversation.", 
          "video": ""
          }, 
          {
          "word": "Carry sth out", 
          "synonym": "", 
          "example": "Mr. Mahmud is carrying out his research on Discourse Analysis.", 
          "video": ""
          }, 
          {
          "word": "Carry sth over", 
          "synonym": "To use or do something at a later time.", 
          "example": "I try not to let my problems at work carry over into my private life.", 
          "video": ""
          }, 
          {
          "word": "Carry sth through", 
          "synonym": "", 
          "example": "It is doubtful whether it will be possible to carry through the education reforms.", 
          "video": ""
          }, 
          {
          "word": "Carry the can.", 
          "synonym": "", 
          "example": "The author didn't turn up for the interview and his agent had to carry the can.", 
          "video": ""
          }, 
          {
          "word": "Carry the torch for", 
          "synonym": "", 
          "example": "He's been carrying the torch for Julie since their college days, before she married Ted.", 
          "video": ""
          }, 
          {
          "word": "Carry weight", 
          "synonym": "", 
          "example": "I'm glad she's on our side", 
          "video": "https://www.youtube.com/embed/S47jdHZC"
          }, 
          {
          "word": "Carry", 
          "synonym": "", 
          "example": "The children have been carrying on all day.", 
          "video": ""
          }, 
          {
          "word": "Cart before the horse", 
          "synonym": "", 
          "example": "Building a school before knowing the age of the population is putting the cart before the horse.", 
          "video": "https://www.youtube.com/embed/B"
          }, 
          {
          "word": "Carte blanche", 
          "synonym": "", 
          "example": "The landlord has given her carte blanche to redecorate her apartment.", 
          "video": ""
          }, 
          {
          "word": "Carve out a niche", 
          "synonym": "", 
          "example": "In today's competitive market it is better to carve out a niche and try to become the best in that area.", 
          "video": ""
          }, 
          {
          "word": "Carve sth out", 
          "synonym": "", 
          "example": "Can he carve a bowl out of such soft wood?", 
          "video": ""
          }, 
          {
          "word": "Carve sth up", 
          "synonym": "", 
          "example": "I will carve you up if you don’t let me play.", 
          "video": ""
          }, 
          {
          "word": "Carve sth up", 
          "synonym": "", 
          "example": "It's tradition for my dad to carve up the beef by his own.", 
          "video": ""
          }, 
          {
          "word": "Carved in stone", 
          "synonym": "", 
          "example": "These proposals are for discussion, they're not carved in stone.", 
          "video": ""
          }, 
          {
          "word": "Carver", 
          "synonym": "", 
          "example": "He used to have his own carver for Qurbani Eid.", 
          "video": ""
          }, 
          {
          "word": "Carvery", 
          "synonym": "", 
          "example": "In this hotel, meat carvery buffet offers a choice of various mouthwatering dishes.", 
          "video": ""
          }, 
          {
          "word": "Cascade", 
          "synonym": "", 
          "example": "Various improvements at the base of the cascade, are being built nowadays.", 
          "video": ""
          }, 
          {
          "word": "Cash cow", 
          "synonym": "", 
          "example": "His latest invention turned out to be a real cash cow.", 
          "video": "https://www.youtube.com/embed/xe4YT"
          }, 
          {
          "word": "Cash in your chips", 
          "synonym": "", 
          "example": "Andy cashed in his chips as soon as business started to slow down.", 
          "video": "https://www.youtube.com/embed/rD6HWZbyJ0g from 1:55 second to 2:07 second"
          }, 
          {
          "word": "Cash in your chips", 
          "synonym": "", 
          "example": "Siam cashed in his chips as soon as business started to slow down.", 
          "video": ""
          }, 
          {
          "word": "Cash", 
          "synonym": "", 
          "example": "Cash", 
          "video": ""
          }, 
          {
          "word": "Casserole", 
          "synonym": "", 
          "example": "Casseroles are used for the food cooked and served in our home.", 
          "video": ""
          }, 
          {
          "word": "Cast a look/glance", 
          "synonym": "", 
          "example": "She cast a quick look in the rear mirror.", 
          "video": ""
          }, 
          {
          "word": "Cast a spell", 
          "synonym": "Incantation, Enchantment, Magic spell, Magic charm", 
          "example": "The drama showed that she cast a spell over her husband.", 
          "video": ""
          }, 
          {
          "word": "Cast aspersions on sb/sth", 
          "synonym": "", 
          "example": "I'm sorry to cast aspersions on Sabina, but her work ethic is really terrible.", 
          "video": ""
          }, 
          {
          "word": "Cast doubt on sb/sth", 
          "synonym": "", 
          "example": "She cast doubt on the integrity of her boss.", 
          "video": ""
          }, 
          {
          "word": "Cast iron stomach", 
          "synonym": "", 
          "example": "You must have a cast", 
          "video": "https://www.youtube.com/embed/Yy51PKdQErQ"
          }, 
          {
          "word": "Cast light on sth", 
          "synonym": "", 
          "example": "We've hired a private investigator to help cast light on the Sagor", 
          "video": ""
          }, 
          {
          "word": "Cast pearls before swine", 
          "synonym": "", 
          "example": "Do not cast your pearls before swine.", 
          "video": ""
          }, 
          {
          "word": "Cast your eye over sth", 
          "synonym": "", 
          "example": "Alim cast his eye over his notes again.", 
          "video": ""
          },
          {
          "word": "Cast your eye over sth", 
          "synonym": "", 
          "example": "Could you cast an eye over this report for me?", 
          "video": ""
          }, 
          {
          "word": "Cast your mind back", 
          "synonym": "", 
          "example": "He cast his mind back to the fatal evening.", 
          "video": ""
          }, 
          {
          "word": "Cast your net wide", 
          "synonym": "", 
          "example": "The security forces are casting their net wider.", 
          "video": ""
          }, 
          {
          "word": "Cast your vote", 
          "synonym": "", 
          "example": "His granddaughter cast her vote for the first time.", 
          "video": ""
          }, 
          {
          "word": "Cast/shed/throw light on  sth", 
          "synonym": "Defining & explaining.", 
          "example": "As an economist, he was able to shed some light on the problem.", 
          "video": "https://www.youtube.com/embed/hefdrylnKZ0"
          }, 
          {
          "word": "Cat nap", 
          "synonym": "", 
          "example": "I am going to have cat nap while you are cooking dinner.", 
          "video": ""
          }, 
          {
          "word": "Catch twenty two", 
          "synonym": "", 
          "example": "I can't get a job without a work permit, and I can't get a work permit without a job.  It's a catch 22 situation!", 
          "video": "https://www.youtube.com/embed/imS"
          }, 
          {
          "word": "Catch up on", 
          "synonym": "", 
          "example": "Can someone catch me up on the latest developments?", 
          "video": "https://www.youtube.com/embed/MxudAGFlUtw"
          }, 
          {
          "word": "Catch up with", 
          "synonym": "Suggestions & proposals.", 
          "example": "We'll think about a present for her and see what we can come up with.", 
          "video": "https://www.youtube.com/embed/anzGRNgbMTA"
          }, 
          {
          "word": "Catch your breath.", 
          "synonym": "Recover.", 
          "example": "I had to stop running to catch my breath.", 
          "video": ""
          }, 
          {
          "word": "Cat’s got one’s tongue", 
          "synonym": "", 
          "example": "It looks like the cat’s got your tongue, Lucy. Are you always this quiet?", 
          "video": ""
          }, 
          {
          "word": "Caught in the crossfire", 
          "synonym": "", 
          "example": "The Health Minister, who resigned today, claims she is an innocent victim caught in the crossfire of the current battle over inflation.", 
          "video": ""
          }, 
          {
          "word": "Caught with one’s pants down", 
          "synonym": "", 
          "example": "My students caught me with my pants down on Monday. I forgot about the field trip.", 
          "video": ""
          }, 
          {
          "word": "Cause a stir", 
          "synonym": "", 
          "example": "The arrival of the actress caused quite a stir in the village.", 
          "video": ""
          }, 
          {
          "word": "Champ at the bit", 
          "synonym": "", 
          "example": "The press conference was delayed for such a long time that the journalists were champing at the bit.", 
          "video": ""
          }, 
          {
          "word": "Chance in a million", 
          "synonym": "", 
          "example": "There's a chance in a million of finding the key I lost on the golf course.", 
          "video": "https://www.youtube.com/embed/yTTnfaLHUgc"
          }, 
          {
          "word": "Chance oneís arm", 
          "synonym": "", 
          "example": "Tony knew there was little hope of getting into Harvard but he decided to chance his arm anyway.", 
          "video": ""
          }, 
          {
          "word": "Chance one’s arm", 
          "synonym": "", 
          "example": "Tony knew there was little hope of getting into Harvard but he decided to chance his arm anyway.", 
          "video": ""
          }, 
          {
          "word": "Chance your arm", 
          "synonym": "", 
          "example": "If you really want something you have to chance your arm.", 
          "video": ""
          }, 
          {
          "word": "Chancy", 
          "synonym": "", 
          "example": "Life is good if you avoid chancy situations.", 
          "video": "https://www.youtube.com/embed/Vpp203g0FKg"
          }, 
          {
          "word": "Chandelier", 
          "synonym": "", 
          "example": "The grand chandelier at the castle weighs a tonne.", 
          "video": "https://www.youtube.com/embed/6aXUz0DIeUE"
          }, 
          {
          "word": "Chandler", 
          "synonym": "", 
          "example": "Chandler are very common around docks.", 
          "video": "https://www.youtube.com/embed/aDuyp9hsgZw"
          }, 
          {
          "word": "Change for the better", 
          "synonym": "", 
          "example": "Replacing paper for digital record is a change for the better.", 
          "video": ""
          }, 
          {
          "word": "Change hands", 
          "synonym": "", 
          "example": "The car I have is really old and had changed hands many times.", 
          "video": ""
          }, 
          {
          "word": "Change of heart", 
          "synonym": "", 
          "example": "He was against charity, but he had a change of heart when he saw the plight of the homeless.", 
          "video": ""
          }, 
          {
          "word": "Change of scene", 
          "synonym": "", 
          "example": "Change of scene might help you feel better.", 
          "video": ""
          }, 
          {
          "word": "Change over", 
          "synonym": "", 
          "example": "We changed over from paper to digital record keeping.", 
          "video": ""
          }, 
          {
          "word": "Change places", 
          "synonym": "", 
          "example": "Lucy and Susan changed places with in the company.", 
          "video": ""
          }, 
          {
          "word": "Change something round", 
          "synonym": "", 
          "example": "The lab looks different since you moved the equipment around.", 
          "video": ""
          }, 
          {
          "word": "Change your mind", 
          "synonym": "", 
          "example": "I was going to go sailing but I changed my mind  when I saw the weather.", 
          "video": "https://www.youtube.com/embed/CXdkw"
          }, 
          {
          "word": "Change your tack", 
          "synonym": "", 
          "example": "Since direct method is not working try changing your tack.", 
          "video": ""
          }, 
          {
          "word": "Change your tune", 
          "synonym": "", 
          "example": "Ever since the mad antics of the president his voters have changed their tune.", 
          "video": ""
          }, 
          {
          "word": "Change your ways", 
          "synonym": "", 
          "example": "You are a very naughty child, you should change your ways", 
          "video": ""
          }, 
          {
          "word": "Changeable", 
          "synonym": "Inconstant, unfixed", 
          "example": "The weather was very changeable last summer.", 
          "video": "https://www.youtube.com/embed/3C_oqJuJKP4"
          }, 
          {
          "word": "Changed man", 
          "synonym": "", 
          "example": "John is no longer leading a life of crime, he is a changed man.", 
          "video": ""
          }, 
          {
          "word": "Channel", 
          "synonym": "", 
          "example": "We have 300 channels but nothing good to watch.", 
          "video": "https://www.youtube.com/embed/rgJHWcSTpHU"
          }, 
          {
          "word": "Chant", 
          "synonym": "", 
          "example": "The protestors where chanting anti government slogans outside.", 
          "video": "https://www.youtube.com/embed/WkPxvONrI8g"
          }, 
          {
          "word": "Chaos", 
          "synonym": "", 
          "example": "The was a chaos at school after a boy brought his pet snake to class.", 
          "video": "https://www.youtube.com/embed/JCa21U3xma0"
          }, 
          {
          "word": "Chapped", 
          "synonym": "", 
          "example": "Use a lot of petroleum gel in winter to avoid chapped lips.", 
          "video": "https://www.youtube.com/embed/RMsZzYR0HmI"
          }, 
          {
          "word": "Chaps", 
          "synonym": "", 
          "example": "Cowboys wore chaps otherwise their clothes wouldnít last very long.", 
          "video": "https://www.youtube.com/embed/dQX"
          }, 
          {
          "word": "Charade", 
          "synonym": "", 
          "example": "Stop this charade, I know non of you really want to go to the picnic!", 
          "video": "https://www.youtube.com/embed/1ehPBnjc"
          }, 
          {
          "word": "Chariot", 
          "synonym": "", 
          "example": "Egyptians and Roman used chariots to conquer their neighbouring countries.", 
          "video": "https://www.youtube.com/embed/joPbNtjMRgQ"
          }, 
          {
          "word": "Charisma", 
          "synonym": "", 
          "example": "John has such charisma that he can slack off and no one ever minds.", 
          "video": "https://www.youtube.com/embed/cne6sPHLhk0"
          }, 
          {
          "word": "Charity begins at home", 
          "synonym": "", 
          "example": "You should really help your poor sister, charity begins at home.", 
          "video": ""
          }, 
          {
          "word": "Charlatan", 
          "synonym": "", 
          "example": "Dr. Ranjit is a Charlatan and a quack! He nearly killed me with his stupidity.", 
          "video": "https://www.youtube.com/embed/W6NAylBQBLE"
          }, 
          {
          "word": "Charleston", 
          "synonym": "", 
          "example": "Many people still dance the Charleston at clubs.", 
          "video": "https://www.youtube.com/embed/Vr3uoNSCpdQ"
          }, 
          {
          "word": "Charley horse", 
          "synonym": "", 
          "example": "I got a bad Charley Horse after swimming for an hour.", 
          "video": "https://www.youtube.com/embed/14CTFGxNX9k"
          }, 
          {
          "word": "Charnel", 
          "synonym": "", 
          "example": "I once went inside a charnel and there was an eerie atmosphere.", 
          "video": "https://www.youtube.com/embed/GprBSQkH"
          }, 
          {
          "word": "Charred", 
          "synonym": "", 
          "example": "The house fire charred my prized book collection.", 
          "video": "https://www.youtube.com/embed/KyRZoPNrfjg"
          }, 
          {
          "word": "Charter", 
          "synonym": "", 
          "example": "Australia is so big and empty charter planes are the best way to travel.", 
          "video": "https://www.youtube.com/embed/cBUwkevJUMo"
          }, 
          {
          "word": "Charter", 
          "synonym": "", 
          "example": "Many companies have charter dictating their code of conduct.", 
          "video": "https://www.youtube.com/embed/cBUwkevJUMo"
          }, 
          {
          "word": "Chary", 
          "synonym": "", 
          "example": "Donít be so chary about this, just do it and you will feel better.", 
          "video": "https://www.youtube.com/embed/1LTA4tDhtbI"
          }, 
          {
          "word": "Chase your own tail", 
          "synonym": "", 
          "example": "He's been chasing his tail all week collecting data but the report is still  not ready.", 
          "video": ""
          }, 
          {
          "word": "Chase", 
          "synonym": "", 
          "example": "I was chasing him but could not catch him as he was too fast.", 
          "video": "https://www.youtube.com/embed/M"
          }, 
          {
          "word": "Chasing rainbows", 
          "synonym": "", 
          "example": "She's trying to get into Oxford, but I think she's chasing rainbows.", 
          "video": ""
          }, 
          {
          "word": "Chasm", 
          "synonym": "", 
          "example": "Mountain climber die mostly due to falling down chasms.", 
          "video": "https://www.youtube.com/embed/zyiMkpyuVwE"
          }, 
          {
          "word": "Chasten", 
          "synonym": "", 
          "example": "Teacher and parent tend to chasten children rather than just ignore them.", 
          "video": "https://www.youtube.com/embed/IYe"
          }, 
          {
          "word": "Chastise", 
          "synonym": "", 
          "example": "I was chastised for doing my presentation poorly.", 
          "video": "https://www.youtube.com/embed/c3p08rsFnAM"
          }, 
          {
          "word": "Chattel", 
          "synonym": "", 
          "example": "I walked around with my chattel during my vacations, hotel rooms are not as safe as you think.", 
          "video": "https://www.youtube.com/embed/m5xJcM"
          }, 
          {
          "word": "Chatty", 
          "synonym": "", 
          "example": "Susan is a chatty girl but she means well.", 
          "video": "https://www.youtube.com/embed/__Bc2Zn58FQ"
          }, 
          {
          "word": "Chatty", 
          "synonym": "Talkative,communicative", 
          "example": "Both Mr.Brown and Peter are chatty and not afraid of the camcorder.", 
          "video": "https://www.youtube.com/embed/uuAOnS5ntRU"
          }, 
          {
          "word": "Chauffeur", 
          "synonym": "", 
          "example": "The chauffeur of the limo rang our door bell during prom night.", 
          "video": "https://www.youtube.com/embed/lCtApc65hgg"
          }, 
          {
          "word": "Chauvinist", 
          "synonym": "", 
          "example": "Most older men from a previous generation are chauvinist.", 
          "video": "https://www.youtube.com/embed/q6gjHBglS8I"
          }, 
          {
          "word": "Cheap and cheerful", 
          "synonym": "", 
          "example": "The little thrift shop down the street is cheap and cheerful.", 
          "video": ""
          }, 
          {
          "word": "Cheap and nasty", 
          "synonym": "", 
          "example": "The razor I bought from the street vendor was cheap and nasty.", 
          "video": ""
          }, 
          {
          "word": "Cheap at half the price", 
          "synonym": "", 
          "example": "That wedding gown was cheap at half the price!", 
          "video": ""
          }, 
          {
          "word": "Cheapen", 
          "synonym": "", 
          "example": "Donít cheapen our friendship by making it about money.", 
          "video": "https://www.youtube.com/embed/Hosy92dmv3M"
          }, 
          {
          "word": "Cheat death", 
          "synonym": "", 
          "example": "I was almost ran over by that bus, talk about cheating death!", 
          "video": ""
          }, 
          {
          "word": "Cheat somebody out of something", 
          "synonym": "", 
          "example": "Robert cheated Lisa out of her hard work.", 
          "video": ""
          }, 
          {
          "word": "Check in", 
          "synonym": "", 
          "example": "I checked in to the hotel right after my flight.", 
          "video": ""
          }, 
          {
          "word": "Check in", 
          "synonym": "Arrivals and departures.", 
          "example": "You'll be unpopular with the airport staff if you don't check in on time.", 
          "video": "https://www.youtube.com/embed/XET9O1YeUOY"
          }, 
          {
          "word": "Check out", 
          "synonym": "", 
          "example": "Check out that new drone on the store window.", 
          "video": ""
          }, 
          {
          "word": "Check out", 
          "synonym": "", 
          "example": "The hotel manager was kind enough to help me during checking out.", 
          "video": ""
          }, 
          {
          "word": "Check out", 
          "synonym": "Hotels & hostels.", 
          "example": "I noticed an elderly lady at reception checking out when we came down for breakfast.", 
          "video": "https://www.youtube.com/embed/AUSn1LtNDKk"
          }, 
          {
          "word": "Check something off", 
          "synonym": "", 
          "example": "Now that my project work is complete I can check it off.", 
          "video": ""
          }, 
          {
          "word": "Check up on somebody", 
          "synonym": "", 
          "example": "My mum checks up on me most evenings to see that I've done my homework.", 
          "video": ""
          }, 
          {
          "word": "Cheddar", 
          "synonym": "", 
          "example": "Most burger have cheddar cheese in them.", 
          "video": "https://www.youtube.com/embed/gN0EjVdWuLc"
          }, 
          {
          "word": "Cheek", 
          "synonym": "", 
          "example": "The cold made my sonís cheeks turn red.", 
          "video": "https://www.youtube.com/embed/LfU01zxTD1c"
          }, 
          {
          "word": "Cheer somebody on", 
          "synonym": "", 
          "example": "My father always cheered me on to follow my dream of becoming an artist.", 
          "video": ""
          }, 
          {
          "word": "Cheer somebody up", 
          "synonym": "", 
          "example": "My mother always tries to cheer me up when I am down.", 
          "video": ""
          }, 
          {
          "word": "Cheer up", 
          "synonym": "Dreamy, ducky.", 
          "example": "He tried to cheer her up but found himself unequal to the task.", 
          "video": "https://www.youtube.com/embed/2NNDFb54Ado"
          }, 
          {
          "word": "Cheesed off", 
          "synonym": "", 
          "example": "I barely spoke to him all night, so I don’t know why he’s cheesed off.", 
          "video": ""
          }, 
          {
          "word": "Chequered", 
          "synonym": "", 
          "example": "I think I will wear the chequered shit Monday morning.", 
          "video": "https://www.youtube.com/embed/Ht3nmlpv190"
          }, 
          {
          "word": "Cherish", 
          "synonym": "", 
          "example": "I cherish my childhood friends as they are the best.", 
          "video": "https://www.youtube.com/embed/fTug8L26Mws"
          }, 
          {
          "word": "Chew over something", 
          "synonym": "", 
          "example": "Before you buy the car chew it over first.", 
          "video": ""
          }, 
          {
          "word": "Chew somebody out", 
          "synonym": "", 
          "example": "The boss chewed out Steve for his mistakes.", 
          "video": ""
          }, 
          {
          "word": "Chew someone out", 
          "synonym": "", 
          "example": "The coach has already chewed out two of his swimmers for arriving late to practice.", 
          "video": "https://www.youtube.com/embed/Rd5F2U8Nvuo"
          }, 
          {
          "word": "Chew something up", 
          "synonym": "", 
          "example": "He chewed through the budget in one week!", 
          "video": ""
          }, 
          {
          "word": "Chew the fat", 
          "synonym": "", 
          "example": "When you are young you tend to chew the fat with every kid on the playground.", 
          "video": ""
          }, 
          {
          "word": "Chic", 
          "synonym": "", 
          "example": "Mary is know for her chic attires.", 
          "video": ""
          }, 
          {
          "word": "Chick flick", 
          "synonym": "", 
          "example": "Chick flicks are Roberts guilty pleasure.", 
          "video": ""
          }, 
          {
          "word": "Chick lit", 
          "synonym": "", 
          "example": "Chick lit is a growing industry these days.", 
          "video": ""
          }, 
          {
          "word": "Chicken feed", 
          "synonym": "", 
          "example": "I got a job during the holidays but the pay was chicken feed.", 
          "video": "https://www.youtube.com/embed/lSpS5okiEaM"
          }, 
          {
          "word": "Chicken out", 
          "synonym": "", 
          "example": "I was going to take a ride Geoff’s Motorcycle, but I chickened out when he gave me a helmet to wear.", 
          "video": ""
          }, 
          {
          "word": "Chicken out", 
          "synonym": "", 
          "example": "Sean chicken out at the last second and did not jump off the cliff.", 
          "video": ""
          }, 
          {
          "word": "Chide", 
          "synonym": "", 
          "example": "Russell chided the gardener for insubordination.", 
          "video": ""
          }, 
          {
          "word": "Child benefit", 
          "synonym": "", 
          "example": "Child benefit sometime cover the rent of the house.", 
          "video": ""
          }, 
          {
          "word": "Child", 
          "synonym": "", 
          "example": "Early morning cartoons are usually child", 
          "video": ""
          }, 
          {
          "word": "Childproof", 
          "synonym": "", 
          "example": "We are childproofing my house due frequent visits from my niece.", 
          "video": ""
          }, 
          {
          "word": "Children should be seen and not heard", 
          "synonym": "", 
          "example": "You kids are being too noisy. Children should be seen and not heard.", 
          "video": ""
          }, 
          {
          "word": "Chill out", 
          "synonym": "", 
          "example": "Chill out and have a beer.", 
          "video": ""
          }, 
          {
          "word": "Chill somebody to the bone", 
          "synonym": "", 
          "example": "This is a film that will chill you to the marrow.", 
          "video": ""
          }, 
          {
          "word": "Chill wind of something", 
          "synonym": "", 
          "example": "Many building companies are facing the chill wind of the recession.", 
          "video": ""
          }, 
          {
          "word": "Chill wind.", 
          "synonym": "", 
          "example": "Many building companies are facing the chill wind of the recession.", 
          "video": ""
          }, 
          {
          "word": "Chilled", 
          "synonym": "", 
          "example": "Charlie is very nice and a chilled person.", 
          "video": "https://www.youtube.com/embed/aoz"
          }, 
          {
          "word": "Chilly", 
          "synonym": "", 
          "example": "The attic was chilly as there was no heating.", 
          "video": ""
          }, 
          {
          "word": "Chilly", 
          "synonym": "Snowy, frosty", 
          "example": "Apart from everything mentioned, the worst thing was the fact that our coach broke down in the middle of nowhere on a chilly rainy day.", 
          "video": "https://www.youtube.com/embed/mN1CMPw0QOo"
          }, 
          {
          "word": "Chin up", 
          "synonym": "", 
          "example": "Chin up! Just because of a small set back you shouldnít give up.", 
          "video": ""
          }, 
          {
          "word": "Chinese whispers.", 
          "synonym": "", 
          "example": "Chinese whispers is a great game it's always hilarious to see what the last person has interpreted by the end!", 
          "video": "https://www.youtube.com/embed/dba5dgoxDhs"
          }, 
          {
          "word": "Chink in somebodyís armour", 
          "synonym": "", 
          "example": "A single chink in our armour at the negotiating table means we could lose out badly.", 
          "video": ""
          }, 
          {
          "word": "Chink", 
          "synonym": "", 
          "example": "There was a chink in the steel door.", 
          "video": "https://www.youtube.com/embed/TqAQK"
          }, 
          {
          "word": "Chink", 
          "synonym": "", 
          "example": "There was a sharp chick when the metal plates hit each other.", 
          "video": "https://www.youtube.com/embed/TqAQK"
          }, 
          {
          "word": "Chip in", 
          "synonym": "", 
          "example": "Might I chip in an say that you are doing a great job.", 
          "video": ""
          }, 
          {
          "word": "Chip in", 
          "synonym": "Interrupting & preventing from speaking", 
          "example": "I'll start and you can all chip in with your comments.", 
          "video": "https://www.youtube.com/embed/DvS_TR"
          }, 
          {
          "word": "Chip off the old block", 
          "synonym": "", 
          "example": "James is a chip off the old block", 
          "video": "https://www.youtube.com/embed/pR"
          }, 
          {
          "word": "Chip on his shoulder", 
          "synonym": "", 
          "example": "Sheís not going to make any friends if she walks around with a chip on her shoulder like that.", 
          "video": ""
          }, 
          {
          "word": "Chip on your shoulder", 
          "synonym": "", 
          "example": "He's got a chip on his shoulder because he's from a working", 
          "video": ""
          }, 
          {
          "word": "Chip something in", 
          "synonym": "", 
          "example": "We all chipped in money to give the school new sport equipment.", 
          "video": ""
          }, 
          {
          "word": "Chippy", 
          "synonym": "", 
          "example": "The boys are being chippy because they lost to us girls.", 
          "video": ""
          }, 
          {
          "word": "Chirpy", 
          "synonym": "Jubilant", 
          "example": "She seemed quite chirpy this morning.", 
          "video": "https://www.youtube.com/embed/3"
          }, 
          {
          "word": "Chivalrous", 
          "synonym": "Gentlemanly", 
          "example": "Example", 
          "video": "https://www.youtube.com/embed/5pC5lQlV4LI"
          }, 
          {
          "word": "Chock", 
          "synonym": "Burst", 
          "example": "The whole room was chock", 
          "video": "https://www.youtube.com/embed/KoWfxAkPjW4"
          }, 
          {
          "word": "Chock", 
          "synonym": "Crowded", 
          "example": "The streets were chock", 
          "video": "https://www.youtube.com/embed/G2nHoP4WYL4"
          }, 
          {
          "word": "Chocoholic", 
          "synonym": "Maniac", 
          "example": "Nine out of ten chocoholics are women.", 
          "video": "https://www.youtube.com/embed/q1jt7eIb96U"
          }, 
          {
          "word": "Choke sth back", 
          "synonym": "Controlling emotions.", 
          "example": "Choking back my anger, I tried to speak calmly.", 
          "video": ""
          }, 
          {
          "word": "Choleric", 
          "synonym": "Furious", 
          "example": "Jeanne was a choleric person and a miser.", 
          "video": "https://www.youtube.com/embed/KPt1Fi3Fl"
          }, 
          {
          "word": "Chomp", 
          "synonym": "Bite.", 
          "example": "He was chomping away on a bar of chocolate.", 
          "video": "https://www.youtube.com/embed/CvVwRN"
          }, 
          {
          "word": "Chop sth down", 
          "synonym": "Cut sth down", 
          "example": "Most of the diseased trees were chopped down last year.", 
          "video": ""
          }, 
          {
          "word": "Chop sth off", 
          "synonym": "Disconnect", 
          "example": "Two of his fingers were chopped off in the accident.", 
          "video": ""
          }, 
          {
          "word": "Chop", 
          "synonym": "Fast and rapid.", 
          "example": "Come on, chop", 
          "video": "https://www.youtube.com/embed/6P"
          }, 
          {
          "word": "Chore", 
          "synonym": "Duty, task", 
          "example": "I find cooking a real chore.", 
          "video": "https://www.youtube.com/embed/T41bhhCzK_s"
          }, 
          {
          "word": "Chore", 
          "synonym": "Labor", 
          "example": "I'll go shopping when I've done my chores.", 
          "video": "https://www.youtube.com/embed/T41bhhCzK_s"
          }, 
          {
          "word": "Chortle", 
          "synonym": "Amused", 
          "example": "She chortled with glee at the news.", 
          "video": "https://www.youtube.com/embed/rBg4Tcg7ENM"
          }, 
          {
          "word": "Chorus", 
          "synonym": "Song form", 
          "example": "They burst into a chorus of Happy Birthday.", 
          "video": "https://www.youtube.com/embed/nqTGzCBZruM"
          }, 
          {
          "word": "Chow down", 
          "synonym": "", 
          "example": "The puppy started chowing down the minute I set down his food bowl.", 
          "video": "https://www.youtube.com/embed/ZRqHzr2nbdg?t=8s"
          }, 
          {
          "word": "Chronic", 
          "synonym": "very bad.", 
          "example": "She suffers from chronic pain in her knees.", 
          "video": "https://www.youtube.com/embed/oVuudsfDako"
          }, 
          {
          "word": "Chronicle", 
          "synonym": "Journal", 
          "example": "Chronicles create a timeline of events, which is implicitly important in both storytelling and historical writing.", 
          "video": "https://www.youtube.com/embed/G7V6FdjyVg8"
          }, 
          {
          "word": "Chronology", 
          "synonym": "Quality time", 
          "example": "I'm not sure of the chronology of events.", 
          "video": "https://www.youtube.com/embed/DJsqlX60JHQ"
          }, 
          {
          "word": "Chubby", 
          "synonym": "Fatty", 
          "example": "Chubby cheeks, dimpled chin.", 
          "video": "https://www.youtube.com/embed/i"
          }, 
          {
          "word": "Chuck sb out", 
          "synonym": "Kick", 
          "example": "He'd been chucked out of a club for fighting.", 
          "video": "https://www.youtube.com/embed/RmqOe2fsGnc"
          }, 
          {
          "word": "Chuck sb under the chin", 
          "synonym": "Affectionate", 
          "example": "'Cheer up,' she said and chucked the little girl under the chin.", 
          "video": ""
          }, 
          {
          "word": "Chuck sth away", 
          "synonym": "Banish", 
          "example": "I've chucked out all my old clothes.", 
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
          }, 
          {
          "word": "Crescendo", 
          "synonym": "Accidental, adagio.", 
          "example": "The music reached a crescendo.", 
          "video": "https://www.youtube.com/embed/KM14a0KF5hA"
          }, 
          {
          "word": "Crescent", 
          "synonym": "Arch, circular.", 
          "example": "The moon was a brightly shining crescent.", 
          "video": "https://www.youtube.com/embed/8eC5QlNe86I"
          }, 
          {
          "word": "Cress", 
          "synonym": "Alfalfa, allium.", 
          "example": "Cultivation of garden cress is practical on both mass scales and on the individual scale.", 
          "video": "https://www.youtube.com/embed/kkNTKKUZOrg"
          }, 
          {
          "word": "Crest                              PICTURE", 
          "synonym": "", 
          "example": "A royal crest.", 
          "video": "https://www.youtube.com/embed/oocV76bN4g4"
          }, 
          {
          "word": "Crest                              TOP", 
          "synonym": "Edges & extremities of objects.", 
          "example": "The crest of a hill/wave.", 
          "video": "https://www.youtube.com/embed/oocV76bN4g4"
          }, 
          {
          "word": "Crest of the wave", 
          "synonym": "", 
          "example": "Our company is going from success to success.  We're on the crest of a wave right now.", 
          "video": ""
          }, 
          {
          "word": "Crest of the wave", 
          "synonym": "", 
          "example": "Our company is going from success to success.  We're on the crest of a wave right now.", 
          "video": ""
          }, 
          {
          "word": "Crestfallen", 
          "synonym": "Feeling sad and unhappy.", 
          "example": "He looked crestfallen at their decision.", 
          "video": "https://www.youtube.com/embed/NkkuljVFdtU"
          }, 
          {
          "word": "Cretin", 
          "synonym": "Stupid and silly people.", 
          "example": "These cretins are peculiarly a feeble", 
          "video": ""
          }, 
          {
          "word": "Crevasse", 
          "synonym": "Geography: caves, cracks & crevices.", 
          "example": "A particular configuration of rope, anchors, and pulleys typically used to extricate a climber after falling into a crevasse.", 
          "video": "https://www.youtube.com/embed/ewnYxpYT7OY"
          }, 
          {
          "word": "Crevice", 
          "synonym": "Cave, cavern.", 
          "example": "The harsh light revealed every crevice and wrinkle in his face.", 
          "video": "https://www.youtube.com/embed/TMmteZGcS3M"
          }, 
          {
          "word": "Crew cut", 
          "synonym": "Barnet, blowout.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/n7o_iqOYjl8"
          }, 
          {
          "word": "Crew neck", 
          "synonym": "Armhole, bodice.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/rQm4sJ9PyKM"
          }, 
          {
          "word": "Crewmember", 
          "synonym": "People who work on boats & ships.", 
          "example": "All crew members should return to the ship by 6 a.m.", 
          "video": ""
          }, 
          {
          "word": "Cri de coeur", 
          "synonym": "Foreign words & phrases used in English.", 
          "example": "The homeless issue is a cri de coeur for myself.", 
          "video": "https://www.youtube.com/embed/aNHG9zWnDCw"
          }, 
          {
          "word": "Crib                                 BED", 
          "synonym": "Beds & parts of beds.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/RMhl5MTVUIo"
          }, 
          {
          "word": "Crib                                 HOME", 
          "synonym": "Accommodation, address.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/RMhl5MTVUIo"
          }, 
          {
          "word": "Crick", 
          "synonym": "Disorders of muscles & the nervous system.", 
          "example": "I got a crick in my neck from painting the ceiling.", 
          "video": "https://www.youtube.com/embed/hI76J6OHB3k"
          }, 
          {
          "word": "Cricket                             INSECT", 
          "synonym": "", 
          "example": "Male crickets are mated with females, in order to fine", 
          "video": "https://www.youtube.com/embed/wtlbAElzCTE"
          }, 
          {
          "word": "Crikey", 
          "synonym": "Expressions of surprise.", 
          "example": "The General don't bark much, he remarked, 'but, crikey, don't he know how to bite!'", 
          "video": "https://www.youtube.com/embed/y1sR"
          }, 
          {
          "word": "Crime doesn't pay", 
          "synonym": "Punishing & punishments.", 
          "example": "", 
          "video": ""
          }, 
          {
          "word": "Crime wave", 
          "synonym": "", 
          "example": "He concludes that changes in genetic factors obviously can not explain the crime wave.", 
          "video": "https://www.youtube.com/embed/uH"
          }, 
          {
          "word": "Crimp", 
          "synonym": "", 
          "example": "Crimp edges of the hamburgers all around to hold in the cheese when it melts and begins to run.", 
          "video": "https://www.youtube.com/embed/s5xsik_98X0"
          }, 
          {
          "word": "Cringe", 
          "synonym": "", 
          "example": "I cringed when I realized what Iíd said.", 
          "video": "https://www.youtube.com/embed/aZmPwPSn6Oc"
          }, 
          {
          "word": "Crinkle", 
          "synonym": "", 
          "example": "She crinkled up her nose in distaste.", 
          "video": "https://www.youtube.com/embed/PQC9WgxpBss"
          }, 
          {
          "word": "Cripes", 
          "synonym": "", 
          "example": "That's more reasonable than the sheepherder story, by cripes!", 
          "video": "https://www.youtube.com/embed/MQjdh5rUzk8"
          }, 
          {
          "word": "Cripple", 
          "synonym": "", 
          "example": "The accident crippled him.", 
          "video": "https://www.youtube.com/embed/sYg61rM7xEc"
          }, 
          {
          "word": "Crisis of confidence", 
          "synonym": "", 
          "example": "With inflation at 500 percent, the country faces a crisis of confidence.", 
          "video": ""
          }, 
          {
          "word": "Crisp                         FOOD", 
          "synonym": "", 
          "example": "I like apple crisp.", 
          "video": "https://www.youtube.com/embed/llNJbj"
          }, 
          {
          "word": "Crisp", 
          "synonym": "", 
          "example": "A packet of salt and vinegar crisps.", 
          "video": "https://www.youtube.com/embed/llNJbj"
          }, 
          {
          "word": "Crisp", 
          "synonym": "", 
          "example": "I like crisp cake.", 
          "video": "https://www.youtube.com/embed/llNJbj"
          }, 
          {
          "word": "Crisp", 
          "synonym": "", 
          "example": "The sound from the new speakers is very crisp.", 
          "video": "https://www.youtube.com/embed/llNJbj"
          }, 
          {
          "word": "Crisp", 
          "synonym": "", 
          "example": "a wonderful crisp spring morning.", 
          "video": "https://www.youtube.com/embed/llNJbj"
          }, 
          {
          "word": "Criss", 
          "synonym": "", 
          "example": "This area of the city is criss", 
          "video": "https://www.youtube.com/embed/hotCoIRJNbE"
          }, 
          {
          "word": "Criteria", 
          "synonym": "", 
          "example": "We have strict criteria for deciding which students will receive a grant.", 
          "video": ""
          }, 
          {
          "word": "Critical mass", 
          "synonym": "", 
          "example": "The challenge is to attract a critical mass of customers that will enable the business to start making a profit.", 
          "video": "https://www.youtube.com/embed/M5V2X2d1f_s"
          }, 
          {
          "word": "Critical", 
          "synonym": "", 
          "example": "Both drivers are critical/in a critical condition = so badly hurt that they might die after the 120 mph crash.", 
          "video": "https://www.youtube.com/embed/B3WCd3PIsJ4"
          }, 
          {
          "word": "Critical", 
          "synonym": "", 
          "example": "She has written a major critical appraisal/study of Saul Bellow's novels.", 
          "video": "https://www.youtube.com/embed/B3WCd3PIsJ4"
          }, 
          {
          "word": "Critical", 
          "synonym": "", 
          "example": "The president's support is critical to this project.", 
          "video": "https://www.youtube.com/embed/B3WCd3PIsJ4"
          }, 
          {
          "word": "Critical", 
          "synonym": "", 
          "example": "The report is highly critical of safety standards at the factory.", 
          "video": "https://www.youtube.com/embed/B3WCd3PIsJ4"
          }, 
          {
          "word": "Critter", 
          "synonym": "A creature.", 
          "example": "He was the healthiest critter ever I see and the laziest.", 
          "video": "https://www.youtube.com/embed/B"
          }, 
          {
          "word": "Croak                             DIE", 
          "synonym": "Slang. to die.", 
          "example": "He had a heart attack and croaked.", 
          "video": "https://www.youtube.com/embed/TQ4M0uGw0bk"
          }, 
          {
          "word": "Croak                            SOUND", 
          "synonym": "", 
          "example": "His sudden croak let us know that he wanted to speak.", 
          "video": "https://www.youtube.com/embed/TQ4M0uGw0bk"
          }, 
          {
          "word": "Crochet", 
          "synonym": "", 
          "example": "When he returned from the store, Dale usually found his mother sitting by the lamp crocheting.", 
          "video": "https://www.youtube.com/embed/pje9RF"
          }, 
          {
          "word": "Crock", 
          "synonym": "", 
          "example": "He keeps his coffee in an earthenware crock.", 
          "video": "https://www.youtube.com/embed/60Jr"
          }, 
          {
          "word": "Crock", 
          "synonym": "", 
          "example": "You are a crock.", 
          "video": "https://www.youtube.com/embed/60Jr"
          }, 
          {
          "word": "Crockery", 
          "synonym": "", 
          "example": "The store sells gift items such as crockery and soaps.", 
          "video": "https://www.youtube.com/embed/nRo5Y1wcibY"
          }, 
          {
          "word": "Crocodile                LINE", 
          "synonym": "", 
          "example": "Will the UK scheme to walk a crocodile of children to school give them independence", 
          "video": "https://www.youtube.com/embed/KLJn1uLb"
          }, 
          {
          "word": "Crocodile tears", 
          "synonym": "", 
          "example": "We do not need to weep crocodile tears: we need action.", 
          "video": "https://www.youtube.com/embed/OTQfI1mN6so"
          }, 
          {
          "word": "Crocus", 
          "synonym": "", 
          "example": "On the pulpit stood a bunch of crocuses crowded into a vase: some Mary's offering.", 
          "video": "https://www.youtube.com/embed/qyHU7zrcFU0"
          }, 
          {
          "word": "Croft", 
          "synonym": "", 
          "example": "The proceedings are similar in the case of a privately", 
          "video": "https://www.youtube.com/embed/MlkHnrrRLls"
          }, 
          {
          "word": "Croissant", 
          "synonym": "", 
          "example": "Pick up some croissants for breakfast tomorrow.", 
          "video": "https://www.youtube.com/embed/a"
          }, 
          {
          "word": "Cromlech", 
          "synonym": "", 
          "example": "The cromlech was used as a calendar to mark the seasons and/or as a sanctuary for tribal divinities.", 
          "video": "https://www.youtube.com/embed/jUH3VmNNUng"
          }, 
          {
          "word": "Crone", 
          "synonym": "", 
          "example": "Gold and silver, and each thing more precious than another, in the crone's castle.", 
          "video": "https://www.youtube.com/embed/hOyAgV8OTTY"
          }, 
          {
          "word": "Crony", 
          "synonym": "", 
          "example": "The general and his cronies are now awaiting trial for drug smuggling.", 
          "video": "https://www.youtube.com/embed/_bBhT1Ek_74"
          }, 
          {
          "word": "Crook", 
          "synonym": "", 
          "example": "Especially crook carried by a shepherd or a bishop.", 
          "video": "https://www.youtube.com/embed/grUqfpnlWEI"
          }, 
          {
          "word": "Crook", 
          "synonym": "", 
          "example": "He crooked a finger for the waitress.", 
          "video": "https://www.youtube.com/embed/grUqfpnlWEI"
          }, 
          {
          "word": "Crook", 
          "synonym": "", 
          "example": "These politicians are just a bunch of crooks.", 
          "video": "https://www.youtube.com/embed/grUqfpnlWEI"
          }, 
          {
          "word": "Crooner", 
          "synonym": "", 
          "example": "The song is in the crooners style.", 
          "video": "https://www.youtube.com/embed/15bxfLJ2g4M"
          }, 
          {
          "word": "Crop up", 
          "synonym": "", 
          "example": "Her name keeps cropping up in conversation.", 
          "video": "https://www.youtube.com/embed/IIhPUTwngXg"
          }, 
          {
          "word": "Crop", 
          "synonym": "", 
          "example": "Grain is stored in their crops and ground by the grit in their gizzard.", 
          "video": "https://www.youtube.com/embed/0UU2OnHi8YU"
          }, 
          {
          "word": "Crop", 
          "synonym": "", 
          "example": "Her hair was cut in a short crop.", 
          "video": "https://www.youtube.com/embed/0UU2OnHi8YU"
          }, 
          {
          "word": "Crop", 
          "synonym": "", 
          "example": "Horse are afraid of crop.", 
          "video": "https://www.youtube.com/embed/0UU2OnHi8YU"
          }, 
          {
          "word": "Crop", 
          "synonym": "", 
          "example": "The judges will select the best from this year's crop of first novels.", 
          "video": "https://www.youtube.com/embed/0UU2OnHi8YU"
          }, 
          {
          "word": "Crop", 
          "synonym": "", 
          "example": "The main crops grown for export are coffee and rice.", 
          "video": "https://www.youtube.com/embed/0UU2OnHi8YU"
          }, 
          {
          "word": "Croquette                FOOD", 
          "synonym": "", 
          "example": "Be sure the croquettes are well covered, then fry brown.", 
          "video": "https://www.youtube.com/embed/Zomp_LjuhNc"
          }, 
          {
          "word": "Crosier", 
          "synonym": "A crozier", 
          "example": "Abbots, abbesses and bishops were buried with their crosiers , the pastoral staffs symbolic of their office.", 
          "video": "https://www.youtube.com/embed/cvMp1GImKRY"
          }, 
          {
          "word": "Cross                       MAKE MARK", 
          "synonym": "", 
          "example": "Cut a cross in the bark with a sharp knife.", 
          "video": "https://www.youtube.com/embed/kd7ZLHX_9ao"
          }, 
          {
          "word": "Cross              BEHAVIOUR", 
          "synonym": "", 
          "example": "she's just a cross we have to bear.", 
          "video": "https://www.youtube.com/embed/kd7ZLHX_9ao"
          }, 
          {
          "word": "Cross my heart and hope to die", 
          "synonym": "", 
          "example": "I'll clean my room tomorrow cross my heart.", 
          "video": "https://www.youtube.com/embed/IimhtX957dE"
          }, 
          {
          "word": "Cross out", 
          "synonym": "Erase, rub.", 
          "example": "If you think it's wrong, cross it out and write it again.", 
          "video": "https://www.youtube.com/embed/m6iD9PaNLbE"
          }, 
          {
          "word": "Cross sb's hand/palm with silver", 
          "synonym": "", 
          "example": "He cross his palm with silver to know his future.", 
          "video": ""
          }, 
          {
          "word": "Cross sb/sth off  sth ", 
          "synonym": "", 
          "example": "Did you cross her name off the guest list?", 
          "video": ""
          }, 
          {
          "word": "Cross swords", 
          "synonym": "", 
          "example": "The board members crossed swords in the selection of a president.", 
          "video": ""
          }, 
          {
          "word": "Cross that bridge when we come to it.", 
          "synonym": "", 
          "example": "'What will happen if we can't repay the loan?' 'We'll cross that bridge when we come to it.'", 
          "video": "https://www.youtube.com/embed/QjfIfP7_VFU"
          }, 
          {
          "word": "Cross to bear.", 
          "synonym": "", 
          "example": "Alzheimer's is a cross to bear for the whole family.", 
          "video": ""
          }, 
          {
          "word": "Cross your arms/fingers/legs", 
          "synonym": "", 
          "example": "She sat down and crossed her legs.", 
          "video": ""
          }, 
          {
          "word": "Cross your fingers", 
          "synonym": "", 
          "example": "I'm just going to cross my fingers and hope it works.", 
          "video": "https://www.youtube.com/embed/xEUqYyXhUEs"
          }, 
          {
          "word": "Cross your fingers", 
          "synonym": "", 
          "example": "I'm just going to cross my fingers and hope it works.", 
          "video": "https://www.youtube.com/embed/uavc_LHwVj4?t=5s"
          }, 
          {
          "word": "Cross your mind", 
          "synonym": "", 
          "example": "It crossed my mind  that the child might be hungry.", 
          "video": "https://www.youtube.com/embed/r3xGfLn3Eak"
          }, 
          {
          "word": "Cross your mind", 
          "synonym": "", 
          "example": "What was the first thing that crossed your mind when you won the prize?", 
          "video": "https://www.youtube.com/embed/LIo5i0"
          }, 
          {
          "word": "Cross yourself", 
          "synonym": "", 
          "example": "Ted said thanks for the evening and Mary crossed herself and invoked some sort of biblical curse.", 
          "video": ""
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "A cross", 
          "video": "https://www.youtube.com/embed/vfC6qtsxGIo"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "After university we bought a camper van and travelled cross", 
          "video": "https://www.youtube.com/embed/lMkYyqXq6xc"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "Athlete always prefare cross", 
          "video": ""
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "Defense attorneys cross", 
          "video": "https://www.youtube.com/embed/8In7HfLzypc"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "Entries are fully cross", 
          "video": "https://www.youtube.com/embed/8vswNgUoEz0"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "He is cross", 
          "video": "https://www.youtube.com/embed/cXtUM1jRBMw"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "I wouldn't cross him if I were you, not if you value your life.", 
          "video": "https://www.youtube.com/embed/kd7ZLHX_9ao"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "In the greenhouse a hive of bees is kept so that cross", 
          "video": "https://www.youtube.com/embed/tL1YJfPI_BE"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "John sat cross", 
          "video": "https://www.youtube.com/embed/X91XNmNIIw0"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "Police dogs are often a cross between a retriever and a German Shepherd.", 
          "video": "https://www.youtube.com/embed/kd7ZLHX_9ao"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "The company uses its TV shows to cross", 
          "video": "https://www.youtube.com/embed/OPgJ2JUsgQE"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "The region is defined by diagonal cross", 
          "video": "https://www.youtube.com/embed/TtuRua_z6kw"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "Their database is used to cross", 
          "video": "https://www.youtube.com/embed/Hpke7IzWfSU"
          }, 
          {
          "word": "Cross", 
          "synonym": "", 
          "example": "Work the border in cross", 
          "video": "https://www.youtube.com/embed/D9N5GOvYuGI"
          }, 
          {
          "word": "Crossbones", 
          "synonym": "Skull and crossbones.", 
          "example": "The skull and crossbones was the best one.", 
          "video": "https://www.youtube.com/embed/u3WFw0JEcNY"
          }, 
          {
          "word": "Crossbow", 
          "synonym": "", 
          "example": "Another form of this sport is shooting with crossbows at a target.", 
          "video": "https://www.youtube.com/embed/aK_ke4rxHRY"
          }, 
          {
          "word": "Crossbreed", 
          "synonym": "", 
          "example": "In animal breeding, 'crossbreed' describes crosses within a single species, while 'hybrid' refers to crosses between different species.", 
          "video": "https://www.youtube.com/embed/kwPSybToERg"
          }, 
          {
          "word": "Crosscheck", 
          "synonym": "", 
          "example": "Always try to cross", 
          "video": "https://www.youtube.com/embed/0Uu"
          }, 
          {
          "word": "Crossfire", 
          "synonym": "", 
          "example": "One boat of refugees was caught in the naval crossfire and sunk.", 
          "video": "https://www.youtube.com/embed/razrZ_636ss"
          }, 
          {
          "word": "Crossover", 
          "synonym": "", 
          "example": "Thereís been a lot of crossover from comic books to movies.", 
          "video": "https://www.youtube.com/embed/uBg4zPb2G1I"
          }, 
          {
          "word": "Crosspatch", 
          "synonym": "Shrew, curmudgeon, discontent.", 
          "example": "I'm a crosspatch to", 
          "video": "https://www.youtube.com/embed/ZyguFP7aLRI"
          }, 
          {
          "word": "Crosswind", 
          "synonym": "", 
          "example": "A strong crosswind gusting to over thirty knots.", 
          "video": "https://www.youtube.com/embed/mbp67k08qz4"
          }, 
          {
          "word": "Crossword puzzle", 
          "synonym": "", 
          "example": "She settled down to do the crossword.", 
          "video": "https://www.youtube.com/embed/k0dWhuzT9KU"
          }, 
          {
          "word": "Crostini", 
          "synonym": "", 
          "example": "Crostini recipe is very sympol.", 
          "video": "https://www.youtube.com/embed/hG6hF22UkZU"
          }, 
          {
          "word": "Crotchet", 
          "synonym": "", 
          "example": "There are then crotchet chords for 15 bars.", 
          "video": "https://www.youtube.com/embed/wS0rb1PleR8"
          }, 
          {
          "word": "Crotchety", 
          "synonym": "", 
          "example": "By the time the meal began, the youngest children were getting tired and crotchety.", 
          "video": "https://www.youtube.com/embed/3epybm6LnsY"
          }, 
          {
          "word": "Crouch", 
          "synonym": "", 
          "example": "She saw him coming and crouched down behind a bush.", 
          "video": "https://www.youtube.com/embed/0ZjnArHrleQ"
          }, 
          {
          "word": "Croup", 
          "synonym": "", 
          "example": "The symptoms of croup stand out differently when compared to other respiratory conditions.", 
          "video": "https://www.youtube.com/embed/6UnPe"
          }, 
          {
          "word": "Croupier", 
          "synonym": "", 
          "example": "I think that there is a difference with the croupier.", 
          "video": "https://www.youtube.com/embed/VVjYn75HvsA"
          }, 
          {
          "word": "Crouton", 
          "synonym": "", 
          "example": "Let boil and serve hot with fried croutons.", 
          "video": "https://www.youtube.com/embed/CZAS_YuCyIs"
          }, 
          {
          "word": "Crow", 
          "synonym": "", 
          "example": "she was awakened in the mornings by cocks crowing.", 
          "video": "https://www.youtube.com/embed/xJVclkYjwT8"
          }, 
          {
          "word": "Crowbar", 
          "synonym": "", 
          "example": "The thieves forced one of the windows open with a crowbar.", 
          "video": "https://www.youtube.com/embed/XXOHBGyC67Y"
          }, 
          {
          "word": "Crowd sth into sth", 
          "synonym": "", 
          "example": "Hordes of commuters crowded into the train.", 
          "video": ""
          }, 
          {
          "word": "Crowd sb/sth out", 
          "synonym": "", 
          "example": "Small local businesses have been crowded out by large multinationals.", 
          "video": ""
          }, 
          {
          "word": "Crux of the matter.", 
          "synonym": "", 
          "example": "The crux of the matter is that he's too old to live alone in that big house.", 
          "video": "https://www.youtube.com/embed/0cOxa3p3U_Q"
          }, 
          {
          "word": "Cry over spilt milk", 
          "synonym": "", 
          "example": "Yes, we made a mistake, but thereís no point in crying over spilled milk.", 
          "video": "https://www.youtube.com/embed/qUwLZRw"
          }, 
          {
          "word": "Cry wolf", 
          "synonym": "", 
          "example": "If you cry wolf too often, people will stop believing you.", 
          "video": "https://www.youtube.com/embed/kXaNqbzK7hU"
          }, 
          {
          "word": "Cry your heart out", 
          "synonym": "", 
          "example": "I cried my heart out out when my best friend moved away.", 
          "video": ""
          }, 
          {
          "word": "Crystal", 
          "synonym": "", 
          "example": "crystal clear water", 
          "video": ""
          }, 
          {
          "word": "CrËme br˚lÈe                  FOOD", 
          "synonym": "Puddings, desserts & ices.", 
          "example": "", 
          "video": "https://www.youtube.com/embed/m9MsdRu5Mnc"
          }, 
          {
          "word": "Cultivate", 
          "synonym": "", 
          "example": "This shrub is cultivated in Europe as a culinary herb.", 
          "video": ""
          }, 
          {
          "word": "Cummerbund", 
          "synonym": "Belt, Sash, Strap.", 
          "example": "A cummerbund is the perfect accessory for a man's tuxedo.", 
          "video": "https://www.youtube.com/embed/gSFITGJ"
          }, 
          {
          "word": "Cumquat", 
          "synonym": "Citrus, Grapefruit, Lemon.", 
          "example": "Add the kumquats to the syrup, lower the heat and poach for 5 minutes.", 
          "video": "https://www.youtube.com/embed/6RghCSL08Fk"
          }, 
          {
          "word": "Cumulonimbus", 
          "synonym": "Cloud, Thundercloud, Mist", 
          "example": "Through the cathedral window I saw dark clouds lined up to the horizon, cumulonimbus hanging like gravid bellies.", 
          "video": "https://www.youtube.com/embed/sr0JbGyPzeM"
          }, 
          {
          "word": "Cumulus", 
          "synonym": "Mound, Heap, Cloud, Pile", 
          "example": "A heap of cumulus clouds drifted, barely visible through the treetops.", 
          "video": "https://www.youtube.com/embed/1tD35DXJp_Y"
          }, 
          {
          "word": "Cunning", 
          "synonym": "Clever, Sly, Shrewd, Tricky", 
          "example": "These disturbed kids can be cunning.", 
          "video": "https://www.youtube.com/embed/qe9X6Wh1Ws8?t=5s"
          }, 
          {
          "word": "Cunning", 
          "synonym": "Foxy, Sharp, Attractive, Pretty", 
          "example": "He is a cunning old character but has got a stunning turn of foot.", 
          "video": "https://www.youtube.com/embed/qe9X6Wh1Ws8?t=5s"
          }, 
          {
          "word": "Cup holder", 
          "synonym": "Case, Container.", 
          "example": "Tossing the hot pan cup holder on the counter, she untied the apron.", 
          "video": "https://www.youtube.com/embed/FFGjDTOyjaE"
          }, 
          {
          "word": "Cup of Joe", 
          "synonym": "", 
          "example": "I am going to the coffee shop for a cup of Joe.", 
          "video": "https://www.youtube.com/embed/GCw6yVprRC4"
          }, 
          {
          "word": "Cup tie", 
          "synonym": "Competition, Game, Match, Race", 
          "example": "Richard had been working for a local paper in Watford and he'd been covering their cup tie with Manchester City.", 
          "video": ""
          }, 
          {
          "word": "Cupful", 
          "synonym": "Bowl, Mug, Teacup, Drink", 
          "example": "Three cupfuls of water.", 
          "video": "https://www.youtube.com/embed/uCLvHBdFP10"
          }, 
          {
          "word": "Cupidity", 
          "synonym": "Craving, Eagerness, Greediness", 
          "example": "Ambition and cupidity were the source of the most deplorable abuses in the Roman Church.", 
          "video": "https://www.youtube.com/embed/Yn4WwG"
          }, 
          {
          "word": "Cupidís bow", 
          "synonym": "Upper lip, Curved shaped, Bow", 
          "example": "Soulful eyes and Cupid's bow lips.", 
          "video": "https://www.youtube.com/embed/Q1pvuzoNf"
          }, 
          {
          "word": "Cupola", 
          "synonym": "Dome, Vault, Belfry", 
          "example": "The cupola of the church in the fortress is 2455 ft.", 
          "video": "https://www.youtube.com/embed/wFHdzFjoO8w"
          }, 
          {
          "word": "Cuppa", 
          "synonym": "Drink of tea, Brew, Cupper", 
          "example": "I've just put the kettle on", 
          "video": "https://www.youtube.com/embed/2vnYuPeDYa4"
          }, 
          {
          "word": "Cur", 
          "synonym": "Coward, Blackground, Creep, Rogue", 
          "example": "He was one of the foremost foes of Piers, who had styled him 'the black cur of Arden,' and with whose death he was closely connected.", 
          "video": "https://www.youtube.com/embed/7jcFO3"
          }, 
          {
          "word": "Cur", 
          "synonym": "Dog, Bounder, Mongrel, Mutt", 
          "example": "The once friendly dog was now a cur, unexpectedly turning on its master.", 
          "video": "https://www.youtube.com/embed/7jcFO3"
          }, 
          {
          "word": "Curate", 
          "synonym": "Minister, Pastor, Priest", 
          "example": "Not only does he curate for the museum, he manages the office and fund", 
          "video": "https://www.youtube.com/embed/"
          }, 
          {
          "word": "Curator", 
          "synonym": "Guardian, Caretaker, Keeper", 
          "example": "She curated the traveling exhibition.", 
          "video": "https://www.youtube.com/embed/1axLVCWnfM8"
          }, 
          {
          "word": "Curb", 
          "synonym": "Control, Restrain, Restrict, Inhibit", 
          "example": "We've got to curb the damage as much as possible.", 
          "video": "https://www.youtube.com/embed/KfqqdLnWKW4?t=5s"
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
          "example": "The project is heading for failure.  Let's cut our losses before it's too late.", 
          "video": ""
          }, 
          {
          "word": "Cut one’s own throat", 
          "synonym": "", 
          "example": "Tony has already missed a lot of classes.  He's cutting his own throat.", 
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
          }, 
          {
          "word": "Dash", 
          "synonym": "Rush, outran.", 
          "example": "The plane dashed away over my head.", 
          "video": "https://www.youtube.com/embed/vstKmvUV_As"
          }, 
          {
          "word": "Dash", 
          "synonym": "Strike, smash.", 
          "example": "The tidal wave dashed the ship against the rocks.", 
          "video": "https://www.youtube.com/embed/vstKmvUV_As"
          }, 
          {
          "word": "Dawn", 
          "synonym": "", 
          "example": "the dawn of civilization", 
          "video": ""
          }, 
          {
          "word": "Dawn", 
          "synonym": "Crack of Dawn, Cock", 
          "example": "The first appearance of light in the sky before sunrise.", 
          "video": "https://www.youtube.com/embed/lj9JwMt8sl4"
          }, 
          {
          "word": "Daydream", 
          "synonym": "", 
          "example": "She just sits in class daydreaming about her horses.", 
          "video": ""
          }, 
          {
          "word": "De facto", 
          "synonym": "", 
          "example": "The society was de facto divided between the rich and the poor", 
          "video": ""
          }, 
          {
          "word": "De trop", 
          "synonym": "Excess, Excessive, Extra , Not wanted , Surplus, Too much , Unwelcome", 
          "example": "She had no grasp of the conversation and felt herself de trop.", 
          "video": ""
          }, 
          {
          "word": "De", 
          "synonym": "", 
          "example": "Robert tried to de", 
          "video": ""
          }, 
          {
          "word": "Dead cert", 
          "synonym": "", 
          "example": "After such praise, his appointment as captain of the team is a dead cert.", 
          "video": ""
          }, 
          {
          "word": "Dead cert", 
          "synonym": "", 
          "example": "After such praise, his appointment as captain of the team is a dead cert.", 
          "video": ""
          }, 
          {
          "word": "Dead duck", 
          "synonym": "", 
          "example": "The new cinema is going to be a dead duck because it's too far away from the town centre.", 
          "video": ""
          }, 
          {
          "word": "Dead duck", 
          "synonym": "", 
          "example": "The new cinema is going to be a dead duck because it's too far away from the town centre.", 
          "video": ""
          }, 
          {
          "word": "Dead in the water", 
          "synonym": "", 
          "example": "Because of the crisis, the planned housing development is now dead in the water.", 
          "video": ""
          }, 
          {
          "word": "Dead in the water", 
          "synonym": "", 
          "example": "Because of the crisis, the planned housing development is now dead in the water.", 
          "video": ""
          }, 
          {
          "word": "Dead loss", 
          "synonym": "", 
          "example": "When it comes to gardening, my brother is a dead loss.", 
          "video": ""
          }, 
          {
          "word": "Dead man walking", 
          "synonym": "", 
          "example": "Because of the way he handled the recent riots, the minister is a dead man walking.", 
          "video": "https://www.youtube.com/embed/2SAbDq63l1Y from 0:21 second"
          }, 
          {
          "word": "Dead man walking.", 
          "synonym": "", 
          "example": "Because of the way he handled the recent riots, the minister is a dead man walking.", 
          "video": ""
          }, 
          {
          "word": "Dead ringer", 
          "synonym": "", 
          "example": "He's a dead ringer for Bono from U2.", 
          "video": "https://www.youtube.com/embed/uYJnPxKfPYs"
          }, 
          {
          "word": "Dead wood", 
          "synonym": "", 
          "example": "The new manager wants to reduce costs by cutting out the dead wood.", 
          "video": ""
          }, 
          {
          "word": "Dead wood", 
          "synonym": "", 
          "example": "The new manager wants to reduce costs by cutting out the dead wood.", 
          "video": "https://www.youtube.com/embed/x1xKGGeLBM8 from 0:08 second"
          }

      ]
    }
  }
};
</script>
