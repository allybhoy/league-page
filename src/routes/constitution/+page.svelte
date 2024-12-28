<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneTwo;
    let two, twoOne, twoTwo;
    let three, threeOne, threeTwo;
    let four, fourOne, fourTwo,fourThree,fourThreeOne, fourFour,fourFive,fourFiveOne,fourFiveTwo,fourSix,fourSeven,fourEight,fourNine;
    let five, fiveOne;
    let six,sixOne,sixTwo,sixThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">EARLSTON FANTASY FOOTBALL LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: League Overview</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneOne)}>1.1 Executive Committee</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneTwo)}>1.2 Living Constitution</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: League Financing</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoOne)}>2.1 League Fee</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(twoTwo)}>2.2 Prize Money</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: League Setup and Competition</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>3.1 Playoff Rankings</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeTwo)}>3.2 Playoff(s)</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Rosters and Lineups</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourOne)}>4.1 The Draft</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourTwo)}>4.2 Free Agency</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourThree)}>4.3 Trades</h4>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(fourThreeOne)}>4.3.1 Trade veto</h5>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourFour)}>4.4 Injured Reserve</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourFive)}>4.5 Starting Lineups</h4>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(fourFiveOne)}>4.5.1 Position Designations </h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(fourFiveTwo)}>4.5.2 Substitutions </h5>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourSix)}>4.6 Bye Week Penalties</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourSeven)}>4.7 Active Ownership Requirements</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourEight)}>4.8 Anti-Tank Rules</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourNine)}>4.9 Rescheduled Games</h4>
     <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: Scoring System</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 Points Totals and Final Score</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: Offseason</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixOne)}>6.1 Removing Managers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixTwo)}>6.2 Replacing Managers</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixThree)}>6.3 Replacement Incentive</h4>
    <hr />
<h2 class="sectionHeading" bind:this={one}>Section 1 League Overview</h2>
        <p>Welcome to EFFL, the Earlston Fantasy Football League.</p>
        <p>This is a 12-team league formed in 2013 in the <a href="http://www.redlionearlston.co.uk/">Red Lion Pub</a> (Earlston) by Chris Powell and Alastair Reid.</p>
        <p>The league is designed to be fun with the winner receiving the Earlston Fantasy Football trophy.</p>

        <p>The league is designed to be a competition between owners, but it not a cut-throat league where anything goes.</p>
        <p>The rules described below are designed to act as a guideline for overall league play, and any disputes will be handled by the executive committee of the league.</p>
        <p>Please remember that the overall goal of this league is to have fun and enjoy the game of football.</p>
        <p>If you have any question or concerns, please do not hesitate to ask.</p>

    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Executive Committee</h3>
    
        <p>The executive committee for EFFL consists of:</p>
            <ul>
 	            <li>Commissioner Alastair Reid</li>
 	            <li>Co-Commissioner Chris Powell</li>
            </ul>
        <p>The executive committee will be responsible for resolving all disputes that are not expressly covered by this constitution.</p>
        <p>If a committee member is involved in the dispute, that member will excuse themselves from the decision process.</p>
        <p>While all owners are encouraged to submit suggestions to the committee, the committee's decision on all matters is final.</p>
        <p>The executive committee will also have access to independent arbitration from external fantasy football commissioners known to the commissioner.</p>

    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Living Constitution</h3>
   
        <p>It is important to note that this is a living, breathing constitution that will change and evolve over the lifetime of this league.</p>
        <p>Changes will happen between seasons as often as possible and will be effective from that point moving forward.</p>
        <p>If you have suggestions for changes, please submit them to one of the executive committee members.</p>
<h2 class="sectionHeading" bind:this={two}>Section 2 League Financing</h2>    
        <p>The EFFL no longer charges league fees.</p>
        <p>Previously these covered the cost of the league and generated a small prize fund.</p>
    <h3 class="subSectionHeading" bind:this={twoOne}>2.1 League Fee</h3>
            <p>There are currently no league fees</p>
        <h3 class="subSectionHeading" bind:this={twoTwo}>2.2 Prize Money</h3>
            <p>There are no monetary prizes</p>   
<h2 class="sectionHeading" bind:this={three}>Section 3 League Setup and Competition</h2>
        <p>The EFFL will consist of 12 different teams.</p>
        <p>The schedule for each team will consist of 14 games over 14 weeks.</p>
        <p>Each team will play the other members of the league in weeks 1 through 11 (11 games).</p>
        <p>The final 3 games are against 3 other teams in an allocated 4 team bracket.</p>
        <p>In season 2024, the 4 team brackets were decided using the previous season draft position i.e. Bracket 1 (1,2,3,4) Bracket 2 (5,6,7,8) and Bracket 3 (9,10,11,12).</p>
        <p>Here're the league breakdown and owner names for those who require it:</p>
