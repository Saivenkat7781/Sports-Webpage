<template>
  <div class="section" id="sectionTwo">
    <h2>Achievements</h2>
    <div class="content">
      <!-- Displaying content dynamically based on the selected item -->
      <p v-if="selectedItem === ''" class = "message"> Select a Sports Person to View their achivements</p>
      <p v-if="selectedItem === 'Messi'">
      <ul>
      <li>FIFA World Cup 2022</li>
      <li>Olympic gold at Beijing 2008</li>
      <li>All-time leading goalscorer: 106</li>
      <li>Most international caps: 178</li>
      <li>Most goals for a South American nation: 106</li>
      <li>Youngest Argentinian to score at a World Cup: 18 years 357 days</li>
      <li>First player to score in four different World Cup tournaments for Argentina</li>
      <li>Most individual World Cup appearances: 26</li>
      <li>Most Argentina World Cup goals: 13</li>
      <li>Only player to score in World Cup group stage, round of 16, quarterfinals, semifinals and final</li>
      </ul>
      </p>
      <p v-else-if="selectedItem === 'Ronaldo'">
       <ul> 
        <li>UEFA European Championship Title (2016)</li>
        <li>UEFA Nations League Title (2019)</li>
        <li>All-time Top Scorer for Portugal:</li>
        <li>Five-time Ballon d'Or Winner</li>
        <li>UEFA European Championship All-Time Top Scorer</li>
        <li>Most Goals in a UEFA European Championship Qualification Campaign.</li>
        <li>Portugal's Captain and Leader</li>
        <li>FIFA World Cup Appearances</li>
        <li>Portugal's All-Time Appearances Leader</li>
        <li>Consistent Goal-scoring Record:</li>
       </ul> 
      </p>
      <p v-else-if="selectedItem === 'Lebron James'">
       <ul> 
        <li>UEFA European Championship Title (2016)</li>
        <li>Olympic Gold Medalist (2008, 2012, 2016)</li>
        <li>FIBA World Championship Gold Medalist (2007)</li>
        <li>Olympic All-Tournament Team (2008, 2012, 2016)</li>
        <li>USA Basketball Male Athlete of the Year (2012)</li>
        <li>NBA Global Games Ambassador</li>
        <li>NBA China Games Ambassador</li>
        <li>NBA Cares Ambassador to the Philippines</li>
        <li>NBA Cares Ambassador to South Africa</li>
        <li>NBA Cares Ambassador to Brazil</li>
        <li>NBA Cares Ambassador to Mexico</li>
      </ul> 
      </p>
      <p v-else-if="selectedItem === 'Virat Kohli'">
       <ul>
        <li>Fastest Player to Reach 8,000, 9,000, 10,000, 11,000, and 12,000 Runs in ODI Cricket.</li>
        <li>First Cricketer to Score 20,000 International Runs in a Single Decade.</li>
        <li>Fastest Century by an Indian Batsman in ODIs.</li>
        <li>Most Runs in a Single IPL Season.</li>
        <li>First Indian Captain to Win a Test Series in Australia.</li>
        <li>Fastest to 8,000 Runs in International T20 Cricket.</li>
        <li>Most Centuries in a Calendar Year by an Indian Batsman.</li>
        <li>Fastest Batsman to Score 8,000 Runs in ODIs.</li>
        <li>First Player to Score Four Consecutive Centuries in IPL.</li>
        <li>Fastest Batsman to Reach 10,000 Runs in ODIs.</li>
       </ul> 
      </p>
      <p v-else-if="selectedItem === 'Roger Federer'">
       <ul>
        <li>20 Grand Slam Singles Titles</li>
        <li>8 Wimbledon Championships</li>
        <li>6 Australian Open Championships</li>
        <li>5 US Open Championships</li>
        <li>1 French Open Championship</li>
        <li>Olympic Gold Medal (Doubles, 2008)</li>   
        <li>ATP Tour World Championships (6 Titles)</li>
        <li>302 Weeks as World No. 1 in Men's Singles</li>
        <li>28 Consecutive Quarterfinals in Grand Slam Tournaments</li>
        <li>Record 20 Consecutive Grand Slam Semifinal Appearances</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Rafael Nadal'">
       <ul>
        <li>20 Grand Slam Singles Titles</li>
        <li>8 Wimbledon Championships</li>
        <li>6 Australian Open Championships</li>
        <li>5 US Open Championships</li>
        <li>1 French Open Championship</li>
        <li>Olympic Gold Medal (Doubles, 2008)</li>
        <li>ATP Tour World Championships (6 Titles)</li>
        <li>302 Weeks as World No. 1 in Men's Singles</li>
        <li>28 Consecutive Quarterfinals in Grand Slam Tournaments</li>
        <li>Record 20 Consecutive Grand Slam Semifinal Appearances</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'John Cena'">
       <ul>
        <li>WWE World Heavyweight Champion (16-time)</li>
        <li>WWE United States Champion (5-time)</li>
        <li>WWE Tag Team Champion (4-time)</li>
        <li>Royal Rumble Winner (2008, 2013)</li>
        <li>Money in the Bank Winner (2012)</li>
        <li>Two-time World Heavyweight Champion</li>
        <li>NXT Champion (1-time)</li>
        <li>WWE Champion of Champions (2013)</li>
        <li>Slammy Award Winner (Multiple Categories)</li>
        <li>Pro Wrestling Illustrated (PWI) Wrestler of the Year (2006, 2007)</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Tiger Woods'">
       <ul>
        <li>Career Grand Slam Winner</li>
        <li>Youngest Masters Champion</li>
        <li>Record Margin of Victory at The Masters</li>
        <li>Four Consecutive Major Wins</li>
        <li>Most Consecutive Weeks as World No. 1 Golfer</li>
        <li>PGA Tour Player of the Year (11 times)</li>
        <li>The Open Championship Record Score</li>
        <li>First Golfer to Win Four Consecutive Grand Slam Titles</li>
        <li>Four-time PGA Championship Winner</li>
        <li>Most Career Prize Money on the PGA Tour</li>
       </ul> 
      </p>
      <p v-else-if="selectedItem === 'Patrick Mahomes'">
       <ul>
        <li>Super Bowl MVP (2020)*</li>
        <li>Super Bowl LIV Champion (2020)</li>
        <li>Pro Bowl Selection (2018, 2019, 2020)</li>
        <li>First Team All-Pro (2018)</li>
        <li>AFC Champion (2019, 2020)</li>
        <li>NFL MVP (2018)</li>
        <li>AFC Offensive Player of the Year (2018, 2019)</li>
        <li>NFL Offensive Player of the Year (2018)</li>
        <li>5000 Yards Passing Club (2018)</li>
        <li>AFC West Champion (2018, 2019, 2020)</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Usain Bolt'">
       <ul>
        <li>Triple Triple at Rio 2016 Olympics</li>
        <li>World Record in 100m, 200m, and 4x100m Relay</li>
        <li>Olympic Gold Medals in Beijing 2008 and London 2012</li>
        <li>Fastest 100m and 200m Times in Olympic History</li>
        <li>11 World Championship Gold Medals</li>
        <li>First Man to Win Consecutive Olympic 100m and 200m Titles</li>
        <li>Fastest 4x100m Relay Split in History</li>
        <li>Laureus World Sportsman of the Year (2009, 2010, 2013, 2017)</li>
        <li>Named IAAF World Athlete of the Year Six Times</li>
        <li>First Man to Hold World Records in 100m, 200m, and 4x100 Relay Simultaneously</li>
       </ul> 
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Section2',
  props: {
    selectedItem: String,
  },
};
</script>

<style scoped>

.section {
  flex: 1;
  overflow-y: auto;
  padding: 20px;
  border: 1px solid #ccc;
  margin: 10px;
  height: 300px; 
  font-family: sans-serif;
}


h2{
  background-color: #B2DFDB;
  font-size: 24px; 
  margin-bottom: 15px; 
}
.message {
  justify-content: center;
  opacity: 0.4;
  font-family: sans-serif;
  text-align: center;
  padding: 20%;
 }
.content {

}
</style>
