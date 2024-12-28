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
   </div>