<table style="height: 1020px" width="755">
<tbody>
<tr>
<td width="172">Team</td>
<td width="153">Owner</td>
<td width="138">Season started</td>
</tr>
<tr>
<td width="172">Tranent Tigers</td>
<td width="153">Nicky</td>
<td width="138">2014</td>
</tr>
<tr>
<td width="172">Kelso 187’s</td>
<td width="153">Euan</td>
<td width="138">2014</td>
</tr>
<tr>
<td width="172">Hillview Patriots</td>
<td width="153">Alan</td>
<td width="138">2021</td>
</tr>
<tr>
<td width="172">Kelsae Avengers</td>
<td width="153">Stuart</td>
<td width="138">2015</td>
</tr>
<tr>
<td width="172">Tweedbank Pirates</td>
<td width="153">Paul</td>
<td width="138">2013 (hiatus 2020-2023)</td>
</tr>
<tr>
<td width="172">Earlstonian Bohemians</td>
<td width="153">Ally</td>
<td width="138">2013</td>
</tr>
<tr>
<td width="172">Kelso Kestrels</td>
<td width="153">Ryan</td>
<td width="138">2017</td>
</tr>
<tr>
<td width="172">SanFranGordon 69ers</td>
<td width="153">Richie</td>
<td width="138">2013</td>
</tr>
<tr>
<td width="172">Earlston Earthquakes</td>
<td width="153">Cozy</td>
<td width="138">2013</td>
</tr>
<tr>
<td width="172">Fog on the Tyne</td>
<td width="153">Stuart</td>
<td width="138">2013</td>
</tr>
<tr>
<td width="172">1st and N10</td>
<td width="153">Duncan</td>
<td width="138">2020</td>
</tr>
<tr>
<td width="172">Nitten Pickaxe</td>
<td width="153">Gav</td>
<td width="138">2013</td>
</tr>
</tbody>
</table>
<p>The Jerman Jaguars, Pilton Panthers, Fife Fire, Oakbank Oddities, Teri Titans and Dodgy Touchdown franchises have been disbanded.</p>
<p>The Mercy Flush, Jimmy's Jerman Jaguars and Ten Stane Nuts were renamed as Tweedbank Pirates, Heidetal Heat/Replacements and SanFran-Gordon 69ers respectively.</p>
    <h3 class="subSectionHeading" bind:this={threeOne}>3.1 Playoff Rankings</h3>
        <p>Teams (where necessary) will be ranked based on the following criteria. If more than one team needs to be ranked then the criteria can be used to eliminate teams into brackets. This will enable further testing of the criteria in isolation with the sole purpose of creating a final ranking for the tied teams:
            <ol>
 	            <li>Overall Winning Percentage</li>
 	            <li>Division Winning Percentage (in division only)</li>
 	            <li>Total Points Scored</li>
 	            <li>Head to Head Result</li>
 	            <li>Total Offensive Points</li>
            </ol>
        </p>
    <h3 class="subSectionHeading" bind:this={threeTwo}>3.2 Playoffs</h3>
        <p>After the completion of the regular season, six teams will make the playoffs. These are selected by order of record. Where division(s) are used, divisional records will be used to decide divisional ranking. division winners will be awarded a playoff spot as the top ranked teams. In Week 15, the 4 lowest ranked teams will play each other, and the 2 highest ranked teams will get a bye. The winners from Week 14 will play the teams with byes in the semi-final championship in Week 16. The winner of each semi-final championship will play each other in the EFFL Super Bowl during Week 17 of the NFL. In all rounds the lowest ranked team will always play the highest ranked team remaining.</p>
    <h2 class="sectionHeading" bind:this={four}>Section 4 Rosters and Lineups</h2> 
        <p>Rosters in EFFL consist of 15 active players from any NFL team plus 1 injured reserve spot and 2 practice squad spots. The maximum number of players in each position is as follows.

QB 3

RB 6

WR 7

TE 3

PK 2

DST 2

