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
</div>
