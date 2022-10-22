# Structure

## Users

### Experience

<details>
    <summary>User Joins</summary>
    <ul>
        <details>
            <summary>Link intergrations</summary>
            <ul>
                <details>
                    <summary>Discord Oauth</summary>
                    <ul>
                        <li>Link messages</li>
                        <li>Link Contacts</li>
                    </ul>
                </details>
                <details>
                    <summary>Canvas Oauth</summary>
                    <ul>
                        <li>Link messages</li>
                        <li>Link notifications</li>
                        <li>Link profiles</li>
                        <li>Add badges via couses</li>
                    </ul>
                </details>
            </ul>
        </details>
        <details>
            <summary>Play edu Games</summary>
            <ul>
                <li>A version of ep -> get points</li>
                <li>Minecraft EDU -> get points</li>
                <li>Solve Problems -> get points</li>
                <li>Solve Bounty Problems -> get currency</li>
            </ul>
        </details>
        <details>
            <summary>Place Bountys</summary>
            <ul>
                <li>place a job bounty (E.G cleaning) -> lose currency</li>
                <li>Place a problem bounty (E.G write some code) -> lose currency</li>
            </ul>
        </details>
        <details>
            <summary>Credit System</summary>
            <ul>
                <details>
                    <summary>[Automatic]</summary>
                    <ul>
                        <li>Gets given a detetion -> lose credit</li>
                        <li>Gets given a demirit -> lose credit</li>
                        <li>Gets given a merit -> gain credit</li>
                        <li>Earn points -> gain credit</li>
                        <li>Place bounty -> gain credit</li>
                        <li>Low credit -> give detention (Credit doesnt lower though)</li>
                    </ul>
                </details>
                <li>Use credit to negate detentions</li>
                <li>If high credit give privliages</li>
            </ul>
        </details>
    </ul>
</details>

### Internial Structure

<details>
<summary> USER </summary>
|KEY                 TYPE
|-----------------------|------------------------|
|INTERGRATION        INTERGRATION[]       
|CREDIT              number               
|POINTS              number               
|CURRENCY            float                
|                                         
|DETENTIONS          DETENTION[]          
|ARCIVED-DETENTIONS  DETENTION[]          
|                                         
|ACRIVES             ARCIVE[]             
</details>

<details>
<summary> INTERGRATION </summary>
|KEY                 TYPE
|-----------------------|------------------------|
|ID                  UUID                 
|PERMS               STRING[]             

</details>

<details>
<summary> DETENTION </summary>
|KEY                 TYPE
|-----------------------|------------------------|
|TIME                DATE                 
|LOCATION            STRING               
|LENGTH              NUMBER               
|DISTRIBOTOR         USER                 
</details>

<details>
<summary> ARCHIVE </summary>
|KEY                 TYPE
|-----------------------|------------------------|
|CREATION TIME       DATE                 
|NAME                STRING               
|VALUE               STRING               
</details>

</ul></details>