No position minimums are set, but line-up criteria is a minimum requirement for active ownership. Only players from the active roster may be used as part of a team's starting lineup. Injury replacements (currently 3) are available on the league site, but these are used within the criteria supplied by Sleeper. It is the responsibility of the owner to ensure they have set these up correctly. Errors will not be rectified. It is imperative the owner notifies the commissioners of any potential issue before the game kicks off if they have any lineup issues.</p>
        <h3 class="subSectionHeading" bind:this={fourOne}>4.1 The Draft</h3>
            <p>The commissioner will designate a draft night each season. Owners are <strong>expected</strong> to attend the main draft in person, but we are able to accommodate remote drafting.

The draft order for the main draft will be determined the previous season's final standings (worst to first) and playoff progression. The draft will be a serpentine order, where the person with the first pick in Round 1 will have the last pick in Round 2 and the first pick in Round 3. When it is the owner's turn to draft, they will have two minutes to make their pick. The commissioner will designate a timekeeper and when the timer expires, an automated pick will be made. Draft picks can be traded, but no owner or team can have fewer than 13 picks in the draft (and vice versa no more than 15).

For the enjoyment of those who can attend the draft absentee owners are expected to autodraft or ask for a league nominated drafter to be supplied. It is the absentee owners responsibility to supply an effective draft plan.</p>
        <h3 class="subSectionHeading" bind:this={fourTwo}>4.2 Free Agency</h3>
            <p>WAIVERS

The EFFL operates a FAAB (Free Agent Acquisition Budget) system for free agency. Each owner is allocated $100 for the season.

In the Sleeper.com system, a waiver is commonly (but not always) a general term for all player adds and drops. The EFFL uses a blind bid waiver request system where at certain points of the NFL week access to players is restricted e.g. players are locked when they play in a game. Sleeper waivers start on Wednesday 0800 AM and are usually resolved at 0810 AM. Dropped players are on waivers for 1 day after any drop from an active roster.</p>
        <h3 class="subSectionHeading" bind:this={fourThree}>4.3 Trades</h3>
            <p>Trading is allowed and encouraged in EFFL, and may be conducted between any owner.

If you are on the receiving end of a trade proposal, you will be notified of the offer on your team page and/or via email or by message. You will be able to click "View Trade" and review whether or not the terms of the trade are acceptable to you. If they are, click "Accept" and your trade will be immediately processed. Only commissioner and/or executive committee can reverse a trade where tanking or non-competitive play is suspected. The committee will not reverse trades due to stupidity or lack of knowledge.

TRADE RULES

The rules for trades in EFFL are as follows:

There is no maximum number of trades that owners can complete in a season.

Trades are processed immediately upon acceptance.

Once your trade clears the review process, the trade will be completed and the players involved in the trade will switch rosters and be available to start for their new teams.

To put a stop to some of the nefarious trade dealings a player who is traded cannot then be traded back to their original team UNLESS that player has been subsequently released to waivers since the first trade.

TRADE DEADLINE

For EFFL, the deadline to complete all trades is by the last game of Week 11.</p>
            <h4 bind:this={fourThreeOne}>4.3.1 Trade Veto</h4>
                <p>The executive committee reserves the right to reverse any trade that they deem inconsistent with league competition and fair-play standards. This veto will only be invoked in extreme cases where it is obvious that one owner is trying to give another owner an unfair advantage. The owners in question may offer reasons why the trade should be allowed, but the decision of the executive committee is final once it has been rendered. If the trade involves a committee member, they may offer reasons for the trade to be allowed will not have a say in the final committee decision.</p>
        <h3 class="subSectionHeading" bind:this={fourFour}>4.4 Injured Reserve</h3>
            <p>During the NFL season, a team may place a player on IR if they appear on their NFL teams Injured Reserve List. The owner may then utilise the blind bid waiver wire process to replace the player on their active roster.
<ol>
 	<li> IR moves are free</li>
 	<li>No free agent who is listed as IR and then drafted or acquired via the waiver wire is eligible for the IR wire (i.e. a player on IR can’t be picked up and stashed on your IR…only active players on your roster are eligible)</li>
 	<li>A team may only have a maximum 3 players on the IR list at any time.</li>
 	<li>The official site for determining a player’s status will be NFL.com</li>
 	<li>A player on the IR list may not be traded to another team</li>
</ol></p>
<p>FREE AGENTS

A free agent is a player who is not currently on a fantasy roster either because that player was not drafted, has not been added to a roster, or has been released by his previous owner and cleared waivers. You can add a free agent player at any time between Wed 0800 until Wed 0759 or the start of that player's game, whichever occurs first. Free Agents dropped during this period and who haven't played in a game are on waivers for 24hrs.

UNDROPPABLE PLAYERS

