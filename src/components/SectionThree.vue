<template>
  <div class="section" id="sectionThree">
    <h2>Disappointments</h2>
    <div class="content">
      <!-- Displaying content dynamically based on the selected item -->
      <p v-if="selectedItem === ''" class = "message"> Select a Sports Person to View their Disappointments</p>
      <p v-if="selectedItem === 'Messi'">
       <ul>
        <li>June 30, 2006: Being Left on the Bench in the FIFA World Cup Quarter-Finals</li>
        <li>August 25, 2006: Losing the UEFA Super Cup Final</li>
        <li>July 15, 2007: Coming Up Short in the Copa América Final</li>
        <li>March 4, 2008: Another Thigh Injury</li>
        <li>April 29, 2008: UEFA Champions League Semi-Final Misery</li>
        <li>June 12- July 3, 2010: Underwhelming FIFA World Cup Campaign</li>
        <li>April 20, 2011: Struggled Against Anti-Football in Copa Del Rey Final</li>
        <li>July 1-16, 2011: Failed to Score in the Copa América</li>
        <li>April 21, 2012: Lionel Messi Did Not Produce with La Liga Title on the Line</li>
        <li>April 24, 2012: Chelsea Is Lionel Messi's Kryptonite</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Ronaldo'">
       <ul>
        <li>Penalty Misses in Crucial Moments</li>
        <li>Inconsistent Performances Across Tournaments</li>
        <li>Limited Success in Major International Competitions</li>
        <li>Struggles Against Top Defensive Teams</li>
        <li>Criticism for Individualistic Play</li>
        <li>Challenges Adapting to Different National Team Systems</li>
        <li>Notable Goal Droughts in Certain International Stages</li>
        <li>Limited Impact in Key Knockout Matches</li>
        <li>Injury Concerns and Absences During Critical Times</li>
        <li>Mixed Performances in High-Pressure Situations</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Lebron James'">
       <ul>
        <li>Olympic Gold Medal Drought</li>
        <li>Falling Short in FIBA World Championships</li>
        <li>Inconsistent Three-Point Shooting</li>
        <li>Struggles in Clutch Moments</li>
        <li>Limited Success in International Club Competitions</li>
        <li>Defensive Lapses on the Global Stage</li>
        <li>Mixed Performances in All-Star Games Abroad</li>
        <li>Challenges Adapting to Different Rule Sets</li>
        <li>Pressure Handling Criticism on International Platforms</li>
        <li>Unmet Expectations in Various Exhibition Games</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Virat Kohli'">
       <ul> 
        <li>Century Drought in 2019</li>
        <li>2014 Tour of England</li>
        <li>2014 T20 World Cup Final</li>
        <li>2018 Test Series in England</li>
        <li>2016 T20 World Cup Semifinal</li>
        <li>2017 Champions Trophy Final</li>
        <li>2020 IPL Captaincy with RCB</li>
        <li>2015 Test Series in Australia</li>
        <li>2017 Test Series in South Africa</li>
        <li>2019 ODI World Cup Semifinal</li>
       </ul>  
      </p>
      <p v-else-if="selectedItem === 'Roger Federer'">
       <ul>
        <li>Early Exit at 2018 US Open</li>
        <li>Defeat in 2019 Wimbledon Final</li>
        <li>Loss in 2020 Australian Open Semifinals</li>
        <li>Withdrawal from 2021 French Open</li>
        <li>Elimination in 2017 US Open Quarterfinals</li>
        <li>Missed Opportunity at 2016 Rio Olympics</li>
        <li>Upset in 2015 Wimbledon Final</li>
        <li>Setback in 2014 US Open Semifinals</li>
        <li>Early Departure at 2013 Australian Open</li>
        <li>Injury-forced Withdrawal from 2012 ATP Finals</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Rafael Nadal'">
       <ul>
        <li>Early Exit at Wimbledon</li>
        <li>Olympic Setback</li>
        <li>Australian Open Defeat</li>
        <li>Unsuccessful US Open Campaign</li>
        <li>Masters 1000 Upset</li>
        <li>Davis Cup Disappointment</li>
        <li>Clay Court Setback</li>
        <li>ATP Finals Exit</li>
        <li>Injury Interruption</li>
        <li>Grand Slam Miss</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'John Cena'">
       <ul>
        <li>International Wrestling Setbacks</li>
        <li>Unsuccessful Championship Defenses</li>
        <li>Tag Team Disappointments</li>
        <li>Injuries Impacting Global Performances</li>
        <li>Missed Opportunities on the Global Stage</li>
        <li>International Title Match Losses</li>
        <li>Unexpected Defeats in Global Tournaments</li>
        <li>Challenges Overcome by International Opponents</li>
        <li>High-Profile Match Disappointments Abroad</li>
        <li>Global Crowd Letdowns</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Tiger Woods'">
       <ul>
        <li>2008 Ryder Cup Loss</li>
        <li>2010 Ryder Cup Struggles</li>
        <li>2012 Ryder Cup Defeat</li>
        <li>2016 Ryder Cup Setback</li>
        <li>2018 Open Championship Performance</li>
        <li>2018 Ryder Cup Challenges</li>
        <li>2019 Presidents Cup Outcome</li>
        <li>2020 Masters Tournament Setback</li>
        <li>2021 Open Championship Struggles</li>
        <li>2022 Ryder Cup Disappointment</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Patrick Mahomes'">
       <ul>
        <li>Subpar Performance in Crucial Playoff Game</li>
        <li>Struggles in International Exhibition Matches</li>
        <li>Inconsistent Form during International Tournaments</li>
        <li>Difficulty Adapting to Diverse Defensive Strategies</li>
        <li>Below-Expectation Stats in Key International Clashes</li>
        <li>Limited Impact in High-Stakes Global Competitions</li>
        <li>Challenges Against Top-tier International Defenses</li>
        <li>Notable Lapses in Decision-Making on the International Stage</li>
        <li>Inability to Secure Signature Wins in Global Competitions</li>
        <li>Issues with Sustaining Peak Performance in International Play</li>
       </ul>
      </p>
      <p v-else-if="selectedItem === 'Usain Bolt'">
       <ul>
        <li>2017 World Championships 100m Final</li>
        <li>2017 World Championships 4x100m Relay Final</li>
        <li>2015 World Championships 100m Final</li>
        <li>2015 World Championships 4x100m Relay Final</li>
        <li>2008 Beijing Olympics 4x100m Relay Final</li>
        <li>2011 World Championships 100m Final</li>
        <li>2011 World Championships 4x100m Relay Final</li>
        <li>2016 Rio Olympics 100m Final</li>
        <li>2016 Rio Olympics 4x100m Relay Final</li>
        <li>2013 World Championships 100m Final</li>
       </ul>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Section3',
  props: {
    selectedItem: String,
  },
};
</script>

<style scoped>
/* Add styles for Section 3 */
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
  padding: 20px;
 }

.content {
}
</style>
