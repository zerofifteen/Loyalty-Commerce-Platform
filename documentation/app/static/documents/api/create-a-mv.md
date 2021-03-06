### Create an MV

To create a new MV, POST the loyalty program member's account details to the loyalty program's MV service and sign the request with your app credentials. In sandbox mode, the LCP never communicates with the loyalty program. All operations are simulated. The LCP simulates different success and failure responses depending on the parameters sent when creating a MV.

Authenticating a member requires a specific set of fields, defined by the specific loyalty program you wish to communicate with. For example, some loyalty programs may require a member ID and password, while others require a member ID, last name, and password.

#### Parameters

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>lp-id</td>
            <td>The identifier of the <a href="#loyalty-programs">loyalty program</a> (LP).</td>
        </tr>
        <tr>
            <td>firstName</td>
            <td>The first name of the loyalty program member.</p>
                <p><strong>Sandbox mode</strong>: To simulate an unknown error from the loyalty program, set the firstName field to "Bugs".</p></td>
        </tr>
        <tr>
            <td>lastName</td>
            <td><p>The last name of the loyalty program member.</p>
                <p><strong>Sandbox mode</strong>: To simulate a non-zero balance, append a space and a positive integer to the lastName field. For example, to simulate a balance of 2000 for John Doe, set lastName to "Doe 2000".</p></td>
        </tr>
        <tr>
            <td>memberId</td>
            <td><p>The member ID of the loyalty program member.</p>
                <p><strong>Sandbox mode</strong>: To simulate a successful MV, set the memberId field to "dVNm" when using the <a href="#loyalty-programs">demo loyalty program</a>.
            </td>
        </tr>
        <tr>
            <td>password</td>
            <td>The password for the member's account. Not required for the demo loyalty program.</td>
        </tr>
        <tr>
            <td>zip</td>
            <td>The zip code or postal code for the member’s account. Not required for the demo loyalty program.</td>
        </tr>
    </tbody>
</table>

#### Returns

The MV object if it was created successfully. Returns an [error](./?doc=reference-manual#errors) if the firstName, lastName or memberId is not provided or if the member could not be validated for the given loyalty program.