In order to establish a competitive and balanced EFFL, we use the experts at NFL.com to maintain a regularly updated list of players who cannot be dropped from your roster once they have been acquired. Players on this list are still eligible to be benched or traded, but not dropped or put on waivers. This feature promotes a fair game for all fantasy users by preventing actions that could compromise the integrity of the game.

***There are currently NO UNDROPPABLE players in the EFFL***</p>
        <h3 class="subSectionHeading" bind:this={fourFive}>4.5 Starting Lineups</h3>
            <p>Starting lineups in EFFL will consist as follows:
<ul>
 	<li>1 quarterback</li>
 	<li>1 running back</li>
 	<li>2 wide receivers</li>
 	<li>1 tight end</li>
 	<li>1 flex (running back, wide receiver)</li>
 	<li>1 super-flex (running back, wide receiver or tight end)</li>
 	<li>1 place kicker</li>
 	<li>1 defense / special teams</li>
</ul>
Owners must submit a competitive starting lineup each week. Failure to do so will result in the executive committee taking temporary ownership of the team.</p>
            <h4 bind:this={fourFiveOne}>4.5.1 Position Designation</h4>
                <p>From time to time, the NFL may change their designation of a particular player from one position to another or a player may line up in multiple positions throughout the game. For example, a wide receiver may be switched to a tight end and vice versa. For the purposes of EFFL we will use designations as assigned by the league host site only. Players may only start and score points based on these designations. See the League Scoring section for more details.</p>
            <h4 bind:this={fourFiveTwo}>4.5.2 Substitutions</h4>
                <div class="subBlock">
                <p>It is acceptable for owners before a game to use the Sleeper auto-subs setting for up to 3 players. It is the owners responsibility to understand the limitations of this setting and its valid use. Any errors caused by malfunctions of the underlying system or software (unless auto-fixed by Sleeper) will only be rectified where proof of the malfunction can be provided to the commissioner or committee.</p>
                </div>
        <h3 class="subSectionHeading" bind:this={fourSix}>4.6 Bye Week Penalties</h3>
            <p>Any owner who starts a player that is on a bye week or officially designated as OUT, regardless of intention, the owner will be forced to drop that player from their active roster. The player will become a free agent and will be eligible to be added to any roster, including the original owner, during the normal free agent policy. It is each owner's responsibility to submit a valid lineup each week and no exceptions will be made.</p>
        <h3 class="subSectionHeading" bind:this={fourSeven}>4.7 Active Ownership Requirements</h3>
            <p>Each owner is expected to actively manage their team each week, even if they are eliminated from any playoff consideration. Owners must submit a competitive lineup each week. If an owner does not submit a lineup for two consecutive weeks, the executive committee will have the right to assume control of the team and manage it for the rest of the season. A committee run team will not make any trades and is only allowed to add or drop players if the team cannot field a legal starting lineup due to injury or bye weeks. Any prize money won by a committee-run team will be distributed evenly to the other active owners in the league.</p>
        <h3 class="subSectionHeading" bind:this={fourEight}>4.8 Anti-Tank Rules</h3>
            <p>EFFL is a competitive league, created for the league owners to have fun playing fantasy football. While the competition may be fierce, this is not considered a cut-throat league. In the spirit of competition and league fairness, owners are not allowed to intentionally create a legal starting lineup that gives the opposing team a clear advantage. The executive committee reserves the right to step in and adjust the starting lineup of a team that is clearly trying to intentionally lose a game. If the committee must adjust a team's lineup in two consecutive weeks or for three or more weeks in any one season, the team will be considered inactive and the executive committee may assume ownership of the team as detailed in the active ownership requirements section.</p>
        <h3 class="subSectionHeading" bind:this={fourNine}>4.9 Rescheduled Games</h3>
            <p>In the event of the NFL cancelling a scheduled game(s) before Wednesday 7pm the game and all non IR-COVID players will be treated as on a bye. This means GMs will need to find suitable alternatives WITHOUT the benefit of IR or taxi. Anything after that can be treated as unexpected and you gain the benefit of IR and taxi spots.

In the event of an unanticipated late cancellation then all players participating will be awarded the median score of the respective position pregame top ranked players (fantasy pros consensus). (Top 20 qb, 48 rb, 48 wr, 20 te, 16 pk, 16 DST).

Where a possible late cancellation may occur GMs have the option to place players on temp-IR (IR and/or taxi) and start alternate players in earlier games. However, GMs using this option cannot take advantage of the median scoring option. All rosters must be balanced to roster limits by 11am Tuesday morning.

