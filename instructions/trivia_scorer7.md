# Trivia Game Scorer 7 - Bonus

Some questions are worth bonus points. Bonus questions are prefixed with `"B"`.
They might appear anywhere in the input.

The bonus can never take the score above 100, but the score prior to the bonus being added can still exceed 100.

<table>
    <tr>
        <td>Input</td>
        <td>Output</td>
        <td>Explanation</td>
    </tr>
    <tr>
        <td>"Y,5,B10"</td>
        <td>16</td>
        <td>Bonus is added</td>
    </tr>
    <tr>
        <td>"Y,95,B10"</td>
        <td>100</td>
        <td>Bonus can not take score over 100</td>
    </tr>
    <tr>
        <td>"Y,105,B10"</td>
        <td>106</td>
        <td>Score without bonus can still exceed 100</td>
    </tr>
</table>

[When done proceed to part 8 (bonus #2)](trivia_scorer8.md)
