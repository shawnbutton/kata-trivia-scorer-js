# Trivia Game Scorer 8 - Bonus
Some questions are two part questions.

Two part questions are in the format `D#a#b`, where `a` = the first answer and `b` is the second answer. `a` and `b` could be `X`, `Y` or a number value.

In order to get any points for those questions they need to get both questions correct (e.g. "Y" or "5"), otherwise they get nothing for those questions.

Examples:

<table>
    <tr>
        <td>Input</td>
        <td>Output</td>
    </tr>
    <tr>
        <td>"D#Y#Y"</td>
        <td>2</td>
    </tr>
    <tr>
        <td>"D#Y#X"</td>
        <td>0</td>
    </tr>
    <tr>
        <td>"D#4#Y"</td>
        <td>5</td>
    </tr>
    <tr>
        <td>"D#4#X"</td>
        <td>0</td>
    </tr>
    <tr>
        <td>"Y,2,D#Y#Y"</td>
        <td>5</td>
    </tr>
</table>

That's it! Ship it!