Where a player plays in 2 or more games in a given league week GMs MUST notify the commissioner of the game in which they wish to accrue points. No notification will result in a default of the first game being counted. If the player is not in a set lineup he will not be able to start for that given week.</p>
    <h2 class="sectionHeading" bind:this={five}>Section 5 Scoring</h2> 
            <p>Scoring in EFFL will be computed to two decimal places. This will allow points to be awarded or deducted for every positive or negative yard and will dramatically reduce the chance of a tie game. Players are awarded fantasy points for each week that they are included in the team's starting lineup. Players may only start at one position in any given week and will only be awarded points as described by their position distinction below.

<strong>OFFENSE</strong>

<strong>Passing Yards: 1 point per 25 yards passing</strong>

<strong>Passing Touchdowns: 4 points</strong>

<strong>Interceptions: -2 points</strong>

<strong>Rushing Yards: 1 point per 10 yards</strong>

Rushing Attempts: 0.1 per attempt

<strong>Rushing Touchdowns: 6 points</strong>

Receptions: 1 point per reception

<strong>Receiving Yards: 1 point per 10 yards</strong>

<strong>Receiving Touchdowns: 6 points</strong>

<strong>Fumble Recovered for a Touchdown: 6 points</strong>

<strong>2-Point Conversions: 2 points</strong>

<strong>Fumbles Lost: -2 points</strong>

<strong>KICKING</strong>

<strong>PAT Made: 1 point</strong>

<strong>FG Made: 0.1 points per yard</strong>

<strong>DEFENSE TEAM</strong>

Opponent Punts: 1

Opponent Fumble Recoveries (Offense/Special Teams): 2

Interceptions Caught: 2

Sacks: 0.5

Blocked Field Goals/Punts: 2

Blocked Extra Points: 1

Safeties (2 and 1 pt): 2 and 1

Opponent 4th Down Stops: 1

Defensive and Special Team TDs: 6

Defensive Conversion returns: 2

Offensive and Special Team Points Against: 12 points -0.5 for each point allowed

<strong>GENERAL SCORING SETTINGS</strong>

<strong>Use Fractional Points: Yes</strong>

<strong>Use Negative Points: Yes</strong>

<strong>HEAD-TO-HEAD SCORING FORMAT</strong>

<strong>The EFFL features head-to-head scoring. Much like the games that take place across the NFL each Sunday, your team will be matched up against another team within your league. Similar to an NFL game being decided on the field with the team scoring the most points earning a win, your fantasy matchup behaves accordingly.</strong>

<strong>Your team will earn points based on the actual statistics and results played out in the NFL that week. If your team earns more points than your opponent, you earn a win in the league standings. Less points? Take a loss. And if your game ends in a tie, you guessed it - a tie in the overall standings. Ties in postseason play are resolved by playoff seeding order i.e. the highest seed advances.</strong></p>
        <h3 class="subSectionHeading" bind:this={fiveOne}>5.1 Points Total and Final Score</h3>
            <p>EFFL will be hosted on <a href="https://sleeper.com/leagues/1136405911293083648">https://sleeper.com/leagues/1136405911293083648</a>. Head to head scoring will be determined each week by the stats from that website. From time to time, the NFL may go back and change the scoring of certain plays later in the week. However, to maintain a sense of fairness and avoid confusion in the league, all head-to-head scoring using Sleeper. Any scoring changes that come out from the NFL after that time will not be applied to the league.</p>
   
    <h2 class="sectionHeading" bind:this={six}>Section 6 Offseason</h2>
            <p>Owners are strongly encouraged to maintain their current contact information. A connection to WhatsApp league chat is usually enough but it’s also helpful to ensure your email on Sleeper is up to date. You should expect to be contacted in July with information about next year's draft. Thanks and welcome to EFFL!</p>
        <h3 bind:this={sixOne}>6.1 Removing Managers</h3>
            <p>Managers who fail to adhere to the rules above and spirit of the league will be removed and replaced. League fees will be refunded, but time involved with the league will not be reimbursed under any circumstances.</p>
    
        <h3 bind:this={sixTwo}>6.2 Replacing Managers</h3>
            <p>When a manager needs to be replaced, the commisiooners will try to find a suitable candidate with some connection to at least a portion of the existing managers. Priority will be placed on managers who are eager to take on a long term commitment and will be very active within the league.</p>
    
        <h3 bind:this={sixThree}>6.3 Replacement Incentive</h3>
            <p>In the event that a manager chooses to quit the league or is removed by a comissioner, an incoming manager may be offered reduced or waived fees</p>
</div>
